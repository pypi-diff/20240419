# Comparing `tmp/bumpsemver-1.0.6.tar.gz` & `tmp/bumpsemver-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpsemver-1.0.6.tar", last modified: Thu Mar 31 06:44:57 2022, max compression
+gzip compressed data, was "bumpsemver-2.0.0.tar", max compression
```

## Comparing `bumpsemver-1.0.6.tar` & `bumpsemver-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,19 @@
-drwxr-xr-x   0 zhaow      (501) staff       (20)        0 2022-03-31 06:44:57.905971 bumpsemver-1.0.6/
--rw-r--r--   0 zhaow      (501) staff       (20)     1066 2021-03-26 22:24:20.000000 bumpsemver-1.0.6/LICENSE
--rw-r--r--   0 zhaow      (501) staff       (20)       57 2021-03-26 22:35:57.000000 bumpsemver-1.0.6/MANIFEST.in
--rw-r--r--   0 zhaow      (501) staff       (20)    12428 2022-03-31 06:44:57.906541 bumpsemver-1.0.6/PKG-INFO
--rw-r--r--   0 zhaow      (501) staff       (20)     9609 2022-03-31 06:43:42.000000 bumpsemver-1.0.6/README.md
-drwxr-xr-x   0 zhaow      (501) staff       (20)        0 2022-03-31 06:44:57.896008 bumpsemver-1.0.6/bumpsemver/
--rw-r--r--   0 zhaow      (501) staff       (20)      110 2022-03-31 06:43:42.000000 bumpsemver-1.0.6/bumpsemver/__init__.py
--rw-r--r--   0 zhaow      (501) staff       (20)      230 2021-06-25 19:11:27.000000 bumpsemver-1.0.6/bumpsemver/__main__.py
--rw-r--r--   0 zhaow      (501) staff       (20)    18790 2022-03-31 06:30:12.000000 bumpsemver-1.0.6/bumpsemver/cli.py
--rw-r--r--   0 zhaow      (501) staff       (20)      720 2021-06-22 09:48:31.000000 bumpsemver-1.0.6/bumpsemver/exceptions.py
-drwxr-xr-x   0 zhaow      (501) staff       (20)        0 2022-03-31 06:44:57.902144 bumpsemver-1.0.6/bumpsemver/files/
--rw-r--r--   0 zhaow      (501) staff       (20)      112 2021-06-22 08:43:45.000000 bumpsemver-1.0.6/bumpsemver/files/__init__.py
--rw-r--r--   0 zhaow      (501) staff       (20)     2289 2021-06-22 11:24:05.000000 bumpsemver-1.0.6/bumpsemver/files/base.py
--rw-r--r--   0 zhaow      (501) staff       (20)     3433 2021-06-22 11:28:13.000000 bumpsemver-1.0.6/bumpsemver/files/generic.py
--rw-r--r--   0 zhaow      (501) staff       (20)     3332 2021-06-22 11:34:51.000000 bumpsemver-1.0.6/bumpsemver/files/json.py
--rw-r--r--   0 zhaow      (501) staff       (20)     3396 2021-06-22 11:28:26.000000 bumpsemver-1.0.6/bumpsemver/files/yaml.py
--rw-r--r--   0 zhaow      (501) staff       (20)     1189 2021-06-22 10:52:01.000000 bumpsemver-1.0.6/bumpsemver/functions.py
--rw-r--r--   0 zhaow      (501) staff       (20)     3471 2021-06-22 10:32:20.000000 bumpsemver-1.0.6/bumpsemver/git.py
--rw-r--r--   0 zhaow      (501) staff       (20)      226 2021-06-22 08:42:40.000000 bumpsemver-1.0.6/bumpsemver/utils.py
--rw-r--r--   0 zhaow      (501) staff       (20)     6153 2021-06-22 10:44:22.000000 bumpsemver-1.0.6/bumpsemver/version_part.py
-drwxr-xr-x   0 zhaow      (501) staff       (20)        0 2022-03-31 06:44:57.900159 bumpsemver-1.0.6/bumpsemver.egg-info/
--rw-r--r--   0 zhaow      (501) staff       (20)    12428 2022-03-31 06:44:57.000000 bumpsemver-1.0.6/bumpsemver.egg-info/PKG-INFO
--rw-r--r--   0 zhaow      (501) staff       (20)      707 2022-03-31 06:44:57.000000 bumpsemver-1.0.6/bumpsemver.egg-info/SOURCES.txt
--rw-r--r--   0 zhaow      (501) staff       (20)        1 2022-03-31 06:44:57.000000 bumpsemver-1.0.6/bumpsemver.egg-info/dependency_links.txt
--rw-r--r--   0 zhaow      (501) staff       (20)       52 2022-03-31 06:44:57.000000 bumpsemver-1.0.6/bumpsemver.egg-info/entry_points.txt
--rw-r--r--   0 zhaow      (501) staff       (20)       33 2022-03-31 06:44:57.000000 bumpsemver-1.0.6/bumpsemver.egg-info/requires.txt
--rw-r--r--   0 zhaow      (501) staff       (20)       17 2022-03-31 06:44:57.000000 bumpsemver-1.0.6/bumpsemver.egg-info/top_level.txt
--rw-r--r--   0 zhaow      (501) staff       (20)       61 2022-03-31 06:44:57.907468 bumpsemver-1.0.6/setup.cfg
--rw-r--r--   0 zhaow      (501) staff       (20)     1239 2022-03-31 06:43:42.000000 bumpsemver-1.0.6/setup.py
-drwxr-xr-x   0 zhaow      (501) staff       (20)        0 2022-03-31 06:44:57.905397 bumpsemver-1.0.6/tests/
--rw-r--r--   0 zhaow      (501) staff       (20)       20 2021-06-22 10:46:46.000000 bumpsemver-1.0.6/tests/__init__.py
--rw-r--r--   0 zhaow      (501) staff       (20)    25847 2022-03-31 06:38:57.000000 bumpsemver-1.0.6/tests/test_cli.py
--rw-r--r--   0 zhaow      (501) staff       (20)      690 2021-06-22 10:47:18.000000 bumpsemver-1.0.6/tests/test_functions.py
--rw-r--r--   0 zhaow      (501) staff       (20)    21157 2022-03-31 06:40:45.000000 bumpsemver-1.0.6/tests/test_git.py
--rw-r--r--   0 zhaow      (501) staff       (20)     7819 2021-06-22 10:48:41.000000 bumpsemver-1.0.6/tests/test_json.py
--rw-r--r--   0 zhaow      (501) staff       (20)      886 2021-06-22 10:47:58.000000 bumpsemver-1.0.6/tests/test_version_part.py
--rw-r--r--   0 zhaow      (501) staff       (20)     8581 2021-06-22 10:48:17.000000 bumpsemver-1.0.6/tests/test_yaml.py
+-rw-r--r--   0        0        0     1066 2024-04-19 19:52:02.757204 bumpsemver-2.0.0/LICENSE
+-rw-r--r--   0        0        0    14259 2024-04-19 19:52:02.758334 bumpsemver-2.0.0/README.md
+-rw-r--r--   0        0        0      108 2024-04-19 19:52:02.758812 bumpsemver-2.0.0/bumpsemver/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-19 19:52:02.759096 bumpsemver-2.0.0/bumpsemver/__main__.py
+-rw-r--r--   0        0        0    20745 2024-04-19 19:52:02.759569 bumpsemver-2.0.0/bumpsemver/cli.py
+-rw-r--r--   0        0        0     3289 2024-04-19 19:52:02.759928 bumpsemver-2.0.0/bumpsemver/exceptions.py
+-rw-r--r--   0        0        0        2 2024-04-19 19:52:02.760205 bumpsemver-2.0.0/bumpsemver/files/__init__.py
+-rw-r--r--   0        0        0     3461 2024-04-19 19:52:02.760539 bumpsemver-2.0.0/bumpsemver/files/base.py
+-rw-r--r--   0        0        0     3629 2024-04-19 19:52:02.761016 bumpsemver-2.0.0/bumpsemver/files/json.py
+-rw-r--r--   0        0        0     3338 2024-04-19 19:52:02.761192 bumpsemver-2.0.0/bumpsemver/files/text.py
+-rw-r--r--   0        0        0     2895 2024-04-19 19:52:02.761346 bumpsemver-2.0.0/bumpsemver/files/toml.py
+-rw-r--r--   0        0        0     3886 2024-04-19 19:52:02.761496 bumpsemver-2.0.0/bumpsemver/files/tomlpath.py
+-rw-r--r--   0        0        0     4313 2024-04-19 19:52:02.761983 bumpsemver-2.0.0/bumpsemver/files/yaml.py
+-rw-r--r--   0        0        0     1150 2024-04-19 19:52:02.762360 bumpsemver-2.0.0/bumpsemver/functions.py
+-rw-r--r--   0        0        0     3541 2024-04-19 19:52:02.762704 bumpsemver-2.0.0/bumpsemver/git.py
+-rw-r--r--   0        0        0      228 2024-04-19 19:52:02.763044 bumpsemver-2.0.0/bumpsemver/utils.py
+-rw-r--r--   0        0        0     5034 2024-04-19 19:52:02.763428 bumpsemver-2.0.0/bumpsemver/version_part.py
+-rw-r--r--   0        0        0     3669 2024-04-19 19:52:02.764207 bumpsemver-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    15453 1970-01-01 00:00:00.000000 bumpsemver-2.0.0/PKG-INFO
```

### Comparing `bumpsemver-1.0.6/LICENSE` & `bumpsemver-2.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Zhao Wang
+Copyright (c) 2024 Zhao Wang
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bumpsemver-1.0.6/PKG-INFO` & `bumpsemver-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,295 +1,381 @@
-Metadata-Version: 2.1
-Name: bumpsemver
-Version: 1.0.6
-Summary: Bump semver for git repos with a single command.
-Home-page: https://github.com/zhaow-de/bumpsemver
-Author: Zhao Wang
-Author-email: zhaow.km@gmail.com
-License: UNKNOWN
-Description: 
-        # bumpsemver
-        
-        **Current version: 1.0.6**
-        
-        A utility to simplify the version bumping for git repos.
-        
-        This application is a rework of the famous `bumpversion` tool. The  
-        [original repo](https://github.com/peritus/bumpversion) seems like abandoned. Several fundamental changes are
-        introduced, which make the fork-and-extend approach infeasible:
-        1. dropped Python 2 support
-        2. boosted the test coverage to 95%+
-        3. dropped many irrelevant features to reduce complexity. (e.g. customized version component support)
-        4. introduced JSON support to make it work for package-lock.json, YAML support to make it work for Ansible plays
-        5. narrowed the versioning scheme to semver-only
-        
-        ## Installation
-        
-        ```bash
-        pip3 install bumpsemver
-        ```
-        
-        ## Usage
-        
-        This application supports both the CLI mode and config file mode.
-        
-        ### Command Line Interface
-        
-        ```bash
-        bumpsemver [options] part [file]
-        ```
-            
-        #### `options`
-        _**(optional)**_<br />
-          
-        Most of the configuration values described below can also be given as an option on the command-line.
-        Additionally, the following options are available:
-        
-        `--dry-run`
-          Don't touch any files, just pretend. Best used with `--verbose`.
-        
-        `--allow-dirty`
-          Normally, bumpsemver will abort if the working directory is dirty to protect
-          yourself from releasing unversioned files and/or overwriting unsaved changes.
-          Use this option to override this check.
-        
-        `--verbose`
-          Print useful information to stderr
-        
-        `-h, --help`
-          Print help and exit
-        
-        #### `part`
-        _**required**_<br />
-        
-        The part of the version to increase. As we support semver only, the valid values include: `major`, `minor`, and `patch`.
-        
-        For example, bumping file `src/VERSION` from 0.5.1 to 0.6.0:
-        
-        ```bash
-        bumpsemver --current-version 0.5.1 minor src/VERSION
-        ```
-        
-        #### `file`
-        _**(optional)**_<br />
-        **default**: none
-        
-        The file that will be modified.
-        
-        If not given, the list of `[bumpsemver:file:…]` sections from the configuration file will be used. If no files are
-        mentioned on the configuration file either, then no files will be modified.
-        
-        For example, bumping file `setup.py` from 1.1.9 to 2.0.0:
-        ```
-        bumpsemver --current-version 1.1.9 major setup.py
-        ```
-        
-        ### Configuration file
-        
-        Options on the command line take precedence over those from the config file, which take precedence over those from the
-        defaults.
-        
-        Example `.bumpsemver.cfg`:
-        
-        ```ini
-        [bumpsemver]
-        current_version = 0.2.9
-        commit = True
-        tag = True
-        
-        [bumpsemver:file:README]
-        ```
-        
-        #### `.bumpsemver.cfg` -- Global configuration
-        
-        General configuration is grouped in a `[bumpsemver]` section.
-        
-        ##### `current_version` 
-        _**required**_<br />
-        **default**: none
-        
-        The current version of the software package before bumping.
-        
-        Also available as CLI argument `--current-version` (e.g. `bumpsemver --current-version 0.5.1 patch`)
-        
-        ##### `tag = (True | False)`
-        _**(optional)**_<br />
-        **default**: False (Don't create a git tag)
-        
-        Whether to create a git tag, that is the new version, prefixed with the character "`r`". Don't forget to `git-push`
-        with the `--tags` flag.
-        
-        Also available as CLI argument `--tag` or `--no-tag`.
-        
-        ##### `sign_tags = (True | False)`
-        _**(optional)**_<br />
-        **default**: False (Don't sign tags)
-        
-        Whether to sign tags.
-        
-        Also available as CLI argument `--sign-tags` or `--no-sign-tags`.
-        
-        ##### `tag_name =`
-        _**(optional)**_<br />
-        **default:** `v{new_version}`
-        
-        The name of the tag that will be created. Only valid when `tag = True`.
-        
-        It can be a template using the [Python Format String Syntax](https://docs.python.org/3/library/string.html#format-string-syntax).  
-        Available in the template context are `current_version` and `new_version` as well as `current_[part]` and `new_[part]`
-        (e.g. '`current_major`' or '`new_patch`'). You can also use the variables `now` or `utcnow` to get a current timestamp.
-        Both accept datetime formatting (when used like as in `{now:%d.%m.%Y}`).
-        
-        Also available as CLI argument `--tag-name`, for example: `bumpsemver --tag-name 'release-{new_version}' patch`
-        
-        In addition, it is also possible to provide a tag message by using CLI `--tag-message TAG_MESSAGE`. Example usage:
-        `bumpsemver --tag-name 'release-{new_version}' --tag-message "Release {new_version}" patch`
-        
-        If neither tag message or sign tag is provided, we use a `lightweight` tag in git. Otherwise, we utilize an `annotated`
-        git tag. Read more about Git tagging [here](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
-        
-        ##### `commit = (True | False)`
-        _**(optional)**_<br />
-        **default:** False (Don't create a commit)
-        
-        Create a commit using git when true.
-        
-        Also available as CLI argument `--commit` or `--no-commit`.
-        
-        ##### `message =`
-        _**(optional)**_<br />
-        **default:** `[OPS] bumped version: {current_version} → {new_version}`
-        
-        The commit message to use when creating a commit. Only valid when using `--commit` / `commit = True`.
-        
-        It can be a template using the [Python Format String Syntax](https://docs.python.org/3/library/string.html#format-string-syntax).  
-        Available in the template context are `current_version` and `new_version` as well as `current_[part]` and `new_[part]`
-        (e.g. '`current_major`' or '`new_patch`'). You can also use the variables `now` or `utcnow` to get a current timestamp.
-        Both accept datetime formatting (when used like as in `{now:%d.%m.%Y}`).
-        
-        Also available as CLI argument `--message`, for example: `bumpsemver --tag-name 'release-{new_version}' patch`
-        
-        In addition, it is also possible to provide a tag message by using CLI `--tag-message TAG_MESSAGE`. Example usage:
-        `bumpsemver --message '[{now:%Y-%m-%d}] Jenkins Build {$BUILD_NUMBER}: {new_version}' patch`
-        
-        #### `.bumpsemver.cfg` -- File specific configuration
-        
-        This configuration is in the section: `[bumpsemver:file:…]` or `[bumpsemver:json:…]`
-        
-        Note: The configuration file format requires each section header to be unique. If you want to process a certain file
-        multiple times (e.g. multiple location to be replaced separately), you may append a description between parens to the
-        `file` keyword: `[bumpsemver:file (special one):…]`. It does not matter what inside the parens, just make it unique.
-        e.g.
-        
-        ```ini
-        [bumpsemver:file(1):README.md]
-        search = current version: {current_version}
-        replace = current version: {new_version}
-        
-        [bumpsemver:file(2):README.md]
-        search = **Version: {current_version}**
-        replace = current version: {new_version}
-        ```
-        
-        ##### `search =`
-        **default:** `{current_version}`
-        
-        Template string how to search for the string to be replaced in the file. Useful if the remotest possibility exists that
-        the current version number might be present multiple times in the file and you mean to only bump one of the occurrences.
-        
-        #### `replace =`
-        **default:** `{new_version}`
-        
-        Template to create the string that will replace the current version number in the file.
-        
-        Given this `requirements.txt`:
-        ```
-            Django>=1.5.6,<1.6
-            MyProject==1.5.6
-        ```
-        using the following `.bumpsemver.cfg` will ensure only the line containing `MyProject` will be changed:
-        ```ini
-        [bumpsemver]
-        current_version = 1.5.6
-        
-        [bumpsemver:file:requirements.txt]
-        search = MyProject=={current_version}
-        replace = MyProject=={new_version}
-        ```
-        
-        With `[bumpsemver:file:…]`, the specified file is processed as plain text file, which in fact makes this application
-        programming language neutral. However, it will be very error prone for complex file for example `package-lock.json`.
-        
-        For randomly sampled 30 projects written in node.js/TypeScript, the classical `bumpversion` or the renovated `bump2version` both made
-        100% mistakes which changed something shouldn't be changed. A typical and relatively complex React projects contains 1000+ npm packages  
-        indirectly. There are too many "version": "1.2.3" in that file. To address this issue, `bumpsemver` added the support of json file.
-        
-        To use it:
-         ```ini
-        [bumpsemver:json:package-lock.json]
-        jsonpath = version 
-        ```
-        
-        Value of the parameter `jsonpath` is a [JSONPath](https://goessner.net/articles/JsonPath/) string. For the typical
-        `package.json` or `package-lock.json`, using `version` or its jQuery-style alternative `$.version` is sufficient.
-        Otherwise, anything can be selected with JSONPath is support, so, nothing we can't do. The underlying JSONPath processor
-        is [jsonpath-ng](https://github.com/h2non/jsonpath-ng). Checkout their document for some examples and hints.
-        
-        The suffix is also supported for json file:
-        ```ini
-        [bumpsemver:json(1):example.json]
-        jsonpath = version
-        
-        [bumpsemver:json( same file):example.json]
-        jsonpath = dependencies[2].*.version
-        
-        [bumpsemver:json (once again):example.json]
-        jsonpath = dependencies[0].*.lodash.dependencies[1].version
-        ```
-        
-        Comparably, YAML is supported for the same reason that we should support native JSON, like
-         ```ini
-        [bumpsemver:yaml:playbook.yml]
-        yamlpath = version 
-        ```
-        OR
-        ```ini
-        [bumpsemver:yaml(1):playbook.yml]
-        yamlpath = *.vars.project_version
-        
-        [bumpsemver:yaml( same file):playbook.yaml]
-        yamlpath = *.vars.version
-        
-        [bumpsemver:yaml (once again):playbook.yaml]
-        yamlpath = *.vars.app_version
-        ```
-        Please note that we use [yamlpath](https://github.com/wwkimball/yamlpath/wiki/Segments-of-a-YAML-Path#yaml-path-standard) instead of
-        `jsonpath` here. `yamlpath` is not a popular "standard" widely adopted. For complex scenarios, it makes sense to test the expression with
-        [yamlpath cli](https://pypi.org/project/yamlpath/) before putting anything in the config file.
-        
-        ## Test
-        
-        Test in Docker container (recommended):
-        ```bash
-        make test
-        ```
-        
-        Local test in the working environment (not recommended):
-        ```bash
-        tox
-        ```
-        
-        To test the compatibility with a specific version of Python, put the version(s) into `./python-versions.txt` one version
-        per line. Then run:
-        ```bash
-        make test
-        ```
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# bumpsemver
+
+[![image](https://img.shields.io/pypi/v/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
+[![image](https://img.shields.io/pypi/l/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
+[![image](https://img.shields.io/pypi/pyversions/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
+[![codecov](https://codecov.io/gh/zhaow-de/bumpsemver/graph/badge.svg?token=WP4O30YLO3)](https://codecov.io/gh/zhaow-de/bumpsemver)
+[![GitHub Actions](https://github.com/zhaow-de/bumpsemver/workflows/CI/badge.svg)](https://github.com/zhaow-de/bumpsemver/actions)
+
+
+Current version: **2.0.0**
+
+## Table of contents
+
+<!--TOC-->
+
+- [Overview](#overview)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Command Line Interface](#command-line-interface)
+- [Configuration file](#configuration-file)
+  - [General config section](#general-config-section)
+  - [File-specific config sections](#file-specific-config-sections)
+  - [File types supported in the file-specific config section](#file-types-supported-in-the-file-specific-config-section)
+    - [Plain text file](#plain-text-file)
+    - [JSON file](#json-file)
+    - [YAML file](#yaml-file)
+    - [TOML file](#toml-file)
+
+<!--TOC-->
+
+## Overview
+
+A utility to simplify the version bumping for git repos.
+
+This application is a rework of the famous `bumpversion` tool. The  
+[original repo](https://github.com/peritus/bumpversion) seems like abandoned. Several fundamental changes are
+introduced, which make the fork-and-extend approach infeasible:
+1. dropped Python 2 support
+2. boosted the test coverage to 95%+
+3. dropped many irrelevant features to reduce complexity. (e.g. customized version component support)
+4. introduced JSON support to make it work for package-lock.json
+5. introduced YAML support to make it work for Ansible playbooks
+6. introduced TOML support to make it work for pyproject.toml 
+7. narrowed the versioning scheme to semver-only
+
+## Installation
+
+```bash
+pip install --upgrade bumpsemver
+```
+
+## Usage
+
+This application supports both the CLI mode and config file mode.
+Options on the command line take precedence over those from the config file, which take precedence over those from the
+defaults.
+
+## Command Line Interface
+
+```bash
+bumpsemver [options] part [file]
+```
+    
+##### **`options`**    _**(optional)**_
+  
+Most of the configuration values described below can also be given as an option on the command-line.
+Additionally, the following options are available:
+
+`--dry-run`
+Don't touch any files, just pretend. Best used with `--verbose`.
+
+`--allow-dirty`
+Normally, bumpsemver will abort if the working directory is dirty to avoid releasing not versioned files
+and/or overwriting unsaved changes. Use this option to override this check.
+
+`--verbose`
+Print useful information about the action details.
+
+`--alloy-checks`
+Perform some extra checks for a private project. Generally irrelevant to the common daily usages.
+
+`-h, --help`
+Print help and exit.
+
+##### **`part`**    _**(required)**_
+
+The part of the version to increase. As we support semver only, the valid values include: `major`, `minor`, and `patch`.
+
+For example, bumping file `src/VERSION` from 0.5.1 to 0.6.0:
+
+```bash
+bumpsemver --current-version 0.5.1 minor src/VERSION
+```
+
+##### **`file`**    _**(optional).**_    _**default**_: none
+
+The file that will be modified.
+
+If not given, the list of `[bumpsemver:*:…]` sections from the configuration file will be used.
+If no files are mentioned on the configuration file either, no files will be modified.
+
+For example, bumping file `setup.py` from 1.1.9 to 2.0.0:
+```
+bumpsemver --current-version 1.1.9 major setup.py
+```
+
+## Configuration file
+
+`bumpsemver` looks up configuration file `.bumpsemver.cfg` at the current directory.
+The config file uses [`ini` syntax](https://en.wikipedia.org/wiki/INI_file).
+It consists of one general section `[bumpsemver]` and zero or more `[bumpsemver:type(suffix):filename]` file sections. 
+
+Example `.bumpsemver.cfg`:
+
+```ini
+[bumpsemver]
+current_version = 0.2.9
+commit = True
+tag = True
+
+[bumpsemver:plaintext:README.md]
+search = Version: **{current_version}**
+replace = Version: **{new_version}**
+
+[bumpsemver:plaintext(header):home.md]
+search = Version: **{current_version}**
+replace = Version: **{new_version}**
+
+[bumpsemver:plaintext(footer 1):home.md]
+search = Current version: {current_version}
+replace = Current version: {new_version}
+
+[bumpsemver:json:example.json]
+jsonpath = foobar.items[1].version
+
+[bumpsemver:yaml:example.yml]
+yamlpath = dummy.version
+
+[bumpsemver:toml:example.toml]
+tomlpath = project.version
+```
+
+### General config section
+
+General configuration is grouped in a `[bumpsemver]` section of `.bumpsemver.cfg`.
+It has the following properties:
+
+##### **`current_version =`**    _**(required).**_    _**default**_: none
+
+The current version of the software package before bumping.
+
+Also available as CLI argument `--current-version` (e.g. `bumpsemver --current-version 0.5.1 patch`)
+
+##### **`tag = (True | False)`**    _**(optional).**_    _**default**_: `False`
+
+Whether to create a git tag, that is the new version, prefixed with the character "`v`".
+
+Also available as CLI argument `--tag` or `--no-tag`.
+
+##### **`sign_tags = (True | False)`**    _**(optional).**_    _**default**_: `False`
+
+Whether to sign tags.
+
+Also available as CLI argument `--sign-tags` or `--no-sign-tags`.
+
+##### **`tag_name =`**    _**(optional).**_    _**default**_: `v{new_version}`
+
+The name of the tag that will be created. Only valid when `tag = True`.
+
+It can be a template using the [Python Format String Syntax](https://docs.python.org/3/library/string.html#format-string-syntax).  
+Available in the template context are `current_version` and `new_version` as well as `current_[part]` and `new_[part]`
+(e.g. '`current_major`' or '`new_patch`'). You can also use the variables `now` or `utcnow` to get a current timestamp.
+Both accept datetime formatting (when used like as in `{now:%d.%m.%Y}`).
+
+Also available as CLI argument `--tag-name`, for example: `bumpsemver --tag-name 'release-{new_version}' patch`
+
+In addition, it is also possible to provide a tag message by using CLI `--tag-message TAG_MESSAGE`. Example usage:
+`bumpsemver --tag-name 'release-{new_version}' --tag-message "Release {new_version}" patch`
+
+If neither tag message nor sign tag is provided, we use a `lightweight` tag in git. Otherwise, we utilize an `annotated`
+git tag. Read more about Git tagging [here](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
+
+##### **`commit = (True | False)`**    _**(optional).**_    _**default**_: `False`
+
+Create a commit using git when true.
+
+Also available as CLI argument `--commit` or `--no-commit`.
+
+##### **`message =`**    _**(optional).**_    _**default**_: `build(repo): bumped version {current_version} → {new_version}`
+
+The commit message to use when creating a commit. Only valid when using `--commit` / `commit = True`.
+
+It can be a template using the [Python Format String Syntax](https://docs.python.org/3/library/string.html#format-string-syntax).  
+Available in the template context are `current_version` and `new_version` as well as `current_[part]` and `new_[part]`
+(e.g. '`current_major`' or '`new_patch`'). You can also use the variables `now` or `utcnow` to get a current timestamp.
+Both accept datetime formatting (when used like as in `{now:%d.%m.%Y}`).
+
+Also available as CLI argument `--message`, for example: `bumpsemver --tag-name 'release-{new_version}' patch`
+
+### File-specific config sections
+
+A file-specific config section is required for each file to specify the handling of the particular file.
+One config file can have zero or more file-specific config sections.
+The section name looks like `[bumpsemver:type:filename]`.
+It specifies the action to be done for a specific file.
+
+We do have the use case that one file has multiple places to change, a popular example is `package-lock.json`:
+```json
+{
+  "name": "rcplus-app-cli",
+  "version": "1.1.0",
+  "lockfileVersion": 3,
+  "requires": true,
+  "packages": {
+    "": {
+      "name": "rcplus-app-cli",
+      "version": "1.1.0",
+      "license": "SEE LICENSE IN LICENSE"
+    }
+  }
+}
+```
+We need two config sections for the same file in this case, but INI format does not allow duplicated section names.
+To make it work we could append a description between parens to the
+`type` keyword: `[bumpsemver:plaintext(special one):…]`. It does not matter what inside the parens, just make it unique.
+For the example below, the two patterns will be applied separately to the same file `README.md`:
+```ini
+[bumpsemver:plaintext(1):README.md]
+search = current version: {current_version}
+replace = current version: {new_version}
+
+[bumpsemver:plaintext(footer):README.md]
+search = **Version: {current_version}**
+replace = **Version: {new_version}**
+```
+
+### File types supported in the file-specific config section
+
+All the famous `bump*version` utilities family has a common pattern to handle the files as a plain text file.
+The advantage of this approach is that in fact it makes the use scenario programming language-neutral.
+Be it a package-lock.json for node.js project, or pyproject.toml for a Python application,
+the `bump*version` is applicable as long as a proper regex pattern for version extraction can be defined.
+
+However, it will bring significant side effect for complex file for example `package-lock.json`.
+A typical (relatively) complex React projects contains 1000+ npm packages indirectly.
+For randomly sampled 30 public projects at GitHub written in node.js/TypeScript,
+the classical `bumpversion` or the renovated `bump2version` both made mistakes
+for all 30 projects which changed something shouldn't be changed.
+
+For instance, the `facebook/create-react-app` application has a large fleet of indirect
+npm dependencies.
+If we define the search pattern as `"version": "4.0.0"`, we will screw up the other 210 packages.
+Or if we are unluckily releasing our app bumping the version from `7.16.0` to `8.0.0`,
+other 132 npm packages in the version lock will be changed to `8.0.0`, which likely do not exist.
+To address this issue, `bumpsemver` added the support of some popular file types
+to access the particular version attribute using a deterministic locator/selector without regex.
+
+The supported file types are:
+* plaintext
+* json
+* yaml
+* toml
+
+#### Plain text file
+
+The file-specific config section looks like:
+```ini
+[bumpsemver:plaintext:filename]
+search = Version: {current_version}
+replace = Version: {new_version}
+```
+
+A deprecated syntax is also supported:
+```ini
+[bumpsemver:file:filename]
+```
+We renamed (in a backward compatible way) `file` or `plaintext` to emphasize
+that the file being processed is considered as a plain text file.
+You can easily destroy a JSON file by a missing a double-quote or a comma in the regex pattern.
+
+This file type should generally only be used for the files that are not JSON, YAML, or TOML.
+`README.md` is a good use case for this one.
+
+`[bumpsemver:plaintext:...]` can have two properties:
+
+##### **`search =`**    _**default**_: `{current_version}`
+
+Template string how to search for the string to be replaced in the file.
+Useful if the remotest possibility exists that the current version number might be present multiple times in the file,
+and you mean to only bump one of the occurrences.
+
+##### **`replace =`**    _**default**_: `{new_version}`
+
+Template to create the string that will replace the current version number in the file.
+
+Given this `requirements.txt`:
+```
+    Django>=1.5.6,<1.6
+    MyProject==1.5.6
+```
+using the following `.bumpsemver.cfg` will ensure only the line containing `MyProject` will be changed:
+```ini
+[bumpsemver]
+current_version = 1.5.6
+
+[bumpsemver:plaintext:requirements.txt]
+search = MyProject=={current_version}
+replace = MyProject=={new_version}
+```
+
+#### JSON file
+
+The file-specific config section looks like:
+```ini
+[bumpsemver:json:package.json]
+jsonpath = version 
+```
+
+It accepts only one property:
+
+##### **`jsonpath =`**    **(required)**    _**default**_: none
+
+Value of the parameter `jsonpath` is a [JSONPath](https://goessner.net/articles/JsonPath/) string,
+it points to the exact property of the version string to be bumped.
+For the typical `package.json`, using `version` or its jQuery-style alternative `$.version` is sufficient.
+Otherwise, anything can be selected with JSONPath is support, so, nothing we can't do.
+The underlying JSONPath processor is [jsonpath-ng](https://github.com/h2non/jsonpath-ng).
+Checkout their document for some examples and hints.
+
+The suffix is also supported for json file:
+```ini
+[bumpsemver:json(1):example.json]
+jsonpath = version
+
+[bumpsemver:json( same file):example.json]
+jsonpath = dependencies[2].*.version
+
+[bumpsemver:json (once again):example.json]
+jsonpath = dependencies[0].*.lodash.dependencies[1].version
+```
+
+#### YAML file
+
+Comparably, YAML is supported for the same reason that we should support native JSON, like
+ ```ini
+[bumpsemver:yaml:playbook.yml]
+yamlpath = version 
+```
+OR
+```ini
+[bumpsemver:yaml(1):playbook.yml]
+yamlpath = *.vars.project_version
+
+[bumpsemver:yaml( same file):playbook.yaml]
+yamlpath = *.vars.version
+
+[bumpsemver:yaml (once again):playbook.yaml]
+yamlpath = *.vars.app_version
+```
+
+Please note that we use
+[yamlpath](https://github.com/wwkimball/yamlpath/wiki/Segments-of-a-YAML-Path#yaml-path-standard) here.
+`yamlpath` is not a popular "standard" widely adopted as `jsonpath`.
+For complex scenarios, it makes sense to test the expression with [yamlpath cli](https://pypi.org/project/yamlpath/)
+before putting anything in the config file.
+
+#### TOML file
+
+The file-specific config section looks like:
+```ini
+[bumpsemver:toml:pyproject.toml]
+tomlpath = tool.poetry.version
+```
+
+For whatever reason toml gets its acceptance and popularity, especially in the Go, Rust, and later Python community.
+Despite the unlogical fashion and religion drives, in fact we have many toml files in the wild.
+For instance `pyproject.toml` is everywhere now.
+
+We cannot even find out a "tomlpath" or similar library to read/update the properties in a toml file by giving a
+string as the "path" to the property.
+We rolled our own tomlpath processor, which is not a standard, but offering similar functionality as yamlpath.
```

### Comparing `bumpsemver-1.0.6/bumpsemver/cli.py` & `bumpsemver-2.0.0/bumpsemver/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 import argparse
 import io
 import logging
 import os
 import re
 import sre_constants
+import subprocess
 import sys
-import warnings
-from configparser import (RawConfigParser, NoOptionError)
+from configparser import NoOptionError, RawConfigParser
 from datetime import datetime
+from typing import Dict, List, Tuple, Type
 
-from bumpsemver import __version__, __title__
+from bumpsemver import __title__, __version__
 from bumpsemver.exceptions import (
-    IncompleteVersionRepresentationException,
-    MissingValueForSerializationException,
-    WorkingDirectoryIsDirtyException,
+    CannotParseVersionError,
+    InvalidConfigSectionError,
+    InvalidFileError,
+    MixedNewLineError,
+    MultiValuesMismatchError,
+    PathNotFoundError,
+    SingleValueMismatchError,
+    VersionNotFoundError,
+    WorkingDirectoryIsDirtyError,
 )
-from bumpsemver.files.generic import ConfiguredGenericFile
+from bumpsemver.files.base import FileTypeBase
 from bumpsemver.files.json import ConfiguredJSONFile
+from bumpsemver.files.text import ConfiguredPlainTextFile
+from bumpsemver.files.toml import ConfiguredTOMLFile
 from bumpsemver.files.yaml import ConfiguredYAMLFile
 from bumpsemver.git import Git
 from bumpsemver.utils import key_value_string
 from bumpsemver.version_part import VersionConfig
 
 python_version = sys.version.split("\n")[0].split(" ")[0]
 DESCRIPTION = f"{__title__}: v{__version__} (using Python v{python_version})"
 
-
 # detect either:
-# bumpsemver:yaml:value
-# bumpsemver:yaml(suffix):value
-# bumpsemver:yaml ( suffix with spaces):value
-# bumpsemver:json:value
-# bumpsemver:json(suffix):value
-# bumpsemver:json ( suffix with spaces):value
-# bumpsemver:file:value
-# bumpsemver:file(suffix):value
-# bumpsemver:file ( suffix with spaces):value
-RE_DETECT_SECTION_TYPE = re.compile(
-    r"^bumpsemver:("
-    r"(?P<file>file)(\s*\(\s*(?P<file_suffix>[^):]+)\)?)?"
-    r"|"
-    r"(?P<json>json)(\s*\(\s*(?P<json_suffix>[^):]+)\)?)?"
-    r"|"
-    r"(?P<yaml>yaml)(\s*\(\s*(?P<yaml_suffix>[^):]+)\)?)?"
-    r"):(?P<value>.+)",
+# bumpsemver:toml:value
+# bumpsemver:toml(suffix):value
+# bumpsemver:toml ( suffix with spaces):value
+RE_CONFIG_SECTION = re.compile(
+    r"^bumpsemver:((?P<file_type>.+?)(\s*\(\s*(?P<file_suffix>[^):]+)\)?)?):(?P<value>.+)",
 )
 
 logger = logging.getLogger(__name__)
 time_context = {"now": datetime.now(), "utcnow": datetime.utcnow()}
 
 OPTIONAL_ARGUMENTS_THAT_TAKE_VALUES = [
     "--config-file",
@@ -57,54 +53,96 @@
     "--search",
     "--replace",
     "--tag-name",
     "--tag-message",
 ]
 
 
-def main(original_args=None):
-    #
-    # determine configuration based on command-line arguments and on-disk configuration files
-    args, known_args, root_parser, positionals = _parse_arguments_phase_1(original_args)
-    _setup_logging(known_args.verbose)
-    vcs_info = _determine_vcs_usability()
-    defaults = _determine_current_version(vcs_info)
-    explicit_config = None
-    if hasattr(known_args, "config_file"):
-        explicit_config = known_args.config_file
-    config_file = _determine_config_file(explicit_config)
-    config, config_file_exists, config_newlines, part_configs, files = _load_configuration(config_file, explicit_config, defaults)
-    known_args, parser2, remaining_argv = _parse_arguments_phase_2(args, defaults, root_parser)
-    version_config = _setup_version_config(known_args, part_configs)
-    current_version = version_config.parse(known_args.current_version)
-    context = {**time_context, **vcs_info}
-    #
-    # calculate the desired new version
-    new_version = _assemble_new_version(context, current_version, defaults, known_args.current_version, positionals, version_config)
-    args, file_names = _parse_arguments_phase_3(remaining_argv, positionals, defaults, parser2)
-    new_version = _parse_new_version(args, new_version, version_config)
-
-    # replace version in target files
-    vcs = _determine_vcs_dirty(defaults)
-    files.extend(ConfiguredGenericFile(file_name, version_config) for file_name in (file_names or positionals[1:]))
-    _check_files_contain_version(files, current_version, context)
-    _replace_version_in_files(files, current_version, new_version, args.dry_run, context)
-    config.remove_option("bumpsemver", "new_version")
-
-    # store the new version
-    _update_config_file(config, config_file, config_newlines, config_file_exists, args.new_version, args.dry_run)
-
-    # commit and tag
-    if vcs:
-        context = _commit_to_vcs(files, config_file, config_file_exists, vcs, args, current_version, new_version)
-        _tag_in_vcs(vcs, context, args)
+class SectionConfig:
+    def __init__(self, handler: Type[FileTypeBase], xpath_supported: bool, props: Dict[str, str]):
+        self.handler = handler
+        self.xpath_supported = xpath_supported
+        self.props = props
+
+
+def main(original_args=None) -> None:
+    try:
+        #
+        # determine configuration based on command-line arguments and on-disk configuration files
+        args, known_args, root_parser, positionals = _parse_arguments_phase_1(original_args)
+        _setup_logging(known_args.verbose)
+        vcs_info = _determine_vcs_usability()
+        defaults = _determine_current_version(vcs_info)
+        explicit_config = None
+        if hasattr(known_args, "config_file"):
+            explicit_config = known_args.config_file
+        config_file = _determine_config_file(explicit_config)
+        config, config_file_exists, config_newlines, files = _load_configuration(config_file, explicit_config, defaults)
+        known_args, parser2, remaining_argv = _parse_arguments_phase_2(args, defaults, root_parser)
+        version_config = _setup_version_config(known_args)
+        current_version = version_config.parse(known_args.current_version)
+        context = {**time_context, **vcs_info}
+        #
+        # calculate the desired new version
+        new_version = _assemble_new_version(
+            current_version, defaults, known_args.current_version, positionals, version_config
+        )
+        args, file_names = _parse_arguments_phase_3(remaining_argv, positionals, defaults, parser2)
+        new_version = _parse_new_version(args, new_version, version_config)
+
+        # replace the version in target files
+        vcs = _determine_vcs_dirty(defaults)
+        files.extend(
+            ConfiguredPlainTextFile(file_name, version_config) for file_name in (file_names or positionals[1:])
+        )
+        _check_files_contain_version(files, current_version, context)
+        _replace_version_in_files(files, current_version, new_version, args.dry_run, context)
+        config.remove_option("bumpsemver", "new_version")
+
+        # store the new version
+        _update_config_file(config, config_file, config_newlines, config_file_exists, args.new_version, args.dry_run)
+
+        # commit and tag
+        if vcs:
+            context = _commit_to_vcs(files, config_file, config_file_exists, vcs, args, current_version, new_version)
+            _tag_in_vcs(vcs, context, args)
+
+        sys.exit(0)
+    except argparse.ArgumentTypeError as exc:
+        logger.error(f"{''.join(exc.args)}")
+        sys.exit(1)
+    except FileNotFoundError as exc:
+        logger.error(f"FileNotFound. {exc!s}")
+        sys.exit(2)
+    except MixedNewLineError as exc:
+        logger.warning(f"{exc.message}")
+        sys.exit(3)
+    except (
+        CannotParseVersionError,
+        InvalidConfigSectionError,
+        InvalidFileError,
+        MultiValuesMismatchError,
+        PathNotFoundError,
+        SingleValueMismatchError,
+        VersionNotFoundError,
+    ) as exc:
+        logger.error(f"{exc.message}")
+        sys.exit(4)
+    except WorkingDirectoryIsDirtyError as exc:
+        logger.error(f"{exc.message}\n\nUse --allow-dirty to override this if you know what you're doing.")
+        sys.exit(5)
+    except subprocess.CalledProcessError:
+        sys.exit(10)
+    except Exception as exc:
+        logger.error(f"Unexpected error occurred: {exc!s}")
+        sys.exit(128)
 
 
 def split_args_in_optional_and_positional(args):
-    # manually parsing positional arguments because stupid argparse can't mix positional and optional arguments
+    # manually parsing positional arguments because with argparse we cannot mix positional and optional arguments
 
     positions = []
     for i, arg in enumerate(args):
 
         previous = None
 
         if i > 0:
@@ -118,17 +156,17 @@
 
     return positionals, args
 
 
 def _parse_arguments_phase_1(original_args):
     positionals, args = split_args_in_optional_and_positional(sys.argv[1:] if original_args is None else original_args)
     if len(positionals[1:]) > 2:
-        warnings.warn(
-            "Giving multiple files on the command line will be deprecated, please use [bumpsemver:file:...] in a config file.",
-            PendingDeprecationWarning,
+        logger.warning(
+            "Giving multiple files on the command line will be deprecated, "
+            "please use [bumpsemver:plaintext:...] in a config file."
         )
     root_parser = argparse.ArgumentParser(add_help=False)
     root_parser.add_argument(
         "--config-file",
         metavar="FILE",
         default=argparse.SUPPRESS,
         required=False,
@@ -148,22 +186,23 @@
         help="Don't abort if working directory is dirty",
         required=False,
     )
     known_args, _ = root_parser.parse_known_args(args)
     return args, known_args, root_parser, positionals
 
 
-def _setup_logging(verbose):
+def _setup_logging(verbose: int) -> None:
     try:
         log_level = [logging.WARNING, logging.INFO, logging.DEBUG][verbose]
     except IndexError:
         log_level = logging.DEBUG
+    logging.basicConfig(format="%(levelname)s:%(message)s")
     root_logger = logging.getLogger("")
     root_logger.setLevel(log_level)
-    logger.debug("Starting {}‚", DESCRIPTION)
+    logger.debug(f"Starting {DESCRIPTION}")
 
 
 def _determine_vcs_usability():
     vcs_info = {}
     if Git.is_usable():
         vcs_info.update(Git.latest_tag_info())
     return vcs_info
@@ -178,88 +217,121 @@
 
 def _determine_config_file(explicit_config):
     if explicit_config:
         return explicit_config
     return ".bumpsemver.cfg"
 
 
+def _config_file_exists(config_file: str, explicit_config: bool) -> bool:
+    config_file_exists = os.path.exists(config_file)
+    if not config_file_exists:
+        message = f"Could not read config file at {config_file}"
+        if explicit_config:
+            raise argparse.ArgumentTypeError(message)
+        logger.info(message)
+        return False
+    return True
+
+
+def _check_section_config(section: str, acceptable_keys: List[str], actual_config: List[str]):
+    unknown_keys = [item for item in actual_config if item not in acceptable_keys]
+    if unknown_keys:
+        raise InvalidConfigSectionError(f"Invalid config file. Unknown keys {unknown_keys} in section '{section}'")
+
+
+def _parse_sections(config: RawConfigParser, defaults, sections):
+    file_types_config = {
+        "plaintext": SectionConfig(
+            ConfiguredPlainTextFile,
+            False,
+            {"search": "{current_version}", "replace": "{new_version}"},
+        ),
+        "file": SectionConfig(
+            ConfiguredPlainTextFile,
+            False,
+            {"search": "{current_version}", "replace": "{new_version}"},
+        ),
+        "json": SectionConfig(ConfiguredJSONFile, True, {"jsonpath": "version"}),
+        "yaml": SectionConfig(ConfiguredYAMLFile, True, {"yamlpath": "version"}),
+        "toml": SectionConfig(ConfiguredTOMLFile, True, {"tomlpath": "version"}),
+    }
+
+    files: List[FileTypeBase] = []
+
+    for section_name in sections:
+        parsed_section_header = RE_CONFIG_SECTION.match(section_name)
+
+        if not parsed_section_header:
+            continue
+
+        section_type = parsed_section_header.groupdict()
+        file_type = section_type.get("file_type")
+        filename = section_type.get("value")
+        section_props = dict(config.items(section_name))
+
+        if not [x for x in file_types_config.keys() if x == file_type]:
+            raise InvalidConfigSectionError(
+                f"Invalid config file. Unknown file type '{file_type}' in section '{section_name}'"
+            )
+
+        type_info = file_types_config.get(file_type)
+
+        _check_section_config(section_name, list(type_info.props.keys()), [*section_props])
+        if file_type == "file":
+            logger.warning("Using 'file' section type is deprecated, please use 'plaintext' instead.")
+
+        for k, v in type_info.props.items():
+            if k not in section_props:
+                section_props[k] = defaults.get(k, v)
+
+        if type_info.xpath_supported:
+            path_key = next(iter(type_info.props.keys()))
+            path = section_props.pop(path_key, None)
+            files.append(type_info.handler(filename, VersionConfig(**section_props), file_type, path))
+        else:
+            files.append(type_info.handler(filename, VersionConfig(**section_props)))
+
+    return files
+
+
 def _load_configuration(config_file, explicit_config, defaults):
     # noinspection PyTypeChecker
     config = RawConfigParser("")
     # don't transform keys to lowercase (which would be the default)
     config.optionxform = lambda option: option
     config.add_section("bumpsemver")
-    config_file_exists = os.path.exists(config_file)
 
-    if not config_file_exists:
-        message = f"Could not read config file at {config_file}"
-        if explicit_config:
-            raise argparse.ArgumentTypeError(message)
-        logger.info(message)
-        return config, config_file_exists, None, {}, []
+    if not _config_file_exists(config_file, explicit_config):
+        return config, False, None, []
 
     logger.info(f"Reading config file {config_file}:")
 
     with open(config_file, "rt", encoding="utf-8") as config_fp:
         config_content = config_fp.read()
         config_newlines = config_fp.newlines
 
     logger.info(config_content)
     config.read_string(config_content)
     log_config = io.StringIO()
     config.write(log_config)
 
     if config.has_option("bumpsemver", "files"):
-        warnings.warn(
-            "'files =' configuration will be deprecated, please use [bumpsemver:file:...]",
-            PendingDeprecationWarning,
-        )
+        logger.warning("'files =' configuration will be deprecated, please use [bumpsemver:file:...]")
 
     defaults.update(dict(config.items("bumpsemver")))
 
     for bool_value_name in ("commit", "tag", "dry_run"):
         try:
             defaults[bool_value_name] = config.getboolean("bumpsemver", bool_value_name)
         except NoOptionError:
             pass  # no default value then
 
-    part_configs = {}
-    files = []
+    files = _parse_sections(config, defaults, config.sections())
 
-    for section_name in config.sections():
-        section_type_match = RE_DETECT_SECTION_TYPE.match(section_name)
-
-        if not section_type_match:
-            continue
-
-        section_type = section_type_match.groupdict()
-        section_value = section_type.get("value")
-        section_config = dict(config.items(section_name))
-
-        filename = section_value
-
-        section_config["part_configs"] = part_configs
-
-        if section_type.get("file"):
-            if "search" not in section_config:
-                section_config["search"] = defaults.get("search", "{current_version}")
-            if "replace" not in section_config:
-                section_config["replace"] = defaults.get("replace", "{new_version}")
-            files.append(ConfiguredGenericFile(filename, VersionConfig(**section_config)))
-        elif section_type.get("json"):
-            jsonpath = section_config.pop("jsonpath", defaults.get("jsonpath", "version"))
-            files.append(ConfiguredJSONFile(filename, jsonpath, VersionConfig(**section_config)))
-        elif section_type.get("yaml"):
-            yamlpath = section_config.pop("yamlpath", defaults.get("yamlpath", "version"))
-            files.append(ConfiguredYAMLFile(filename, yamlpath, VersionConfig(**section_config)))
-        else:
-            # the other cases must not be possible, because the regex matching at the beginning of this function should filter them out
-            pass
-
-    return config, config_file_exists, config_newlines, part_configs, files
+    return config, True, config_newlines, files
 
 
 def _parse_arguments_phase_2(args, defaults, root_parser):
     parser2 = argparse.ArgumentParser(prog="bumpsemver", add_help=False, parents=[root_parser])
     parser2.set_defaults(**defaults)
     parser2.add_argument(
         "--current-version",
@@ -282,35 +354,31 @@
     known_args, remaining_argv = parser2.parse_known_args(args)
 
     defaults.update(vars(known_args))
 
     return known_args, parser2, remaining_argv
 
 
-def _setup_version_config(known_args, part_configs):
+def _setup_version_config(known_args):
     try:
-        version_config = VersionConfig(search=known_args.search, replace=known_args.replace, part_configs=part_configs)
+        version_config = VersionConfig(search=known_args.search, replace=known_args.replace)
     except sre_constants.error:
         sys.exit(1)
     return version_config
 
 
-def _assemble_new_version(context, current_version, defaults, arg_current_version, positionals, version_config):
+def _assemble_new_version(current_version, defaults, arg_current_version, positionals, version_config):
     new_version = None
     if "new_version" not in defaults and arg_current_version:
         try:
             if current_version and positionals:
                 logger.info(f"Attempting to increment part '{positionals[0]}'")
                 new_version = current_version.bump(positionals[0], version_config.order())
                 logger.info(f"Values are now: {key_value_string(new_version.values)}")
-                defaults["new_version"] = version_config.serialize(new_version, context)
-        except MissingValueForSerializationException as err:
-            logger.info(f"Opportunistic finding of new_version failed: {err.message}")
-        except IncompleteVersionRepresentationException as err:
-            logger.info(f"Opportunistic finding of new_version failed: {err.message}")
+                defaults["new_version"] = version_config.serialize(new_version)
         except KeyError:
             logger.info("Opportunistic finding of new_version failed")
     return new_version
 
 
 def _parse_arguments_phase_3(remaining_argv, positionals, defaults, parser2):
     parser3 = argparse.ArgumentParser(
@@ -391,36 +459,28 @@
         default=defaults.get("tag_name", "r{new_version}"),
     )
     parser3.add_argument(
         "--tag-message",
         metavar="TAG_MESSAGE",
         dest="tag_message",
         help="Tag message",
-        default=defaults.get(
-            "tag_message",
-            "build(repo): bumped version {current_version} → {new_version}"
-        ),
+        default=defaults.get("tag_message", "build(repo): bumped version {current_version} → {new_version}"),
     )
     parser3.add_argument(
         "--message",
         metavar="COMMIT_MSG",
         help="Commit message",
-        default=defaults.get(
-            "message", "build(repo): bumped version {current_version} → {new_version}"
-        ),
+        default=defaults.get("message", "build(repo): bumped version {current_version} → {new_version}"),
     )
     file_names = []
     if "files" in defaults:
         assert defaults["files"] is not None
         file_names = defaults["files"].split(" ")
     parser3.add_argument("part", help="Part of the version to be bumped.")
-    parser3.add_argument(
-        "files", metavar="file", nargs="*", help="Files to change",
-        default=file_names
-    )
+    parser3.add_argument("files", metavar="file", nargs="*", help="Files to change", default=file_names)
     args = parser3.parse_args(remaining_argv + positionals)
 
     if args.dry_run:
         logger.info("Dry run active, won't touch any files.")
 
     return args, file_names
 
@@ -434,31 +494,30 @@
 
 def _determine_vcs_dirty(defaults):
     if not Git.is_usable():
         return None
 
     try:
         Git.assert_non_dirty()
-    except WorkingDirectoryIsDirtyException as err:
+    except WorkingDirectoryIsDirtyError:
         if defaults["allow_dirty"]:
             return None
-        logger.warning(f"{err.message}\n\nUse --allow-dirty to override this if you know what you're doing.")
         raise
 
     return Git
 
 
-def _check_files_contain_version(files, current_version, context):
+def _check_files_contain_version(files, current_version, context: Dict[str, Tuple[str, datetime]]):
     # make sure files exist and contain version string
     logger.info(f"Asserting files {', '.join([str(f) for f in files])} contain the version string...")
     for file_item in files:
         file_item.should_contain_version(current_version, context)
 
 
-def _replace_version_in_files(files, current_version, new_version, dry_run, context):
+def _replace_version_in_files(files, current_version, new_version, dry_run, context: Dict[str, Tuple[str, datetime]]):
     # change version string in files
     for file_item in files:
         file_item.replace(current_version, new_version, context, dry_run)
 
 
 def _update_config_file(config, config_file, config_newlines, config_file_exists, new_version, dry_run):
     config.set("bumpsemver", "current_version", new_version)
@@ -472,22 +531,22 @@
         logger.info(new_config.getvalue())
 
         if write_to_config_file:
             with open(config_file, "wt", encoding="utf-8", newline=config_newlines) as config_fp:
                 config_fp.write(new_config.getvalue().strip() + "\n")
 
     except UnicodeEncodeError:
-        warnings.warn(
+        logger.warning(
             "Unable to write UTF-8 to config file, because of an old configparser version. "
             "Update with `pip install --upgrade configparser`."
         )
 
 
 def _commit_to_vcs(files, config_file, config_file_exists, vcs, args, current_version, new_version):
-    commit_files = [f.path for f in files]
+    commit_files = [f.filename for f in files]
     if config_file_exists:
         commit_files.append(config_file)
     assert vcs.is_usable(), f"Did find '{vcs.__name__}' unusable, unable to commit."
     do_commit = args.commit and not args.dry_run
     logger.info(f"{'Would prepare' if not do_commit else 'Preparing'} {vcs.__name__} commit")
     for path in commit_files:
         logger.info(f"{'Would add' if not do_commit else 'Adding'} changes in file '{path}' to {vcs.__name__}")
@@ -501,23 +560,27 @@
     }
     context.update(time_context)
     context.update({f"current_{part}": current_version[part].value for part in current_version})
     context.update({f"new_{part}": new_version[part].value for part in new_version})
 
     commit_message = args.message.format(**context)
 
-    logger.info(f"{'Would commit' if not do_commit else 'Committing'} to {vcs.__name__} with message '{commit_message}'")
+    logger.info(
+        f"{'Would commit' if not do_commit else 'Committing'} to {vcs.__name__} with message '{commit_message}'"
+    )
     if do_commit:
         vcs.commit(message=commit_message, context=context)
     return context
 
 
 def _tag_in_vcs(vcs, context, args):
     sign_tags = args.sign_tags
     tag_name = args.tag_name.format(**context)
     tag_message = args.tag_message.format(**context)
     do_tag = args.tag and not args.dry_run
-    logger.info(f"{'Would tag' if not do_tag else 'Tagging'} `{tag_name}` "
-                f"{f'with message `{tag_message}`' if tag_message else 'without message'} "
-                f"in {vcs.__name__} and {'signing' if sign_tags else 'not signing'}")
+    logger.info(
+        f"{'Would tag' if not do_tag else 'Tagging'} `{tag_name}` "
+        f"{f'with message `{tag_message}`' if tag_message else 'without message'} "
+        f"in {vcs.__name__} and {'signing' if sign_tags else 'not signing'}"
+    )
     if do_tag:
-        vcs.tag(sign_tags, tag_name, tag_message)
+        vcs.tag(tag_name, sign_tags, tag_message)
```

### Comparing `bumpsemver-1.0.6/bumpsemver/files/generic.py` & `bumpsemver-2.0.0/bumpsemver/files/text.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 import logging
+from datetime import datetime
+from typing import Dict, Union
 
-from bumpsemver.version_part import Version
-
-from bumpsemver.exceptions import VersionNotFoundException
-from bumpsemver.files import FileTypes
+from bumpsemver.exceptions import VersionNotFoundError
 from bumpsemver.files.base import FileTypeBase
+from bumpsemver.version_part import Version, VersionConfig
 
 logger = logging.getLogger(__name__)
 
 
-class ConfiguredGenericFile(FileTypeBase):
+class ConfiguredPlainTextFile(FileTypeBase):
 
-    def __init__(self, path, version_config):
-        self.path = path
-        self._version_config = version_config
-        self.file_type = FileTypes.GENERIC
-        super().__init__(path, version_config, FileTypes.GENERIC, logger)
+    def __init__(self, filename, version_config: VersionConfig):
+        super().__init__(filename, version_config, "plaintext", None, logger)
 
     def should_contain_version(self, version: Version, context: dict) -> None:
         """
         Raise VersionNotFound if the version number isn't present in this file.
 
         Return normally if the version number is in fact present.
         """
-        context["current_version"] = self._version_config.serialize(version, context)
+        context["current_version"] = self._version_config.serialize(version)
         search_expression = self._version_config.search.format(**context)
 
         if self.contains(search_expression):
             return
 
-        # the `search` pattern did not match, but the original supplied version number (representing the same version part values) might
-        # match instead.
+        # the `search` pattern did not match,
+        # but the original supplied version number (representing the same version part values) might match instead.
 
-        # check whether `search` isn't customized, i.e. should match only very specific parts of the file
+        # check whether `search` isn't customized, i.e., should match only very specific parts of the file
         search_pattern_is_default = self._version_config.search == "{current_version}"
 
         if search_pattern_is_default and self.contains(version.original):
-            # original version is present and we're not looking for something more specific -> this is accepted as a match
+            # the original version is present, and we're not looking for something more specific
+            # -> this is accepted as a match
             return
 
-        # version not found
-        raise VersionNotFoundException(f"Did not find '{search_expression}' in file: '{self.path}'")
+        raise VersionNotFoundError(search_expression, self.filename)
 
     def contains(self, search: str) -> bool:
         if not search:
             return False
 
-        with open(self.path, "rt", encoding="utf-8") as orig_fp:
+        with open(self.filename, "rt", encoding="utf-8") as orig_fp:
             search_lines = search.splitlines()
             lookbehind = []
 
             for lineno, line in enumerate(orig_fp.readlines()):
                 lookbehind.append(line.rstrip("\n"))
 
                 if len(lookbehind) > len(search_lines):
                     lookbehind = lookbehind[1:]
 
-                if search_lines[0] in lookbehind[0] and search_lines[-1] in lookbehind[-1] and search_lines[1:-1] == lookbehind[1:-1]:
-                    logger.info(f"Found '{search}' in {self.path} at line {lineno - (len(lookbehind) - 1)}: {line.rstrip()}")
+                if (
+                    search_lines[0] in lookbehind[0]
+                    and search_lines[-1] in lookbehind[-1]
+                    and search_lines[1:-1] == lookbehind[1:-1]
+                ):
+                    logger.info(
+                        f"Found '{search}' in {self.filename} at line {lineno - (len(lookbehind) - 1)}: {line.rstrip()}"
+                    )
                     return True
         return False
 
-    def replace(self, current_version: Version, new_version: Version, context: dict, dry_run: bool) -> None:
+    def replace(
+        self, current_version: Version, new_version: Version, context: Dict[str, Union[str, datetime]], dry_run: bool
+    ) -> None:
 
-        with open(self.path, "rt", encoding="utf-8") as orig_fp:
+        with open(self.filename, "rt", encoding="utf-8") as orig_fp:
             file_content_before = orig_fp.read()
 
-        context["current_version"] = self._version_config.serialize(current_version, context)
-        context["new_version"] = self._version_config.serialize(new_version, context)
+        context["current_version"] = self._version_config.serialize(current_version)
+        context["new_version"] = self._version_config.serialize(new_version)
 
         search_for = self._version_config.search.format(**context)
         replace_with = self._version_config.replace.format(**context)
 
         file_content_after = file_content_before.replace(search_for, replace_with)
 
-        if file_content_before == file_content_after:
-            file_content_after = file_content_before.replace(current_version.original, replace_with)
-
         self.update_file(file_content_before, file_content_after, dry_run)
 
     def __repr__(self):
-        return f"<bumpsemver.files.ConfiguredGenericFile:{self.path}>"
+        return f"<bumpsemver.files.ConfiguredPlainTextFile:{self.filename}>"
```

### Comparing `bumpsemver-1.0.6/bumpsemver/files/json.py` & `bumpsemver-2.0.0/bumpsemver/files/json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,88 @@
-import collections
 import io
 import json
 import logging
-from json import JSONDecodeError
+from datetime import datetime
+from typing import Dict, Union
 
 from jsonpath_ng import parse
+from jsonpath_ng.lexer import JsonPathLexerError
 
-from bumpsemver.version_part import Version
-from bumpsemver.exceptions import VersionNotFoundException
-from bumpsemver.files import FileTypes
+from bumpsemver.exceptions import (
+    InvalidFileError,
+    MultiValuesMismatchError,
+    PathNotFoundError,
+    SingleValueMismatchError,
+)
 from bumpsemver.files.base import FileTypeBase
+from bumpsemver.version_part import Version, VersionConfig
 
 logger = logging.getLogger(__name__)
 
 
 def _get_json_value(obj, path):
     json_path_expr = parse(path)
-    match = json_path_expr.find(obj)
-    return match[0].value
+    return [item.value for item in json_path_expr.find(obj)]
 
 
 def _set_json_value(obj, path, value):
     json_path_expr = parse(path)
-    json_path_expr.find(obj)
     json_path_expr.update(obj, value)
 
 
 class ConfiguredJSONFile(FileTypeBase):
-    def __init__(self, path, jsonpath, version_config):
-        super().__init__(path, version_config, FileTypes.JSON, logger)
-        self.json_path = jsonpath
+    def __init__(self, filename: str, version_config: VersionConfig, file_type="json", jsonpath: str = None):
+        super().__init__(filename, version_config, file_type, jsonpath, logger)
 
     def should_contain_version(self, version: Version, context: dict) -> None:
-        current_version = self._version_config.serialize(version, context)
+        current_version = self._version_config.serialize(version)
         context["current_version"] = current_version
 
         if self.contains(current_version):
             return
 
-        # version not found
-        raise VersionNotFoundException(f"Did not find '{current_version}' at jsonpath '{self.json_path}' in file: '{self.path}'")
-
     def contains(self, search: str) -> bool:
         try:
-            with io.open(self.path, "rt", encoding="utf-8") as orig_fp:
+            with io.open(self.filename, "rt", encoding="utf-8") as orig_fp:
                 data = json.load(orig_fp)
-            return _get_json_value(data, self.json_path) == search
-        except LookupError as err:
-            logger.error(f"invalid path expression: {str(err)}", exc_info=err)
-            return False
-        except JSONDecodeError as err:
-            raise err
-
-    def replace(self, current_version: Version, new_version: Version, context: dict, dry_run: bool) -> None:
-        with io.open(self.path, "rt", encoding="utf-8") as orig_fp:
+            nodes = _get_json_value(data, self.xpath)
+            if (len(nodes) == 1 and nodes[0] != search) or len(nodes) == 0:
+                raise SingleValueMismatchError(self.xpath, "json", self.filename, nodes[0], search)
+            else:
+                for node in nodes:
+                    if node != search:
+                        raise MultiValuesMismatchError(self.xpath, "json", self.filename, nodes, search)
+            return True
+        except (JsonPathLexerError, LookupError) as exc:
+            raise PathNotFoundError(self.xpath, "json", self.filename) from exc
+        except json.JSONDecodeError as exc:
+            raise InvalidFileError(self.filename, "json") from exc
+
+    def replace(
+        self, current_version: Version, new_version: Version, context: Dict[str, Union[str, datetime]], dry_run: bool
+    ) -> None:
+        with io.open(self.filename, "rt", encoding="utf-8") as orig_fp:
             file_content_before = orig_fp.read()
-            # the object_pairs_hook allows us to load the json in a way that key order is preserved and will keep the file diff
-            # to a minimum
+            # the object_pairs_hook allows us to load the json in a way that key order
+            # is preserved and will keep the file diff to a minimum
             #
-            # noinspection PyTypeChecker
-            data = json.loads(file_content_before, object_pairs_hook=collections.OrderedDict)
+            data = json.loads(file_content_before)
 
-        current_version = self._version_config.serialize(current_version, context)
-        context["current_version"] = current_version
-        new_version = self._version_config.serialize(new_version, context)
-        context["new_version"] = new_version
+        current_version_str = self._version_config.serialize(current_version)
+        context["current_version"] = current_version_str
+        new_version_str = self._version_config.serialize(new_version)
+        context["new_version"] = new_version_str
 
-        if _get_json_value(data, self.json_path) == current_version:
-            _set_json_value(data, self.json_path, new_version)
+        _set_json_value(data, self.xpath, new_version_str)
         # ensure_ascii: we're writing utf-8 files, so we don't need ascii support
-        # allow_nan: JSON does not have an understanding of infinity or nan, so it’s forbidden
+        # allow_nan: JSON does not have an understanding of infinity or nan, so it is forbidden
         # indent: indent of 2 spaces is common practise
-        # separators: the default separators leave a trailing space after every comma. when using indentation, this results in awkward
-        #             line-endings with a leading space
-        file_content_after = json.dumps(data, ensure_ascii=False, allow_nan=False, indent=2, separators=(",", ": ")) + "\n"
+        # separators: the default separators leave a trailing space after every comma. when using indentation,
+        #             this results in awkward line-endings with a leading space
+        file_content_after = (
+            json.dumps(data, ensure_ascii=False, allow_nan=False, indent=2, separators=(",", ": ")) + "\n"
+        )
 
         self.update_file(file_content_before, file_content_after, dry_run)
 
     def __repr__(self):
-        return f"<bumpsemver.files.ConfiguredJSONFile:{self.path}>"
+        return f"<bumpsemver.files.ConfiguredJSONFile:{self.filename}>"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bumpsemver-1.0.6/bumpsemver/files/yaml.py` & `bumpsemver-2.0.0/bumpsemver/files/toml.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,69 @@
 import logging
-from types import SimpleNamespace
+from datetime import datetime
+from typing import Dict, Union
 
-from ruamel.yaml.compat import StringIO
-from yamlpath import Processor, YAMLPath
-from yamlpath.common import Parsers
-from yamlpath.exceptions import YAMLPathException
-from yamlpath.wrappers import ConsolePrinter
+from tomlkit.exceptions import EmptyKeyError, KeyAlreadyPresent, NonExistentKey, ParseError, UnexpectedCharError
 
-from bumpsemver.exceptions import BumpVersionException, VersionNotFoundException
-from bumpsemver.files import FileTypes
+from bumpsemver.exceptions import (
+    InvalidFileError,
+    MultiValuesMismatchError,
+    PathNotFoundError,
+    SingleValueMismatchError,
+)
 from bumpsemver.files.base import FileTypeBase
-from bumpsemver.version_part import Version
+from bumpsemver.files.tomlpath import TomlPath
+from bumpsemver.version_part import Version, VersionConfig
 
 logger = logging.getLogger(__name__)
 
 
-class InvalidYAMLException(BumpVersionException):
-    def __init__(self, message):
-        super().__init__(message)
-        self.message = message
-
-
-class ConfiguredYAMLFile(FileTypeBase):
-    def __init__(self, path, yamlpath, version_config):
-        super().__init__(path, version_config, FileTypes.YAML, logger)
-        self.yaml = Parsers.get_yaml_editor()
-        self.yaml_path = yamlpath
-        self.yaml_logging_args = SimpleNamespace(quiet=True, verbose=False, debug=False)
-        self.yaml_log = ConsolePrinter(self.yaml_logging_args)
+class ConfiguredTOMLFile(FileTypeBase):
+    def __init__(self, filename: str, version_config: VersionConfig, file_type="toml", tomlpath: str = None):
+        super().__init__(filename, version_config, file_type, tomlpath, logger)
 
     def should_contain_version(self, version: Version, context: dict) -> None:
-        current_version = self._version_config.serialize(version, context)
+        current_version = self._version_config.serialize(version)
         context["current_version"] = current_version
 
-        if self.contains(current_version):
-            return
-
-        # version not found
-        raise VersionNotFoundException(f"Did not find '{current_version}' at yamlpath '{self.yaml_path}' in file: '{self.path}'")
-
-    def contains(self, search: str) -> bool:
         try:
-            processor = self.__get_processor()
-            yaml_path = YAMLPath(self.yaml_path)
-            nodes_found = list(processor.get_nodes(yaml_path, mustexist=True))
-            matched = True
-            for node in nodes_found:
-                if node.node != search:
-                    matched = False
-            return matched
-        except YAMLPathException as ex:
-            logger.error(f"invalid path expression: {str(ex)}", exc_info=ex)
-            return False
-
-    def __dump(self, data) -> str:
-        stream = StringIO()
-        self.yaml.dump(data, stream)
-        return stream.getvalue()
-
-    def __get_processor(self):
-        (yaml_data, doc_loaded) = Parsers.get_yaml_data(self.yaml, self.yaml_log, self.path)
-        if not doc_loaded:
-            raise InvalidYAMLException(f"Failed in reading YAML file '{self.path}'")
-        processor = Processor(self.yaml_log, yaml_data)
-        return processor
-
-    def replace(self, current_version: Version, new_version: Version, context: dict, dry_run: bool) -> None:
-        processor = self.__get_processor()
-        file_content_before = self.__dump(processor.data)
+            self.contains(current_version)
+        except KeyError:
+            pass
 
-        current_version = self._version_config.serialize(current_version, context)
-        context["current_version"] = current_version
-        new_version = self._version_config.serialize(new_version, context)
-        context["new_version"] = new_version
-
-        yaml_path = YAMLPath(self.yaml_path)
-        for node in processor.get_nodes(yaml_path, mustexist=True):
-            if node.node == current_version:
-                processor.set_value(node.path, new_version)
-
-        file_content_after = self.__dump(processor.data)
+    def contains(self, search: str) -> bool:
+        if not TomlPath.is_valid(self.xpath):
+            raise PathNotFoundError(self.xpath, "toml", self.filename) from None
 
-        self.update_file(file_content_before, file_content_after, dry_run)
+        try:
+            with open(self.filename, "rt") as fin:
+                content = fin.read()
+                value = TomlPath.query(content, self.xpath)
+                if value is None or value == []:
+                    raise NonExistentKey(self.xpath)
+                if isinstance(value, list):
+                    for item in value:
+                        if item != search:
+                            raise MultiValuesMismatchError(self.xpath, "toml", self.filename, value, search)
+                elif value != search:
+                    raise SingleValueMismatchError(self.xpath, "toml", self.filename, value, search)
+                return True
+        except (EmptyKeyError, KeyAlreadyPresent, ParseError, UnexpectedCharError) as exc:
+            raise InvalidFileError(self.filename, "toml") from exc
+        except (IndexError, NonExistentKey) as exc:
+            raise PathNotFoundError(self.xpath, "toml", self.filename) from exc
+
+    def replace(
+        self, current_version: Version, new_version: Version, context: Dict[str, Union[str, datetime]], dry_run: bool
+    ) -> None:
+        current_version_str = self._version_config.serialize(current_version)
+        context["current_version"] = current_version_str
+        new_version_str = self._version_config.serialize(new_version)
+        context["new_version"] = new_version_str
+
+        with open(self.filename, "rt") as fin:
+            content = fin.read()
+            value = TomlPath.update(content, self.xpath, new_version_str)
+            self.update_file(content, value, dry_run)
 
     def __repr__(self):
-        return f"<bumpsemver.ConfiguredYAMLFile:{self.path}>"
+        return f"<bumpsemver.files.ConfiguredTOMLFile:{self.filename}>"
```

### Comparing `bumpsemver-1.0.6/bumpsemver/functions.py` & `bumpsemver-2.0.0/bumpsemver/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import re
 
 
 class NumericFunction:
     """
     This is a class that provides a numeric function for version parts.
-    It simply starts with the provided first_value (0 by default) and increases it following the sequence of integer numbers.
+    It simply starts with the provided first_value (0 by default) and increases it following the sequence of
+    integer numbers.
 
-    This function also supports alphanumeric parts, altering just the numeric part (e.g. 'r3' --> 'r4'). Only the first numeric group
-    found in the part is considered (e.g. 'r3-001' --> 'r4-001').
+    This function also supports alphanumeric parts, altering just the numeric part (e.g. 'r3' --> 'r4').
+    Only the first numeric group found in the part is considered (e.g. 'r3-001' --> 'r4-001').
     """
 
     FIRST_NUMERIC = re.compile(r"([^\d]*)(\d+)(.*)")
 
     def __init__(self, first_value=None):
 
         if first_value is not None:
             try:
                 _, _, _ = self.FIRST_NUMERIC.search(first_value).groups()
             except AttributeError:
-                # pylint: disable=raise-missing-from
-                raise ValueError(f"The given first value {first_value} does not contain any digit")
+                raise ValueError(f"The given first value {first_value} does not contain any digit") from None
         else:
             first_value = 0
 
         self.first_value = str(first_value)
 
     def bump(self, value):
         part_prefix, part_numeric, part_suffix = self.FIRST_NUMERIC.search(value).groups()
```

### Comparing `bumpsemver-1.0.6/bumpsemver/git.py` & `bumpsemver-2.0.0/bumpsemver/git.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 import errno
 import logging
 import os
 import subprocess
+from pathlib import Path
 from tempfile import NamedTemporaryFile
+from typing import Optional, Union
 
-from bumpsemver.exceptions import (WorkingDirectoryIsDirtyException)
+from bumpsemver.exceptions import WorkingDirectoryIsDirtyError
 
 logger = logging.getLogger(__name__)
 
 
 class Git:
 
     @classmethod
-    def commit(cls, message, context, extra_args=None):
+    def commit(cls, message: str, context, extra_args=None):
         extra_args = extra_args or []
         with NamedTemporaryFile("wb", delete=False) as temp_fp:
             temp_fp.write(message.encode("utf-8"))
         env = os.environ.copy()
         for key in ("current_version", "new_version"):
             env[str("BUMPSEMVER_" + key.upper())] = str(context[key])
         try:
-            subprocess.check_output(["git", "commit", "-F", temp_fp.name] + extra_args, env=env)
+            subprocess.check_output(["git", "commit", "-F", temp_fp.name, *extra_args], env=env)
         except subprocess.CalledProcessError as exc:
             err_msg = f"Failed to run {exc.cmd}: return code {exc.returncode}, output: {exc.output}"
             logger.exception(err_msg)
             raise exc
         finally:
             os.unlink(temp_fp.name)
 
     @classmethod
     def is_usable(cls):
         try:
-            return subprocess.call(["git", "rev-parse", "--git-dir"], stderr=subprocess.PIPE, stdout=subprocess.PIPE) == 0
+            return (
+                subprocess.call(["git", "rev-parse", "--git-dir"], stderr=subprocess.PIPE, stdout=subprocess.PIPE) == 0
+            )
         except OSError as err:
             if err.errno in (errno.ENOENT, errno.EACCES):
                 return False
-            raise
 
     @classmethod
     def assert_non_dirty(cls):
         lines = [
             line.strip()
             for line in subprocess.check_output(["git", "status", "--porcelain"]).splitlines()
             if not line.strip().startswith(b"??")
         ]
 
         if lines:
-            raise WorkingDirectoryIsDirtyException("Git working directory is not clean:\n{}".format(b"\n".join(lines).decode()))
+            raise WorkingDirectoryIsDirtyError(lines)
 
     @classmethod
     def latest_tag_info(cls):
         try:
             # git-describe doesn't update the git-index, so we do that
             subprocess.check_output(["git", "update-index", "--refresh"])
 
@@ -84,19 +87,19 @@
         info["commit_sha"] = describe_out.pop().lstrip("g")
         info["distance_to_latest_tag"] = int(describe_out.pop())
         info["current_version"] = "-".join(describe_out).lstrip("r")
 
         return info
 
     @classmethod
-    def add_path(cls, path):
-        subprocess.check_output(["git", "add", "--update", path])
+    def add_path(cls, path: Union[str, Path]):
+        subprocess.check_output(["git", "add", "--update", str(path)])
 
     @classmethod
-    def tag(cls, sign, name, message):
+    def tag(cls, name: str, sign: bool = False, message: Optional[str] = None) -> None:
         """
         Create a tag of the new_version in Git.
 
         If only name is given, bumpversion uses a lightweight tag.
         Otherwise, it utilizes an annotated tag.
         """
         command = ["git", "tag", name]
```

### Comparing `bumpsemver-1.0.6/bumpsemver/version_part.py` & `bumpsemver-2.0.0/bumpsemver/version_part.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import logging
 import re
 import string
+from typing import Dict, List, Optional
 
-from bumpsemver.exceptions import (MissingValueForSerializationException, IncompleteVersionRepresentationException)
+from bumpsemver.exceptions import (
+    CannotParseVersionError,
+)
 from bumpsemver.functions import NumericFunction
 from bumpsemver.utils import key_value_string
 
 logger = logging.getLogger(__name__)
 
 
 class NumericVersionPartConfiguration:
     function_cls = NumericFunction
 
-    def __init__(self, *args, **kwds):
-        self.function = self.function_cls(*args, **kwds)
+    def __init__(self, *args, **kwargs):
+        self.function = self.function_cls(*args, **kwargs)
 
     @property
     def first_value(self):
         return str(self.function.first_value)
 
-    def bump(self, value=None):
+    def bump(self, value=None) -> str:
         return self.function.bump(value)
 
 
 class VersionPart:
     """
     This class represents part of a version number. It contains a self.config
     object that rules how the part behaves when increased or reset.
     """
 
-    def __init__(self, value, config=None):
+    def __init__(self, value: str, config=None):
         self._value = value
 
         if config is None:
             config = NumericVersionPartConfiguration()
 
         self.config = config
 
@@ -57,15 +60,15 @@
         return self.value == other.value
 
     def null(self):
         return VersionPart(self.config.first_value, self.config)
 
 
 class Version:
-    def __init__(self, values, original=None):
+    def __init__(self, values: Dict[str, VersionPart], original=None):
         self.values = dict(values)
         self.original = original
 
     def __getitem__(self, key):
         return self.values[key]
 
     def __len__(self):
@@ -73,15 +76,15 @@
 
     def __iter__(self):
         return iter(self.values)
 
     def __repr__(self):
         return f"<bumpsemver.Version:{key_value_string(self.values)}>"
 
-    def bump(self, part_name, order):
+    def bump(self, part_name: str, order: List[str]):
         bumped = False
 
         new_values = {}
 
         for label in order:
             if label not in self.values:
                 continue
@@ -95,107 +98,79 @@
 
         new_version = Version(new_values)
 
         return new_version
 
 
 def labels_for_format(serialize_format):
-    return (
-        label for _, label, _, _ in string.Formatter().parse(serialize_format)
-        if label
-    )
+    return (label for _, label, _, _ in string.Formatter().parse(serialize_format) if label)
 
 
 class VersionConfig:
     """
-    Holds a complete representation of a version string
+    Holds a complete representation of a version string.
     """
 
-    def __init__(self, search=None, replace=None, part_configs=None):
-
+    def __init__(
+        self,
+        search: str = None,
+        replace: str = None,
+    ):
         self.parse_regex = re.compile(r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)", re.VERBOSE)
         self.serialize_format = "{major}.{minor}.{patch}"
 
-        if not part_configs:
-            part_configs = {}
-
-        self.part_configs = part_configs
         self.search = search
         self.replace = replace
 
     def order(self):
-        # currently, order depends on the first given serialization format this seems like a good idea because this should be the most
-        # complete format
+        # currently, order depends on the first given serialization format this seems like enough
+        # because this should be the most complete format
         return labels_for_format(self.serialize_format)
 
-    def parse(self, version_string):
+    def parse(self, version_string: str = None) -> Optional[Version]:
         if not version_string:
             return None
 
         regexp_one_line = "".join([line.split("#")[0].strip() for line in self.parse_regex.pattern.splitlines()])
 
         logger.info(f"Parsing version '{version_string}' using regexp '{regexp_one_line}'")
 
         match = self.parse_regex.search(version_string)
 
         _parsed = {}
         if not match:
-            logger.warning(f"Evaluating 'parse' option: '{self.parse_regex.pattern}' does not parse current version '{version_string}'")
+            logger.warning(
+                f"Evaluating 'parse' option: '{self.parse_regex.pattern}' "
+                f"does not parse current version '{version_string}'"
+            )
             return None
 
         for key, value in match.groupdict().items():
-            _parsed[key] = VersionPart(value, self.part_configs.get(key))
+            _parsed[key] = VersionPart(value, None)
 
         version = Version(_parsed, version_string)
 
         logger.info(f"Parsed the following values: {key_value_string(version.values)}")
 
         return version
 
-    def _serialize(self, version, serialize_format, context, raise_if_incomplete=False):
+    # noinspection PyMethodMayBeStatic
+    def _serialize(self, version: Version, serialize_format: str) -> str:
         """
         Attempts to serialize a version with the given serialization format.
-
-        Raises MissingValueForSerializationException if not serializable
         """
-        values = context.copy()
+        values: Dict[str, VersionPart] = {}
         for key in version:
             values[key] = version[key]
 
-        try:
-            # test whether all parts required in the format have values
-            serialized = serialize_format.format(**values)
-
-        except KeyError as err:
-            missing_key = getattr(err, "message", err.args[0])
-            # pylint: disable=raise-missing-from
-            raise MissingValueForSerializationException(
-                f"Did not find key {repr(missing_key)} in {repr(version)} when serializing version number"
-            )
-
-        keys_needing_representation = set()
-
-        for key in self.order():
-            value = values[key]
-
-            if not isinstance(value, VersionPart):
-                # values coming from environment variables don't need representation
-                continue
-
-            keys_needing_representation.add(key)
-
-        required_by_format = set(labels_for_format(serialize_format))
-
-        # try whether all parsed keys are represented
-        if raise_if_incomplete:
-            if not keys_needing_representation <= required_by_format:
-                raise IncompleteVersionRepresentationException(
-                    "Could not represent '{}' in format '{}'".format("', '".join(keys_needing_representation ^ required_by_format),
-                                                                     serialize_format)
-                )
+        # test whether all parts required in the format have values
+        serialized = serialize_format.format(**values)
 
         return serialized
 
-    def serialize(self, version, context):
-        serialized = self._serialize(version, self.serialize_format, context)
-        logger.debug(f"Serialized to '{serialized}'")
-        return serialized
+    def serialize(self, version: Version) -> str:
+        try:
+            serialized = self._serialize(version, self.serialize_format)
+            logger.debug(f"Serialized to '{serialized}'")
+            return serialized
+        except TypeError as exc:
+            raise CannotParseVersionError() from exc
```

### Comparing `bumpsemver-1.0.6/bumpsemver.egg-info/PKG-INFO` & `bumpsemver-2.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,295 +1,413 @@
 Metadata-Version: 2.1
 Name: bumpsemver
-Version: 1.0.6
-Summary: Bump semver for git repos with a single command.
+Version: 2.0.0
+Summary: Bump semver for git repos with a single command
 Home-page: https://github.com/zhaow-de/bumpsemver
+License: MIT
+Keywords: bumpsemver,semver,version,release
 Author: Zhao Wang
 Author-email: zhaow.km@gmail.com
-License: UNKNOWN
-Description: 
-        # bumpsemver
-        
-        **Current version: 1.0.6**
-        
-        A utility to simplify the version bumping for git repos.
-        
-        This application is a rework of the famous `bumpversion` tool. The  
-        [original repo](https://github.com/peritus/bumpversion) seems like abandoned. Several fundamental changes are
-        introduced, which make the fork-and-extend approach infeasible:
-        1. dropped Python 2 support
-        2. boosted the test coverage to 95%+
-        3. dropped many irrelevant features to reduce complexity. (e.g. customized version component support)
-        4. introduced JSON support to make it work for package-lock.json, YAML support to make it work for Ansible plays
-        5. narrowed the versioning scheme to semver-only
-        
-        ## Installation
-        
-        ```bash
-        pip3 install bumpsemver
-        ```
-        
-        ## Usage
-        
-        This application supports both the CLI mode and config file mode.
-        
-        ### Command Line Interface
-        
-        ```bash
-        bumpsemver [options] part [file]
-        ```
-            
-        #### `options`
-        _**(optional)**_<br />
-          
-        Most of the configuration values described below can also be given as an option on the command-line.
-        Additionally, the following options are available:
-        
-        `--dry-run`
-          Don't touch any files, just pretend. Best used with `--verbose`.
-        
-        `--allow-dirty`
-          Normally, bumpsemver will abort if the working directory is dirty to protect
-          yourself from releasing unversioned files and/or overwriting unsaved changes.
-          Use this option to override this check.
-        
-        `--verbose`
-          Print useful information to stderr
-        
-        `-h, --help`
-          Print help and exit
-        
-        #### `part`
-        _**required**_<br />
-        
-        The part of the version to increase. As we support semver only, the valid values include: `major`, `minor`, and `patch`.
-        
-        For example, bumping file `src/VERSION` from 0.5.1 to 0.6.0:
-        
-        ```bash
-        bumpsemver --current-version 0.5.1 minor src/VERSION
-        ```
-        
-        #### `file`
-        _**(optional)**_<br />
-        **default**: none
-        
-        The file that will be modified.
-        
-        If not given, the list of `[bumpsemver:file:…]` sections from the configuration file will be used. If no files are
-        mentioned on the configuration file either, then no files will be modified.
-        
-        For example, bumping file `setup.py` from 1.1.9 to 2.0.0:
-        ```
-        bumpsemver --current-version 1.1.9 major setup.py
-        ```
-        
-        ### Configuration file
-        
-        Options on the command line take precedence over those from the config file, which take precedence over those from the
-        defaults.
-        
-        Example `.bumpsemver.cfg`:
-        
-        ```ini
-        [bumpsemver]
-        current_version = 0.2.9
-        commit = True
-        tag = True
-        
-        [bumpsemver:file:README]
-        ```
-        
-        #### `.bumpsemver.cfg` -- Global configuration
-        
-        General configuration is grouped in a `[bumpsemver]` section.
-        
-        ##### `current_version` 
-        _**required**_<br />
-        **default**: none
-        
-        The current version of the software package before bumping.
-        
-        Also available as CLI argument `--current-version` (e.g. `bumpsemver --current-version 0.5.1 patch`)
-        
-        ##### `tag = (True | False)`
-        _**(optional)**_<br />
-        **default**: False (Don't create a git tag)
-        
-        Whether to create a git tag, that is the new version, prefixed with the character "`r`". Don't forget to `git-push`
-        with the `--tags` flag.
-        
-        Also available as CLI argument `--tag` or `--no-tag`.
-        
-        ##### `sign_tags = (True | False)`
-        _**(optional)**_<br />
-        **default**: False (Don't sign tags)
-        
-        Whether to sign tags.
-        
-        Also available as CLI argument `--sign-tags` or `--no-sign-tags`.
-        
-        ##### `tag_name =`
-        _**(optional)**_<br />
-        **default:** `v{new_version}`
-        
-        The name of the tag that will be created. Only valid when `tag = True`.
-        
-        It can be a template using the [Python Format String Syntax](https://docs.python.org/3/library/string.html#format-string-syntax).  
-        Available in the template context are `current_version` and `new_version` as well as `current_[part]` and `new_[part]`
-        (e.g. '`current_major`' or '`new_patch`'). You can also use the variables `now` or `utcnow` to get a current timestamp.
-        Both accept datetime formatting (when used like as in `{now:%d.%m.%Y}`).
-        
-        Also available as CLI argument `--tag-name`, for example: `bumpsemver --tag-name 'release-{new_version}' patch`
-        
-        In addition, it is also possible to provide a tag message by using CLI `--tag-message TAG_MESSAGE`. Example usage:
-        `bumpsemver --tag-name 'release-{new_version}' --tag-message "Release {new_version}" patch`
-        
-        If neither tag message or sign tag is provided, we use a `lightweight` tag in git. Otherwise, we utilize an `annotated`
-        git tag. Read more about Git tagging [here](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
-        
-        ##### `commit = (True | False)`
-        _**(optional)**_<br />
-        **default:** False (Don't create a commit)
-        
-        Create a commit using git when true.
-        
-        Also available as CLI argument `--commit` or `--no-commit`.
-        
-        ##### `message =`
-        _**(optional)**_<br />
-        **default:** `[OPS] bumped version: {current_version} → {new_version}`
-        
-        The commit message to use when creating a commit. Only valid when using `--commit` / `commit = True`.
-        
-        It can be a template using the [Python Format String Syntax](https://docs.python.org/3/library/string.html#format-string-syntax).  
-        Available in the template context are `current_version` and `new_version` as well as `current_[part]` and `new_[part]`
-        (e.g. '`current_major`' or '`new_patch`'). You can also use the variables `now` or `utcnow` to get a current timestamp.
-        Both accept datetime formatting (when used like as in `{now:%d.%m.%Y}`).
-        
-        Also available as CLI argument `--message`, for example: `bumpsemver --tag-name 'release-{new_version}' patch`
-        
-        In addition, it is also possible to provide a tag message by using CLI `--tag-message TAG_MESSAGE`. Example usage:
-        `bumpsemver --message '[{now:%Y-%m-%d}] Jenkins Build {$BUILD_NUMBER}: {new_version}' patch`
-        
-        #### `.bumpsemver.cfg` -- File specific configuration
-        
-        This configuration is in the section: `[bumpsemver:file:…]` or `[bumpsemver:json:…]`
-        
-        Note: The configuration file format requires each section header to be unique. If you want to process a certain file
-        multiple times (e.g. multiple location to be replaced separately), you may append a description between parens to the
-        `file` keyword: `[bumpsemver:file (special one):…]`. It does not matter what inside the parens, just make it unique.
-        e.g.
-        
-        ```ini
-        [bumpsemver:file(1):README.md]
-        search = current version: {current_version}
-        replace = current version: {new_version}
-        
-        [bumpsemver:file(2):README.md]
-        search = **Version: {current_version}**
-        replace = current version: {new_version}
-        ```
-        
-        ##### `search =`
-        **default:** `{current_version}`
-        
-        Template string how to search for the string to be replaced in the file. Useful if the remotest possibility exists that
-        the current version number might be present multiple times in the file and you mean to only bump one of the occurrences.
-        
-        #### `replace =`
-        **default:** `{new_version}`
-        
-        Template to create the string that will replace the current version number in the file.
-        
-        Given this `requirements.txt`:
-        ```
-            Django>=1.5.6,<1.6
-            MyProject==1.5.6
-        ```
-        using the following `.bumpsemver.cfg` will ensure only the line containing `MyProject` will be changed:
-        ```ini
-        [bumpsemver]
-        current_version = 1.5.6
-        
-        [bumpsemver:file:requirements.txt]
-        search = MyProject=={current_version}
-        replace = MyProject=={new_version}
-        ```
-        
-        With `[bumpsemver:file:…]`, the specified file is processed as plain text file, which in fact makes this application
-        programming language neutral. However, it will be very error prone for complex file for example `package-lock.json`.
-        
-        For randomly sampled 30 projects written in node.js/TypeScript, the classical `bumpversion` or the renovated `bump2version` both made
-        100% mistakes which changed something shouldn't be changed. A typical and relatively complex React projects contains 1000+ npm packages  
-        indirectly. There are too many "version": "1.2.3" in that file. To address this issue, `bumpsemver` added the support of json file.
-        
-        To use it:
-         ```ini
-        [bumpsemver:json:package-lock.json]
-        jsonpath = version 
-        ```
-        
-        Value of the parameter `jsonpath` is a [JSONPath](https://goessner.net/articles/JsonPath/) string. For the typical
-        `package.json` or `package-lock.json`, using `version` or its jQuery-style alternative `$.version` is sufficient.
-        Otherwise, anything can be selected with JSONPath is support, so, nothing we can't do. The underlying JSONPath processor
-        is [jsonpath-ng](https://github.com/h2non/jsonpath-ng). Checkout their document for some examples and hints.
-        
-        The suffix is also supported for json file:
-        ```ini
-        [bumpsemver:json(1):example.json]
-        jsonpath = version
-        
-        [bumpsemver:json( same file):example.json]
-        jsonpath = dependencies[2].*.version
-        
-        [bumpsemver:json (once again):example.json]
-        jsonpath = dependencies[0].*.lodash.dependencies[1].version
-        ```
-        
-        Comparably, YAML is supported for the same reason that we should support native JSON, like
-         ```ini
-        [bumpsemver:yaml:playbook.yml]
-        yamlpath = version 
-        ```
-        OR
-        ```ini
-        [bumpsemver:yaml(1):playbook.yml]
-        yamlpath = *.vars.project_version
-        
-        [bumpsemver:yaml( same file):playbook.yaml]
-        yamlpath = *.vars.version
-        
-        [bumpsemver:yaml (once again):playbook.yaml]
-        yamlpath = *.vars.app_version
-        ```
-        Please note that we use [yamlpath](https://github.com/wwkimball/yamlpath/wiki/Segments-of-a-YAML-Path#yaml-path-standard) instead of
-        `jsonpath` here. `yamlpath` is not a popular "standard" widely adopted. For complex scenarios, it makes sense to test the expression with
-        [yamlpath cli](https://pypi.org/project/yamlpath/) before putting anything in the config file.
-        
-        ## Test
-        
-        Test in Docker container (recommended):
-        ```bash
-        make test
-        ```
-        
-        Local test in the working environment (not recommended):
-        ```bash
-        tox
-        ```
-        
-        To test the compatibility with a specific version of Python, put the version(s) into `./python-versions.txt` one version
-        per line. Then run:
-        ```bash
-        make test
-        ```
-        
-Platform: UNKNOWN
+Requires-Python: >=3.10,<4
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Version Control
+Classifier: Topic :: System :: Software Distribution
+Requires-Dist: jsonpath-ng
+Requires-Dist: ruamel.yaml
+Requires-Dist: tomlkit
+Requires-Dist: yamlpath
+Project-URL: Repository, https://github.com/zhaow-de/bumpsemver
 Description-Content-Type: text/markdown
+
+# bumpsemver
+
+[![image](https://img.shields.io/pypi/v/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
+[![image](https://img.shields.io/pypi/l/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
+[![image](https://img.shields.io/pypi/pyversions/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
+[![codecov](https://codecov.io/gh/zhaow-de/bumpsemver/graph/badge.svg?token=WP4O30YLO3)](https://codecov.io/gh/zhaow-de/bumpsemver)
+[![GitHub Actions](https://github.com/zhaow-de/bumpsemver/workflows/CI/badge.svg)](https://github.com/zhaow-de/bumpsemver/actions)
+
+
+Current version: **2.0.0**
+
+## Table of contents
+
+<!--TOC-->
+
+- [Overview](#overview)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Command Line Interface](#command-line-interface)
+- [Configuration file](#configuration-file)
+  - [General config section](#general-config-section)
+  - [File-specific config sections](#file-specific-config-sections)
+  - [File types supported in the file-specific config section](#file-types-supported-in-the-file-specific-config-section)
+    - [Plain text file](#plain-text-file)
+    - [JSON file](#json-file)
+    - [YAML file](#yaml-file)
+    - [TOML file](#toml-file)
+
+<!--TOC-->
+
+## Overview
+
+A utility to simplify the version bumping for git repos.
+
+This application is a rework of the famous `bumpversion` tool. The  
+[original repo](https://github.com/peritus/bumpversion) seems like abandoned. Several fundamental changes are
+introduced, which make the fork-and-extend approach infeasible:
+1. dropped Python 2 support
+2. boosted the test coverage to 95%+
+3. dropped many irrelevant features to reduce complexity. (e.g. customized version component support)
+4. introduced JSON support to make it work for package-lock.json
+5. introduced YAML support to make it work for Ansible playbooks
+6. introduced TOML support to make it work for pyproject.toml 
+7. narrowed the versioning scheme to semver-only
+
+## Installation
+
+```bash
+pip install --upgrade bumpsemver
+```
+
+## Usage
+
+This application supports both the CLI mode and config file mode.
+Options on the command line take precedence over those from the config file, which take precedence over those from the
+defaults.
+
+## Command Line Interface
+
+```bash
+bumpsemver [options] part [file]
+```
+    
+##### **`options`**    _**(optional)**_
+  
+Most of the configuration values described below can also be given as an option on the command-line.
+Additionally, the following options are available:
+
+`--dry-run`
+Don't touch any files, just pretend. Best used with `--verbose`.
+
+`--allow-dirty`
+Normally, bumpsemver will abort if the working directory is dirty to avoid releasing not versioned files
+and/or overwriting unsaved changes. Use this option to override this check.
+
+`--verbose`
+Print useful information about the action details.
+
+`--alloy-checks`
+Perform some extra checks for a private project. Generally irrelevant to the common daily usages.
+
+`-h, --help`
+Print help and exit.
+
+##### **`part`**    _**(required)**_
+
+The part of the version to increase. As we support semver only, the valid values include: `major`, `minor`, and `patch`.
+
+For example, bumping file `src/VERSION` from 0.5.1 to 0.6.0:
+
+```bash
+bumpsemver --current-version 0.5.1 minor src/VERSION
+```
+
+##### **`file`**    _**(optional).**_    _**default**_: none
+
+The file that will be modified.
+
+If not given, the list of `[bumpsemver:*:…]` sections from the configuration file will be used.
+If no files are mentioned on the configuration file either, no files will be modified.
+
+For example, bumping file `setup.py` from 1.1.9 to 2.0.0:
+```
+bumpsemver --current-version 1.1.9 major setup.py
+```
+
+## Configuration file
+
+`bumpsemver` looks up configuration file `.bumpsemver.cfg` at the current directory.
+The config file uses [`ini` syntax](https://en.wikipedia.org/wiki/INI_file).
+It consists of one general section `[bumpsemver]` and zero or more `[bumpsemver:type(suffix):filename]` file sections. 
+
+Example `.bumpsemver.cfg`:
+
+```ini
+[bumpsemver]
+current_version = 0.2.9
+commit = True
+tag = True
+
+[bumpsemver:plaintext:README.md]
+search = Version: **{current_version}**
+replace = Version: **{new_version}**
+
+[bumpsemver:plaintext(header):home.md]
+search = Version: **{current_version}**
+replace = Version: **{new_version}**
+
+[bumpsemver:plaintext(footer 1):home.md]
+search = Current version: {current_version}
+replace = Current version: {new_version}
+
+[bumpsemver:json:example.json]
+jsonpath = foobar.items[1].version
+
+[bumpsemver:yaml:example.yml]
+yamlpath = dummy.version
+
+[bumpsemver:toml:example.toml]
+tomlpath = project.version
+```
+
+### General config section
+
+General configuration is grouped in a `[bumpsemver]` section of `.bumpsemver.cfg`.
+It has the following properties:
+
+##### **`current_version =`**    _**(required).**_    _**default**_: none
+
+The current version of the software package before bumping.
+
+Also available as CLI argument `--current-version` (e.g. `bumpsemver --current-version 0.5.1 patch`)
+
+##### **`tag = (True | False)`**    _**(optional).**_    _**default**_: `False`
+
+Whether to create a git tag, that is the new version, prefixed with the character "`v`".
+
+Also available as CLI argument `--tag` or `--no-tag`.
+
+##### **`sign_tags = (True | False)`**    _**(optional).**_    _**default**_: `False`
+
+Whether to sign tags.
+
+Also available as CLI argument `--sign-tags` or `--no-sign-tags`.
+
+##### **`tag_name =`**    _**(optional).**_    _**default**_: `v{new_version}`
+
+The name of the tag that will be created. Only valid when `tag = True`.
+
+It can be a template using the [Python Format String Syntax](https://docs.python.org/3/library/string.html#format-string-syntax).  
+Available in the template context are `current_version` and `new_version` as well as `current_[part]` and `new_[part]`
+(e.g. '`current_major`' or '`new_patch`'). You can also use the variables `now` or `utcnow` to get a current timestamp.
+Both accept datetime formatting (when used like as in `{now:%d.%m.%Y}`).
+
+Also available as CLI argument `--tag-name`, for example: `bumpsemver --tag-name 'release-{new_version}' patch`
+
+In addition, it is also possible to provide a tag message by using CLI `--tag-message TAG_MESSAGE`. Example usage:
+`bumpsemver --tag-name 'release-{new_version}' --tag-message "Release {new_version}" patch`
+
+If neither tag message nor sign tag is provided, we use a `lightweight` tag in git. Otherwise, we utilize an `annotated`
+git tag. Read more about Git tagging [here](https://git-scm.com/book/en/v2/Git-Basics-Tagging).
+
+##### **`commit = (True | False)`**    _**(optional).**_    _**default**_: `False`
+
+Create a commit using git when true.
+
+Also available as CLI argument `--commit` or `--no-commit`.
+
+##### **`message =`**    _**(optional).**_    _**default**_: `build(repo): bumped version {current_version} → {new_version}`
+
+The commit message to use when creating a commit. Only valid when using `--commit` / `commit = True`.
+
+It can be a template using the [Python Format String Syntax](https://docs.python.org/3/library/string.html#format-string-syntax).  
+Available in the template context are `current_version` and `new_version` as well as `current_[part]` and `new_[part]`
+(e.g. '`current_major`' or '`new_patch`'). You can also use the variables `now` or `utcnow` to get a current timestamp.
+Both accept datetime formatting (when used like as in `{now:%d.%m.%Y}`).
+
+Also available as CLI argument `--message`, for example: `bumpsemver --tag-name 'release-{new_version}' patch`
+
+### File-specific config sections
+
+A file-specific config section is required for each file to specify the handling of the particular file.
+One config file can have zero or more file-specific config sections.
+The section name looks like `[bumpsemver:type:filename]`.
+It specifies the action to be done for a specific file.
+
+We do have the use case that one file has multiple places to change, a popular example is `package-lock.json`:
+```json
+{
+  "name": "rcplus-app-cli",
+  "version": "1.1.0",
+  "lockfileVersion": 3,
+  "requires": true,
+  "packages": {
+    "": {
+      "name": "rcplus-app-cli",
+      "version": "1.1.0",
+      "license": "SEE LICENSE IN LICENSE"
+    }
+  }
+}
+```
+We need two config sections for the same file in this case, but INI format does not allow duplicated section names.
+To make it work we could append a description between parens to the
+`type` keyword: `[bumpsemver:plaintext(special one):…]`. It does not matter what inside the parens, just make it unique.
+For the example below, the two patterns will be applied separately to the same file `README.md`:
+```ini
+[bumpsemver:plaintext(1):README.md]
+search = current version: {current_version}
+replace = current version: {new_version}
+
+[bumpsemver:plaintext(footer):README.md]
+search = **Version: {current_version}**
+replace = **Version: {new_version}**
+```
+
+### File types supported in the file-specific config section
+
+All the famous `bump*version` utilities family has a common pattern to handle the files as a plain text file.
+The advantage of this approach is that in fact it makes the use scenario programming language-neutral.
+Be it a package-lock.json for node.js project, or pyproject.toml for a Python application,
+the `bump*version` is applicable as long as a proper regex pattern for version extraction can be defined.
+
+However, it will bring significant side effect for complex file for example `package-lock.json`.
+A typical (relatively) complex React projects contains 1000+ npm packages indirectly.
+For randomly sampled 30 public projects at GitHub written in node.js/TypeScript,
+the classical `bumpversion` or the renovated `bump2version` both made mistakes
+for all 30 projects which changed something shouldn't be changed.
+
+For instance, the `facebook/create-react-app` application has a large fleet of indirect
+npm dependencies.
+If we define the search pattern as `"version": "4.0.0"`, we will screw up the other 210 packages.
+Or if we are unluckily releasing our app bumping the version from `7.16.0` to `8.0.0`,
+other 132 npm packages in the version lock will be changed to `8.0.0`, which likely do not exist.
+To address this issue, `bumpsemver` added the support of some popular file types
+to access the particular version attribute using a deterministic locator/selector without regex.
+
+The supported file types are:
+* plaintext
+* json
+* yaml
+* toml
+
+#### Plain text file
+
+The file-specific config section looks like:
+```ini
+[bumpsemver:plaintext:filename]
+search = Version: {current_version}
+replace = Version: {new_version}
+```
+
+A deprecated syntax is also supported:
+```ini
+[bumpsemver:file:filename]
+```
+We renamed (in a backward compatible way) `file` or `plaintext` to emphasize
+that the file being processed is considered as a plain text file.
+You can easily destroy a JSON file by a missing a double-quote or a comma in the regex pattern.
+
+This file type should generally only be used for the files that are not JSON, YAML, or TOML.
+`README.md` is a good use case for this one.
+
+`[bumpsemver:plaintext:...]` can have two properties:
+
+##### **`search =`**    _**default**_: `{current_version}`
+
+Template string how to search for the string to be replaced in the file.
+Useful if the remotest possibility exists that the current version number might be present multiple times in the file,
+and you mean to only bump one of the occurrences.
+
+##### **`replace =`**    _**default**_: `{new_version}`
+
+Template to create the string that will replace the current version number in the file.
+
+Given this `requirements.txt`:
+```
+    Django>=1.5.6,<1.6
+    MyProject==1.5.6
+```
+using the following `.bumpsemver.cfg` will ensure only the line containing `MyProject` will be changed:
+```ini
+[bumpsemver]
+current_version = 1.5.6
+
+[bumpsemver:plaintext:requirements.txt]
+search = MyProject=={current_version}
+replace = MyProject=={new_version}
+```
+
+#### JSON file
+
+The file-specific config section looks like:
+```ini
+[bumpsemver:json:package.json]
+jsonpath = version 
+```
+
+It accepts only one property:
+
+##### **`jsonpath =`**    **(required)**    _**default**_: none
+
+Value of the parameter `jsonpath` is a [JSONPath](https://goessner.net/articles/JsonPath/) string,
+it points to the exact property of the version string to be bumped.
+For the typical `package.json`, using `version` or its jQuery-style alternative `$.version` is sufficient.
+Otherwise, anything can be selected with JSONPath is support, so, nothing we can't do.
+The underlying JSONPath processor is [jsonpath-ng](https://github.com/h2non/jsonpath-ng).
+Checkout their document for some examples and hints.
+
+The suffix is also supported for json file:
+```ini
+[bumpsemver:json(1):example.json]
+jsonpath = version
+
+[bumpsemver:json( same file):example.json]
+jsonpath = dependencies[2].*.version
+
+[bumpsemver:json (once again):example.json]
+jsonpath = dependencies[0].*.lodash.dependencies[1].version
+```
+
+#### YAML file
+
+Comparably, YAML is supported for the same reason that we should support native JSON, like
+ ```ini
+[bumpsemver:yaml:playbook.yml]
+yamlpath = version 
+```
+OR
+```ini
+[bumpsemver:yaml(1):playbook.yml]
+yamlpath = *.vars.project_version
+
+[bumpsemver:yaml( same file):playbook.yaml]
+yamlpath = *.vars.version
+
+[bumpsemver:yaml (once again):playbook.yaml]
+yamlpath = *.vars.app_version
+```
+
+Please note that we use
+[yamlpath](https://github.com/wwkimball/yamlpath/wiki/Segments-of-a-YAML-Path#yaml-path-standard) here.
+`yamlpath` is not a popular "standard" widely adopted as `jsonpath`.
+For complex scenarios, it makes sense to test the expression with [yamlpath cli](https://pypi.org/project/yamlpath/)
+before putting anything in the config file.
+
+#### TOML file
+
+The file-specific config section looks like:
+```ini
+[bumpsemver:toml:pyproject.toml]
+tomlpath = tool.poetry.version
+```
+
+For whatever reason toml gets its acceptance and popularity, especially in the Go, Rust, and later Python community.
+Despite the unlogical fashion and religion drives, in fact we have many toml files in the wild.
+For instance `pyproject.toml` is everywhere now.
+
+We cannot even find out a "tomlpath" or similar library to read/update the properties in a toml file by giving a
+string as the "path" to the property.
+We rolled our own tomlpath processor, which is not a standard, but offering similar functionality as yamlpath.
+
```

