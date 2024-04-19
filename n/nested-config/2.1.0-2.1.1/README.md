# Comparing `tmp/nested_config-2.1.0.tar.gz` & `tmp/nested_config-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nested_config-2.1.0.tar", max compression
+gzip compressed data, was "nested_config-2.1.1.tar", max compression
```

## Comparing `nested_config-2.1.0.tar` & `nested_config-2.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3146 2024-04-18 21:02:18.859923 nested_config-2.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1097 2024-04-15 20:59:09.993709 nested_config-2.1.0/LICENSE
--rw-r--r--   0        0        0     9665 2024-04-18 23:04:04.222666 nested_config-2.1.0/README.md
--rw-r--r--   0        0        0     1856 2024-04-18 19:39:03.493579 nested_config-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-04-18 18:00:20.433917 nested_config-2.1.0/src/nested_config/__init__.py
--rw-r--r--   0        0        0     6199 2024-04-18 19:38:20.097488 nested_config-2.1.0/src/nested_config/_pydantic.py
--rw-r--r--   0        0        0      457 2024-04-16 23:16:09.316884 nested_config-2.1.0/src/nested_config/_types.py
--rw-r--r--   0        0        0     6291 2024-04-18 17:59:31.681832 nested_config-2.1.0/src/nested_config/expand.py
--rw-r--r--   0        0        0     2969 2024-04-17 18:58:24.182981 nested_config-2.1.0/src/nested_config/loaders.py
--rw-r--r--   0        0        0      268 2024-04-04 20:38:25.984470 nested_config-2.1.0/src/nested_config/version.py
--rw-r--r--   0        0        0    11077 1970-01-01 00:00:00.000000 nested_config-2.1.0/setup.py
--rw-r--r--   0        0        0    11351 1970-01-01 00:00:00.000000 nested_config-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3320 2024-04-19 16:44:19.627499 nested_config-2.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1097 2024-04-15 20:59:09.993709 nested_config-2.1.1/LICENSE
+-rw-r--r--   0        0        0     9665 2024-04-18 23:04:04.222666 nested_config-2.1.1/README.md
+-rw-r--r--   0        0        0     1784 2024-04-19 16:42:46.411300 nested_config-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      569 2024-04-19 16:33:38.650127 nested_config-2.1.1/src/nested_config/__init__.py
+-rw-r--r--   0        0        0     6199 2024-04-18 19:38:20.097488 nested_config-2.1.1/src/nested_config/_pydantic.py
+-rw-r--r--   0        0        0      457 2024-04-16 23:16:09.316884 nested_config-2.1.1/src/nested_config/_types.py
+-rw-r--r--   0        0        0     8329 2024-04-19 16:43:18.947369 nested_config-2.1.1/src/nested_config/expand.py
+-rw-r--r--   0        0        0     2969 2024-04-17 18:58:24.182981 nested_config-2.1.1/src/nested_config/loaders.py
+-rw-r--r--   0        0        0      268 2024-04-04 20:38:25.984470 nested_config-2.1.1/src/nested_config/version.py
+-rw-r--r--   0        0        0    11033 1970-01-01 00:00:00.000000 nested_config-2.1.1/setup.py
+-rw-r--r--   0        0        0    11277 1970-01-01 00:00:00.000000 nested_config-2.1.1/PKG-INFO
```

### Comparing `nested_config-2.1.0/CHANGELOG.md` & `nested_config-2.1.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [2.1.1] - 2024-04-19
+
+- Export ConfigExpansionError in `__init__.py`
+- Fix/update docstrings
+
 ## [2.1.0] - 2024-04-18
 
 ### Added
 
 - `nested_config.expand_config` - Recursively read in any config file(s) into a dict based
   on model class(es). This is now the primary functionality, superseeding
   `validate_config`, which will be deprecated.
@@ -68,14 +73,15 @@
 ## [1.1.3] - 2021-07-30
 
 - Add README
 - Simplify PurePosixPath validator
 - Export `TomlParsingError` from rtoml for downstream exception handling (without needing to explicitly
   import rtoml).
 
-[Unreleased]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.1.0...master
+[Unreleased]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.1.1...master
+[2.1.1]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.1.0...v2.1.1
 [2.1.0]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.0.3...v2.1.0
 [2.0.3]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.0.2...v2.0.3
 [2.0.2]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.0.1...v2.0.2
 [2.0.1]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v2.0.0...v2.0.1
 [2.0.0]: https://gitlab.com/osu-nrsg/nested-config/-/compare/v1.1.3...v2.0.0
 [1.1.3]: https://gitlab.com/osu-nrsg/nested-config/-/tags/v1.1.3
```

### Comparing `nested_config-2.1.0/LICENSE` & `nested_config-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nested_config-2.1.0/README.md` & `nested_config-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nested_config-2.1.0/pyproject.toml` & `nested_config-2.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "nested-config"
-version = "2.1.0"
+version = "2.1.1"
 description = """\
-Parse configuration files that include paths to other config files into Pydantic model\
- instances. Also support pathlib.PurePath on Pydantic 1.8+.\
+Parse configuration files that include paths to other config files into a single\
+ configuration object\
 """
 authors = ["Randall Pittman <pittmara@oregonstate.edu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.com/osu-nrsg/nested-config"
-keywords = ["pydantic", "config", "configuration files"]
+keywords = ["config", "configuration files"]
 classifiers = [
-    "Development Status :: 4 - Beta",
-    "Framework :: Pydantic",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
```

### Comparing `nested_config-2.1.0/src/nested_config/_pydantic.py` & `nested_config-2.1.1/src/nested_config/_pydantic.py`

 * *Files identical despite different names*

### Comparing `nested_config-2.1.0/src/nested_config/loaders.py` & `nested_config-2.1.1/src/nested_config/loaders.py`

 * *Files identical despite different names*

### Comparing `nested_config-2.1.0/setup.py` & `nested_config-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 {':python_version < "3.11"': ['tomli>=2.0.0,<3.0.0'],
  ':python_version >= "3.12"': ['setuptools>=69.5.1,<70.0.0'],
  'pydantic': ['pydantic>=1.8,<3.0.0'],
  'yaml': ['pyyaml>=5.1.0,<7.0.0']}
 
 setup_kwargs = {
     'name': 'nested-config',
-    'version': '2.1.0',
-    'description': 'Parse configuration files that include paths to other config files into Pydantic modelinstances. Also support pathlib.PurePath on Pydantic 1.8+.',
+    'version': '2.1.1',
+    'description': 'Parse configuration files that include paths to other config files into a singleconfiguration object',
     'long_description': '# nested-config <!-- omit in toc -->\n\n<span style="font-size: larger">If you\'ve ever wanted to have the option of replacing part\n of a configuration file with a path to another configuration file that contains those\nsub-parameters, then _nested-config_ might be for you.</span>\n\n_nested-config_ allows you to parse configuration files that contain references to other\nconfiguration files using a series of [models](#model). If a model includes a [nested\nmodel](#nested-model) as one of its attributes and _nested-config_ finds a string value\nfor that parameter in the configuration file instead of an associative\narray[^assoc-array], then it assumes that this string is a path to another configuration\nfile that should be parsed and whose contents should replace the string in the main\nconfiguration file. If the string appears to be a relative path, it is assumed to be\nrelative to the path of its parent configuration file.\n\n## Contents\n\n- [Contents](#contents)\n- [Basic Usage](#basic-usage)\n- [Nomenclature](#nomenclature)\n  - [loader](#loader)\n  - [model](#model)\n  - [nested model](#nested-model)\n  - [config dict](#config-dict)\n- [API](#api)\n  - [`nested_config.expand_config(config_path, model, *, default_suffix = None)`](#nested_configexpand_configconfig_path-model--default_suffix--none)\n  - [`nested_config.config_dict_loaders`](#nested_configconfig_dict_loaders)\n    - [Included loaders](#included-loaders)\n    - [Adding loaders](#adding-loaders)\n  - [_Deprecated features in v2.1.0, to be removed in v3.0.0_](#deprecated-features-in-v210-to-be-removed-in-v300)\n- [Pydantic 1.0/2.0 Compatibility](#pydantic-1020-compatibility)\n- [Footnotes](#footnotes)\n\n## Basic Usage\n\nGiven the following configuration files `/tmp/house.toml` and `/tmp/tmp2/dimensions.toml`:\n\n<figure>\n<figcaption>Figure 1: /tmp/house.toml</figcaption>\n\n```toml\nname = "my house"\ndimensions = "tmp2/dimensions.toml"\n```\n\n</figure>\n\n<figure>\n<figcaption>Figure 2: /tmp/tmp2/dimensions.toml</figcaption>\n\n```toml\nlength = 10\nwidth = 20\n```\n\n</figure>\n\nYou can expand these into a single dict with the following:\n\n<figure>\n<figcaption>Figure 3: Expand /tmp/house.toml</figcaption>\n\n```python\nimport nested_config\n\nclass Dimensions:\n    length: int\n    width: int\n\n\nclass House:\n    name: str\n    dimensions: Dimensions\n\n\nhouse_dict = nested_config.expand_config("/tmp/house.toml", House)\nprint(house_dict)\n# {\'name\': \'my house\', \'dimensions\': {\'length\': 10, \'width\': 20}}\n```\n\nNote that in `/tmp/house.toml`, `dimensions` is not a mapping but is a path to another\ntoml file at a path relative to `house.toml`.\n\nSee [tests](https://gitlab.com/osu-nrsg/nested-config/-/tree/master/tests) for more\ndetailed use-cases, such as where the root model contains lists or dicts of other models\nand when those may be included in the root config file or specified as paths to sub-config\nfiles.\n\n## Nomenclature\n\n### loader\n\nA _loader_ is a function that reads a config file and returns a `dict` containing the\nkey-value pairs from the file. _nested-config_ includes loaders for JSON, TOML, and (if\nPyYAML is installed) YAML. For example, the JSON loader looks like this:\n\n```python\nimport json\n\ndef json_load(path):\n    with open(path, "rb") as fobj:\n        return json.load(fobj)\n```\n\n### model\n\n_nested-config_ uses the term _model_ to refer to a class definition that includes\nannotated attributes. For example, this model, `Dimensions`, includes three attributes,\neach of float type, `x`, `y`, and `z`:\n\n```python\nclass Dimensions:\n    x: float\n    y: float\n    z: float\n```\n\nA model can be decorated as a [dataclass][dataclasses] or using [`attrs.define`][attrs] or\ncan subclass [`pydantic.BaseModel`][pydantic] to provide some method for instantiating an\nobject instance of the model but they aren\'t necessary to use _nested-config_.\n\nThe only criterion for a type to be a model is that is has a `__dict__` attribute that\nincludes an `__annotations__` member. _Note: This does **not** mean that **instances** of\nthe model must have a `__dict__` attribute. For example, instances of classes with\n`__slots__` and `NamedTuple` instances may not have a `__dict__` attribute._\n\n### nested model\n\nA _nested model_ is a model that is included within another model as one of its class\nattributes. For example, the below model `House` includes an `name` of string type, and an\nattribute `dimensions` of `Dimensions` type (defined above). Since `Dimensions` is a\n_model_ type, this is an example of a _nested model_.\n\n```python\nclass House:\n    name: str\n    dimensions: Dimensions\n```\n\n### config dict\n\nA _config dict_ is simply a `dict` with string keys such as may be obtained by reading in\nconfiguration text. For example reading in a string of TOML text with `tomllib.loads`\nreturns a _config dict_.\n\n```python\nimport tomllib\n\nconfig = "x = 2\\ny = 3"\nprint(tomllib.loads(config))\n# {\'x\': 2, \'y\': 3}\n```\n\n## API\n\n### `nested_config.expand_config(config_path, model, *, default_suffix = None)`\n\nThis function first loads the config file at `config_path` into a [config\ndict](#config-dict) using the appropriate [loader](#loader). It then uses the attribute\nannotations of [`model`](#model) and/or any [nested models](#nested-model) within `model`\nto see if any of the string values in the configuration file correspond to a nested model.\nFor each such case, the string is assumed to be a path and is loaded into another config\ndict which replaces the string value in the parent config dict. This continues until all\npaths are converted and then the fully-expanded config dict is returned.\n\nNote that all non-absolute string paths are assumed to be relative to the path of their\nparent config file.\n\nThe loader for a given config file is determined by file extension (AKA suffix). If\n`default_suffix` is specified, any config file with an unknown suffix or no suffix will be\nassumed to be of that type, e.g. `".toml"`. (Otherwise this is an error.) It is possible\nfor one config file to include a path to a config file of a different format, so long as\neach file has the appropriate suffix and there is a loader for that suffix.\n\n### `nested_config.config_dict_loaders`\n\n`config_dict_loaders` is a `dict` that maps file suffixes to [loaders](#loader).\n\n#### Included loaders\n\n_nested-config_ automatically loads the following files based on extension:\n\n| Format | Extensions(s) | Library                                    |\n| ------ | ------------- | ------------------------------------------ |\n| JSON   | .json         | `json` (stdlib)                            |\n| TOML   | .toml         | `tomllib` (Python 3.11+ stdlib) or `tomli` |\n| YAML   | .yaml, .yml   | `pyyaml` (extra dependency[^yaml-extra])   |\n\n#### Adding loaders\n\nTo add a loader for another file extension, simply update `config_dict_loaders`:\n\n```python\nimport nested_config\nfrom nested_config import ConfigDict  # alias for dict[str, Any]\n\ndef dummy_loader(config_path: Path | str) -> ConfigDict:\n    return {"a": 1, "b": 2}\n\nnested_config.config_dict_loaders[".dmy"] = dummy_loader\n\n# or add another extension for an existing loader\nnested_config.config_dict_loaders[".jsn"] = nested_config.config_dict_loaders[".json"]\n\n# or use a different library to replace an existing loader\nimport rtoml\n\ndef rtoml_load(path) -> ConfigDict:\n    with open(path, "rb") as fobj:\n        return rtoml.load(fobj)\n\nnested_config.config_dict_loaders[".toml"] = rtoml_load\n```\n\n### _Deprecated features in v2.1.0, to be removed in v3.0.0_\n\nThe following functionality is available only if Pydantic is installed:\n\n- `nested_config.validate_config()` expands a configuration file according to a Pydantic\n  model and then validates the config dictionary into an instance of the Pydantic model.\n- `nested_config.BaseModel` can be used as a replacement for `pydantic.BaseModel` to\n  include a `from_config()` classmethod on all models that uses\n  `nested_config.validate_config()` to create an instance of the model.\n- By importing `nested_config`, `PurePath` validators and JSON encoders are added to\n  `pydantic` in Pydantic 1.8-1.10 (they are included in Pydantic 2.0+)\n\n## Pydantic 1.0/2.0 Compatibility\n\nThe [pydantic functionality](#deprecated-features-in-v210-to-be-removed-in-v300) in\nnested-config is runtime compatible with Pydantic 1.8+ and Pydantic 2.0.\n\nThe follow table gives info on how to configure the [mypy](https://www.mypy-lang.org/) and\n[Pyright](https://microsoft.github.io/pyright) type checkers to properly work, depending\non the version of Pydantic you are using.\n\n| Pydantic Version | [mypy config][1]            | mypy cli                    | [Pyright config][2]                         |\n|------------------|-----------------------------|-----------------------------|---------------------------------------------|\n| 2.0+             | `always_false = PYDANTIC_1` | `--always-false PYDANTIC_1` | `defineConstant = { "PYDANTIC_1" = false }` |\n| 1.8-1.10         | `always_true = PYDANTIC_1`  | `--always-true PYDANTIC_1`  | `defineConstant = { "PYDANTIC_1" = true }`  |\n\n## Footnotes\n\n[^yaml-extra]: Install `pyyaml` separately with `pip` or install _nested-config_ with\n               `pip install nested-config[yaml]`.\n\n[^assoc-array]: Each language uses one or more names for an associative arrays. JSON calls\n                it an _object_, YAML calls is a _mapping_, and TOML calls is a _table_.\n                Any of course in Python it\'s a _dictionary_, or `dict`.\n\n[1]: https://mypy.readthedocs.io/en/latest/config_file.html\n[2]: https://microsoft.github.io/pyright/#/configuration\n[dataclasses]: https://docs.python.org/3/library/dataclasses.html\n[attrs]: https://www.attrs.org\n[pydantic]: https://pydantic.dev\n',
     'author': 'Randall Pittman',
     'author_email': 'pittmara@oregonstate.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/osu-nrsg/nested-config',
     'package_dir': package_dir,
```

### Comparing `nested_config-2.1.0/PKG-INFO` & `nested_config-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: nested-config
-Version: 2.1.0
-Summary: Parse configuration files that include paths to other config files into Pydantic modelinstances. Also support pathlib.PurePath on Pydantic 1.8+.
+Version: 2.1.1
+Summary: Parse configuration files that include paths to other config files into a singleconfiguration object
 Home-page: https://gitlab.com/osu-nrsg/nested-config
 License: MIT
-Keywords: pydantic,config,configuration files
+Keywords: config,configuration files
 Author: Randall Pittman
 Author-email: pittmara@oregonstate.edu
 Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Pydantic
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

