# Comparing `tmp/f_lib-0.2.0.tar.gz` & `tmp/f_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f_lib-0.2.0.tar", max compression
+gzip compressed data, was "f_lib-0.3.0.tar", max compression
```

## Comparing `f_lib-0.2.0.tar` & `f_lib-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,31 @@
--rw-r--r--   0        0        0    11341 2023-12-28 02:27:00.042867 f_lib-0.2.0/LICENSE
--rw-r--r--   0        0        0      466 2023-12-28 02:27:00.042867 f_lib-0.2.0/README.md
--rw-r--r--   0        0        0      571 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/__init__.py
--rw-r--r--   0        0        0     2724 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/_environment.py
--rw-r--r--   0        0        0     3090 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/_os_info.py
--rw-r--r--   0        0        0     2605 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/_system_info.py
--rw-r--r--   0        0        0       55 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/aws/__init__.py
--rw-r--r--   0        0        0       22 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/aws/aws_lambda/__init__.py
--rw-r--r--   0        0        0     5001 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/aws/aws_lambda/type_defs.py
--rw-r--r--   0        0        0      149 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/constants.py
--rw-r--r--   0        0        0      181 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/mixins/__init__.py
--rw-r--r--   0        0        0     5749 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/mixins/_cli_interface.py
--rw-r--r--   0        0        0      576 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/mixins/_del_cached_prop.py
--rw-r--r--   0        0        0        0 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/py.typed
--rw-r--r--   0        0        0     1319 2023-12-28 02:27:00.042867 f_lib-0.2.0/f_lib/utils/__init__.py
--rw-r--r--   0        0        0     5791 2023-12-28 02:27:19.306886 f_lib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 f_lib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-04-19 14:44:08.307933 f_lib-0.3.0/LICENSE
+-rw-r--r--   0        0        0      731 2024-04-19 14:44:08.307933 f_lib-0.3.0/README.md
+-rw-r--r--   0        0        0     1020 2024-04-19 14:44:29.596317 f_lib-0.3.0/f_lib/__init__.py
+-rw-r--r--   0        0        0     2725 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/_environment.py
+-rw-r--r--   0        0        0     3091 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/_os_info.py
+-rw-r--r--   0        0        0     2606 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/_system_info.py
+-rw-r--r--   0        0        0       55 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/aws/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/aws/aws_lambda/__init__.py
+-rw-r--r--   0        0        0     5002 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/aws/aws_lambda/type_defs.py
+-rw-r--r--   0        0        0      150 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/constants.py
+-rw-r--r--   0        0        0      731 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/__init__.py
+-rw-r--r--   0        0        0     6814 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/_console_handler.py
+-rw-r--r--   0        0        0     1327 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/_constants.py
+-rw-r--r--   0        0        0     2717 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/_extendable_highlighter.py
+-rw-r--r--   0        0        0     2775 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/_fluid_log_render.py
+-rw-r--r--   0        0        0     3533 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/_log_level.py
+-rw-r--r--   0        0        0     5488 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/_logger.py
+-rw-r--r--   0        0        0     4019 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/_prefix_adaptor.py
+-rw-r--r--   0        0        0     3433 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/_setup_logging.py
+-rw-r--r--   0        0        0      303 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/settings/__init__.py
+-rw-r--r--   0        0        0     1218 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/settings/_console_logging_settings.py
+-rw-r--r--   0        0        0     1918 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/settings/_logging_settings.py
+-rw-r--r--   0        0        0     1285 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/settings/_sources.py
+-rw-r--r--   0        0        0     3759 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/logging/utils.py
+-rw-r--r--   0        0        0      182 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/mixins/__init__.py
+-rw-r--r--   0        0        0     5632 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/mixins/_cli_interface.py
+-rw-r--r--   0        0        0      577 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/mixins/_del_cached_prop.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/py.typed
+-rw-r--r--   0        0        0     1320 2024-04-19 14:44:08.307933 f_lib-0.3.0/f_lib/utils/__init__.py
+-rw-r--r--   0        0        0     6415 2024-04-19 14:44:29.596317 f_lib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 f_lib-0.3.0/PKG-INFO
```

### Comparing `f_lib-0.2.0/LICENSE` & `f_lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f_lib-0.2.0/f_lib/_environment.py` & `f_lib-0.3.0/f_lib/_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Environment object class."""
+
 import json
 import logging
 import os
 from pathlib import Path
 from typing import Self
 
 from ._system_info import SystemInfo
```

### Comparing `f_lib-0.2.0/f_lib/_os_info.py` & `f_lib-0.3.0/f_lib/_os_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Operating system information."""
+
 from __future__ import annotations
 
 import os
 import platform
 from functools import cached_property
 from pathlib import Path
 from typing import TYPE_CHECKING, ClassVar, cast, final
```

### Comparing `f_lib-0.2.0/f_lib/_system_info.py` & `f_lib-0.3.0/f_lib/_system_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """System information."""
+
 from __future__ import annotations
 
 import platform
 import sys
 from functools import cached_property
 from typing import ClassVar, Literal, cast, final
```

### Comparing `f_lib-0.2.0/f_lib/aws/aws_lambda/type_defs.py` & `f_lib-0.3.0/f_lib/aws/aws_lambda/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Type definitions for AWS Lambda."""
+
 from typing import Any, TypedDict
 
 LambdaDict = dict[str, Any]
 
 
 class LambdaCognitoIdentity(TypedDict):
     """Amazon Cognito identity that authorized a request."""
```

### Comparing `f_lib-0.2.0/f_lib/mixins/_cli_interface.py` & `f_lib-0.3.0/f_lib/mixins/_cli_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI interface mixin."""
+
 from __future__ import annotations
 
 import logging
 import shutil
 import subprocess
 from typing import IO, TYPE_CHECKING, ClassVar, Literal, cast, overload
 
@@ -51,65 +52,57 @@
 
         Returns:
             The full command to be passed into a subprocess.
 
         """
         cmd = [
             cls.EXECUTABLE,
-            *(
-                __command
-                if isinstance(__command, list)
-                else ([__command] if __command else [])
-            ),
+            *(__command if isinstance(__command, list) else ([__command] if __command else [])),
         ]
         cmd.extend(convert_kwargs_to_shell_list(**kwargs))
         LOGGER.debug("generated command: %s", convert_list_to_shell_str(cmd))
         return cmd
 
     @overload
     def _run_command(
         self,
         command: Iterable[str] | str,
         *,
         capture_output: Literal[True],
         env: dict[str, str] | None = ...,
-    ) -> str:
-        ...
+    ) -> str: ...
 
     @overload
     def _run_command(
         self,
         command: Iterable[str] | str,
         *,
         capture_output: bool = ...,
         env: dict[str, str] | None = ...,
         suppress_output: Literal[True] = ...,
-    ) -> str:
-        ...
+    ) -> str: ...
 
     @overload
     def _run_command(
         self,
         command: Iterable[str] | str,
         *,
         env: dict[str, str] | None = ...,
         suppress_output: Literal[False],
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @overload
     def _run_command(
         self,
         command: Iterable[str] | str,
         *,
         capture_output: bool = ...,
         env: dict[str, str] | None = ...,
         suppress_output: bool = ...,
-    ) -> str | None:
-        ...
+    ) -> str | None: ...
 
     def _run_command(
         self,
         command: Iterable[str] | str,
         *,
         capture_output: bool = False,
         env: dict[str, str] | None = None,
@@ -125,17 +118,15 @@
                 string. If ``suppress_output`` is ``True``, this will be ignored.
             env: Environment variables.
             suppress_output: If ``True``, the output of the subprocess written
                 to ``sys.stdout`` and ``sys.stderr`` will be captured and
                 returned as a string instead of being being written directly.
 
         """
-        cmd_str = (
-            command if isinstance(command, str) else convert_list_to_shell_str(command)
-        )
+        cmd_str = command if isinstance(command, str) else convert_list_to_shell_str(command)
         LOGGER.debug("running command: %s", cmd_str)
         if suppress_output:
             return subprocess.check_output(
                 cmd_str,
                 cwd=self.cwd,
                 env=env or self.env.vars,
                 shell=True,  # noqa: S602
```

### Comparing `f_lib-0.2.0/f_lib/mixins/_del_cached_prop.py` & `f_lib-0.3.0/f_lib/mixins/_del_cached_prop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Delete cached property mixin."""
+
 from __future__ import annotations
 
 from contextlib import suppress
 
 
 class DelCachedPropMixin:
     """Mixin to handle safely clearing the value of :func:`functools.cached_property`."""
```

### Comparing `f_lib-0.2.0/f_lib/utils/__init__.py` & `f_lib-0.3.0/f_lib/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities."""
+
 from __future__ import annotations
 
 import platform
 import shlex
 import subprocess
 from typing import TYPE_CHECKING, Any, cast
```

### Comparing `f_lib-0.2.0/pyproject.toml` & `f_lib-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-[build-system]
-build-backend = "poetry.core.masonry.api"
-requires = ["poetry-core"]
-
 [tool.poetry]
 name = "f-lib"
-version = "0.2.0"
+version = "0.3.0"
 authors = ["Kyle Finley <kyle@finley.sh>"]
 classifiers = [
+  # https://pypi.org/classifiers/
+  "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Utilities",
+  "Typing :: Typed",
 ]
 description = "Python library created by Kyle Finley, for Kyle Finley."
 documentation = "https://f-lib.readthedocs.io"
 homepage = "https://f-lib.readthedocs.io"
 keywords = []
 license = "Apache-2.0"
 maintainers = []
@@ -26,61 +25,66 @@
 ]
 readme = "README.md"
 repository = "https://github.com/ITProKyle/f-lib"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 platformdirs = "^4.1.0"
+pydantic = "^2.6.4"
+pydantic-settings = "^2.2.1"  # TODO (kyle): update once released https://github.com/pydantic/pydantic-settings/pull/255
+rich = "^13.7.1"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.6.0"
+pre-commit = "^3.7.0"
 
 [tool.poetry.group.docs.dependencies]
 doc8 = "^1.1.1"
-furo = "^2023.9.10"
-sphinx = "^7.2.6"
-sphinx-autobuild = "^2021.3.14"
+furo = "^2024.1.29"
+sphinx = "^7.3.7"
+sphinx-autobuild = "^2024.4.16"
 sphinx-copybutton = "^0.5.2"
 sphinx-design = "^0.5.0"
-sphinxcontrib-apidoc = "^0.4.0"
+sphinxcontrib-apidoc = "^0.5.0"
 sphinxcontrib-jquery = "^4.1"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.12.0"
-ruff = "^0.1.9"
+black = "^24.4.0"
+ruff = "^0.4.1"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.4.3"
-pytest-cov = "^4.1.0"
-pytest-mock = "^3.12.0"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+pytest-mock = "^3.14.0"
 pytest-subprocess = "^1.5.0"
-pytest-sugar = "^0.9.7"
-pytest-xdist = "^3.3.1"
+pytest-sugar = "^1.0.0"
+pytest-xdist = "^3.5.0"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/ITProKyle/f-lib/issues"
+bugs = "https://github.com/ITProKyle/f-lib/issues"
+changelog = "https://github.com/ITProKyle/f-lib/releases"
+issues = "https://github.com/ITProKyle/f-lib/issues"
 
 [tool.black]
 force-exclude = '''
 /(
     \.eggs
   | \.git
   | \.venv
   | _build
   | build
   | dist
   | node_modules
 )/
 '''
 include = '\.pyi?$'
-line-length = 88
+line-length = 100
 target-version = ["py311", "py312"]
 
 [tool.coverage.report]
 exclude_lines = [
   "@overload",
   "cov: ignore",  # standard exclude comment
   "if TYPE_CHECKING:",  # excluded blocks
@@ -148,16 +152,21 @@
   "wip: isolate tests currently being worked on.",
 ]
 python_classes = ["Test*"]
 python_files = ["test_*.py"]
 python_functions = ["test_*"]
 testpaths = ["tests"]
 
-[tool.ruff]  # https://beta.ruff.rs/docs/settings/#top-level
+[tool.ruff]  # https://docs.astral.sh/ruff/settings/#top-level
 force-exclude = true
+line-length = 120
+show-fixes = true
+target-version = "py311"
+
+[tool.ruff.lint]  # https://docs.astral.sh/ruff/settings/#lint
 ignore = [
   "ANN101",  # Missing type annotation for `self` in method
   "ANN102",  # Missing type annotation for `cls` in classmethod
   "COM812",  # Trailing comma missing
   "D203",  # 1 blank line required before class docstring
   "D213",  # Multi-line docstring summary should start at the second line
   "D215",  # Section underline is over-indented
@@ -168,48 +177,49 @@
   "D409",  # Section underline should match the length of its name
   "ERA001",  # Found commented-out code  # NOTE (kyle): incorrectly detects cspell
   "FIX002",  # Line contains TODO
   "TD003",  # Missing issue link on the line following this TODO
   "TID252",  # Relative imports from parent modules are banned
 ]
 ignore-init-module-imports = true
-line-length = 120
 select = ["ALL"]
-show-fixes = true
-target-version = "py311"
 
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]  # https://docs.astral.sh/ruff/settings/#lintextend-per-file-ignores
 "*.py" = [
   "PYI024",  # Use `typing.NamedTuple` instead of `collections.namedtuple` - should only apply to pyi
 ]
 "tests/*" = [
   "FBT001",  # Boolean positional arg in function definition - this is fine here
   "FBT003",  # Boolean positional value in function call - this is fine here
   "PT004",  # Fixture does not return anything, add leading underscore
   "S101",  # Use of `assert` detected - this is fine here
   "S108",  # Probable insecure usage of temporary file or directory
   "S604",  # Function call with `shell=True` parameter identified - this is fine here
   "SLF001",  # Private member accessed - fine in tests
 ]
 
-[tool.ruff.flake8-type-checking]  # https://beta.ruff.rs/docs/settings/#flake8-type-checking
+[tool.ruff.lint.flake8-type-checking]  # https://docs.astral.sh/ruff/settings/#lint_flake8-type-checking_runtime-evaluated-base-classes
 runtime-evaluated-base-classes = [
   "pydantic.BaseModel",
   "pydantic.BeforeValidator",
 ]
 
-[tool.ruff.pydocstyle]  # https://beta.ruff.rs/docs/settings/#pydocstyle
+[tool.ruff.lint.pydocstyle]  # https://docs.astral.sh/ruff/settings/#lintpydocstyle
 convention = "google"
 
-[tool.ruff.pylint]  # https://beta.ruff.rs/docs/settings/#pylint
+[tool.ruff.lint.pylint]  # https://docs.astral.sh/ruff/settings/#lintpylint
 allow-magic-value-types = ["bytes", "int", "str"]
 max-args = 15
 max-returns = 10
 
 [tool.tomlsort]
 all = true
 in_place = true
-sort_first = ["tool.poetry"]
+sort_first = ["tool", "tool.poetry"]
 spaces_before_inline_comment = 2
 trailing_comma_inline_array = true
 overrides."tool.poetry".first = ["name", "version"]
 overrides."tool.poetry.dependencies".first = ["python"]
+
+[build-system]
+build-backend = "poetry_dynamic_versioning.backend"
+requires = ["poetry-core>=1.0.7", "poetry-dynamic-versioning>=1.2.0,<2.0.0"]
```

