# Comparing `tmp/nested_config-2.0.3.post0.tar.gz` & `tmp/nested_config-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nested_config-2.0.3.post0.tar", max compression
+gzip compressed data, was "nested_config-2.1.0.tar", max compression
```

## Comparing `nested_config-2.0.3.post0.tar` & `nested_config-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,12 @@
--rw-r--r--   0        0        0     2113 2024-04-15 21:39:00.350241 nested_config-2.0.3.post0/CHANGELOG.md
--rw-r--r--   0        0        0     1097 2024-04-15 20:59:09.993709 nested_config-2.0.3.post0/LICENSE
--rw-r--r--   0        0        0     5660 2024-04-15 21:52:31.943871 nested_config-2.0.3.post0/README.md
--rw-r--r--   0        0        0     1650 2024-04-15 21:53:00.415928 nested_config-2.0.3.post0/pyproject.toml
--rw-r--r--   0        0        0     1112 2024-04-09 18:47:44.042630 nested_config-2.0.3.post0/src/nested_config/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-12 23:58:03.989077 nested_config-2.0.3.post0/src/nested_config/_compat.py
--rw-r--r--   0        0        0      762 2024-04-04 20:38:25.984470 nested_config-2.0.3.post0/src/nested_config/_types.py
--rw-r--r--   0        0        0     1423 2024-04-12 22:01:56.593748 nested_config-2.0.3.post0/src/nested_config/_validators.py
--rw-r--r--   0        0        0     1870 2024-04-09 18:46:53.558529 nested_config-2.0.3.post0/src/nested_config/base_model.py
--rw-r--r--   0        0        0      326 2024-04-08 16:13:11.863062 nested_config-2.0.3.post0/src/nested_config/json.py
--rw-r--r--   0        0        0     3116 2024-04-10 16:36:48.265421 nested_config-2.0.3.post0/src/nested_config/loaders.py
--rw-r--r--   0        0        0     5888 2024-04-12 23:42:37.854933 nested_config-2.0.3.post0/src/nested_config/parsing.py
--rw-r--r--   0        0        0      268 2024-04-04 20:38:25.984470 nested_config-2.0.3.post0/src/nested_config/version.py
--rw-r--r--   0        0        0     6916 1970-01-01 00:00:00.000000 nested_config-2.0.3.post0/setup.py
--rw-r--r--   0        0        0     7233 1970-01-01 00:00:00.000000 nested_config-2.0.3.post0/PKG-INFO
+-rw-r--r--   0        0        0     3146 2024-04-18 21:02:18.859923 nested_config-2.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1097 2024-04-15 20:59:09.993709 nested_config-2.1.0/LICENSE
+-rw-r--r--   0        0        0     9665 2024-04-18 23:04:04.222666 nested_config-2.1.0/README.md
+-rw-r--r--   0        0        0     1856 2024-04-18 19:39:03.493579 nested_config-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-04-18 18:00:20.433917 nested_config-2.1.0/src/nested_config/__init__.py
+-rw-r--r--   0        0        0     6199 2024-04-18 19:38:20.097488 nested_config-2.1.0/src/nested_config/_pydantic.py
+-rw-r--r--   0        0        0      457 2024-04-16 23:16:09.316884 nested_config-2.1.0/src/nested_config/_types.py
+-rw-r--r--   0        0        0     6291 2024-04-18 17:59:31.681832 nested_config-2.1.0/src/nested_config/expand.py
+-rw-r--r--   0        0        0     2969 2024-04-17 18:58:24.182981 nested_config-2.1.0/src/nested_config/loaders.py
+-rw-r--r--   0        0        0      268 2024-04-04 20:38:25.984470 nested_config-2.1.0/src/nested_config/version.py
+-rw-r--r--   0        0        0    11077 1970-01-01 00:00:00.000000 nested_config-2.1.0/setup.py
+-rw-r--r--   0        0        0    11351 1970-01-01 00:00:00.000000 nested_config-2.1.0/PKG-INFO
```

### Comparing `nested_config-2.0.3.post0/CHANGELOG.md` & `nested_config-2.1.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,37 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [2.1.0] - 2024-04-18
+
+### Added
+
+- `nested_config.expand_config` - Recursively read in any config file(s) into a dict based
+  on model class(es). This is now the primary functionality, superseeding
+  `validate_config`, which will be deprecated.
+
+### Changed
+
+- Pydantic is now an extra (optional) dependency, only needed to use the below [deprecated
+  syntax](#2.1.0-deprecated). All Pydantic stuff has been merged into a single module and
+  emits deprecation warnings when used.
+- Improved deb build and test scripts
+
+### Deprecated <a name="2.1.0-deprecated"></a>
+
+- Pydantic PurePath validator and JSON encoder -- Doesn't need to be part of this project
+  and not needed in Pydantic 2+
+- Pydantic validation integration -- This project started out as being specifically for
+  working with Pydantic models and was tightly integrated with Pydantic, but that is no
+  longer necessary. Use with Pydantic or attrs or whatever is better left to the user.
+
 ## [2.0.3] - 2024-04-15
 
 - Fix typing issue regression for Pydantic < 2.0 introduced in last release
 - Move package to `src` directory
 
 ## [2.0.2] - 2024-04-12
 
@@ -45,13 +68,14 @@
 ## [1.1.3] - 2021-07-30
 
 - Add README
 - Simplify PurePosixPath validator
 - Export `TomlParsingError` from rtoml for downstream exception handling (without needing to explicitly
   import rtoml).
 
-[Unreleased]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.0.3...master
+[Unreleased]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.1.0...master
+[2.1.0]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.0.3...v2.1.0
 [2.0.3]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.0.2...v2.0.3
 [2.0.2]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.0.1...v2.0.2
 [2.0.1]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.0.0...v2.0.1
 [2.0.0]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v1.1.3...v2.0.0
 [1.1.3]: https://gitlab.com/osu-nrsg/nested-config/-/tags/v1.1.3
```

### Comparing `nested_config-2.0.3.post0/LICENSE` & `nested_config-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nested_config-2.0.3.post0/pyproject.toml` & `nested_config-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nested-config"
-version = "2.0.3.post0"
+version = "2.1.0"
 description = """\
 Parse configuration files that include paths to other config files into Pydantic model\
  instances. Also support pathlib.PurePath on Pydantic 1.8+.\
 """
 authors = ["Randall Pittman <pittmara@oregonstate.edu>"]
 readme = "README.md"
 license = "MIT"
@@ -24,35 +24,42 @@
 include = ["CHANGELOG.md"]
 
 [tool.poetry.urls]
 Changes = "https://gitlab.com/osu-nrsg/nested-config/-/blob/master/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = ">=1.8,<3.0.0"
+pydantic = {version = ">=1.8,<3.0.0", optional = true}
 single-version = "^1.6.0"
 tomli = {version = "^2.0.0", python = "<3.11"}
 typing-extensions = "^4.6.0"
 pyyaml = {version = ">=5.1.0,<7.0.0", optional = true}
+setuptools = {version = "^69.5.1", python = ">=3.12"}
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^7.22.0"
 ruff = "^0.3.5"
 pytest = "^8.1.1"
 mypy = "^1.9.0"
 types-pyyaml = ">=5.1.0"
 
 [tool.poetry.extras]
 yaml = ["pyyaml"]
+pydantic = ["pydantic"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 90
 
 [tool.ruff.lint.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.pyright]
 defineConstant = { "PYDANTIC_1" = false }  # change to true for Pydantic <2.0
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    "ignore::DeprecationWarning:nested_config._pydantic"
+]
```

### Comparing `nested_config-2.0.3.post0/src/nested_config/loaders.py` & `nested_config-2.1.0/src/nested_config/loaders.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,21 @@
 if sys.version_info < (3, 11):
     from tomli import load as toml_load_fobj
 else:
     from tomllib import load as toml_load_fobj
 
 from nested_config._types import ConfigDict, ConfigDictLoader, PathLike
 
-YAML_INSTALLED = False
-with contextlib.suppress(ImportError):
-    import yaml  # type: ignore
-
-    YAML_INSTALLED = True
-
 
 class NoLoaderError(Exception):
-    def __init__(self, suffix: str):
-        super().__init__(f"There is no loader for file extension {suffix}")
+    def __init__(self, suffix: str, default_suffix: Optional[str]):
+        msg_tail = ""
+        if default_suffix:
+            msg_tail = f" nor a loader for default suffix {default_suffix}"
+        super().__init__(f"There is no loader for file extension {suffix}{msg_tail}.")
 
 
 class ConfigLoaderError(Exception):
     def __init__(self, config_path: Path) -> None:
         super().__init__(f"There was a problem loading config file {config_path}")
 
 
@@ -44,54 +41,41 @@
 
 config_dict_loaders: Dict[str, ConfigDictLoader] = {
     ".toml": toml_load,
     ".json": json_load,
 }
 """Mapping of config file extension to config file loader"""
 
-
-if YAML_INSTALLED:
+# Add YAML loader, if available
+with contextlib.suppress(ImportError):
+    import yaml
 
     def yaml_load(path: PathLike) -> ConfigDict:
         """Load a YAML config file (safely)"""
         with open(path, "r") as fobj:
             return yaml.safe_load(fobj)
 
     config_dict_loaders[".yaml"] = yaml_load
     config_dict_loaders[".yml"] = yaml_load
 
 
-def _get_loader(config_path: Path):
+def _get_loader(config_path: Path, default_suffix: Optional[str] = None):
     """Get the loader for the specified suffix, or a loader from default suffix"""
     try:
         try:
             return config_dict_loaders[config_path.suffix]
         except KeyError:
-            if default_loader := _get_default_loader():
-                return default_loader
+            if default_suffix:
+                return config_dict_loaders[default_suffix]
             raise
     except KeyError:
-        raise NoLoaderError(config_path.suffix) from None
-
-
-def _get_default_loader() -> Optional[ConfigDictLoader]:
-    try:
-        return config_dict_loaders["DEFAULT"]
-    except KeyError:
-        return None
-
-
-def set_default_loader(default_suffix: str):
-    try:
-        config_dict_loaders["DEFAULT"] = config_dict_loaders[default_suffix]
-    except KeyError:
-        raise NoLoaderError(default_suffix) from None
+        raise NoLoaderError(config_path.suffix, default_suffix) from None
 
 
-def load_config(config_path: Path) -> ConfigDict:
+def load_config(config_path: Path, default_suffix: Optional[str] = None) -> ConfigDict:
     """Select a loader based on the suffix (extension) of the config file and try to load
     the config using that loader. E.g. for .toml, use the TOML loader.
 
     Inputs
     ------
     config_path
         Path to the config file
@@ -104,12 +88,12 @@
     Raises
     ------
     NoLoaderError (via _get_loader)
         No loader could be found for the suffix (or default suffix, if provided)
     ConfigLoaderError
         There was an error running the loader (e.g. in tomllib or yaml or json)
     """
-    loader = _get_loader(config_path)
+    loader = _get_loader(config_path, default_suffix)
     try:
         return loader(config_path)
     except Exception as ex:
         raise ConfigLoaderError(config_path) from ex
```

### Comparing `nested_config-2.0.3.post0/src/nested_config/parsing.py` & `nested_config-2.1.0/src/nested_config/expand.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,146 +1,162 @@
 """parsing.py - Functions to parse config files (e.g. TOML) into Pydantic model instances,
 possibly with nested models specified by string paths."""
 
+import functools
+import inspect
 import typing
 from pathlib import Path
-from typing import Optional, Type
+from typing import Any, Dict, Optional
 
-import pydantic
-
-from nested_config import _compat
 from nested_config._types import (
     UNION_TYPES,
     ConfigDict,
     PathLike,
-    PydModelT,
-    ispydmodel,
 )
-from nested_config.loaders import load_config, set_default_loader
+from nested_config.loaders import load_config
 
 
-def validate_config(
+def expand_config(
     config_path: PathLike,
-    model: Type[PydModelT],
+    model: type,
     *,
     default_suffix: Optional[str] = None,
-) -> PydModelT:
-    """Load a config file into a Pydantic model. The config file may contain string paths
-    where nested models would be expected. These are preparsed into their respective
-    models.
-
-    If paths to nested models are relative, they are assumed to be relative to the path of
-    their parent config file.
-
-    Input
-    -----
-    config_path
-        A string or pathlib.Path to the config file to parse
+) -> ConfigDict:
+    expander = ConfigExpander(default_suffix=default_suffix)
+    return expander.expand(config_path, model)
+
+
+class ConfigExpansionError(RuntimeError):
+    pass
+
+
+@functools.lru_cache
+def get_model_annotations(model: type) -> Dict[str, Any]:
+    """Get the aggregated annotations of all members of a model"""
+    annotations: Dict[str, Any] = {}
+    for cls in inspect.getmro(model)[::-1]:
+        annotations.update(cls.__dict__.get("__annotations__", {}))
+    return annotations
+
+
+def get_modelfield_annotation(model: type, field_name: str):
+    """Try to get the field annotation for some type, e.g. a dataclass or Pydantic
     model
-        The Pydantic model to use for creating the config object
-    default_suffix
-        If there is no loader for the config file suffix (or the config file has no
-        suffix) try to load the config with the loader specified by this extension, e.g.
-        '.toml' or '.yml'
+
+    Inputs
+    ------
+    model
+        The template class from which we want field annotations.
+    field_name
+        Name of the field to get
+
     Returns
     -------
-    A Pydantic object of the type specified by the model input.
+    The type annotation of the chosen field
 
     Raises
     ------
-    NoLoaderError
-        No loader is available for the config file extension
-    ConfigLoaderError
-        There was a problem loading a config file with its loader
-    pydantic.ValidationError
-        The data fields or types in the file do not match the model.
-
+    ConfigExpansionError
+        There is no field of that name in the specified model
     """
-    if default_suffix:
-        set_default_loader(default_suffix)
-    # Input arg coercion
-    config_path = Path(config_path)
-    # Get the config dict and the model fields
-    config_dict = load_config(config_path)
-    # preparse the config (possibly loading nested configs)
-    config_dict = _preparse_config_dict(config_dict, model, config_path)
-    # Create and validate the config object
-    return _compat.parse_obj(model, config_dict)
-
-
-def _preparse_config_dict(
-    config_dict: ConfigDict, model: Type[pydantic.BaseModel], config_path: Path
-):
-    return {
-        key: _preparse_config_value(
-            value, _compat.get_modelfield_annotation(model, key), config_path
-        )
-        for key, value in config_dict.items()
-    }
-
-
-def _preparse_config_value(field_value, field_annotation, config_path: Path):
-    """Check if a model field contains a path to another model and parse it accordingly"""
-    # If the annotation is optional, get the enclosed annotation
-    field_annotation = _get_optional_ann(field_annotation)
-    # ###
-    # N cases:
-    # 1. Config value is not a string, list, or dict
-    # 2. Config value is a dict, model expects a model
-    # 3. Config value is a string, model expects a model
-    # 4. Config value is a list, model expects a list of some type
-    # 5. Config value is a dict, model expects a dict with values of a particular model
-    #    type
-    # 6. A string, list, or dict that doesn't match cases 2-5
-    # ###
 
-    # 1.
-    if not isinstance(field_value, (str, list, dict)):
-        return field_value
-    # 2.
-    if isinstance(field_value, dict) and ispydmodel(field_annotation, pydantic.BaseModel):
-        return _preparse_config_dict(field_value, field_annotation, config_path)
-    # 3.
-    if isinstance(field_value, str) and ispydmodel(field_annotation, pydantic.BaseModel):
-        return _parse_path_str_into_pydmodel(field_value, field_annotation, config_path)
-    # 4.
-    if isinstance(field_value, list) and (
-        listval_annotation := _get_list_value_ann(field_annotation)
-    ):
-        return [
-            _preparse_config_value(li, listval_annotation, config_path)
-            for li in field_value
-        ]
-    # 5.
-    if isinstance(field_value, dict) and (
-        dictval_annotation := _get_dict_value_ann(field_annotation)
+    try:
+        return get_model_annotations(model)[field_name]
+    except KeyError:
+        raise ConfigExpansionError(
+            f"Model type {model} does not have a field named {field_name}"
+        ) from None
+
+
+def is_model(val: Any) -> bool:
+    return hasattr(val, "__dict__") and "__annotations__" in val.__dict__
+
+
+class ConfigExpander:
+    def __init__(self, *, default_suffix: Optional[str] = None):
+        self.default_suffix = default_suffix
+
+    def expand(self, config_path: PathLike, model: type) -> ConfigDict:
+        config_path = Path(config_path)
+        config_dict = load_config(config_path, self.default_suffix)
+        return self._preparse_config_dict(config_dict, model, config_path)
+
+    def _preparse_config_dict(
+        self, config_dict: ConfigDict, model: type, config_path: Path
     ):
         return {
-            key: _preparse_config_value(value, dictval_annotation, config_path)
-            for key, value in field_value.items()
+            key: self._preparse_config_value(
+                value, get_modelfield_annotation(model, key), config_path
+            )
+            for key, value in config_dict.items()
         }
-    # 6.
-    return field_value
 
+    def _preparse_config_value(
+        self, field_value: str, field_annotation: Any, config_path: Path
+    ):
+        """Check if a model field contains a path to another model and parse it
+        accordingly"""
+        # If the annotation is optional, get the enclosed annotation
+        field_annotation = _get_optional_ann(field_annotation)
+        # ###
+        # N cases:
+        # 1. Config value is not a string, list, or dict
+        # 2. Config value is a dict, model expects a model
+        # 3. Config value is a string, model expects a model
+        # 4. Config value is a list, model expects a list of some type
+        # 5. Config value is a dict, model expects a dict with values of some type
+        # 6. A string, list, or dict that doesn't match cases 2-5
+        # ###
+
+        # 1.
+        if not isinstance(field_value, (str, list, dict)):
+            return field_value
+        # 2.
+        if isinstance(field_value, dict) and is_model(field_annotation):
+            return self._preparse_config_dict(field_value, field_annotation, config_path)
+        # 3.
+        if isinstance(field_value, str) and is_model(field_annotation):
+            return self._expand_path_str_into_model(
+                field_value, field_annotation, config_path
+            )
+        # 4.
+        if isinstance(field_value, list) and (
+            listval_annotation := _get_list_value_ann(field_annotation)
+        ):
+            return [
+                self._preparse_config_value(li, listval_annotation, config_path)
+                for li in field_value
+            ]
+        # 5.
+        if isinstance(field_value, dict) and (
+            dictval_annotation := _get_dict_value_ann(field_annotation)
+        ):
+            return {
+                key: self._preparse_config_value(value, dictval_annotation, config_path)
+                for key, value in field_value.items()
+            }
+        # 6.
+        return field_value
 
-def _parse_path_str_into_pydmodel(
-    path_str: str, model: Type[PydModelT], parent_path: Path
-) -> PydModelT:
-    """Convert a path string to a path (possibly relative to a parent config path) and
-    create an instance of a Pydantic model"""
-    path = Path(path_str)
-    if not path.is_absolute():
-        # Assume it's relative to the parent config path
-        path = parent_path.parent / path
-    if not path.is_file():
-        raise FileNotFoundError(
-            f"Config file '{parent_path}' contains a path to another config file"
-            f" '{path_str}' that could not be found."
-        )
-    return validate_config(path, model)
+    def _expand_path_str_into_model(
+        self, path_str: str, model: type, parent_path: Path
+    ) -> ConfigDict:
+        """Convert a path string to a path (possibly relative to a parent config path) and
+        use expand() to load that config file, possibly expanding further sub-config
+        files based on the model type."""
+        path = Path(path_str)
+        if not path.is_absolute():
+            # Assume it's relative to the parent config path
+            path = parent_path.parent / path
+        if not path.is_file():
+            raise FileNotFoundError(
+                f"Config file '{parent_path}' contains a path to another config file"
+                f" '{path_str}' that could not be found."
+            )
+        return self.expand(path, model)
 
 
 def _get_optional_ann(annotation):
     """Convert a possibly Optional annotation to its underlying annotation"""
     annotation_origin = typing.get_origin(annotation)
     annotation_args = typing.get_args(annotation)
     if annotation_origin in UNION_TYPES and annotation_args[1] is type(None):
```

### Comparing `nested_config-2.0.3.post0/PKG-INFO` & `nested_config-2.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,210 +1,254 @@
-Metadata-Version: 2.1
-Name: nested-config
-Version: 2.0.3.post0
-Summary: Parse configuration files that include paths to other config files into Pydantic modelinstances. Also support pathlib.PurePath on Pydantic 1.8+.
-Home-page: https://gitlab.com/osu-nrsg/nested-config
-License: MIT
-Keywords: pydantic,config,configuration files
-Author: Randall Pittman
-Author-email: pittmara@oregonstate.edu
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Pydantic
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: yaml
-Requires-Dist: pydantic (>=1.8,<3.0.0)
-Requires-Dist: pyyaml (>=5.1.0,<7.0.0) ; extra == "yaml"
-Requires-Dist: single-version (>=1.6.0,<2.0.0)
-Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version < "3.11"
-Requires-Dist: typing-extensions (>=4.6.0,<5.0.0)
-Project-URL: Changes, https://gitlab.com/osu-nrsg/nested-config/-/blob/master/CHANGELOG.md
-Project-URL: Repository, https://gitlab.com/osu-nrsg/nested-config
-Description-Content-Type: text/markdown
-
-# nested-config README
-
-**nested-config** provides for parsing configuration files that include paths to other
-config files into [Pydantic](https://github.com/samuelcolvin/pydantic/) model instances.
-It also supports validating and JSON-encoding `pathlib.PurePath` on Pydantic 1.8+.
-
-## Usage
-
-### Config loading
-
-**nested-config** may be used in your project in two main ways.
-
-1. You may simply call `nested_config.validate_config()` with a config file path and a
-   Pydantic model which may or may not include nested Pydantic models. If there are nested
-   models and the config file has string values for those fields, those values are
-   interpreted as paths to other config files and those are recursively read into their
-   respective Pydantic models using `validate_config()`. The `default_suffix` kwarg allows
-   for specifying the file suffix (extension) to assume if the config file has no suffix
-   or its suffix is not in the `nested_config.config_dict_loaders` dict.
-
-   Example including mixed configuration file types and `default_suffix` (Note that PyYAML
-   is an extra dependency required for parsing yaml files):
-
-   **house.yaml**
-
-   ```yaml
-   name: my house
-   dimensions: dimensions
-   ```
-
-   **dimensions** (TOML type)
-
-   ```toml
-   length = 10
-   width = 20
-   ```
-
-   **parse_house.py**
-
-   ```python
-   import pydantic
-   import yaml
-
-   from nested_config import validate_config
-
-   class Dimensions(pydantic.BaseModel):
-       length: int
-       width: int
-
-
-   class House(pydantic.BaseModel):
-       name: str
-       dimensions: Dimensions
-
-
-   house = validate_config("house.yaml", House, default_suffix=".toml")
-   house  # House(name='my house', dimensions=Dimensions(length=10, width=20))
-   ```
-
-2. Alternatively, you can use `nested_config.BaseModel` which subclasses
-   `pydantic.BaseModel` and adds a `from_config` classmethod:
-
-   **house.toml**
-
-   ```toml
-   name = "my house"
-   dimensions = "dimensions.toml"
-   ```
-
-   **dimensions.toml**
-
-   ```toml
-   length = 12.6
-   width = 25.3
-   ```
-
-   **parse_house.py**
-
-   ```python
-   import nested_config
-
-   class Dimensions(nested_config.BaseModel):
-       length: float
-       width: float
-
-
-   class House(nested_config.BaseModel):
-       name: str
-       dimensions: Dimensions
-
-
-   house = House.from_config("house.toml", House)
-   house  # House(name='my house', dimensions=Dimensions(length=12.6, width=25.3))
-   ```
+# nested-config <!-- omit in toc -->
+
+<span style="font-size: larger">If you've ever wanted to have the option of replacing part
+ of a configuration file with a path to another configuration file that contains those
+sub-parameters, then _nested-config_ might be for you.</span>
+
+_nested-config_ allows you to parse configuration files that contain references to other
+configuration files using a series of [models](#model). If a model includes a [nested
+model](#nested-model) as one of its attributes and _nested-config_ finds a string value
+for that parameter in the configuration file instead of an associative
+array[^assoc-array], then it assumes that this string is a path to another configuration
+file that should be parsed and whose contents should replace the string in the main
+configuration file. If the string appears to be a relative path, it is assumed to be
+relative to the path of its parent configuration file.
+
+## Contents
+
+- [Contents](#contents)
+- [Basic Usage](#basic-usage)
+- [Nomenclature](#nomenclature)
+  - [loader](#loader)
+  - [model](#model)
+  - [nested model](#nested-model)
+  - [config dict](#config-dict)
+- [API](#api)
+  - [`nested_config.expand_config(config_path, model, *, default_suffix = None)`](#nested_configexpand_configconfig_path-model--default_suffix--none)
+  - [`nested_config.config_dict_loaders`](#nested_configconfig_dict_loaders)
+    - [Included loaders](#included-loaders)
+    - [Adding loaders](#adding-loaders)
+  - [_Deprecated features in v2.1.0, to be removed in v3.0.0_](#deprecated-features-in-v210-to-be-removed-in-v300)
+- [Pydantic 1.0/2.0 Compatibility](#pydantic-1020-compatibility)
+- [Footnotes](#footnotes)
+
+## Basic Usage
+
+Given the following configuration files `/tmp/house.toml` and `/tmp/tmp2/dimensions.toml`:
+
+<figure>
+<figcaption>Figure 1: /tmp/house.toml</figcaption>
+
+```toml
+name = "my house"
+dimensions = "tmp2/dimensions.toml"
+```
+
+</figure>
+
+<figure>
+<figcaption>Figure 2: /tmp/tmp2/dimensions.toml</figcaption>
+
+```toml
+length = 10
+width = 20
+```
+
+</figure>
+
+You can expand these into a single dict with the following:
+
+<figure>
+<figcaption>Figure 3: Expand /tmp/house.toml</figcaption>
+
+```python
+import nested_config
+
+class Dimensions:
+    length: int
+    width: int
+
+
+class House:
+    name: str
+    dimensions: Dimensions
 
-   In this case, if you need to specify a default loader, just use
-   `nested_config.set_default_loader(suffix)` before using `BaseModel.from_config()`.
+
+house_dict = nested_config.expand_config("/tmp/house.toml", House)
+print(house_dict)
+# {'name': 'my house', 'dimensions': {'length': 10, 'width': 20}}
+```
+
+Note that in `/tmp/house.toml`, `dimensions` is not a mapping but is a path to another
+toml file at a path relative to `house.toml`.
 
 See [tests](https://gitlab.com/osu-nrsg/nested-config/-/tree/master/tests) for more
-detailed use-cases, such as where the root pydantic model contains lists or dicts of other
-models and when those may be included in the root config file or specified as paths to
-sub-config files.
+detailed use-cases, such as where the root model contains lists or dicts of other models
+and when those may be included in the root config file or specified as paths to sub-config
+files.
+
+## Nomenclature
+
+### loader
+
+A _loader_ is a function that reads a config file and returns a `dict` containing the
+key-value pairs from the file. _nested-config_ includes loaders for JSON, TOML, and (if
+PyYAML is installed) YAML. For example, the JSON loader looks like this:
+
+```python
+import json
+
+def json_load(path):
+    with open(path, "rb") as fobj:
+        return json.load(fobj)
+```
+
+### model
+
+_nested-config_ uses the term _model_ to refer to a class definition that includes
+annotated attributes. For example, this model, `Dimensions`, includes three attributes,
+each of float type, `x`, `y`, and `z`:
+
+```python
+class Dimensions:
+    x: float
+    y: float
+    z: float
+```
+
+A model can be decorated as a [dataclass][dataclasses] or using [`attrs.define`][attrs] or
+can subclass [`pydantic.BaseModel`][pydantic] to provide some method for instantiating an
+object instance of the model but they aren't necessary to use _nested-config_.
+
+The only criterion for a type to be a model is that is has a `__dict__` attribute that
+includes an `__annotations__` member. _Note: This does **not** mean that **instances** of
+the model must have a `__dict__` attribute. For example, instances of classes with
+`__slots__` and `NamedTuple` instances may not have a `__dict__` attribute._
+
+### nested model
+
+A _nested model_ is a model that is included within another model as one of its class
+attributes. For example, the below model `House` includes an `name` of string type, and an
+attribute `dimensions` of `Dimensions` type (defined above). Since `Dimensions` is a
+_model_ type, this is an example of a _nested model_.
+
+```python
+class House:
+    name: str
+    dimensions: Dimensions
+```
+
+### config dict
+
+A _config dict_ is simply a `dict` with string keys such as may be obtained by reading in
+configuration text. For example reading in a string of TOML text with `tomllib.loads`
+returns a _config dict_.
+
+```python
+import tomllib
+
+config = "x = 2\ny = 3"
+print(tomllib.loads(config))
+# {'x': 2, 'y': 3}
+```
+
+## API
+
+### `nested_config.expand_config(config_path, model, *, default_suffix = None)`
+
+This function first loads the config file at `config_path` into a [config
+dict](#config-dict) using the appropriate [loader](#loader). It then uses the attribute
+annotations of [`model`](#model) and/or any [nested models](#nested-model) within `model`
+to see if any of the string values in the configuration file correspond to a nested model.
+For each such case, the string is assumed to be a path and is loaded into another config
+dict which replaces the string value in the parent config dict. This continues until all
+paths are converted and then the fully-expanded config dict is returned.
+
+Note that all non-absolute string paths are assumed to be relative to the path of their
+parent config file.
 
-### Included loaders
+The loader for a given config file is determined by file extension (AKA suffix). If
+`default_suffix` is specified, any config file with an unknown suffix or no suffix will be
+assumed to be of that type, e.g. `".toml"`. (Otherwise this is an error.) It is possible
+for one config file to include a path to a config file of a different format, so long as
+each file has the appropriate suffix and there is a loader for that suffix.
 
-**nested-config** automatically loads the following files based on extension:
+### `nested_config.config_dict_loaders`
+
+`config_dict_loaders` is a `dict` that maps file suffixes to [loaders](#loader).
+
+#### Included loaders
+
+_nested-config_ automatically loads the following files based on extension:
 
 | Format | Extensions(s) | Library                                    |
 | ------ | ------------- | ------------------------------------------ |
 | JSON   | .json         | `json` (stdlib)                            |
 | TOML   | .toml         | `tomllib` (Python 3.11+ stdlib) or `tomli` |
 | YAML   | .yaml, .yml   | `pyyaml` (extra dependency[^yaml-extra])   |
 
-### Adding loaders
+#### Adding loaders
 
-To add a loader for another file extension, simply update the `config_dict_loaders` dict:
+To add a loader for another file extension, simply update `config_dict_loaders`:
 
 ```python
 import nested_config
 from nested_config import ConfigDict  # alias for dict[str, Any]
 
-def dummy_loader(config_path: Path) -> ConfigDict:
+def dummy_loader(config_path: Path | str) -> ConfigDict:
     return {"a": 1, "b": 2}
 
 nested_config.config_dict_loaders[".dmy"] = dummy_loader
 
 # or add another extension for an existing loader
 nested_config.config_dict_loaders[".jsn"] = nested_config.config_dict_loaders[".json"]
-```
-
-### `PurePath` handling
-
-A bonus feature of **nested-config** is that it provides for validation and JSON encoding
-of `pathlib.PurePath` and its subclasses in Pydantic <2.0 (this is built into Pydantic
-2.0+). All that is needed is an import of `nested_config`. Example:
-
-```python
-from pathlib import PurePosixPath
 
-import nested_config
-import pydantic
+# or use a different library to replace an existing loader
+import rtoml
 
+def rtoml_load(path) -> ConfigDict:
+    with open(path, "rb") as fobj:
+        return rtoml.load(fobj)
 
-class RsyncDestination(pydantic.BaseModel):
-    remote_server: str
-    remote_path: PurePosixPath
+nested_config.config_dict_loaders[".toml"] = rtoml_load
+```
 
+### _Deprecated features in v2.1.0, to be removed in v3.0.0_
 
-dest = RsyncDestination(remote_server="rsync.example.com", remote_path="/data/incoming")
+The following functionality is available only if Pydantic is installed:
 
-dest  # RsyncDestination(remote_server='rsync.example.com', remote_path=PurePosixPath('/data/incoming'))
-dest.json()  # '{"remote_server":"rsync.example.com","remote_path":"/data/incoming"}'
-
-```
+- `nested_config.validate_config()` expands a configuration file according to a Pydantic
+  model and then validates the config dictionary into an instance of the Pydantic model.
+- `nested_config.BaseModel` can be used as a replacement for `pydantic.BaseModel` to
+  include a `from_config()` classmethod on all models that uses
+  `nested_config.validate_config()` to create an instance of the model.
+- By importing `nested_config`, `PurePath` validators and JSON encoders are added to
+  `pydantic` in Pydantic 1.8-1.10 (they are included in Pydantic 2.0+)
 
 ## Pydantic 1.0/2.0 Compatibility
 
+The [pydantic functionality](#deprecated-features-in-v210-to-be-removed-in-v300) in
 nested-config is runtime compatible with Pydantic 1.8+ and Pydantic 2.0.
 
 The follow table gives info on how to configure the [mypy](https://www.mypy-lang.org/) and
 [Pyright](https://microsoft.github.io/pyright) type checkers to properly work, depending
 on the version of Pydantic you are using.
 
 | Pydantic Version | [mypy config][1]            | mypy cli                    | [Pyright config][2]                         |
 |------------------|-----------------------------|-----------------------------|---------------------------------------------|
 | 2.0+             | `always_false = PYDANTIC_1` | `--always-false PYDANTIC_1` | `defineConstant = { "PYDANTIC_1" = false }` |
 | 1.8-1.10         | `always_true = PYDANTIC_1`  | `--always-true PYDANTIC_1`  | `defineConstant = { "PYDANTIC_1" = true }`  |
 
 ## Footnotes
 
-[^yaml-extra]: Install `pyyaml` separately with `pip` or install **nested-config** with
+[^yaml-extra]: Install `pyyaml` separately with `pip` or install _nested-config_ with
                `pip install nested-config[yaml]`.
 
+[^assoc-array]: Each language uses one or more names for an associative arrays. JSON calls
+                it an _object_, YAML calls is a _mapping_, and TOML calls is a _table_.
+                Any of course in Python it's a _dictionary_, or `dict`.
+
 [1]: https://mypy.readthedocs.io/en/latest/config_file.html
 [2]: https://microsoft.github.io/pyright/#/configuration
-
+[dataclasses]: https://docs.python.org/3/library/dataclasses.html
+[attrs]: https://www.attrs.org
+[pydantic]: https://pydantic.dev
```

