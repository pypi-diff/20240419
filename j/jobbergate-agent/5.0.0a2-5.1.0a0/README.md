# Comparing `tmp/jobbergate_agent-5.0.0a2.tar.gz` & `tmp/jobbergate_agent-5.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_agent-5.0.0a2.tar", max compression
+gzip compressed data, was "jobbergate_agent-5.1.0a0.tar", max compression
```

## Comparing `jobbergate_agent-5.0.0a2.tar` & `jobbergate_agent-5.1.0a0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1077 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/LICENSE
--rw-r--r--   0        0        0     1346 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/README.md
--rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/clients/__init__.py
--rw-r--r--   0        0        0     3597 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/clients/cluster_api.py
--rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/internals/__init__.py
--rw-r--r--   0        0        0     4305 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/internals/update.py
--rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/__init__.py
--rw-r--r--   0        0        0      150 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/constants.py
--rw-r--r--   0        0        0     2805 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/schemas.py
--rw-r--r--   0        0        0    11259 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/submit.py
--rw-r--r--   0        0        0     3676 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/update.py
--rw-r--r--   0        0        0      491 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/main.py
--rw-r--r--   0        0        0     2759 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/settings.py
--rw-r--r--   0        0        0     2627 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/tasks.py
--rw-r--r--   0        0        0        0 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/__init__.py
--rw-r--r--   0        0        0     4663 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/exception.py
--rw-r--r--   0        0        0     1440 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/logging.py
--rw-r--r--   0        0        0     1414 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/plugin.py
--rw-r--r--   0        0        0     2153 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/scheduler.py
--rw-r--r--   0        0        0      730 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/sentry.py
--rw-r--r--   0        0        0     2500 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/jobbergate_agent/utils/user_mapper.py
--rw-r--r--   0        0        0     3235 2024-04-10 20:48:36.580898 jobbergate_agent-5.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/LICENSE
+-rw-r--r--   0        0        0     1346 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/clients/__init__.py
+-rw-r--r--   0        0        0     3597 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/clients/cluster_api.py
+-rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/internals/__init__.py
+-rw-r--r--   0        0        0     4305 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/internals/update.py
+-rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/constants.py
+-rw-r--r--   0        0        0      636 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/report_health.py
+-rw-r--r--   0        0        0     2805 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/schemas.py
+-rw-r--r--   0        0        0    11828 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/submit.py
+-rw-r--r--   0        0        0     3676 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/update.py
+-rw-r--r--   0        0        0      491 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/main.py
+-rw-r--r--   0        0        0     2759 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/settings.py
+-rw-r--r--   0        0        0     3035 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/__init__.py
+-rw-r--r--   0        0        0     4663 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/exception.py
+-rw-r--r--   0        0        0     1440 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/logging.py
+-rw-r--r--   0        0        0     1414 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/plugin.py
+-rw-r--r--   0        0        0     2153 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/scheduler.py
+-rw-r--r--   0        0        0      730 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/sentry.py
+-rw-r--r--   0        0        0     2500 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/user_mapper.py
+-rw-r--r--   0        0        0     3295 2024-04-19 17:22:06.554111 jobbergate_agent-5.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.1.0a0/PKG-INFO
```

### Comparing `jobbergate_agent-5.0.0a2/LICENSE` & `jobbergate_agent-5.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/README.md` & `jobbergate_agent-5.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/clients/cluster_api.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/clients/cluster_api.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/internals/update.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/internals/update.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/schemas.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/submit.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/submit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import asyncio
-import functools
 import os
 import pwd
+from dataclasses import dataclass
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from buzz import DoExceptParams
-from jobbergate_core.tools.sbatch import InfoHandler, SubmissionHandler, inject_sbatch_params
+from jobbergate_core.tools.sbatch import InfoHandler, SubmissionHandler, SubprocessHandler, inject_sbatch_params
 from loguru import logger
 
 from jobbergate_agent.clients.cluster_api import backend_client as jobbergate_api_client
 from jobbergate_agent.jobbergate.constants import FileType
 from jobbergate_agent.jobbergate.schemas import JobScriptFile, PendingJobSubmission, SlurmJobData
 from jobbergate_agent.jobbergate.update import fetch_job_data
 from jobbergate_agent.settings import SETTINGS
@@ -158,27 +158,34 @@
                 id=job_submission_id,
                 report_message=report_message,
             ),
         )
         response.raise_for_status()
 
 
-@functools.lru_cache(maxsize=64)
-def run_as_user(username):
-    """Provide to subprocess.run a way to run a command as the user."""
-    # Get the uid and gid from the username
-    pwan = pwd.getpwnam(username)
-    uid = pwan.pw_uid
-    gid = pwan.pw_gid
-
-    def preexec():  # Function to be run in the child process before the subprocess call
-        os.setgid(gid)
-        os.setuid(uid)
-
-    return preexec
+@dataclass
+class SubprocessAsUserHandler(SubprocessHandler):
+    """Subprocess handler that runs as a given user."""
+
+    username: str
+
+    def __post_init__(self):
+        pwan = pwd.getpwnam(self.username)
+        self.uid = pwan.pw_uid
+        self.gid = pwan.pw_gid
+
+    def run(self, *args, **kwargs):
+        kwargs.update(user=self.uid, group=self.gid)
+        # Tests indicate that the change on the working directory precedes the change of user on the subprocess.
+        # With that, the user running the agent can face permission denied errors on cwd,
+        # depending on the setting on the filesystem and permissions on the directory.
+        # To avoid this, we change the working directory after changing to the submitter user using preexec_fn.
+        if cwd := kwargs.pop("cwd", None):
+            kwargs["preexec_fn"] = lambda: os.chdir(cwd)
+        return super().run(*args, **kwargs)
 
 
 async def submit_job_script(
     pending_job_submission: PendingJobSubmission,
     user_mapper: SlurmUserMapper,
 ) -> int:
     """
@@ -204,26 +211,26 @@
         do_except=_reject_handler,
     ):
         email = pending_job_submission.owner_email
         mapper_class_name = user_mapper.__class__.__name__
         logger.debug(f"Fetching username for email '{email}' with mapper {mapper_class_name}")
         username = user_mapper[email]
         logger.debug(f"Using local slurm user '{username}' for job submission")
-        preexec_fn = run_as_user(username)
+        subprocess_handler = SubprocessAsUserHandler(username)
 
     submit_dir = pending_job_submission.execution_directory or SETTINGS.DEFAULT_SLURM_WORK_DIR
     if not submit_dir.exists() or not submit_dir.is_absolute():
         message = f"The execution directory must exist and be an absolute path, but got '{submit_dir.as_posix()}'"
         await mark_as_rejected(pending_job_submission.id, message)
         raise JobSubmissionError(message)
 
     sbatch_handler = SubmissionHandler(
         sbatch_path=SETTINGS.SBATCH_PATH,
         submission_directory=submit_dir,
-        preexec_fn=preexec_fn,
+        subprocess_handler=subprocess_handler,
     )
 
     with TemporaryDirectory(prefix=str(pending_job_submission.id), suffix=pending_job_submission.name) as tmp_dir:
         tmp_dir_path = Path(tmp_dir)
         async with handle_errors_async(
             "Error processing job-script files",
             raise_exc_class=JobSubmissionError,
```

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/jobbergate/update.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/update.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/settings.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/settings.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/tasks.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/tasks.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Union
 
 from buzz import handle_errors
 from loguru import logger
 
 from jobbergate_agent.clients.cluster_api import backend_client
 from jobbergate_agent.internals.update import self_update_agent
+from jobbergate_agent.jobbergate.report_health import report_health_status
 from jobbergate_agent.jobbergate.submit import submit_pending_jobs
 from jobbergate_agent.jobbergate.update import update_active_jobs
 from jobbergate_agent.settings import SETTINGS
 from jobbergate_agent.utils.logging import log_error, logger_wraps
 from jobbergate_agent.utils.scheduler import BaseScheduler, Job
 
 
@@ -34,14 +35,24 @@
 def pending_submissions_task(scheduler: BaseScheduler) -> Job:
     """
     Schedule a task to submit pending jobs every ``TASK_JOBS_INTERVAL_SECONDS`` seconds.
     """
     return scheduler.add_job(submit_pending_jobs, "interval", seconds=SETTINGS.TASK_JOBS_INTERVAL_SECONDS)
 
 
+def status_report_task(scheduler: BaseScheduler) -> Job:
+    """
+    Schedule a task to report the status.
+    """
+    seconds_between_calls = SETTINGS.TASK_JOBS_INTERVAL_SECONDS
+    return scheduler.add_job(
+        report_health_status, "interval", seconds=seconds_between_calls, kwargs={"interval": seconds_between_calls}
+    )
+
+
 @logger_wraps()
 async def trigger_garbage_collections(interval_between_calls: int = 60) -> None:
     """Trigger maintenance tasks on the Jobbergate API."""
     for path in (
         "/jobbergate/job-script-templates/upload/garbage-collector",
         "/jobbergate/job-scripts/upload/garbage-collector",
         "/jobbergate/job-scripts/clean-unused-entries",
```

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/exception.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/exception.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/logging.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/plugin.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/plugin.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/scheduler.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/sentry.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/sentry.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/jobbergate_agent/utils/user_mapper.py` & `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/user_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.0.0a2/pyproject.toml` & `jobbergate_agent-5.1.0a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-agent"
-version = "5.0.0a2"
+version = "5.1.0a0"
 description = "Jobbergate Agent"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -44,14 +44,15 @@
 
 [tool.poetry.scripts]
 jg-run = "jobbergate_agent.main:main"
 
 [tool.poetry.plugins.'jobbergate_agent.tasks']
 active-jobs = 'jobbergate_agent.tasks:active_submissions_task'
 pending-jobs = 'jobbergate_agent.tasks:pending_submissions_task'
+report-status = 'jobbergate_agent.tasks:status_report_task'
 garbage-collection = 'jobbergate_agent.tasks:garbage_collection_task'
 self-update = 'jobbergate_agent.tasks:self_update_task'
 
 [tool.poetry.plugins.'jobbergate_agent.user_mapper']
 single-user-mapper = "jobbergate_agent.utils.user_mapper:SingleUserMapper"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `jobbergate_agent-5.0.0a2/PKG-INFO` & `jobbergate_agent-5.1.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-agent
-Version: 5.0.0a2
+Version: 5.1.0a0
 Summary: Jobbergate Agent
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: apscheduler (==3.10.3)
 Requires-Dist: auto-name-enum (>=2.0.0,<3.0.0)
 Requires-Dist: httpx (==0.24.1)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0) ; python_version < "3.10"
-Requires-Dist: jobbergate-core (==5.0.0a2)
+Requires-Dist: jobbergate-core (==5.1.0a0)
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: py-buzz (>=4.0.0,<5.0.0)
 Requires-Dist: pydantic (==1.10.12)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-jose (==3.3.0)
 Requires-Dist: sentry-sdk (>=1.1.0,<2.0.0)
```

