# Comparing `tmp/pop_cli-4.1.0.tar.gz` & `tmp/pop_cli-4.2.0.tar.gz`

## Comparing `pop_cli-4.1.0.tar` & `pop_cli-4.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-4.1.0/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 pop_cli-4.1.0/src/__main__.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pop_cli-4.1.0/src/config.yaml
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 pop_cli-4.1.0/src/hub/cli.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-4.1.0/src/hub/config.py
--rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 pop_cli-4.1.0/src/hub/console.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 pop_cli-4.1.0/src/hub/init.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pop_cli-4.1.0/src/hub/ref.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-4.1.0/src/hub/state.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/integration/test_init.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/integration/test_ref.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-4.1.0/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-4.1.0/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-4.1.0/README.rst
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pop_cli-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-4.2.0/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 pop_cli-4.2.0/src/__main__.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pop_cli-4.2.0/src/config.yaml
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 pop_cli-4.2.0/src/hub/cli.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-4.2.0/src/hub/config.py
+-rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 pop_cli-4.2.0/src/hub/console.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pop_cli-4.2.0/src/hub/init.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pop_cli-4.2.0/src/hub/ref.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-4.2.0/src/hub/state.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-4.2.0/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-4.2.0/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-4.2.0/README.rst
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pop_cli-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-4.2.0/PKG-INFO
```

### Comparing `pop_cli-4.1.0/.pre-commit-config.yaml` & `pop_cli-4.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/src/__main__.py` & `pop_cli-4.2.0/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/src/config.yaml` & `pop_cli-4.2.0/src/config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/src/hub/cli.py` & `pop_cli-4.2.0/src/hub/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/src/hub/config.py` & `pop_cli-4.2.0/src/hub/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/src/hub/console.py` & `pop_cli-4.2.0/src/hub/console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/src/hub/init.py` & `pop_cli-4.2.0/src/hub/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     # If no cli was defined, then use the first part of the passed ref as the authoritative cli
     cli = opt.cli.cli or ref.split(".")[0]
     await hub.log.debug(f"Using cli: {cli}")
 
     # Try to restore the hub state
     hub_state_file = await hub.cli.state.restore(opt)
 
-    if opt.cli.cli or (
-        (cli in hub._dynamic.config.cli_config) and (cli not in opt.get("pop", {}).get("global_clis", ()))
+    if (opt.cli.cli != cli) and (
+        opt.cli.cli
+        or ((cli in hub._dynamic.config.cli_config) and (cli not in opt.get("pop", {}).get("global_clis", ())))
     ):
         await hub.log.debug(f"Loading cli: {cli}")
         # Reload hub.OPT with the cli arguments not consumed by the initial hub
         await hub.cli.config.override(cli, opt)
         args = []
         kwargs = {}
     else:
```

### Comparing `pop_cli-4.1.0/src/hub/ref.py` & `pop_cli-4.2.0/src/hub/ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/src/hub/state.py` & `pop_cli-4.2.0/src/hub/state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/tests/conftest.py` & `pop_cli-4.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/tests/integration/test_cli.py` & `pop_cli-4.2.0/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/tests/integration/test_config.py` & `pop_cli-4.2.0/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/tests/integration/test_console.py` & `pop_cli-4.2.0/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/tests/integration/test_init.py` & `pop_cli-4.2.0/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/tests/integration/test_ref.py` & `pop_cli-4.2.0/tests/integration/test_ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/tests/integration/test_state.py` & `pop_cli-4.2.0/tests/integration/test_state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/.gitignore` & `pop_cli-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/README.rst` & `pop_cli-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-4.1.0/pyproject.toml` & `pop_cli-4.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "4.1.0"
+version = "4.2.0"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `pop_cli-4.1.0/PKG-INFO` & `pop_cli-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 4.1.0
+Version: 4.2.0
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

