# Comparing `tmp/microbeseq_nbdev_example-0.0.4.tar.gz` & `tmp/microbeseq_nbdev_example-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microbeseq_nbdev_example-0.0.4.tar", last modified: Fri Mar 22 13:57:41 2024, max compression
+gzip compressed data, was "microbeseq_nbdev_example-0.0.5.tar", last modified: Fri Apr 19 06:52:22 2024, max compression
```

## Comparing `microbeseq_nbdev_example-0.0.4.tar` & `microbeseq_nbdev_example-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 b246297    (502) staff       (20)        0 2024-03-22 13:57:41.496701 microbeseq_nbdev_example-0.0.4/
--rw-rw-r--   0 b246297    (502) staff       (20)     1094 2024-03-22 13:56:55.000000 microbeseq_nbdev_example-0.0.4/LICENSE
--rw-rw-r--   0 b246297    (502) staff       (20)      230 2024-03-22 13:56:56.000000 microbeseq_nbdev_example-0.0.4/MANIFEST.in
--rw-r--r--   0 b246297    (502) staff       (20)     1170 2024-03-22 13:57:41.496470 microbeseq_nbdev_example-0.0.4/PKG-INFO
--rw-r--r--   0 b246297    (502) staff       (20)      318 2024-03-22 13:56:53.000000 microbeseq_nbdev_example-0.0.4/README.md
-drwxr-xr-x   0 b246297    (502) staff       (20)        0 2024-03-22 13:57:41.494486 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/
--rw-r--r--   0 b246297    (502) staff       (20)       22 2024-03-22 13:57:37.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/__init__.py
--rw-r--r--   0 b246297    (502) staff       (20)     2355 2024-03-22 13:57:37.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/_modidx.py
-drwxr-xr-x   0 b246297    (502) staff       (20)        0 2024-03-22 13:57:41.496011 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/config/
--rw-r--r--   0 b246297    (502) staff       (20)     1366 2024-03-22 13:56:56.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/config/config.default.env
--rw-r--r--   0 b246297    (502) staff       (20)      451 2024-03-22 13:56:56.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/config/config.default.yaml
--rw-r--r--   0 b246297    (502) staff       (20)     9959 2024-03-22 13:57:37.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/core.py
--rw-r--r--   0 b246297    (502) staff       (20)     1930 2024-03-22 13:57:37.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/hello_world.py
-drwxr-xr-x   0 b246297    (502) staff       (20)        0 2024-03-22 13:57:41.496205 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/
--rw-r--r--   0 b246297    (502) staff       (20)     1170 2024-03-22 13:57:41.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/PKG-INFO
--rw-r--r--   0 b246297    (502) staff       (20)      637 2024-03-22 13:57:41.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/SOURCES.txt
--rw-r--r--   0 b246297    (502) staff       (20)        1 2024-03-22 13:57:41.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/dependency_links.txt
--rw-r--r--   0 b246297    (502) staff       (20)      201 2024-03-22 13:57:41.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/entry_points.txt
--rw-r--r--   0 b246297    (502) staff       (20)        1 2024-03-22 13:57:06.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/not-zip-safe
--rw-r--r--   0 b246297    (502) staff       (20)       45 2024-03-22 13:57:41.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/requires.txt
--rw-r--r--   0 b246297    (502) staff       (20)       55 2024-03-22 13:57:41.000000 microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/top_level.txt
--rw-r--r--   0 b246297    (502) staff       (20)     1051 2024-03-22 13:57:37.000000 microbeseq_nbdev_example-0.0.4/settings.ini
--rw-r--r--   0 b246297    (502) staff       (20)       38 2024-03-22 13:57:41.496742 microbeseq_nbdev_example-0.0.4/setup.cfg
--rw-r--r--   0 b246297    (502) staff       (20)     2606 2024-03-22 13:57:05.000000 microbeseq_nbdev_example-0.0.4/setup.py
+drwxr-xr-x   0 b246297    (502) staff       (20)        0 2024-04-19 06:52:22.054404 microbeseq_nbdev_example-0.0.5/
+-rw-rw-r--   0 b246297    (502) staff       (20)     1094 2024-04-19 06:48:29.000000 microbeseq_nbdev_example-0.0.5/LICENSE
+-rw-rw-r--   0 b246297    (502) staff       (20)      230 2024-04-19 06:48:29.000000 microbeseq_nbdev_example-0.0.5/MANIFEST.in
+-rw-r--r--   0 b246297    (502) staff       (20)     1170 2024-04-19 06:52:22.054180 microbeseq_nbdev_example-0.0.5/PKG-INFO
+-rw-r--r--   0 b246297    (502) staff       (20)      318 2024-04-19 06:48:27.000000 microbeseq_nbdev_example-0.0.5/README.md
+drwxr-xr-x   0 b246297    (502) staff       (20)        0 2024-04-19 06:52:22.052146 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/
+-rw-r--r--   0 b246297    (502) staff       (20)       22 2024-04-19 06:52:19.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/__init__.py
+-rw-r--r--   0 b246297    (502) staff       (20)     2355 2024-04-19 06:52:19.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/_modidx.py
+drwxr-xr-x   0 b246297    (502) staff       (20)        0 2024-04-19 06:52:22.053622 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/config/
+-rw-r--r--   0 b246297    (502) staff       (20)     1366 2024-04-19 06:48:29.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/config/config.default.env
+-rw-r--r--   0 b246297    (502) staff       (20)      451 2024-04-19 06:48:29.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/config/config.default.yaml
+-rw-r--r--   0 b246297    (502) staff       (20)     8458 2024-04-19 06:52:19.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/core.py
+-rw-r--r--   0 b246297    (502) staff       (20)     1930 2024-04-19 06:52:19.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/hello_world.py
+drwxr-xr-x   0 b246297    (502) staff       (20)        0 2024-04-19 06:52:22.053847 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/
+-rw-r--r--   0 b246297    (502) staff       (20)     1170 2024-04-19 06:52:22.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/PKG-INFO
+-rw-r--r--   0 b246297    (502) staff       (20)      637 2024-04-19 06:52:22.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/SOURCES.txt
+-rw-r--r--   0 b246297    (502) staff       (20)        1 2024-04-19 06:52:22.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/dependency_links.txt
+-rw-r--r--   0 b246297    (502) staff       (20)      201 2024-04-19 06:52:22.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/entry_points.txt
+-rw-r--r--   0 b246297    (502) staff       (20)        1 2024-04-19 06:48:40.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/not-zip-safe
+-rw-r--r--   0 b246297    (502) staff       (20)       45 2024-04-19 06:52:22.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/requires.txt
+-rw-r--r--   0 b246297    (502) staff       (20)       55 2024-04-19 06:52:22.000000 microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/top_level.txt
+-rw-r--r--   0 b246297    (502) staff       (20)     1070 2024-04-19 06:52:19.000000 microbeseq_nbdev_example-0.0.5/settings.ini
+-rw-r--r--   0 b246297    (502) staff       (20)       38 2024-04-19 06:52:22.054450 microbeseq_nbdev_example-0.0.5/setup.cfg
+-rw-r--r--   0 b246297    (502) staff       (20)     2606 2024-04-19 06:48:38.000000 microbeseq_nbdev_example-0.0.5/setup.py
```

### Comparing `microbeseq_nbdev_example-0.0.4/LICENSE` & `microbeseq_nbdev_example-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `microbeseq_nbdev_example-0.0.4/PKG-INFO` & `microbeseq_nbdev_example-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microbeseq_nbdev_example
-Version: 0.0.4
+Version: 0.0.5
 Summary: TODO
 Home-page: https://github.com/$GIT_USER_NAME/microbeseq_nbdev_example
 Author: $GIT_USER_NAME
 Author-email: kimleeng@gmail.com
 License: MIT License
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/_modidx.py` & `microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/_modidx.py`

 * *Files identical despite different names*

### Comparing `microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/config/config.default.env` & `microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/config/config.default.env`

 * *Files identical despite different names*

### Comparing `microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/core.py` & `microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,41 +64,20 @@
 
     # Order of precedence: .env file > environment variables > default values
     # When developing, making a change to the config will not be reflected until the environment is restarted
 
     # Set the env vars first, this is needed for the card.yaml to replace ENV variables
     # NOTE: You need to adjust PROJECT_NAME to your package name for this to work, the exception is only for dev purposes
     # This here checks if your package is installed, such as through pypi or through pip install -e  [.dev] for development. If it is then it'll go there and use the config files there as your default values.
-    spec = importlib.util.find_spec(PACKAGE_NAME)
-    if (
-        DEV_MODE
-    ):  # Means we are in development and can reference the package path directly as it's relative to this code.
-        try:
-            dotenv.load_dotenv(
-                f"{PACKAGE_DIR}/config/config.default.env", override=False
-            )
-        except Exception as e:
-            print(f"Error: {PACKAGE_DIR}/config/config.default.env does not exist")
-            return False
-    elif (
-        spec is not None
-    ):  # Means the package is installed and we should get defaults from the package
-        module = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(
-            module
-        )  # load the module which means we know where the package is with module.__path__[0]
-        try:
-            dotenv.load_dotenv(
-                f"{module.__path__[0]}/config/config.default.env", override=False
-            )
-        except Exception as e:
-            print(
-                f"Error: {module.__path__[0]}/config/config.default.env does not exist"
-            )
-            return False
+    try:
+        dotenv.load_dotenv(f"{PACKAGE_DIR}/config/config.default.env", override=False)
+    except Exception as e:
+        print(f"Error: {PACKAGE_DIR}/config/config.default.env does not exist")
+        return False
+
     # 2. set values from file:
     if os.path.isfile(config_path):
         dotenv.load_dotenv(config_path, override=overide_env_vars)
 
     return True
 
 # %% ../nbs/00_core.ipynb 15
@@ -108,35 +87,21 @@
 
 def get_config(config_path: str = None, overide_env_vars: bool = True) -> dict:
     if config_path is None:
         config_path = ""
     # First sets environment with variables from config_path, then uses those variables to fill in appropriate values in the config.yaml file, the yaml file is then returned as a dict
     # If you want user env variables to take precedence over the config.yaml file then set overide_env_vars to False
     set_env_variables(config_path, overide_env_vars)
-    if (
-        DEV_MODE
-    ):  # Means we are in development and can reference the package path directly as it's relative to this code.
-        config: dict = envyaml.EnvYAML(
-            os.environ.get(
-                "CORE_YAML_CONFIG_FILE", f"{PACKAGE_DIR}/config/config.default.yaml"
-            ),
-            strict=False,
-        ).export()
-    else:
-        spec = importlib.util.find_spec(PACKAGE_NAME)
-        if spec is not None:
-            module = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(module)
-            config: dict = envyaml.EnvYAML(
-                os.environ.get(
-                    "CORE_YAML_CONFIG_FILE",
-                    f"{module.__path__[0]}/config/config.default.yaml",
-                ),
-                strict=False,
-            ).export()
+
+    config: dict = envyaml.EnvYAML(
+        os.environ.get(
+            "CORE_YAML_CONFIG_FILE", f"{PACKAGE_DIR}/config/config.default.yaml"
+        ),
+        strict=False,
+    ).export()
 
     return config
 
 # %% ../nbs/00_core.ipynb 17
 # create a os.PathLike object
 config = get_config(os.environ.get("CORE_CONFIG_FILE", ""))
```

### Comparing `microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example/hello_world.py` & `microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example/hello_world.py`

 * *Files identical despite different names*

### Comparing `microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/PKG-INFO` & `microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microbeseq_nbdev_example
-Version: 0.0.4
+Version: 0.0.5
 Summary: TODO
 Home-page: https://github.com/$GIT_USER_NAME/microbeseq_nbdev_example
 Author: $GIT_USER_NAME
 Author-email: kimleeng@gmail.com
 License: MIT License
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microbeseq_nbdev_example-0.0.4/microbeseq_nbdev_example.egg-info/SOURCES.txt` & `microbeseq_nbdev_example-0.0.5/microbeseq_nbdev_example.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microbeseq_nbdev_example-0.0.4/settings.ini` & `microbeseq_nbdev_example-0.0.5/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = microbeseq_nbdev_example
 lib_name = microbeseq_nbdev_example
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = MIT
 black_formatting = 1
 doc_path = _docs
 lib_path = microbeseq_nbdev_example
 nbs_path = nbs
 recursive = True
@@ -22,15 +22,16 @@
 author_email = kimleeng@gmail.com
 copyright = 2024 onwards, $GIT_USER_NAME
 description = TODO
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = $GIT_USER_NAME
-requirements = fastcore python_dotenv envyaml pandas
+requirements = fastcore
+pip_requirements = python_dotenv envyaml pandas
 console_scripts = 
 	core_hello_world=microbeseq_nbdev_example.core:cli
 	hello_two_world=microbeseq_nbdev_example.hello_world:cli
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
```

### Comparing `microbeseq_nbdev_example-0.0.4/setup.py` & `microbeseq_nbdev_example-0.0.5/setup.py`

 * *Files identical despite different names*

