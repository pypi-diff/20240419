# Comparing `tmp/unidep-0.56.0.tar.gz` & `tmp/unidep-0.57.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidep-0.56.0.tar", last modified: Thu Apr  4 12:37:26 2024, max compression
+gzip compressed data, was "unidep-0.57.0.tar", last modified: Fri Apr 19 14:19:01 2024, max compression
```

## Comparing `unidep-0.56.0.tar` & `unidep-0.57.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:26.834399 unidep-0.56.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-04 12:37:16.000000 unidep-0.56.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    62612 2024-04-04 12:37:26.834399 unidep-0.56.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    60991 2024-04-04 12:37:16.000000 unidep-0.56.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-04 12:37:16.000000 unidep-0.56.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:37:26.834399 unidep-0.56.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:26.830399 unidep-0.56.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_conda_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    16223 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_parse_yaml_local_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    71403 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_unidep.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-04 12:37:16.000000 unidep-0.56.0/tests/test_version_conflicts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:26.830399 unidep-0.56.0/unidep/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    42572 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    20304 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_conda_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    13056 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    22028 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_dependencies_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_hatch_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_pytest_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6917 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_setuptools_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/platform_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-04-04 12:37:16.000000 unidep-0.56.0/unidep/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:37:26.834399 unidep-0.56.0/unidep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    62612 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 12:37:26.000000 unidep-0.56.0/unidep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.013119 unidep-0.57.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-19 14:18:47.000000 unidep-0.57.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    62612 2024-04-19 14:19:01.013119 unidep-0.57.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    60991 2024-04-19 14:18:47.000000 unidep-0.57.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-19 14:18:47.000000 unidep-0.57.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:19:01.013119 unidep-0.57.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.005119 unidep-0.57.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19103 2024-04-19 14:18:47.000000 unidep-0.57.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-04-19 14:18:47.000000 unidep-0.57.0/tests/test_conda_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16223 2024-04-19 14:18:47.000000 unidep-0.57.0/tests/test_parse_yaml_local_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71403 2024-04-19 14:18:47.000000 unidep-0.57.0/tests/test_unidep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-19 14:18:47.000000 unidep-0.57.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-19 14:18:47.000000 unidep-0.57.0/tests/test_version_conflicts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.009119 unidep-0.57.0/unidep/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45835 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/_conda_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20304 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/_conda_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13056 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21927 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/_dependencies_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/_hatch_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/_pytest_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6917 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/_setuptools_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/platform_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-04-19 14:18:47.000000 unidep-0.57.0/unidep/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.009119 unidep-0.57.0/unidep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    62612 2024-04-19 14:19:00.000000 unidep-0.57.0/unidep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-19 14:19:01.000000 unidep-0.57.0/unidep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:19:00.000000 unidep-0.57.0/unidep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 14:19:00.000000 unidep-0.57.0/unidep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 14:19:00.000000 unidep-0.57.0/unidep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 14:19:00.000000 unidep-0.57.0/unidep.egg-info/top_level.txt
```

### Comparing `unidep-0.56.0/LICENSE` & `unidep-0.57.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/PKG-INFO` & `unidep-0.57.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidep
-Version: 0.56.0
+Version: 0.57.0
 Summary: Unified Conda and Pip requirements management.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/unidep
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
```

### Comparing `unidep-0.56.0/README.md` & `unidep-0.57.0/README.md`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/pyproject.toml` & `unidep-0.57.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 max-complexity = 18
 
 [tool.mypy]
 python_version = "3.7"
 
 # Use bump-my-version, e.g., call `bump-my-version bump minor`
 [tool.bumpversion]
-current_version = "0.56.0"
+current_version = "0.57.0"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "v{new_version}"
 
 [[tool.bumpversion.files]]
 filename = "unidep/_version.py"
```

### Comparing `unidep-0.56.0/tests/test_conda_lock.py` & `unidep-0.57.0/tests/test_conda_lock.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/tests/test_parse_yaml_local_dependencies.py` & `unidep-0.57.0/tests/test_parse_yaml_local_dependencies.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/tests/test_unidep.py` & `unidep-0.57.0/tests/test_unidep.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/tests/test_utils.py` & `unidep-0.57.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/tests/test_version_conflicts.py` & `unidep-0.57.0/tests/test_version_conflicts.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep/__init__.py` & `unidep-0.57.0/unidep/__init__.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep/_cli.py` & `unidep-0.57.0/unidep/_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 from __future__ import annotations
 
 import argparse
 import functools
 import importlib.util
+import itertools
 import json
 import os
 import platform
 import shutil
 import subprocess
 import sys
 from pathlib import Path
@@ -59,14 +60,15 @@
             if action.help is not None:
                 return action.help.replace("[", r"\[")
             return None
 except ImportError:  # pragma: no cover
     from argparse import HelpFormatter as _HelpFormatter  # type: ignore[assignment]
 
 _DEP_FILES = "`requirements.yaml` or `pyproject.toml`"
+CondaExecutable = Literal["conda", "mamba", "micromamba"]
 
 
 def _add_common_args(  # noqa: PLR0912, C901
     sub_parser: argparse.ArgumentParser,
     options: set[str],
 ) -> None:  # pragma: no cover
     if "directory" in options:
@@ -586,15 +588,15 @@
         else:
             files[i] = path_with_extras.path_with_extras
     if missing:
         print(f"❌ One or more files ({', '.join(missing)}) not found.")
         sys.exit(1)
 
 
-def _identify_conda_executable() -> str:  # pragma: no cover
+def _identify_conda_executable() -> CondaExecutable:  # pragma: no cover
     """Identify the conda executable to use.
 
     This function checks for micromamba, mamba, and conda in that order.
     """
     if shutil.which("micromamba"):
         return "micromamba"
     if shutil.which("mamba"):
@@ -608,22 +610,98 @@
 def _format_inline_conda_package(package: str) -> str:
     pkg = parse_package_str(package)
     if pkg.pin is None:
         return pkg.name
     return f'{pkg.name}"{pkg.pin.strip()}"'
 
 
-def _maybe_exe(conda_executable: str) -> str:
+def _maybe_exe(conda_executable: CondaExecutable) -> str:
     """Add .exe on Windows."""
     if os.name == "nt":  # pragma: no cover
-        return f"{conda_executable}.exe"
+        if conda_executable in ("micromamba", "mamba") and os.environ.get("MAMBA_EXE"):
+            return os.environ["MAMBA_EXE"]
+        if os.environ.get("CONDA_EXE"):
+            return os.environ["CONDA_EXE"]
+
+        executables = [f"{conda_executable}.exe", conda_executable]
+        for exe in executables:
+            path = shutil.which(exe)
+            if path is not None:
+                return path
+
+        print(
+            "🔍 Going to search in different common paths"
+            f" because `{conda_executable}` was not found in PATH.",
+        )
+        return _find_windows_path(conda_executable)
     return conda_executable
 
 
-def _conda_cli_command_json(conda_executable: str, *args: str) -> dict[str, list[str]]:
+def _capitalize_dir(path: str, *, capitalize: bool = True, index: int = -1) -> str:
+    """Capitalize or lowercase a directory in a path, on Windows only."""
+    sep = "\\"
+    parts = path.split(sep)
+    if capitalize:
+        parts[index] = parts[index].capitalize()
+    else:
+        parts[index] = parts[index].lower()
+    return sep.join(parts)
+
+
+@functools.lru_cache(1)
+def _find_windows_path(conda_executable: CondaExecutable) -> str:
+    """Find the path to the conda executable on Windows."""
+    searched = []
+    conda_roots = [
+        r"%USERPROFILE%\Anaconda3",  # https://stackoverflow.com/a/58211115
+        r"%USERPROFILE%\Miniconda3",  # https://stackoverflow.com/a/76545804
+        r"C:\Anaconda3",  # https://stackoverflow.com/a/44597801
+        r"C:\Miniconda3",  # https://stackoverflow.com/a/53685910
+        r"C:\ProgramData\Anaconda3",  # https://stackoverflow.com/a/58211115
+        r"C:\ProgramData\Miniconda3",  # https://stackoverflow.com/a/51003321
+    ]
+    if conda_executable == "mamba":
+        conda_roots = [
+            r"C:\ProgramData\mambaforge",  # https://github.com/mamba-org/mamba/issues/1756#issuecomment-1517284831
+            r"%USERPROFILE%\AppData\Local\mambaforge",  # https://stackoverflow.com/a/75612393
+            # First try native mamba locations, then Conda locations (in
+            # case `conda install mamba` was used)
+            *conda_roots,
+        ]
+    if conda_executable == "micromamba":
+        conda_roots = [
+            # Default installation directory based on the installation script
+            # https://raw.githubusercontent.com/mamba-org/micromamba-releases/main/install.ps1
+            r"%LOCALAPPDATA%\micromamba",
+        ]
+
+    extensions = (".exe", "", ".bat")
+    subs = ("condabin\\", "Scripts\\", "")  # The "" is for micromamba
+    for root, sub, ext, cap in itertools.product(
+        conda_roots,
+        subs,
+        extensions,
+        (True, False),
+    ):
+        # @sbalk reported that his `anaconda3` folder is lowercase
+        path = rf"{_capitalize_dir(root, capitalize=cap)}\{sub}{conda_executable}{ext}"
+        path = os.path.expandvars(path)
+        searched.append(path)
+        if os.path.exists(path):  # noqa: PTH110
+            return path
+    msg = f"Could not find {conda_executable}."
+    searched_str = "\n👉 ".join(searched)
+    msg = f"Could not find {conda_executable}. Searched in:\n👉 {searched_str}"
+    raise FileNotFoundError(msg)
+
+
+def _conda_cli_command_json(
+    conda_executable: CondaExecutable,
+    *args: str,
+) -> dict[str, list[str]]:
     """Run a conda command and return the JSON output."""
     try:
         result = subprocess.run(
             [_maybe_exe(conda_executable), *args, "--json"],  # noqa: S603
             capture_output=True,
             text=True,
             check=True,
@@ -634,52 +712,54 @@
         raise
     except json.JSONDecodeError as e:  # pragma: no cover
         print(f"Failed to parse JSON: {e}")
         raise
 
 
 @functools.lru_cache(maxsize=None)
-def _conda_env_list(conda_executable: str) -> list[str]:
+def _conda_env_list(conda_executable: CondaExecutable) -> list[str]:
     """Get a list of conda environments."""
     return _conda_cli_command_json(conda_executable, "env", "list")["envs"]
 
 
 @functools.lru_cache(maxsize=None)
-def _conda_info(conda_executable: str) -> dict:
+def _conda_info(conda_executable: CondaExecutable) -> dict:
     return _conda_cli_command_json(conda_executable, "info")
 
 
-def _conda_root_prefix(conda_executable: str) -> Path:  # pragma: no cover
+def _conda_root_prefix(conda_executable: CondaExecutable) -> Path:  # pragma: no cover
     """Get the root prefix of the conda installation."""
     if os.environ.get("MAMBA_ROOT_PREFIX"):
         return Path(os.environ["MAMBA_ROOT_PREFIX"])
     if os.environ.get("CONDA_ROOT"):
         return Path(os.environ["CONDA_ROOT"])
     info_dict = _conda_info(conda_executable)
     if conda_executable in ("conda", "mamba"):
         prefix = info_dict.get("root_prefix") or info_dict["conda_prefix"]
     else:
         assert conda_executable == "micromamba"
         prefix = info_dict["base environment"]
     return Path(prefix)
 
 
-def _conda_env_dirs(conda_executable: str) -> list[Path]:  # pragma: no cover
+def _conda_env_dirs(
+    conda_executable: CondaExecutable,
+) -> list[Path]:  # pragma: no cover
     """Get a list of conda environment directories."""
     info_dict = _conda_info(conda_executable)
     if conda_executable in ("conda", "mamba"):
         envs_dirs = info_dict["envs_dirs"]
     else:
         assert conda_executable == "micromamba"
         envs_dirs = info_dict["envs directories"]
     return [Path(d) for d in envs_dirs]
 
 
 def _conda_env_name_to_prefix(
-    conda_executable: str,
+    conda_executable: CondaExecutable,
     conda_env_name: str,
 ) -> Path:  # pragma: no cover
     """Get the prefix of a conda environment."""
     # Based on `conda.base.context.locate_prefix_by_name`
     # https://github.com/conda/conda/blob/72fe69dac8b2fef351c511c813493fef17f295e1/conda/base/context.py#L1976-L1977
     root_prefix = _conda_root_prefix(conda_executable)
     if conda_env_name in ("base", "root"):
@@ -696,15 +776,15 @@
         f"Could not find conda prefix with name `{conda_env_name}`."
         f" Available prefixes:\n👉 {envs_str}"
     )
     raise ValueError(msg)
 
 
 def _python_executable(
-    conda_executable: str,
+    conda_executable: CondaExecutable,
     conda_env_name: str | None,
     conda_env_prefix: Path | None,
 ) -> str:
     """Get the Python executable to use for a conda environment."""
     if conda_env_name is None and conda_env_prefix is None:
         return sys.executable
     if conda_env_name:
@@ -742,15 +822,15 @@
     print(f"📦 Installing project with `{' '.join(pip_command)}`\n")
     if not dry_run:
         subprocess.run(pip_command, check=True)  # noqa: S603
 
 
 def _install_command(  # noqa: PLR0912
     *files: Path,
-    conda_executable: str,
+    conda_executable: CondaExecutable,
     conda_env_name: str | None,
     conda_env_prefix: Path | None,
     dry_run: bool,
     editable: bool,
     skip_local: bool = False,
     skip_pip: bool = False,
     skip_conda: bool = False,
@@ -863,15 +943,15 @@
 
     if not dry_run:  # pragma: no cover
         print("✅ All dependencies installed successfully.")
 
 
 def _install_all_command(
     *,
-    conda_executable: str,
+    conda_executable: CondaExecutable,
     conda_env_name: str | None,
     conda_env_prefix: Path | None,
     dry_run: bool,
     editable: bool,
     depth: int,
     directory: Path,
     skip_local: bool = False,
```

### Comparing `unidep-0.56.0/unidep/_conda_env.py` & `unidep-0.57.0/unidep/_conda_env.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep/_conda_lock.py` & `unidep-0.57.0/unidep/_conda_lock.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep/_conflicts.py` & `unidep-0.57.0/unidep/_conflicts.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep/_dependencies_parsing.py` & `unidep-0.57.0/unidep/_dependencies_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,18 +479,14 @@
     return identifier
 
 
 # Alias for backwards compatibility
 parse_yaml_requirements = parse_requirements
 
 
-def _is_same_path(path1: Path, path2: Path) -> bool:
-    return path1.resolve() == path2.resolve()
-
-
 def _extract_local_dependencies(
     path: Path,
     base_path: Path,
     processed: set[Path],
     dependencies: dict[str, set[str]],
     *,
     check_pip_installable: bool = True,
```

### Comparing `unidep-0.56.0/unidep/_hatch_integration.py` & `unidep-0.57.0/unidep/_hatch_integration.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep/_pytest_plugin.py` & `unidep-0.57.0/unidep/_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep/_setuptools_integration.py` & `unidep-0.57.0/unidep/_setuptools_integration.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep/platform_definitions.py` & `unidep-0.57.0/unidep/platform_definitions.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep/utils.py` & `unidep-0.57.0/unidep/utils.py`

 * *Files identical despite different names*

### Comparing `unidep-0.56.0/unidep.egg-info/PKG-INFO` & `unidep-0.57.0/unidep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidep
-Version: 0.56.0
+Version: 0.57.0
 Summary: Unified Conda and Pip requirements management.
 Author-email: Bas Nijholt <bas@nijho.lt>
 Project-URL: Homepage, https://github.com/basnijholt/unidep
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
```

### Comparing `unidep-0.56.0/unidep.egg-info/SOURCES.txt` & `unidep-0.57.0/unidep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

