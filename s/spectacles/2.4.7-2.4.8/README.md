# Comparing `tmp/spectacles-2.4.7.tar.gz` & `tmp/spectacles-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectacles-2.4.7.tar", max compression
+gzip compressed data, was "spectacles-2.4.8.tar", max compression
```

## Comparing `spectacles-2.4.7.tar` & `spectacles-2.4.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1082 2021-11-18 20:00:49.748916 spectacles-2.4.7/LICENSE
--rw-r--r--   0        0        0     3192 2022-11-08 19:17:18.791087 spectacles-2.4.7/README.md
--rw-r--r--   0        0        0     2379 2024-03-24 22:22:14.661068 spectacles-2.4.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-01 19:35:01.756973 spectacles-2.4.7/spectacles/__init__.py
--rw-r--r--   0        0        0    33719 2024-02-01 19:35:01.758019 spectacles-2.4.7/spectacles/cli.py
--rw-r--r--   0        0        0    39198 2024-02-19 17:48:48.562090 spectacles-2.4.7/spectacles/client.py
--rw-r--r--   0        0        0     5725 2024-02-01 19:35:01.759196 spectacles-2.4.7/spectacles/exceptions.py
--rw-r--r--   0        0        0     3596 2024-02-01 19:35:01.760489 spectacles-2.4.7/spectacles/logger.py
--rw-r--r--   0        0        0    18470 2024-02-01 19:35:01.761930 spectacles-2.4.7/spectacles/lookml.py
--rw-r--r--   0        0        0     3226 2024-02-01 19:35:01.763569 spectacles-2.4.7/spectacles/models.py
--rw-r--r--   0        0        0     5455 2024-02-01 19:35:01.764332 spectacles-2.4.7/spectacles/printer.py
--rw-r--r--   0        0        0     1459 2024-02-01 19:35:01.764661 spectacles-2.4.7/spectacles/project_select.py
--rw-r--r--   0        0        0        0 2022-11-08 19:17:18.797644 spectacles-2.4.7/spectacles/py.typed
--rw-r--r--   0        0        0    22737 2024-03-24 22:22:14.661703 spectacles-2.4.7/spectacles/runner.py
--rw-r--r--   0        0        0     1291 2024-02-07 14:29:12.583042 spectacles-2.4.7/spectacles/tracking.py
--rw-r--r--   0        0        0     3320 2024-02-01 19:35:01.773330 spectacles-2.4.7/spectacles/utils.py
--rw-r--r--   0        0        0      317 2024-02-01 19:35:01.775261 spectacles-2.4.7/spectacles/validators/__init__.py
--rw-r--r--   0        0        0     7269 2024-02-01 19:35:01.776148 spectacles-2.4.7/spectacles/validators/content.py
--rw-r--r--   0        0        0     4858 2024-02-01 19:35:01.778264 spectacles-2.4.7/spectacles/validators/data_test.py
--rw-r--r--   0        0        0     2290 2024-02-01 19:35:01.778818 spectacles-2.4.7/spectacles/validators/lookml.py
--rw-r--r--   0        0        0    22392 2024-02-19 17:48:48.562889 spectacles-2.4.7/spectacles/validators/sql.py
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 spectacles-2.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1082 2019-10-02 19:47:43.000000 spectacles-2.4.8/LICENSE
+-rw-r--r--   0        0        0     3192 2022-11-21 17:52:41.756936 spectacles-2.4.8/README.md
+-rw-r--r--   0        0        0     2379 2024-04-19 14:54:19.766158 spectacles-2.4.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-07 13:53:18.822598 spectacles-2.4.8/spectacles/__init__.py
+-rw-r--r--   0        0        0    35199 2024-04-19 14:54:19.766988 spectacles-2.4.8/spectacles/cli.py
+-rw-r--r--   0        0        0    39349 2024-04-19 14:54:19.767618 spectacles-2.4.8/spectacles/client.py
+-rw-r--r--   0        0        0     5725 2024-02-07 13:53:18.824740 spectacles-2.4.8/spectacles/exceptions.py
+-rw-r--r--   0        0        0     3596 2024-02-07 13:53:18.824979 spectacles-2.4.8/spectacles/logger.py
+-rw-r--r--   0        0        0    18470 2024-02-07 13:53:18.825222 spectacles-2.4.8/spectacles/lookml.py
+-rw-r--r--   0        0        0     3226 2024-02-07 13:53:18.825399 spectacles-2.4.8/spectacles/models.py
+-rw-r--r--   0        0        0     5455 2024-02-07 13:53:18.825856 spectacles-2.4.8/spectacles/printer.py
+-rw-r--r--   0        0        0     1459 2024-02-07 13:53:18.825964 spectacles-2.4.8/spectacles/project_select.py
+-rw-r--r--   0        0        0        0 2022-08-26 11:43:56.097650 spectacles-2.4.8/spectacles/py.typed
+-rw-r--r--   0        0        0    24833 2024-04-19 14:54:19.768200 spectacles-2.4.8/spectacles/runner.py
+-rw-r--r--   0        0        0     1291 2024-02-07 13:53:18.826609 spectacles-2.4.8/spectacles/tracking.py
+-rw-r--r--   0        0        0     3320 2024-02-07 13:53:18.827372 spectacles-2.4.8/spectacles/utils.py
+-rw-r--r--   0        0        0      317 2024-02-07 13:53:18.827931 spectacles-2.4.8/spectacles/validators/__init__.py
+-rw-r--r--   0        0        0     7269 2024-02-07 13:53:18.828465 spectacles-2.4.8/spectacles/validators/content.py
+-rw-r--r--   0        0        0     4922 2024-04-19 14:54:19.769021 spectacles-2.4.8/spectacles/validators/data_test.py
+-rw-r--r--   0        0        0     2407 2024-04-19 14:54:19.769506 spectacles-2.4.8/spectacles/validators/lookml.py
+-rw-r--r--   0        0        0    22392 2024-02-12 16:45:14.304045 spectacles-2.4.8/spectacles/validators/sql.py
+-rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 spectacles-2.4.8/PKG-INFO
```

### Comparing `spectacles-2.4.7/LICENSE` & `spectacles-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/README.md` & `spectacles-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/pyproject.toml` & `spectacles-2.4.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectacles"
-version = "2.4.7"
+version = "2.4.8"
 description = "A command-line, continuous integration tool for Looker and LookML."
 authors = ["Spectacles <hello@spectacles.dev>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
     "Looker",
     "LookML",
```

### Comparing `spectacles-2.4.7/spectacles/cli.py` & `spectacles-2.4.8/spectacles/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 
 import httpx
 import yaml
 from yaml.parser import ParserError
 
 import spectacles.printer as printer
 import spectacles.tracking as tracking
-from spectacles.client import DEFAULT_API_VERSION, LookerClient
+from spectacles.client import (
+    DEFAULT_API_VERSION,
+    LOOKML_VALIDATION_TIMEOUT,
+    LookerClient,
+)
 from spectacles.exceptions import (
     GenericValidationError,
     LookerApiError,
     SpectaclesException,
 )
 from spectacles.logger import GLOBAL_LOGGER as logger
 from spectacles.logger import set_file_handler
 from spectacles.runner import Runner
 from spectacles.utils import log_duration
+from spectacles.validators.data_test import DATA_TEST_CONCURRENCY
 
 __version__ = importlib.metadata.version("spectacles")
 
 
 class ConfigFileAction(argparse.Action):
     """Parses an arbitrary config file and assigns its values as arg defaults."""
 
@@ -322,14 +327,15 @@
                 remote_reset=args.remote_reset,
                 concurrency=args.concurrency,
                 profile=args.profile,
                 runtime_threshold=args.runtime_threshold,
                 chunk_size=args.chunk_size,
                 pin_imports=pin_imports,
                 ignore_hidden=args.ignore_hidden,
+                use_personal_branch=args.use_personal_branch,
             )
         )
     elif args.command == "assert":
         asyncio.run(
             run_assert(
                 project=args.project,
                 ref=ref,
@@ -337,14 +343,16 @@
                 base_url=args.base_url,
                 client_id=args.client_id,
                 client_secret=args.client_secret,
                 port=args.port,
                 api_version=args.api_version,
                 remote_reset=args.remote_reset,
                 pin_imports=pin_imports,
+                use_personal_branch=args.use_personal_branch,
+                concurrency=args.concurrency,
             )
         )
     elif args.command == "content":
         asyncio.run(
             run_content(
                 project=args.project,
                 ref=ref,
@@ -356,14 +364,15 @@
                 api_version=args.api_version,
                 remote_reset=args.remote_reset,
                 incremental=args.incremental,
                 target=args.target,
                 exclude_personal=args.exclude_personal,
                 folders=[restore_dash(arg) for arg in args.folders],
                 pin_imports=pin_imports,
+                use_personal_branch=args.use_personal_branch,
             )
         )
     elif args.command == "lookml":
         asyncio.run(
             run_lookml(
                 project=args.project,
                 ref=ref,
@@ -371,14 +380,16 @@
                 client_id=args.client_id,
                 client_secret=args.client_secret,
                 port=args.port,
                 api_version=args.api_version,
                 remote_reset=args.remote_reset,
                 severity=args.severity,
                 pin_imports=pin_imports,
+                use_personal_branch=args.use_personal_branch,
+                timeout=args.timeout,
             )
         )
 
     if not args.do_not_track:
         tracking.track_invocation_end(
             args.base_url,
             args.command,
@@ -525,14 +536,27 @@
     )
     base_subparser.add_argument(
         "--branch",
         action=EnvVarAction,
         env_var="LOOKER_GIT_BRANCH",
         help="The branch of your project that Spectacles will use to run queries.",
     )
+    base_subparser.add_argument(
+        "--use-personal-branch",
+        action=EnvVarStoreTrueAction,
+        env_var="SPECTACLES_USE_PERSONAL_BRANCH",
+        help="Use the user's personal branch instead of creating a temporary branch for the tests.",
+    )
+    base_subparser.add_argument(
+        "--pin-imports",
+        nargs="+",
+        default=[],
+        help="Pin locally imported Looker projects to a specific ref (Git branch or commit) during validation. \
+            Provide these arguments in project_name:ref format.",
+    )
     group = base_subparser.add_mutually_exclusive_group()
     group.add_argument(
         "--remote-reset",
         action=EnvVarStoreTrueAction,
         env_var="SPECTACLES_REMOTE_RESET",
         help="When set to true, the SQL validator will tell Looker to reset the \
             user's branch to the revision of the branch that is on the remote. \
@@ -542,21 +566,14 @@
         "--commit-ref",
         action=EnvVarAction,
         env_var="LOOKER_COMMIT_REF",
         help="The commit of your project that Spectacles will test against. \
             In order to test a specific commit, Spectacles will create a new branch \
             for the tests and then delete the branch when it is finished.",
     )
-    group.add_argument(
-        "--pin-imports",
-        nargs="+",
-        default=[],
-        help="Pin locally imported Looker projects to a specific ref (Git branch or commit) during validation. \
-            Provide these arguments in project_name:ref format.",
-    )
     return base_subparser
 
 
 def _build_select_subparser(
     subparser_action: argparse._SubParsersAction,  # type: ignore[type-arg]
     base_subparser: ArgumentParser,
 ) -> ArgumentParser:
@@ -598,14 +615,20 @@
         help=(
             "Specify a level of validation error severity to trigger test failure. "
             "Spectacles will display all errors, regardless of severity, "
             "but only errors at or higher than this level will cause this "
             "validator to fail. The default is 'warning'."
         ),
     )
+    subparser.add_argument(
+        "--timeout",
+        type=int,
+        default=LOOKML_VALIDATION_TIMEOUT,
+        help="Specify the timeout for the LookML validation in seconds.",
+    )
     _build_validator_subparser(subparser_action, subparser)
 
 
 def _build_sql_subparser(
     subparser_action: argparse._SubParsersAction,  # type: ignore[type-arg]
     base_subparser: ArgumentParser,
 ) -> None:
@@ -705,14 +728,24 @@
     """
     subparser = subparser_action.add_parser(
         "assert", parents=[base_subparser], help="Run Looker data tests."
     )
     _build_validator_subparser(subparser_action, subparser)
     _build_select_subparser(subparser_action, subparser)
 
+    subparser.add_argument(
+        "--concurrency",
+        type=int,
+        default=DATA_TEST_CONCURRENCY,
+        help=(
+            "Specify the number of concurrent queries you want to have running "
+            f"against your data warehouse. The default is {DATA_TEST_CONCURRENCY}."
+        ),
+    )
+
 
 def _build_content_subparser(
     subparser_action: argparse._SubParsersAction,  # type: ignore[type-arg]
     base_subparser: ArgumentParser,
 ) -> None:
     subparser = subparser_action.add_parser(
         "content", parents=[base_subparser], help="Run Looker content validation."
@@ -775,24 +808,26 @@
     client_id: str,
     client_secret: str,
     port: int,
     api_version: float,
     remote_reset: bool,
     severity: str,
     pin_imports: Dict[str, str],
+    use_personal_branch: bool,
+    timeout: int,
 ) -> None:
     # Don't trust env to ignore .netrc credentials
     async_client = httpx.AsyncClient(trust_env=False)
     try:
         client = LookerClient(
             async_client, base_url, client_id, client_secret, port, api_version
         )
-        runner = Runner(client, project, remote_reset, pin_imports)
+        runner = Runner(client, project, remote_reset, pin_imports, use_personal_branch)
 
-        results = await runner.validate_lookml(ref, severity)
+        results = await runner.validate_lookml(ref, severity, timeout)
     finally:
         await async_client.aclose()
 
     errors = sorted(results["errors"], key=lambda x: x["metadata"]["file_path"] or "a")
     unique_files = sorted(
         set(
             error["metadata"]["file_path"]
@@ -833,22 +868,23 @@
     api_version: float,
     remote_reset: bool,
     incremental: bool,
     target: str,
     exclude_personal: bool,
     folders: List[str],
     pin_imports: Dict[str, str],
+    use_personal_branch: bool,
 ) -> None:
     # Don't trust env to ignore .netrc credentials
     async_client = httpx.AsyncClient(trust_env=False)
     try:
         client = LookerClient(
             async_client, base_url, client_id, client_secret, port, api_version
         )
-        runner = Runner(client, project, remote_reset, pin_imports)
+        runner = Runner(client, project, remote_reset, pin_imports, use_personal_branch)
 
         results = await runner.validate_content(
             ref,
             filters,
             incremental,
             target,
             exclude_personal,
@@ -892,24 +928,26 @@
     base_url: str,
     client_id: str,
     client_secret: str,
     port: int,
     api_version: float,
     remote_reset: bool,
     pin_imports: Dict[str, str],
+    use_personal_branch: bool,
+    concurrency: int,
 ) -> None:
     # Don't trust env to ignore .netrc credentials
     async_client = httpx.AsyncClient(trust_env=False)
     try:
         client = LookerClient(
             async_client, base_url, client_id, client_secret, port, api_version
         )
-        runner = Runner(client, project, remote_reset, pin_imports)
+        runner = Runner(client, project, remote_reset, pin_imports, use_personal_branch)
 
-        results = await runner.validate_data_tests(ref, filters)
+        results = await runner.validate_data_tests(ref, filters, concurrency)
     finally:
         await async_client.aclose()
 
     for test in sorted(results["tested"], key=lambda x: (x["model"], x["explore"])):
         message = f"{test['model']}.{test['explore']}"
         printer.print_validation_result(status=test["status"], source=message)
 
@@ -952,24 +990,25 @@
     target: str,
     remote_reset: bool,
     concurrency: int,
     profile: bool,
     runtime_threshold: int,
     chunk_size: int,
     pin_imports: Dict[str, str],
+    use_personal_branch: bool,
     ignore_hidden: bool,
 ) -> None:
     """Runs and validates the SQL for each selected LookML dimension."""
     # Don't trust env to ignore .netrc credentials
     async_client = httpx.AsyncClient(trust_env=False)
     try:
         client = LookerClient(
             async_client, base_url, client_id, client_secret, port, api_version
         )
-        runner = Runner(client, project, remote_reset, pin_imports)
+        runner = Runner(client, project, remote_reset, pin_imports, use_personal_branch)
 
         results = await runner.validate_sql(
             ref,
             filters,
             fail_fast,
             incremental,
             target,
```

### Comparing `spectacles-2.4.7/spectacles/client.py` & `spectacles-2.4.8/spectacles/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import spectacles.utils as utils
 from spectacles.exceptions import LookerApiError, SpectaclesException
 from spectacles.logger import GLOBAL_LOGGER as logger
 from spectacles.models import JsonDict
 
 DEFAULT_API_VERSION = 4.0
 TIMEOUT_SEC = 300
+LOOKML_VALIDATION_TIMEOUT = 7200
 MAX_ASYNC_CONNECTIONS = 200
 DEFAULT_MAX_TRIES = 3
 BACKOFF_EXCEPTIONS = (
     TimeoutException,
     HTTPStatusError,
     ConnectError,
     LookerApiError,
@@ -253,15 +254,15 @@
                     "Spectacles is using, please save it and try again."
                 ),
                 response=response,
             ) from error
         self.workspace = workspace
 
     @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
-    async def get_all_branches(self, project: str) -> List[str]:
+    async def get_all_branches(self, project: str) -> List[JsonDict]:
         """Returns a list of git branches in the project repository.
 
         Args:
             project: Name of the Looker project to use.
         """
         logger.debug(f"Getting all Git branches in project '{project}'")
         url = utils.compose_url(
@@ -278,15 +279,15 @@
                 detail=(
                     f"Unable to get all Git branches in project '{project}'. "
                     "Please try again."
                 ),
                 response=response,
             ) from error
 
-        return [branch["name"] for branch in response.json()]
+        return response.json()  # type: ignore[no-any-return]
 
     @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
     async def checkout_branch(self, project: str, branch: str) -> None:
         """Checks out a new git branch. Only works in dev workspace.
 
         Args:
             project: Name of the Looker project to use.
@@ -858,18 +859,22 @@
                 response=response,
             ) from error
 
         result = response.json()
         return result  # type: ignore[no-any-return]
 
     @backoff.on_exception(backoff.expo, BACKOFF_EXCEPTIONS, max_tries=DEFAULT_MAX_TRIES)
-    async def lookml_validation(self, project: str) -> JsonDict:
-        logger.debug(f"Validating LookML for project '{project}'")
+    async def lookml_validation(
+        self, project: str, timeout: int = LOOKML_VALIDATION_TIMEOUT
+    ) -> JsonDict:
+        logger.debug(
+            f"Validating LookML for project '{project}' with timeout {timeout} seconds."
+        )
         url = utils.compose_url(self.api_url, path=["projects", project, "validate"])
-        response = await self.post(url=url, timeout=7200)
+        response = await self.post(url=url, timeout=timeout)
 
         try:
             response.raise_for_status()
         except httpx.HTTPStatusError as error:
             raise LookerApiError(
                 name="unable-to-validate-lookml",
                 title=f"Couldn't validate LookML in project {project}.",
```

### Comparing `spectacles-2.4.7/spectacles/exceptions.py` & `spectacles-2.4.8/spectacles/exceptions.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/spectacles/logger.py` & `spectacles-2.4.8/spectacles/logger.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/spectacles/lookml.py` & `spectacles-2.4.8/spectacles/lookml.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/spectacles/models.py` & `spectacles-2.4.8/spectacles/models.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/spectacles/printer.py` & `spectacles-2.4.8/spectacles/printer.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/spectacles/project_select.py` & `spectacles-2.4.8/spectacles/project_select.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/spectacles/runner.py` & `spectacles-2.4.8/spectacles/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import asyncio
 import itertools
 import re
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Set, Tuple
 
-from spectacles.client import LookerClient
+from spectacles.client import LOOKML_VALIDATION_TIMEOUT, LookerClient
 from spectacles.exceptions import LookerApiError, SpectaclesException, SqlError
 from spectacles.logger import GLOBAL_LOGGER as logger
 from spectacles.lookml import CompiledSql, Explore, build_project
 from spectacles.models import JsonDict, SkipReason
 from spectacles.printer import print_header
 from spectacles.utils import time_hash
 from spectacles.validators import (
     ContentValidator,
     DataTestValidator,
     LookMLValidator,
     SqlValidator,
 )
+from spectacles.validators.data_test import DATA_TEST_CONCURRENCY
 from spectacles.validators.sql import (
     DEFAULT_CHUNK_SIZE,
     DEFAULT_QUERY_CONCURRENCY,
     DEFAULT_RUNTIME_THRESHOLD,
 )
 
 
@@ -39,28 +40,31 @@
 
 class LookerBranchManager:
     def __init__(
         self,
         client: LookerClient,
         project: str,
         remote_reset: bool = False,
+        use_personal_branch: bool = False,
         pin_imports: Optional[Dict[str, str]] = None,
         skip_imports: Optional[List[str]] = None,
     ):
         """Context manager for Git branch checkout, creation, and deletion."""
         logger.debug(f"Setting up branch manager in project '{project}'")
         self.client = client
         self.project = project
         self.remote_reset = remote_reset
         self.pin_imports = pin_imports or {}
         self.history: List[ProjectState] = []
 
         self.commit: Optional[str] = None
         self.branch: Optional[str] = None
         self.is_temp_branch: bool = False
+        self.use_personal_branch: bool = use_personal_branch
+        self.personal_branch: Optional[str] = None
         self.import_managers: List[LookerBranchManager] = []
         self.skip_imports: List[str] = [] if skip_imports is None else skip_imports
 
     def __call__(
         self, ref: Optional[str] = None, ephemeral: Optional[bool] = None
     ) -> "LookerBranchManager":
         logger.debug("")
@@ -103,34 +107,38 @@
         state: ProjectState = await self.get_project_state()
         self.workspace: str = state.workspace
         self.history = [state]
         # A branch was passed, so we check it out in dev mode.
         if self.branch:
             await self.update_workspace("dev")
             if self.ephemeral:
-                self.branch = await self.checkout_temp_branch("origin/" + self.branch)
+                new_branch = await self.checkout_ephemeral_branch(
+                    "origin/" + self.branch
+                )
+                if not self.use_personal_branch:
+                    self.branch = new_branch
             else:
                 await self.client.checkout_branch(self.project, self.branch)
                 if self.remote_reset:
                     await self.client.reset_to_remote(self.project)
         # A commit was passed, so we non-destructively create a temporary branch we can
         # hard reset to the commit.
         elif self.commit:
-            self.branch = await self.checkout_temp_branch(self.commit)
+            self.branch = await self.checkout_ephemeral_branch(self.commit)
         # Neither branch nor commit were passed, so go to production.
         else:
             if self.init_state.workspace == "production":
                 prod_state = self.init_state
             else:
                 await self.update_workspace("production")
                 prod_state = await self.get_project_state()
             self.branch = prod_state.branch
             self.commit = prod_state.commit
             if self.ephemeral:
-                self.branch = await self.checkout_temp_branch(prod_state.commit)
+                self.branch = await self.checkout_ephemeral_branch(prod_state.commit)
 
         logger.debug(
             f"Set project '{self.project}' to branch '{self.branch}' @ "
             f"{(self.commit or 'HEAD')[:6]} in {self.workspace} workspace "
             f"[ephemeral = {self.ephemeral}]"
         )
 
@@ -158,14 +166,15 @@
                 elif project not in self.skip_imports:
                     import_ref = self.pin_imports.get(project, None)
                     manager = LookerBranchManager(
                         self.client,
                         project,
                         pin_imports=self.pin_imports,
                         skip_imports=self.skip_imports,
+                        use_personal_branch=self.use_personal_branch,
                     )
                     await manager(ref=import_ref, ephemeral=True).__aenter__()
                     self.import_managers.append(manager)
                     self.skip_imports.append(project)
                 else:
                     logger.debug(
                         f"Skipping project '{project}', which is already imported"
@@ -245,14 +254,35 @@
         try:
             manifest = await self.client.get_manifest(self.project)
         except LookerApiError:
             return []
         else:
             return [p["name"] for p in manifest["imports"] if not p["is_remote"]]
 
+    async def checkout_personal_branch(self, ref: str) -> str:
+        """Updates the user's personal branch to the git ref."""
+        await self.update_workspace("dev")
+        if not self.personal_branch:
+            self.personal_branch = await self.get_personal_branch()
+        await self.client.checkout_branch(self.project, self.personal_branch)
+        await self.client.reset_to_remote(self.project)
+        await self.client.hard_reset_branch(self.project, self.personal_branch, ref)
+        return self.personal_branch
+
+    async def get_personal_branch(self) -> str:
+        """Finds the name of the user's personal branch."""
+        branches = await self.client.get_all_branches(self.project)
+        for branch in branches:
+            if branch["personal"] and not branch["readonly"]:
+                return str(branch["name"])
+        raise ValueError(
+            f"Personal branch not found for client ID {self.client.client_id} "
+            f"in project '{self.project}'"
+        )
+
     async def checkout_temp_branch(self, ref: str) -> str:
         """Creates a temporary branch off a commit or off production."""
         # Save the dev mode state so we have somewhere to delete the temp branch
         # from later. We can't delete branches from prod workspace.
         await self.update_workspace("dev")
         self.history.append(await self.get_project_state())
         name = "tmp_spectacles_" + time_hash()
@@ -262,14 +292,22 @@
             f"project '{self.project}'"
         )
         await self.client.create_branch(self.project, name)
         await self.client.hard_reset_branch(self.project, name, ref)
         self.is_temp_branch = True
         return name
 
+    async def checkout_ephemeral_branch(self, ref: str) -> str:
+        """Either check out temp or personal branch and hard-reset."""
+        if self.use_personal_branch:
+            branch = await self.checkout_personal_branch(ref)
+        else:
+            branch = await self.checkout_temp_branch(ref)
+        return branch
+
 
 class Runner:
     """Runs validations and returns JSON-style dictionaries with validation results.
 
     Args:
         base_url: Base URL for the Looker instance, e.g. https://mycompany.looker.com.
         project: Name of the Looker project to use.
@@ -286,19 +324,24 @@
 
     def __init__(
         self,
         client: LookerClient,
         project: str,
         remote_reset: bool = False,
         pin_imports: Optional[Dict[str, str]] = None,
+        use_personal_branch: bool = False,
     ):
         self.project = project
         self.client = client
         self.branch_manager = LookerBranchManager(
-            client, project, remote_reset, pin_imports or {}
+            client,
+            project,
+            remote_reset,
+            pin_imports=pin_imports or {},
+            use_personal_branch=use_personal_branch,
         )
 
     async def validate_sql(
         self,
         ref: Optional[str] = None,
         filters: Optional[List[str]] = None,
         fail_fast: bool = True,
@@ -440,14 +483,15 @@
         results = project.get_results(validator="sql", fail_fast=fail_fast)
         return results
 
     async def validate_data_tests(
         self,
         ref: Optional[str] = None,
         filters: Optional[List[str]] = None,
+        concurrency: int = DATA_TEST_CONCURRENCY,
     ) -> JsonDict:
         if filters is None:
             filters = ["*/*"]
         async with self.branch_manager(ref):
             validator = DataTestValidator(self.client)
             logger.info(
                 "Building LookML project hierarchy for project "
@@ -458,24 +502,29 @@
             )
             explore_count = project.count_explores()
             print_header(
                 f"Running data tests based on {explore_count} "
                 f"{'explore' if explore_count == 1 else 'explores'}"
             )
             tests = await validator.get_tests(project)
-            await validator.validate(tests)
+            await validator.validate(tests, concurrency)
 
         results = project.get_results(validator="data_test")
         return results
 
-    async def validate_lookml(self, ref: Optional[str], severity: str) -> JsonDict:
+    async def validate_lookml(
+        self,
+        ref: Optional[str],
+        severity: str,
+        timeout: int = LOOKML_VALIDATION_TIMEOUT,
+    ) -> JsonDict:
         async with self.branch_manager(ref=ref):
             validator = LookMLValidator(self.client)
             print_header(f"Validating LookML in project {self.project} [{severity}]")
-            results = await validator.validate(self.project, severity)
+            results = await validator.validate(self.project, severity, timeout)
         return results
 
     async def validate_content(
         self,
         ref: Optional[str] = None,
         filters: Optional[List[str]] = None,
         incremental: bool = False,
```

### Comparing `spectacles-2.4.7/spectacles/tracking.py` & `spectacles-2.4.8/spectacles/tracking.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/spectacles/utils.py` & `spectacles-2.4.8/spectacles/utils.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/spectacles/validators/content.py` & `spectacles-2.4.8/spectacles/validators/content.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/spectacles/validators/data_test.py` & `spectacles-2.4.8/spectacles/validators/data_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from dataclasses import dataclass
 from typing import List, Optional
 
 from spectacles.client import LookerClient
 from spectacles.exceptions import DataTestError, SpectaclesException
 from spectacles.lookml import Explore, Project
 
-QUERY_SLOT_LIMIT = 15  # This is the per-user query limit in Looker for most instances
+DATA_TEST_CONCURRENCY = (
+    15  # This is the per-user query limit in Looker for most instances
+)
 
 
 @dataclass
 class DataTest:
     name: str
     explore: Explore
     project_name: str
@@ -90,17 +92,19 @@
                     "If you're using --explores, make sure your project "
                     "has data tests that reference those models or explores."
                 ),
             )
 
         return selected_tests
 
-    async def validate(self, tests: List[DataTest]) -> List[DataTestError]:
+    async def validate(
+        self, tests: List[DataTest], concurrency: int = DATA_TEST_CONCURRENCY
+    ) -> List[DataTestError]:
         data_test_errors: List[DataTestError] = []
-        query_slot = asyncio.Semaphore(QUERY_SLOT_LIMIT)
+        query_slot = asyncio.Semaphore(concurrency)
 
         async def run_test(test: DataTest, query_slot: asyncio.Semaphore) -> None:
             async with query_slot:
                 results = await self.client.run_lookml_test(
                     test.project_name, model=test.explore.model_name, test=test.name
                 )
                 test.explore.queried = True
```

### Comparing `spectacles-2.4.7/spectacles/validators/lookml.py` & `spectacles-2.4.8/spectacles/validators/lookml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Optional
 
-from spectacles.client import LookerClient
+from spectacles.client import LOOKML_VALIDATION_TIMEOUT, LookerClient
 from spectacles.exceptions import LookMLError
 
 # Define constants for severity levels
 SUCCESS = 0
 INFO = 10
 WARNING = 20
 ERROR = 30
@@ -27,19 +27,24 @@
         project: Name of the LookML project to validate.
 
     """
 
     def __init__(self, client: LookerClient):
         self.client = client
 
-    async def validate(self, project: str, severity: str = "warning") -> Dict[str, Any]:
+    async def validate(
+        self,
+        project: str,
+        severity: str = "warning",
+        timeout: int = LOOKML_VALIDATION_TIMEOUT,
+    ) -> Dict[str, Any]:
         severity_level: int = NAME_TO_LEVEL[severity]
         validation_results = await self.client.cached_lookml_validation(project)
         if not validation_results or validation_results.get("stale"):
-            validation_results = await self.client.lookml_validation(project)
+            validation_results = await self.client.lookml_validation(project, timeout)
         errors = []
         lookml_url: Optional[str] = None
         for error in validation_results["errors"]:
             if error["file_path"]:
                 lookml_url = (
                     self.client.base_url
                     + "/projects/"
```

### Comparing `spectacles-2.4.7/spectacles/validators/sql.py` & `spectacles-2.4.8/spectacles/validators/sql.py`

 * *Files identical despite different names*

### Comparing `spectacles-2.4.7/PKG-INFO` & `spectacles-2.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectacles
-Version: 2.4.7
+Version: 2.4.8
 Summary: A command-line, continuous integration tool for Looker and LookML.
 License: MIT
 Keywords: Looker,LookML,CI,continuous integration,testing,validation
 Author: Spectacles
 Author-email: hello@spectacles.dev
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

