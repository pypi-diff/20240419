# Comparing `tmp/env_wrangler-0.1.2.tar.gz` & `tmp/env_wrangler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_wrangler-0.1.2.tar", last modified: Thu Apr 18 17:29:23 2024, max compression
+gzip compressed data, was "env_wrangler-0.1.3.tar", last modified: Fri Apr 19 14:22:44 2024, max compression
```

## Comparing `env_wrangler-0.1.2.tar` & `env_wrangler-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.195319 env_wrangler-0.1.2/
--rw-r--r--   0 tsantor    (501) staff       (20)      206 2024-04-15 19:14:54.000000 env_wrangler-0.1.2/AUTHORS.md
--rw-r--r--   0 tsantor    (501) staff       (20)      413 2024-04-18 17:26:33.000000 env_wrangler-0.1.2/HISTORY.md
--rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-15 19:14:54.000000 env_wrangler-0.1.2/LICENSE
--rw-r--r--   0 tsantor    (501) staff       (20)      143 2024-04-17 21:29:57.000000 env_wrangler-0.1.2/MANIFEST.in
--rw-r--r--   0 tsantor    (501) staff       (20)     3518 2024-04-18 17:29:23.195046 env_wrangler-0.1.2/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)     1883 2024-04-18 14:26:34.000000 env_wrangler-0.1.2/README.md
--rw-r--r--   0 tsantor    (501) staff       (20)     4977 2024-04-17 19:42:37.000000 env_wrangler-0.1.2/pyproject.toml
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.190333 env_wrangler-0.1.2/requirements/
--rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-16 17:02:52.000000 env_wrangler-0.1.2/requirements/requirements.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-17 19:20:46.000000 env_wrangler-0.1.2/requirements/requirements_dev.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-16 17:02:52.000000 env_wrangler-0.1.2/requirements/requirements_test.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-18 17:29:23.195383 env_wrangler-0.1.2/setup.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-15 19:14:54.000000 env_wrangler-0.1.2/setup.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.187605 env_wrangler-0.1.2/src/
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.192103 env_wrangler-0.1.2/src/env_wrangler/
--rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-04-18 17:25:04.000000 env_wrangler-0.1.2/src/env_wrangler/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)     6182 2024-04-18 16:19:08.000000 env_wrangler-0.1.2/src/env_wrangler/cli.py
--rw-r--r--   0 tsantor    (501) staff       (20)       85 2024-04-18 13:55:19.000000 env_wrangler-0.1.2/src/env_wrangler/constants.py
--rw-r--r--   0 tsantor    (501) staff       (20)     4034 2024-04-18 17:24:36.000000 env_wrangler-0.1.2/src/env_wrangler/core.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.193393 env_wrangler-0.1.2/src/env_wrangler/data/
--rw-r--r--   0 tsantor    (501) staff       (20)      576 2024-04-18 17:09:45.000000 env_wrangler-0.1.2/src/env_wrangler/data/env-wrangler.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)     1273 2024-04-18 13:55:19.000000 env_wrangler-0.1.2/src/env_wrangler/settings.py
--rw-r--r--   0 tsantor    (501) staff       (20)      454 2024-04-18 14:10:28.000000 env_wrangler-0.1.2/src/env_wrangler/utils.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.194744 env_wrangler-0.1.2/src/env_wrangler.egg-info/
--rw-r--r--   0 tsantor    (501) staff       (20)     3518 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)      680 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       54 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/entry_points.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/requires.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       13 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/top_level.txt
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.194423 env_wrangler-0.1.2/tests/
--rw-r--r--   0 tsantor    (501) staff       (20)     5681 2024-04-18 17:28:35.000000 env_wrangler-0.1.2/tests/test_core.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1243 2024-04-17 20:38:54.000000 env_wrangler-0.1.2/tests/test_settings.py
--rw-r--r--   0 tsantor    (501) staff       (20)      441 2024-04-18 14:10:38.000000 env_wrangler-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:22:44.579365 env_wrangler-0.1.3/
+-rw-r--r--   0 tsantor    (501) staff       (20)      206 2024-04-15 19:14:54.000000 env_wrangler-0.1.3/AUTHORS.md
+-rw-r--r--   0 tsantor    (501) staff       (20)      546 2024-04-19 14:21:43.000000 env_wrangler-0.1.3/HISTORY.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-15 19:14:54.000000 env_wrangler-0.1.3/LICENSE
+-rw-r--r--   0 tsantor    (501) staff       (20)      143 2024-04-17 21:29:57.000000 env_wrangler-0.1.3/MANIFEST.in
+-rw-r--r--   0 tsantor    (501) staff       (20)     3651 2024-04-19 14:22:44.579140 env_wrangler-0.1.3/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)     1883 2024-04-18 14:26:34.000000 env_wrangler-0.1.3/README.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     4977 2024-04-17 19:42:37.000000 env_wrangler-0.1.3/pyproject.toml
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:22:44.576308 env_wrangler-0.1.3/requirements/
+-rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-16 17:02:52.000000 env_wrangler-0.1.3/requirements/requirements.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-17 19:20:46.000000 env_wrangler-0.1.3/requirements/requirements_dev.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-16 17:02:52.000000 env_wrangler-0.1.3/requirements/requirements_test.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-19 14:22:44.579413 env_wrangler-0.1.3/setup.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-15 19:14:54.000000 env_wrangler-0.1.3/setup.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:22:44.574651 env_wrangler-0.1.3/src/
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:22:44.577203 env_wrangler-0.1.3/src/env_wrangler/
+-rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-04-19 14:21:49.000000 env_wrangler-0.1.3/src/env_wrangler/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     6327 2024-04-19 14:01:51.000000 env_wrangler-0.1.3/src/env_wrangler/cli.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      121 2024-04-19 13:58:26.000000 env_wrangler-0.1.3/src/env_wrangler/constants.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     4150 2024-04-19 14:08:14.000000 env_wrangler-0.1.3/src/env_wrangler/core.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:22:44.578237 env_wrangler-0.1.3/src/env_wrangler/data/
+-rw-r--r--   0 tsantor    (501) staff       (20)      680 2024-04-19 14:19:54.000000 env_wrangler-0.1.3/src/env_wrangler/data/env-wrangler.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)     1273 2024-04-18 13:55:19.000000 env_wrangler-0.1.3/src/env_wrangler/settings.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      454 2024-04-18 14:10:28.000000 env_wrangler-0.1.3/src/env_wrangler/utils.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:22:44.578891 env_wrangler-0.1.3/src/env_wrangler.egg-info/
+-rw-r--r--   0 tsantor    (501) staff       (20)     3651 2024-04-19 14:22:44.000000 env_wrangler-0.1.3/src/env_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)      680 2024-04-19 14:22:44.000000 env_wrangler-0.1.3/src/env_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-19 14:22:44.000000 env_wrangler-0.1.3/src/env_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       54 2024-04-19 14:22:44.000000 env_wrangler-0.1.3/src/env_wrangler.egg-info/entry_points.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-04-19 14:22:44.000000 env_wrangler-0.1.3/src/env_wrangler.egg-info/requires.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       13 2024-04-19 14:22:44.000000 env_wrangler-0.1.3/src/env_wrangler.egg-info/top_level.txt
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-19 14:22:44.578706 env_wrangler-0.1.3/tests/
+-rw-r--r--   0 tsantor    (501) staff       (20)     5791 2024-04-19 14:17:22.000000 env_wrangler-0.1.3/tests/test_core.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1243 2024-04-17 20:38:54.000000 env_wrangler-0.1.3/tests/test_settings.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      441 2024-04-18 14:10:38.000000 env_wrangler-0.1.3/tests/test_utils.py
```

### Comparing `env_wrangler-0.1.2/LICENSE` & `env_wrangler-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.2/PKG-INFO` & `env_wrangler-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-wrangler
-Version: 0.1.2
+Version: 0.1.3
 Summary: Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/env-wrangler.git
 Project-URL: Issues, https://github.com/tsantor/env-wrangler/issues
 Project-URL: Changelog, https://github.com/tsantor/env-wrangler/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -85,14 +85,18 @@
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/env-wrangler/issues) on Github.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.3 (2024-04-19)
+
+- Added `ignore_keys` to config for keys (exact key names) to always ignore even if they contain `key_word`.
+
 ## 0.1.2 (2024-04-18)
 
 - Bug fix for if a env value contains an "=". We only split on the first "=" so we get key,value from .env.
 
 ## 0.1.1 (2024-04-18)
 
 - Write secrets files non-destructively
```

### Comparing `env_wrangler-0.1.2/README.md` & `env_wrangler-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.2/pyproject.toml` & `env_wrangler-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.2/src/env_wrangler/cli.py` & `env_wrangler-0.1.3/src/env_wrangler/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 from pathlib import Path
 
 import click  # https://click.palletsprojects.com/
 
 from .constants import DEFAULT_SECTION
+from .constants import IGNORE_KEYS_SETTING
 from .constants import KEY_WORDS_SETTING
 from .core import envs_to_dict
 from .core import filter_keys_by_substring
 from .core import mask_sensitive_data_in_file
 from .core import remove_masked_values
 from .core import save_dict_to_env_file
 from .core import save_dict_to_json_file
@@ -114,22 +115,23 @@
             ),
             fg="yellow",
             err=True,
         )
         return
 
     key_words = get_config_value_as_list(config, DEFAULT_SECTION, KEY_WORDS_SETTING)
+    ignore_keys = get_config_value_as_list(config, DEFAULT_SECTION, IGNORE_KEYS_SETTING)
 
     masked_files = []
     target_envs = get_config_value_as_list(config, DEFAULT_SECTION, "envs")
     for file_path in target_envs:
         file = path / file_path
         if file.exists():
             masked_files.append(file)
-            mask_sensitive_data_in_file(file, key_words)
+            mask_sensitive_data_in_file(file, key_words, ignore_keys)
 
     # Let the user know which files were masked
     if masked_files:
         click.echo("Masked sensitive data in the following envs:")
         for file in masked_files:
             click.echo(f"   {home_agnostic_path(file)}")
```

### Comparing `env_wrangler-0.1.2/src/env_wrangler/core.py` & `env_wrangler-0.1.3/src/env_wrangler/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,29 +64,34 @@
     Filters a dictionary to remove masked values.
 
     :param input_dict: Dictionary to be filtered.
     """
     return {key: value for key, value in input_dict.items() if value != MASK_VALUE}
 
 
-def mask_sensitive_data_in_file(file_path: str, filter_keys: list) -> Path:
+def mask_sensitive_data_in_file(
+    file_path: str, filter_keys: list, ignore_keys=None
+) -> Path:
     """Mask sensitive data in a .env file.
 
     Args:
         file_path (str): The path to the .env file.
         filter_keys (list): The keys to mask in the .env file.
     """
     file_path = Path(file_path).expanduser()
     lines = file_path.read_text().splitlines()
 
+    ignore_keys = ignore_keys or []
+
     masked_lines = []
     for line in lines:
-        for key in filter_keys:
-            if key in line.split("=")[0]:
-                line = line.split("=")[0] + f"={MASK_VALUE}"  # noqa: PLW2901
+        for check_key in filter_keys:
+            key, _ = line.split("=", 1)
+            if check_key in key and key not in ignore_keys:
+                line = key + f"={MASK_VALUE}"  # noqa: PLW2901
         masked_lines.append(line)
 
     file_path.write_text("\n".join(masked_lines))
     return file_path
 
 
 def unmask_sensitive_data_in_file(file_path: str, replacements: dict) -> Path:
@@ -98,16 +103,16 @@
     """
     file_path = Path(file_path).expanduser()
     lines = file_path.read_text().splitlines()
 
     replaced_lines = []
     for line in lines:
         for key, value in replacements.items():
-            if key in line.split("=")[0]:
-                line = line.split("=")[0] + "=" + value  # noqa: PLW2901
+            if key in line.split("=", 1)[0]:
+                line = line.split("=", 1)[0] + "=" + value  # noqa: PLW2901
         replaced_lines.append(line)
 
     file_path.write_text("\n".join(replaced_lines))
     return file_path
 
 
 def json_to_env(json_file_path: str, env_file_path: str) -> Path:
```

### Comparing `env_wrangler-0.1.2/src/env_wrangler/data/env-wrangler.cfg` & `env_wrangler-0.1.3/src/env_wrangler/data/env-wrangler.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,8 @@
 [default]
 ; Any environment variable that contains one of the following key words will be considered a secret
 ; KEY, USER, PASS, TOKEN may be too broad and may result in false positives so use with caution
 key_words = ACCESS_KEY, ACCESS_TOKEN, API_KEY, API_SECRET, AUTH_KEY, AUTH_TOKEN, CLIENT_ID, CLIENT_SECRET, CONSUMER_KEY, CREDENTIALS, ENCRYPTION_KEY, HASH, JWT_SECRET, KEY, MASTER_KEY, OAUTH_TOKEN, PASS, PASSWORD, PRIVATE_KEY, SALT, SECRET, STORAGE_KEY, SUBSCRIPTION_ID, TOKEN, USER
+; Any environment variable exactly matches one of the following key words will be ignored
+ignore_keys =
 ; The env files that will be considered for extraction
 envs = .env, .django, .postgres
```

### Comparing `env_wrangler-0.1.2/src/env_wrangler/settings.py` & `env_wrangler-0.1.3/src/env_wrangler/settings.py`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.2/src/env_wrangler.egg-info/PKG-INFO` & `env_wrangler-0.1.3/src/env_wrangler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-wrangler
-Version: 0.1.2
+Version: 0.1.3
 Summary: Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/env-wrangler.git
 Project-URL: Issues, https://github.com/tsantor/env-wrangler/issues
 Project-URL: Changelog, https://github.com/tsantor/env-wrangler/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -85,14 +85,18 @@
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/env-wrangler/issues) on Github.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
+## 0.1.3 (2024-04-19)
+
+- Added `ignore_keys` to config for keys (exact key names) to always ignore even if they contain `key_word`.
+
 ## 0.1.2 (2024-04-18)
 
 - Bug fix for if a env value contains an "=". We only split on the first "=" so we get key,value from .env.
 
 ## 0.1.1 (2024-04-18)
 
 - Write secrets files non-destructively
```

### Comparing `env_wrangler-0.1.2/src/env_wrangler.egg-info/SOURCES.txt` & `env_wrangler-0.1.3/src/env_wrangler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.2/tests/test_core.py` & `env_wrangler-0.1.3/tests/test_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -112,26 +112,31 @@
 
     assert remove_masked_values(input_dict) == expected_dict
 
 
 def test_mask_sensitive_data_in_file(tmp_path):
     # Create a .env file in the temporary directory
     env_file = tmp_path / ".env"
-    env_file.write_text("SECRET_KEY=secret\nPASSWORD=password\nFOO=bar\nBAR=baz")
+    env_file.write_text(
+        "SECRET_KEY=secret\nPASSWORD=password\nFOO=bar\nBAR=baz\nIGNORED_KEY=ignored"
+    )
 
     # Call mask_sensitive_data with the path to the .env file and a list of sensitive keys
-    output_file = mask_sensitive_data_in_file(str(env_file), ["SECRET_KEY", "PASSWORD"])
+    output_file = mask_sensitive_data_in_file(
+        str(env_file), ["KEY", "PASSWORD"], ["IGNORED_KEY"]
+    )
 
     # Load the .env file and check that the sensitive keys have been masked
     env_vars = dotenv_values(str(env_file))
     assert isinstance(output_file, Path)
     assert env_vars["SECRET_KEY"] == MASK_VALUE  # noqa: S105
     assert env_vars["PASSWORD"] == MASK_VALUE  # noqa: S105
     assert env_vars["FOO"] == "bar"
     assert env_vars["BAR"] == "baz"
+    assert env_vars["IGNORED_KEY"] == "ignored"
 
 
 def test_unmask_sensitive_data_in_file(tmp_path):
     # Create a .env file in the temporary directory with masked sensitive data
     env_file = tmp_path / ".env"
     env_file.write_text(
         f"SECRET_KEY={MASK_VALUE}\nPASSWORD={MASK_VALUE}\nFOO=bar\nBAR=baz"
@@ -161,11 +166,11 @@
     env_file = tmp_path / ".env"
 
     # Call json_to_env with the paths to the JSON and .env files
     output_file = json_to_env(str(json_file), str(env_file))
 
     # Load the .env file and check that it contains the correct data
     env_lines = env_file.read_text().splitlines()
-    env_data = dict(line.split("=") for line in env_lines)
+    env_data = dict(line.split("=", 1) for line in env_lines)
 
     assert isinstance(output_file, Path)
     assert env_data == data
```

### Comparing `env_wrangler-0.1.2/tests/test_settings.py` & `env_wrangler-0.1.3/tests/test_settings.py`

 * *Files identical despite different names*

