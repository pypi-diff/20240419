# Comparing `tmp/cookieplone-0.3.0.tar.gz` & `tmp/cookieplone-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookieplone-0.3.0.tar", max compression
+gzip compressed data, was "cookieplone-0.4.0.tar", max compression
```

## Comparing `cookieplone-0.3.0.tar` & `cookieplone-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1142 2024-04-19 01:23:35.441045 cookieplone-0.3.0/README.md
--rw-r--r--   0        0        0       22 2024-04-19 01:27:14.538901 cookieplone-0.3.0/cookieplone/__init__.py
--rw-r--r--   0        0        0      191 2024-04-16 22:18:14.202809 cookieplone-0.3.0/cookieplone/__main__.py
--rw-r--r--   0        0        0     5546 2024-04-19 00:05:39.265993 cookieplone-0.3.0/cookieplone/cli.py
--rw-r--r--   0        0        0     1203 2024-04-17 19:41:55.848797 cookieplone-0.3.0/cookieplone/data.py
--rw-r--r--   0        0        0      452 2024-04-18 19:29:44.648761 cookieplone-0.3.0/cookieplone/exceptions.py
--rw-r--r--   0        0        0     2401 2024-04-18 17:59:28.841529 cookieplone-0.3.0/cookieplone/filters/__init__.py
--rw-r--r--   0        0        0     3522 2024-04-18 23:56:24.228008 cookieplone-0.3.0/cookieplone/generator.py
--rw-r--r--   0        0        0     1347 2024-04-18 23:57:11.861636 cookieplone-0.3.0/cookieplone/repository.py
--rw-r--r--   0        0        0      394 2024-04-18 19:18:47.072810 cookieplone-0.3.0/cookieplone/settings.py
--rw-r--r--   0        0        0       60 2024-04-17 16:17:54.105869 cookieplone-0.3.0/cookieplone/utils/__init__.py
--rw-r--r--   0        0        0     2696 2024-04-18 17:54:31.026810 cookieplone-0.3.0/cookieplone/utils/commands/__init__.py
--rw-r--r--   0        0        0     3710 2024-04-19 00:07:35.659983 cookieplone-0.3.0/cookieplone/utils/console.py
--rw-r--r--   0        0        0      243 2024-04-18 17:23:34.273811 cookieplone-0.3.0/cookieplone/utils/containers.py
--rw-r--r--   0        0        0      486 2024-04-18 22:26:25.935421 cookieplone-0.3.0/cookieplone/utils/files.py
--rw-r--r--   0        0        0      887 2024-04-16 23:39:28.137531 cookieplone-0.3.0/cookieplone/utils/sanity.py
--rw-r--r--   0        0        0     4516 2024-04-18 22:47:44.003042 cookieplone-0.3.0/cookieplone/utils/validators.py
--rw-r--r--   0        0        0     2780 2024-04-18 17:23:34.273620 cookieplone-0.3.0/cookieplone/utils/versions.py
--rw-r--r--   0        0        0     2196 2024-04-19 01:26:29.201409 cookieplone-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 cookieplone-0.3.0/setup.py
--rw-r--r--   0        0        0     2568 1970-01-01 00:00:00.000000 cookieplone-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1142 2024-04-19 01:23:35.441045 cookieplone-0.4.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-19 16:43:53.053792 cookieplone-0.4.0/cookieplone/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-16 22:18:14.202809 cookieplone-0.4.0/cookieplone/__main__.py
+-rw-r--r--   0        0        0     5548 2024-04-19 16:42:39.978057 cookieplone-0.4.0/cookieplone/cli.py
+-rw-r--r--   0        0        0     1203 2024-04-17 19:41:55.848797 cookieplone-0.4.0/cookieplone/data.py
+-rw-r--r--   0        0        0      452 2024-04-18 19:29:44.648761 cookieplone-0.4.0/cookieplone/exceptions.py
+-rw-r--r--   0        0        0     2401 2024-04-18 17:59:28.841529 cookieplone-0.4.0/cookieplone/filters/__init__.py
+-rw-r--r--   0        0        0     4160 2024-04-19 16:43:08.774062 cookieplone-0.4.0/cookieplone/generator.py
+-rw-r--r--   0        0        0     1347 2024-04-18 23:57:11.861636 cookieplone-0.4.0/cookieplone/repository.py
+-rw-r--r--   0        0        0      394 2024-04-18 19:18:47.072810 cookieplone-0.4.0/cookieplone/settings.py
+-rw-r--r--   0        0        0       60 2024-04-17 16:17:54.105869 cookieplone-0.4.0/cookieplone/utils/__init__.py
+-rw-r--r--   0        0        0     2696 2024-04-18 17:54:31.026810 cookieplone-0.4.0/cookieplone/utils/commands/__init__.py
+-rw-r--r--   0        0        0     3710 2024-04-19 00:07:35.659983 cookieplone-0.4.0/cookieplone/utils/console.py
+-rw-r--r--   0        0        0      243 2024-04-18 17:23:34.273811 cookieplone-0.4.0/cookieplone/utils/containers.py
+-rw-r--r--   0        0        0      486 2024-04-18 22:26:25.935421 cookieplone-0.4.0/cookieplone/utils/files.py
+-rw-r--r--   0        0        0      887 2024-04-16 23:39:28.137531 cookieplone-0.4.0/cookieplone/utils/sanity.py
+-rw-r--r--   0        0        0     4516 2024-04-18 22:47:44.003042 cookieplone-0.4.0/cookieplone/utils/validators.py
+-rw-r--r--   0        0        0     2780 2024-04-18 17:23:34.273620 cookieplone-0.4.0/cookieplone/utils/versions.py
+-rw-r--r--   0        0        0     2196 2024-04-19 01:26:29.201409 cookieplone-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 cookieplone-0.4.0/setup.py
+-rw-r--r--   0        0        0     2568 1970-01-01 00:00:00.000000 cookieplone-0.4.0/PKG-INFO
```

### Comparing `cookieplone-0.3.0/README.md` & `cookieplone-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/cookieplone/cli.py` & `cookieplone-0.4.0/cookieplone/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
 def prompt_for_template(base_path: Path) -> str:
     """Parse cookiecutter.json in base_path and prompt user to choose."""
     templates = get_template_options(base_path)
     choices = {i[0]: i[1] for i in templates}
     console.welcome_screen(templates)
-    answer = Prompt.ask("Select a template", choices=list(choices.keys()), default=1)
+    answer = Prompt.ask("Select a template", choices=list(choices.keys()), default="1")
     return choices[answer]
 
 
 def version_info() -> str:
     """Return the Cookieplone version, location and Python powering it."""
     python_version = sys.version
     location = Path(__file__).parent
```

### Comparing `cookieplone-0.3.0/cookieplone/data.py` & `cookieplone-0.4.0/cookieplone/data.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/cookieplone/filters/__init__.py` & `cookieplone-0.4.0/cookieplone/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/cookieplone/generator.py` & `cookieplone-0.4.0/cookieplone/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 import json
 from collections import OrderedDict
 from pathlib import Path
 
-import typer
 from cookiecutter import exceptions as exc
 from cookiecutter.main import cookiecutter
 
 from cookieplone.exceptions import GeneratorException
 from cookieplone.utils import console, files
 
+REMOVE_FILES = [".github"]
+
 
 def _remove_internal_keys(context: OrderedDict) -> dict:
     """Remove internal and computed keys."""
     new_context = {
         key: value for key, value in context.items() if not key.startswith("_")
     }
     return new_context
 
 
+def _get_repository_root(context: OrderedDict, template: str) -> Path:
+    """Return the templates root."""
+    repository = context.get("_checkout") or context.get("_template")
+    if not repository:
+        raise exc.RepositoryNotFound()
+    repository = Path(repository).resolve()
+    if not repository:
+        raise exc.RepositoryNotFound()
+    elif not (repository / template).exists():
+        # We are probably inside a template folder,
+        # try to check the parent
+        repository = repository.parent
+        if not (repository / template).exists():
+            raise exc.RepositoryNotFound()
+    return repository
+
+
 def generate(
     repository,
     tag,
     no_input,
     extra_context,
     replay,
     overwrite_if_exists,
@@ -31,15 +49,15 @@
     passwd,
     template,
     skip_if_file_exists,
     keep_project_on_failure,
 ) -> Path:
     try:
         result = cookiecutter(
-            repository,
+            f"{repository}",  # cookiecutter expects this to be a string
             tag,
             no_input,
             extra_context=extra_context,
             replay=replay,
             overwrite_if_exists=overwrite_if_exists,
             output_dir=output_dir,
             config_file=config_file,
@@ -69,30 +87,31 @@
         """
         raise GeneratorException(message=msg, original=undefined_err)  # noQA:B904
     else:
         return Path(result)
 
 
 def generate_subtemplate(
-    template: str, output_dir: Path, folder_name: str, context: OrderedDict
+    template: str,
+    output_dir: Path,
+    folder_name: str,
+    context: OrderedDict,
+    remove_files: list[str] | None = None,
 ) -> Path:
     # Extract path to repository
-    repository = context.get("_checkout") or context.get("_template")
-
-    if not repository or not (Path(repository) / template).exists():
-        # TODO: Error message
-        raise typer.Exit(code=1)
+    repository = _get_repository_root(context, template)
     # Cleanup context
     extra_context = _remove_internal_keys(context)
     ## Add folder name again
     extra_context["__folder_name"] = folder_name
-    ## Disable GHA for subcomponent
-    extra_context["__gha_enable"] = False
     # Enable quiet mode
     console.enable_quiet_mode()
+    # Files to be removed
+    if remove_files is None:
+        remove_files = REMOVE_FILES
     # Call generate
     try:
         result = generate(
             repository,
             None,  # We should have the tag already locally
             True,  # No input
             extra_context,
@@ -108,11 +127,11 @@
         )
     except GeneratorException as exc:
         console.disable_quiet_mode()
         raise exc
     else:
         console.disable_quiet_mode()
         path = Path(result)
-        # Remove GHA folder
-        files.remove_gha(path)
+        if remove_files:
+            files.remove_files(path, remove_files)
         # Return path
         return path
```

### Comparing `cookieplone-0.3.0/cookieplone/repository.py` & `cookieplone-0.4.0/cookieplone/repository.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/cookieplone/utils/commands/__init__.py` & `cookieplone-0.4.0/cookieplone/utils/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/cookieplone/utils/console.py` & `cookieplone-0.4.0/cookieplone/utils/console.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/cookieplone/utils/sanity.py` & `cookieplone-0.4.0/cookieplone/utils/sanity.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/cookieplone/utils/validators.py` & `cookieplone-0.4.0/cookieplone/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/cookieplone/utils/versions.py` & `cookieplone-0.4.0/cookieplone/utils/versions.py`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/pyproject.toml` & `cookieplone-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cookieplone-0.3.0/setup.py` & `cookieplone-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'typer[all]>=0.12.3,<0.13.0']
 
 entry_points = \
 {'console_scripts': ['cookieplone = cookieplone.__main__:main']}
 
 setup_kwargs = {
     'name': 'cookieplone',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Create Plone projects, addons, documentation with ease!',
     'long_description': '<p align="center">\n    <img alt="Plone Logo" width="200px" src="https://raw.githubusercontent.com/plone/.github/main/plone-logo.png">\n</p>\n\n<h1 align="center">\n  cookieplone\n</h1>\n\n\n<div align="center">\n\n[![PyPI](https://img.shields.io/pypi/v/cookieplone)](https://pypi.org/project/cookieplone/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cookieplone)](https://pypi.org/project/cookieplone/)\n[![PyPI - Wheel](https://img.shields.io/pypi/wheel/cookieplone)](https://pypi.org/project/cookieplone/)\n[![PyPI - License](https://img.shields.io/pypi/l/cookieplone)](https://pypi.org/project/cookieplone/)\n[![PyPI - Status](https://img.shields.io/pypi/status/cookieplone)](https://pypi.org/project/cookieplone/)\n\n\n[![Tests](https://github.com/plone/cookieplone/actions/workflows/main.yml/badge.svg)](https://github.com/plone/cookieplone/actions/workflows/main.yml)\n\n[![GitHub contributors](https://img.shields.io/github/contributors/plone/cookieplone)](https://github.com/plone/cookieplone)\n[![GitHub Repo stars](https://img.shields.io/github/stars/plone/cookieplone?style=social)](https://github.com/plone/cookieplone)\n\n</div>\n',
     'author': 'Plone Community',
     'author_email': 'dev@plone.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/plone/cookieplone',
```

### Comparing `cookieplone-0.3.0/PKG-INFO` & `cookieplone-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookieplone
-Version: 0.3.0
+Version: 0.4.0
 Summary: Create Plone projects, addons, documentation with ease!
 Home-page: https://github.com/plone/cookieplone
 Author: Plone Community
 Author-email: dev@plone.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

