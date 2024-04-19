# Comparing `tmp/env_wrangler-0.1.1.tar.gz` & `tmp/env_wrangler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "env_wrangler-0.1.1.tar", last modified: Thu Apr 18 16:30:21 2024, max compression
+gzip compressed data, was "env_wrangler-0.1.2.tar", last modified: Thu Apr 18 17:29:23 2024, max compression
```

## Comparing `env_wrangler-0.1.1.tar` & `env_wrangler-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.388373 env_wrangler-0.1.1/
--rw-r--r--   0 tsantor    (501) staff       (20)      206 2024-04-15 19:14:54.000000 env_wrangler-0.1.1/AUTHORS.md
--rw-r--r--   0 tsantor    (501) staff       (20)      187 2024-04-15 19:14:54.000000 env_wrangler-0.1.1/HISTORY.md
--rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-15 19:14:54.000000 env_wrangler-0.1.1/LICENSE
--rw-r--r--   0 tsantor    (501) staff       (20)      143 2024-04-17 21:29:57.000000 env_wrangler-0.1.1/MANIFEST.in
--rw-r--r--   0 tsantor    (501) staff       (20)     3292 2024-04-18 16:30:21.388098 env_wrangler-0.1.1/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)     1883 2024-04-18 14:26:34.000000 env_wrangler-0.1.1/README.md
--rw-r--r--   0 tsantor    (501) staff       (20)     4977 2024-04-17 19:42:37.000000 env_wrangler-0.1.1/pyproject.toml
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.383588 env_wrangler-0.1.1/requirements/
--rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-16 17:02:52.000000 env_wrangler-0.1.1/requirements/requirements.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-17 19:20:46.000000 env_wrangler-0.1.1/requirements/requirements_dev.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-16 17:02:52.000000 env_wrangler-0.1.1/requirements/requirements_test.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-18 16:30:21.388438 env_wrangler-0.1.1/setup.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-15 19:14:54.000000 env_wrangler-0.1.1/setup.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.381051 env_wrangler-0.1.1/src/
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.385187 env_wrangler-0.1.1/src/env_wrangler/
--rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-04-18 16:01:14.000000 env_wrangler-0.1.1/src/env_wrangler/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)     6182 2024-04-18 16:19:08.000000 env_wrangler-0.1.1/src/env_wrangler/cli.py
--rw-r--r--   0 tsantor    (501) staff       (20)       85 2024-04-18 13:55:19.000000 env_wrangler-0.1.1/src/env_wrangler/constants.py
--rw-r--r--   0 tsantor    (501) staff       (20)     4031 2024-04-18 16:26:57.000000 env_wrangler-0.1.1/src/env_wrangler/core.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.386390 env_wrangler-0.1.1/src/env_wrangler/data/
--rw-r--r--   0 tsantor    (501) staff       (20)      564 2024-04-18 16:12:33.000000 env_wrangler-0.1.1/src/env_wrangler/data/env-wrangler.cfg
--rw-r--r--   0 tsantor    (501) staff       (20)     1273 2024-04-18 13:55:19.000000 env_wrangler-0.1.1/src/env_wrangler/settings.py
--rw-r--r--   0 tsantor    (501) staff       (20)      454 2024-04-18 14:10:28.000000 env_wrangler-0.1.1/src/env_wrangler/utils.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.387836 env_wrangler-0.1.1/src/env_wrangler.egg-info/
--rw-r--r--   0 tsantor    (501) staff       (20)     3292 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)      680 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       54 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/entry_points.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/requires.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       13 2024-04-18 16:30:21.000000 env_wrangler-0.1.1/src/env_wrangler.egg-info/top_level.txt
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 16:30:21.387431 env_wrangler-0.1.1/tests/
--rw-r--r--   0 tsantor    (501) staff       (20)     5595 2024-04-18 15:41:07.000000 env_wrangler-0.1.1/tests/test_core.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1243 2024-04-17 20:38:54.000000 env_wrangler-0.1.1/tests/test_settings.py
--rw-r--r--   0 tsantor    (501) staff       (20)      441 2024-04-18 14:10:38.000000 env_wrangler-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.195319 env_wrangler-0.1.2/
+-rw-r--r--   0 tsantor    (501) staff       (20)      206 2024-04-15 19:14:54.000000 env_wrangler-0.1.2/AUTHORS.md
+-rw-r--r--   0 tsantor    (501) staff       (20)      413 2024-04-18 17:26:33.000000 env_wrangler-0.1.2/HISTORY.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     1058 2024-04-15 19:14:54.000000 env_wrangler-0.1.2/LICENSE
+-rw-r--r--   0 tsantor    (501) staff       (20)      143 2024-04-17 21:29:57.000000 env_wrangler-0.1.2/MANIFEST.in
+-rw-r--r--   0 tsantor    (501) staff       (20)     3518 2024-04-18 17:29:23.195046 env_wrangler-0.1.2/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)     1883 2024-04-18 14:26:34.000000 env_wrangler-0.1.2/README.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     4977 2024-04-17 19:42:37.000000 env_wrangler-0.1.2/pyproject.toml
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.190333 env_wrangler-0.1.2/requirements/
+-rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-04-16 17:02:52.000000 env_wrangler-0.1.2/requirements/requirements.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      213 2024-04-17 19:20:46.000000 env_wrangler-0.1.2/requirements/requirements_dev.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      474 2024-04-16 17:02:52.000000 env_wrangler-0.1.2/requirements/requirements_test.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-18 17:29:23.195383 env_wrangler-0.1.2/setup.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)       69 2024-04-15 19:14:54.000000 env_wrangler-0.1.2/setup.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.187605 env_wrangler-0.1.2/src/
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.192103 env_wrangler-0.1.2/src/env_wrangler/
+-rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-04-18 17:25:04.000000 env_wrangler-0.1.2/src/env_wrangler/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     6182 2024-04-18 16:19:08.000000 env_wrangler-0.1.2/src/env_wrangler/cli.py
+-rw-r--r--   0 tsantor    (501) staff       (20)       85 2024-04-18 13:55:19.000000 env_wrangler-0.1.2/src/env_wrangler/constants.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     4034 2024-04-18 17:24:36.000000 env_wrangler-0.1.2/src/env_wrangler/core.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.193393 env_wrangler-0.1.2/src/env_wrangler/data/
+-rw-r--r--   0 tsantor    (501) staff       (20)      576 2024-04-18 17:09:45.000000 env_wrangler-0.1.2/src/env_wrangler/data/env-wrangler.cfg
+-rw-r--r--   0 tsantor    (501) staff       (20)     1273 2024-04-18 13:55:19.000000 env_wrangler-0.1.2/src/env_wrangler/settings.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      454 2024-04-18 14:10:28.000000 env_wrangler-0.1.2/src/env_wrangler/utils.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.194744 env_wrangler-0.1.2/src/env_wrangler.egg-info/
+-rw-r--r--   0 tsantor    (501) staff       (20)     3518 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)      680 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       54 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/entry_points.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       27 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/requires.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       13 2024-04-18 17:29:23.000000 env_wrangler-0.1.2/src/env_wrangler.egg-info/top_level.txt
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-18 17:29:23.194423 env_wrangler-0.1.2/tests/
+-rw-r--r--   0 tsantor    (501) staff       (20)     5681 2024-04-18 17:28:35.000000 env_wrangler-0.1.2/tests/test_core.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1243 2024-04-17 20:38:54.000000 env_wrangler-0.1.2/tests/test_settings.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      441 2024-04-18 14:10:38.000000 env_wrangler-0.1.2/tests/test_utils.py
```

### Comparing `env_wrangler-0.1.1/LICENSE` & `env_wrangler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.1/PKG-INFO` & `env_wrangler-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-wrangler
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/env-wrangler.git
 Project-URL: Issues, https://github.com/tsantor/env-wrangler/issues
 Project-URL: Changelog, https://github.com/tsantor/env-wrangler/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -85,10 +85,19 @@
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/env-wrangler/issues) on Github.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
-## 0.0.1 (2024-04-15)
+## 0.1.2 (2024-04-18)
+
+- Bug fix for if a env value contains an "=". We only split on the first "=" so we get key,value from .env.
+
+## 0.1.1 (2024-04-18)
+
+- Write secrets files non-destructively
+- Sort keys for secrets files
+
+## 0.1.0 (2024-04-15)
 
 - First release
```

### Comparing `env_wrangler-0.1.1/README.md` & `env_wrangler-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.1/pyproject.toml` & `env_wrangler-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.1/src/env_wrangler/cli.py` & `env_wrangler-0.1.2/src/env_wrangler/cli.py`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.1/src/env_wrangler/core.py` & `env_wrangler-0.1.2/src/env_wrangler/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def save_dict_to_env_file(data: dict, file_path: str) -> Path:
     """Save a dictionary to an env file (non-destructive)."""
     if not data:
         return None
     file_path = Path(file_path).expanduser()
     if file_path.exists():
         existing_data = dict(
-            line.split("=") for line in file_path.read_text().splitlines() if line
+            line.split("=", 1) for line in file_path.read_text().splitlines() if line
         )
         existing_data.update(data)
         data = existing_data
     # We ensure it is sorted before writing
     env_content = "\n".join([f"{key}={value}" for key, value in sorted(data.items())])
     file_path.write_text(env_content)
     return file_path
```

### Comparing `env_wrangler-0.1.1/src/env_wrangler/data/env-wrangler.cfg` & `env_wrangler-0.1.2/src/env_wrangler/data/env-wrangler.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 [default]
 ; Any environment variable that contains one of the following key words will be considered a secret
-; KEY, USER, TOKEN may be too broad and may result in false positives so use with caution
-key_words = ACCESS_KEY, ACCESS_TOKEN, API_KEY, API_SECRET, AUTH_KEY, AUTH_TOKEN, CLIENT_ID, CLIENT_SECRET, CONSUMER_KEY, CREDENTIALS, ENCRYPTION_KEY, HASH, JWT_SECRET, KEY, MASTER_KEY, OAUTH_TOKEN, PASSWORD, PRIVATE_KEY, SALT, SECRET, STORAGE_KEY, SUBSCRIPTION_ID, TOKEN, USER
+; KEY, USER, PASS, TOKEN may be too broad and may result in false positives so use with caution
+key_words = ACCESS_KEY, ACCESS_TOKEN, API_KEY, API_SECRET, AUTH_KEY, AUTH_TOKEN, CLIENT_ID, CLIENT_SECRET, CONSUMER_KEY, CREDENTIALS, ENCRYPTION_KEY, HASH, JWT_SECRET, KEY, MASTER_KEY, OAUTH_TOKEN, PASS, PASSWORD, PRIVATE_KEY, SALT, SECRET, STORAGE_KEY, SUBSCRIPTION_ID, TOKEN, USER
 ; The env files that will be considered for extraction
 envs = .env, .django, .postgres
```

### Comparing `env_wrangler-0.1.1/src/env_wrangler/settings.py` & `env_wrangler-0.1.2/src/env_wrangler/settings.py`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.1/src/env_wrangler.egg-info/PKG-INFO` & `env_wrangler-0.1.2/src/env_wrangler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: env-wrangler
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extract secrets from .env files into their own file (either `.secrets` or `secrets.json`). Also provides `mask` and `unmask` options. The resulting secrets file can be leveraged to get your secrets into a 3rd party secrets manager like AWS Secrets Manager or something else.
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: Repository, https://github.com/tsantor/env-wrangler.git
 Project-URL: Issues, https://github.com/tsantor/env-wrangler/issues
 Project-URL: Changelog, https://github.com/tsantor/env-wrangler/blob/master/HISTORY.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -85,10 +85,19 @@
 
 If you experience any issues, please create an [issue](https://github.com/tsantor/env-wrangler/issues) on Github.
 
 # History
 
 All notable changes to this project will be documented in this file. This project adheres to [Semantic Versioning](http://semver.org/).
 
-## 0.0.1 (2024-04-15)
+## 0.1.2 (2024-04-18)
+
+- Bug fix for if a env value contains an "=". We only split on the first "=" so we get key,value from .env.
+
+## 0.1.1 (2024-04-18)
+
+- Write secrets files non-destructively
+- Sort keys for secrets files
+
+## 0.1.0 (2024-04-15)
 
 - First release
```

### Comparing `env_wrangler-0.1.1/src/env_wrangler.egg-info/SOURCES.txt` & `env_wrangler-0.1.2/src/env_wrangler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `env_wrangler-0.1.1/tests/test_core.py` & `env_wrangler-0.1.2/tests/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,26 +48,32 @@
     file_path = tmp_path / "test.json"
     output_file = save_dict_to_json_file(data, str(file_path))
 
     assert output_file is None
 
 
 def test_save_dict_to_env_file(tmp_path):
-    data = {"key1": "value1", "key2": "value2", "key3": "value3", "key4": "value4"}
+    data = {
+        "key1": "value1",
+        "key2": "value2",
+        "key3": "value3",
+        "key4": "value4",
+        "key5": "value==5",  # Test bug fix
+    }
     file_path = tmp_path / "test.env"
     # Write only a few keys to the file to test that the function appends new keys
     file_path.write_text("key1=value1\nkey2=value2")
     output_file = save_dict_to_env_file(data, str(file_path))
 
     file_path = Path(file_path)
     lines = file_path.read_text().splitlines()
 
     loaded_data = {}
     for line in lines:
-        key, value = line.split("=")
+        key, value = line.split("=", 1)
         loaded_data[key] = value
 
     assert isinstance(output_file, Path)
     assert loaded_data == data
 
 
 def test_save_empty_dict_to_env_file(tmp_path):
```

### Comparing `env_wrangler-0.1.1/tests/test_settings.py` & `env_wrangler-0.1.2/tests/test_settings.py`

 * *Files identical despite different names*

