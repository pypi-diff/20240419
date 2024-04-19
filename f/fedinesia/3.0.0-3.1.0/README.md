# Comparing `tmp/fedinesia-3.0.0.tar.gz` & `tmp/fedinesia-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedinesia-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fedinesia-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedinesia-3.0.0.tar` & `fedinesia-3.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3544 2023-12-16 07:32:50.402722 fedinesia-3.0.0/README.rst
--rw-r--r--   0        0        0     2382 2024-03-24 00:52:57.903722 fedinesia-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      618 2024-03-24 00:52:57.903722 fedinesia-3.0.0/src/fedinesia/__init__.py
--rw-r--r--   0        0        0    11982 2024-03-24 00:52:57.907055 fedinesia-3.0.0/src/fedinesia/amnesia.py
--rw-r--r--   0        0        0    12472 2024-03-24 00:52:57.907055 fedinesia-3.0.0/src/fedinesia/config.py
--rw-r--r--   0        0        0     7655 2024-03-24 00:52:57.907055 fedinesia-3.0.0/src/fedinesia/util.py
--rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 fedinesia-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3544 2024-04-19 09:32:31.690687 fedinesia-3.1.0/README.rst
+-rw-r--r--   0        0        0     2484 2024-04-19 09:32:31.690687 fedinesia-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      618 2024-04-19 09:32:31.690687 fedinesia-3.1.0/src/fedinesia/__init__.py
+-rw-r--r--   0        0        0    11337 2024-04-19 09:32:31.690687 fedinesia-3.1.0/src/fedinesia/amnesia.py
+-rw-r--r--   0        0        0    12472 2024-04-19 09:32:31.690687 fedinesia-3.1.0/src/fedinesia/config.py
+-rw-r--r--   0        0        0     7655 2024-04-19 09:32:31.690687 fedinesia-3.1.0/src/fedinesia/util.py
+-rw-r--r--   0        0        0     4863 1970-01-01 00:00:00.000000 fedinesia-3.1.0/PKG-INFO
```

### Comparing `fedinesia-3.0.0/README.rst` & `fedinesia-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `fedinesia-3.0.0/pyproject.toml` & `fedinesia-3.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,44 +7,50 @@
 description = 'Deletes old posts from fediverse accounts. Confirmed working with Mastodon, Pleroma (and Forks), and Takahe'
 readme = "README.rst"
 authors = [
   { name = "marvin8", email = "marvin8@tuta.io" },
 ]
 requires-python = ">=3.9, <3.13"
 license = {text = "AGPL-3.0-or-later"}
-version = "3.0.0"
+version = "3.1.0"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
     "loguru>=0.7.2",
-    "minimal-activitypub>=1.1.0",
+    "minimal-activitypub>=1.2.0",
     "msgspec>=0.18.6",
     "python-dateutil>=2.9.0.post0",
+    "stamina>=24.2.0",
     "tomli>=2.0.1",
     "tqdm>=4.66.2",
-    "typer>=0.10.0",
-    "typing-extensions>=4.10.0",
+    "typer>=0.12.3",
+    "typing-extensions>=4.11.0",
 ]
 
 [project.scripts]
 fedinesia = "fedinesia.amnesia:start"
 
 [project.urls]
 Documentation = "https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/README.rst"
 Issues = "https://codeberg.org/MarvinsMastodonTools/fedinesia/issues"
 Source = "https://codeberg.org/MarvinsMastodonTools/fedinesia"
 Changelog = "https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/CHANGELOG.rst"
 
+[project.optional-dependencies]
+dev = [
+    "constable>=0.3.1",
+]
+
 [tool.interrogate]
 ignore-init-method = true
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = false
 ignore-private = false
 ignore-property-decorators = false
@@ -78,7 +84,9 @@
 warn_unused_configs = true
 no_implicit_reexport = true
 
 [tool.scriv]
 categories = "Breaking, Added, Changed, Deprecated, Removed, Fixed, Security"
 format = "rst"
 version = "literal: pyproject.toml: project.version"
+
+[tool.pdm]
```

### Comparing `fedinesia-3.0.0/src/fedinesia/__init__.py` & `fedinesia-3.1.0/src/fedinesia/__init__.py`

 * *Files identical despite different names*

### Comparing `fedinesia-3.0.0/src/fedinesia/amnesia.py` & `fedinesia-3.1.0/src/fedinesia/amnesia.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,22 +25,26 @@
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import msgspec
+import stamina
 import typer
 from dateutil.parser import isoparse
 from httpx import AsyncClient
 from httpx import HTTPError
 from loguru import logger as log
 from minimal_activitypub.client_2_server import ActivityPub
 from minimal_activitypub.client_2_server import ActivityPubError
+from minimal_activitypub.client_2_server import NetworkError
+from minimal_activitypub.client_2_server import NotFoundError
 from minimal_activitypub.client_2_server import RatelimitError
+from stamina import retry_context
 from tqdm import tqdm
 from tqdm import trange
 from typing_extensions import Annotated
 
 from fedinesia import UTC
 from fedinesia import Status
 from fedinesia import __display_name__
@@ -56,22 +60,23 @@
 
     for handler in logging_config.get("handlers"):
         if handler.get("sink") == "sys.stdout":
             handler["sink"] = sys.stdout
 
     log.configure(**logging_config)
 
+stamina.instrumentation.set_on_retry_hooks([])
+
 
 @log.catch
-async def main(  # noqa: C901, PLR0912, PLR0913, PLR0915
+async def main(  # noqa: C901, PLR0912, PLR0915
     config_file: str,
     is_dry_run: bool,
     audit_log_file: Optional[str],
-    audit_log_style: Optional[str],
-    batch_size: Optional[int],
+    audit_log_style: Optional[AuditLog.Style],
     limit: Optional[int],
 ) -> None:
     """Perform app function."""
     config = await setup_shop(config_file=config_file)
 
     oldest_to_keep = datetime.now(tz=UTC) - timedelta(seconds=config.bot.delete_after)
 
@@ -94,15 +99,17 @@
         )
 
         audit_log = None
         if audit_log_file:
             log.info(f"A record of all deleted statuses will be recorded in the audit log file at {audit_log_file}")
             audit_log = AuditLog.open(audit_log_file=audit_log_file, style=audit_log_style)
 
-        statuses = await instance.get_account_statuses(account_id=user_info["id"])
+        for attempt in retry_context(on=NetworkError, attempts=3):
+            with attempt:
+                statuses = await instance.get_account_statuses(account_id=user_info["id"])
     except RatelimitError:
         log.info(
             f"RateLimited during startup, [red]Please wait until[/red] {instance.ratelimit_reset} before trying again"
         )
         sys.exit(429)
     except (HTTPError, ActivityPubError):
         log.exception("!!! Cannot continue.")
@@ -155,19 +162,21 @@
             if limit and len(statuses_to_delete) >= limit:
                 break
 
             # Get More statuses if available:
             log.debug("get next batch of statuses if available.")
             log.debug(f"{instance.pagination=}")
             if instance.pagination["next"]["max_id"] or instance.pagination["next"]["min_id"]:
-                statuses = await instance.get_account_statuses(
-                    account_id=user_info["id"],
-                    max_id=instance.pagination["next"]["max_id"],
-                    min_id=instance.pagination["next"]["min_id"],
-                )
+                for attempt in retry_context(on=NetworkError):
+                    with attempt:
+                        statuses = await instance.get_account_statuses(
+                            account_id=user_info["id"],
+                            max_id=instance.pagination["next"]["max_id"],
+                            min_id=instance.pagination["next"]["min_id"],
+                        )
                 log.debug(f"scrolling - {len(statuses)=}")
                 if len(statuses) == 0:
                     break
             else:
                 break
 
         except RatelimitError:
@@ -187,66 +196,41 @@
             log.opt(colors=True).info(
                 f"<red>Would</red> delete status" f" {status.get('url')} from {status.get('created_at')}"
             )
         log.opt(colors=True).info(f"<bold>Total of {total_statuses_to_delete} statuses would be deleted.</>")
 
     # Dry-run has not been specified... delete statuses!
     else:
-        await delete_statuses(
-            instance=instance,
-            statuses_to_delete=statuses_to_delete,
-            audit=audit_log,
-            batch_size=batch_size,
-        )
+        await delete_statuses(instance=instance, statuses_to_delete=statuses_to_delete, audit=audit_log)
         log.info(f"All old statuses deleted! Total of {total_statuses_to_delete} statuses deleted")
 
     if audit_log:
         audit_log.close()
     await client.aclose()
 
 
-async def delete_statuses(
-    instance: ActivityPub,
-    statuses_to_delete: List[Status],
-    audit: Optional[AuditLog],
-    batch_size: Optional[int],
-) -> None:
+async def delete_statuses(instance: ActivityPub, statuses_to_delete: List[Status], audit: Optional[AuditLog]) -> None:
     """Delete all statuses that should be deleted."""
     title = "Deleting statuses"
     total_statuses_to_delete = len(statuses_to_delete)
-    if total_statuses_to_delete > 0:
-        with tqdm(
-            desc=f"{title:.<60}",
-            ncols=120,
-            total=total_statuses_to_delete,
-            unit="statuses",
-            position=0,
-            bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt} at {rate_fmt}",
-        ) as progress_bar:
-            while len(statuses_to_delete) > 0:
-                tasks = []
-                for status in statuses_to_delete:
-                    tasks.append(delete_single_status(status=status, instance=instance, audit=audit))
-                    if batch_size and len(tasks) >= batch_size:
-                        break
-
-                responses = await asyncio.gather(*tasks)
-
-                # Filter out any responses that are None...
-                # Those encountered Rate Limiting
-                deleted_statuses = [status for status in responses if status is not None]
-                log.debug(f"delete_statuses - {len(deleted_statuses)=}")
-
-                progress_bar.update(len(deleted_statuses))
-
-                if len(deleted_statuses) < len(statuses_to_delete):
-                    await sleep_off_ratelimiting(instance=instance)
-
-                for status in deleted_statuses:
-                    statuses_to_delete.remove(status)
+    for status in tqdm(
+        iterable=statuses_to_delete,
+        desc=f"{title:.<60}",
+        ncols=120,
+        total=total_statuses_to_delete,
+        unit="statuses",
+        position=0,
+        bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt} at {rate_fmt}",
+    ):
+        try:
+            for attempt in retry_context(on=NetworkError):
+                with attempt:
+                    await delete_single_status(status=status, instance=instance, audit=audit)
+        except RatelimitError:
+            await sleep_off_ratelimiting(instance=instance)
 
 
 async def sleep_off_ratelimiting(
     instance: ActivityPub,
 ) -> None:
     """Wait for rate limiting to be over."""
     log.debug(
@@ -277,44 +261,39 @@
     log.debug(f"delete_single_status(status={status['id']}, instance={instance.instance})")
     return_status: Optional[Status] = status
     try:
         await instance.delete_status(status=status)
         log.debug(f"delete_single_status - Deleted status {status.get('url')} from {status.get('created_at')}")
         if audit:
             audit.add_entry(status=status)
-    except RatelimitError:
-        log.debug(
-            f"delete_single_status - {status['id']=} - {instance.ratelimit_remaining=} - {instance.ratelimit_reset=}"
-        )
-        return_status = None
+    except NotFoundError:
+        log.debug("Status for deletion not found. No problem then :)")
     except ActivityPubError as error:
         log.debug(f"delete_single_status - encountered error: {error}")
         log.debug(f"delete_single_status - status: {json.dumps(status, indent=4)}")
         raise error
 
     return return_status
 
 
 def start() -> None:
     """Start app."""
     typer.run(typer_async_shim)
 
 
-def typer_async_shim(  # noqa PLR0913
+def typer_async_shim(
     config_file: Annotated[str, typer.Option("-c", "--config-file")] = "config.json",
     audit_log_file: Annotated[Optional[str], typer.Option("-a", "--audit-log-file")] = None,
     audit_log_style: Optional[AuditLog.Style] = AuditLog.Style.PLAIN,
-    batch_size: Annotated[Optional[int], typer.Option("-b", "--batch-size")] = None,
     limit: Annotated[Optional[int], typer.Option("-l", "--limit")] = None,
     dry_run: Annotated[bool, typer.Option("-d", "--dry-run")] = False,
 ) -> None:
     """Delete fediverse history. For more information look at https://codeberg.org/MarvinsMastodonTools/fedinesia."""
     asyncio.run(
         main(
             config_file=config_file,
             is_dry_run=dry_run,
             audit_log_file=audit_log_file,
             audit_log_style=audit_log_style,
-            batch_size=batch_size,
             limit=limit,
         )
     )
```

### Comparing `fedinesia-3.0.0/src/fedinesia/config.py` & `fedinesia-3.1.0/src/fedinesia/config.py`

 * *Files identical despite different names*

### Comparing `fedinesia-3.0.0/src/fedinesia/util.py` & `fedinesia-3.1.0/src/fedinesia/util.py`

 * *Files identical despite different names*

### Comparing `fedinesia-3.0.0/PKG-INFO` & `fedinesia-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: fedinesia
-Version: 3.0.0
+Version: 3.1.0
 Summary: Deletes old posts from fediverse accounts. Confirmed working with Mastodon, Pleroma (and Forks), and Takahe
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.9, <3.13
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru>=0.7.2
-Requires-Dist: minimal-activitypub>=1.1.0
+Requires-Dist: minimal-activitypub>=1.2.0
 Requires-Dist: msgspec>=0.18.6
 Requires-Dist: python-dateutil>=2.9.0.post0
+Requires-Dist: stamina>=24.2.0
 Requires-Dist: tomli>=2.0.1
 Requires-Dist: tqdm>=4.66.2
-Requires-Dist: typer>=0.10.0
-Requires-Dist: typing-extensions>=4.10.0
+Requires-Dist: typer>=0.12.3
+Requires-Dist: typing-extensions>=4.11.0
+Requires-Dist: constable>=0.3.1 ; extra == "dev"
 Project-URL: Changelog, https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/CHANGELOG.rst
 Project-URL: Documentation, https://codeberg.org/MarvinsMastodonTools/fedinesia/src/branch/main/README.rst
 Project-URL: Issues, https://codeberg.org/MarvinsMastodonTools/fedinesia/issues
 Project-URL: Source, https://codeberg.org/MarvinsMastodonTools/fedinesia
+Provides-Extra: dev
 
 """"""""""""""""""""""""""
 Fedinesia
 """"""""""""""""""""""""""
 
 |Repo| |CI| |Downloads|
```

