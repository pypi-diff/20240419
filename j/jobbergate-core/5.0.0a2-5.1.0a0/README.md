# Comparing `tmp/jobbergate_core-5.0.0a2.tar.gz` & `tmp/jobbergate_core-5.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_core-5.0.0a2.tar", max compression
+gzip compressed data, was "jobbergate_core-5.1.0a0.tar", max compression
```

## Comparing `jobbergate_core-5.0.0a2.tar` & `jobbergate_core-5.1.0a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1082 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/LICENSE
--rw-r--r--   0        0        0      371 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/README.md
--rw-r--r--   0        0        0      330 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/jobbergate_core/__init__.py
--rw-r--r--   0        0        0      367 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/jobbergate_core/auth/__init__.py
--rw-r--r--   0        0        0      279 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/jobbergate_core/auth/exceptions.py
--rw-r--r--   0        0        0    11832 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/jobbergate_core/auth/handler.py
--rw-r--r--   0        0        0     5529 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/jobbergate_core/auth/token.py
--rw-r--r--   0        0        0        0 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/jobbergate_core/py.typed
--rw-r--r--   0        0        0        0 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/jobbergate_core/tools/__init__.py
--rw-r--r--   0        0        0     6334 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/jobbergate_core/tools/sbatch.py
--rw-r--r--   0        0        0      209 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/jobbergate_core/version.py
--rw-r--r--   0        0        0     1813 2024-04-10 20:48:38.060053 jobbergate_core-5.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 jobbergate_core-5.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/LICENSE
+-rw-r--r--   0        0        0      371 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/README.md
+-rw-r--r--   0        0        0      330 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/jobbergate_core/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/jobbergate_core/auth/__init__.py
+-rw-r--r--   0        0        0      279 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/jobbergate_core/auth/exceptions.py
+-rw-r--r--   0        0        0    11832 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/jobbergate_core/auth/handler.py
+-rw-r--r--   0        0        0     5529 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/jobbergate_core/auth/token.py
+-rw-r--r--   0        0        0        0 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/jobbergate_core/py.typed
+-rw-r--r--   0        0        0        0 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/jobbergate_core/tools/__init__.py
+-rw-r--r--   0        0        0     6411 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/jobbergate_core/tools/sbatch.py
+-rw-r--r--   0        0        0      209 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/jobbergate_core/version.py
+-rw-r--r--   0        0        0     1813 2024-04-19 17:22:07.528119 jobbergate_core-5.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 jobbergate_core-5.1.0a0/PKG-INFO
```

### Comparing `jobbergate_core-5.0.0a2/LICENSE` & `jobbergate_core-5.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_core-5.0.0a2/jobbergate_core/auth/handler.py` & `jobbergate_core-5.1.0a0/jobbergate_core/auth/handler.py`

 * *Files identical despite different names*

### Comparing `jobbergate_core-5.0.0a2/jobbergate_core/auth/token.py` & `jobbergate_core-5.1.0a0/jobbergate_core/auth/token.py`

 * *Files identical despite different names*

### Comparing `jobbergate_core-5.0.0a2/jobbergate_core/tools/sbatch.py` & `jobbergate_core-5.1.0a0/jobbergate_core/tools/sbatch.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 import re
 import shlex
 import subprocess
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Any, Callable, ClassVar, Sequence
+from typing import Any, ClassVar, Sequence
 
 from buzz import check_expressions
 from loguru import logger
 
 
 def inject_sbatch_params(job_script_data_as_string: str, sbatch_params: list[str], header: str | None = None) -> str:
     """
@@ -47,36 +47,35 @@
         job_script_data_as_string[:insert_index] + inner_string + job_script_data_as_string[insert_index:]
     )
 
     logger.debug("Done injecting sbatch params into job script")
     return new_job_script_data_as_string
 
 
-@dataclass(frozen=True)
-class Command:
-    preexec_fn: Callable | None = None
+@dataclass
+class SubprocessHandler:
 
-    def run_command(self, cmd: Sequence[str], **kwargs) -> subprocess.CompletedProcess:
-        """Runs a command as the user."""
+    def run(self, cmd: Sequence[str], **kwargs) -> subprocess.CompletedProcess:
         logger.debug("Running command '{}' with kwargs: {}", " ".join(cmd), kwargs)
         try:
-            result = subprocess.run(cmd, preexec_fn=self.preexec_fn, check=True, shell=False, **kwargs)
+            result = subprocess.run(cmd, check=True, shell=False, **kwargs)
             logger.trace("Command returned code {} with result: {}", result.returncode, result.stdout)
             return result
         except subprocess.CalledProcessError as e:
             message = f"Failed to run command with code {e.returncode}: {e.stderr or e.stdout}"
             logger.error(message)
             raise RuntimeError(message) from e
 
 
 @dataclass(frozen=True)
-class InfoHandler(Command):
+class InfoHandler:
     """Get info from jobs on the cluster."""
 
     scontrol_path: Path = Path("/usr/bin/scontrol")
+    subprocess_handler: SubprocessHandler = field(default_factory=SubprocessHandler)
 
     def __post_init__(self):
         with check_expressions("Check paths", raise_exc_class=ValueError) as check:
             check(self.scontrol_path.is_absolute(), "scontrol_path is not an absolute path")
             check(self.scontrol_path.exists(), "scontrol_path does not exist")
 
     def get_job_info(self, slurm_id: int) -> dict[str, Any]:
@@ -84,15 +83,15 @@
         command = (
             self.scontrol_path.as_posix(),
             "show",
             "job",
             shlex.quote(str(slurm_id)),
             "--json",
         )
-        completed_process = self.run_command(command, capture_output=True, text=True)
+        completed_process = self.subprocess_handler.run(command, capture_output=True, text=True)
         data = json.loads(completed_process.stdout)
         try:
             job_info = data["jobs"][0]
             logger.debug(f"Information for {slurm_id=} is: {job_info}")
             return job_info
         except KeyError as e:
             message = f"Failed to parse job info from {completed_process.stdout}"
@@ -101,19 +100,20 @@
         except IndexError as e:
             message = f"Job not fount: {slurm_id}"
             logger.warning(message)
             raise RuntimeError(message) from e
 
 
 @dataclass(frozen=True)
-class SubmissionHandler(Command):
+class SubmissionHandler:
     """Submits sbatch jobs to the cluster."""
 
     sbatch_path: Path = Path("/usr/bin/sbatch")
     submission_directory: Path = field(default_factory=Path.cwd)
+    subprocess_handler: SubprocessHandler = field(default_factory=SubprocessHandler)
 
     sbatch_output_parser: ClassVar[re.Pattern] = re.compile(r"^(?P<id>\d+)(,(?P<cluster_name>.+))?$")
 
     def __post_init__(self):
         with check_expressions("Check paths", raise_exc_class=ValueError) as check:
             check(self.sbatch_path.is_absolute(), "sbatch_path is not an absolute path")
             check(self.sbatch_path.exists(), "sbatch_path does not exist")
@@ -124,15 +124,17 @@
         """Runs sbatch as the user to submit a job script and returns the slurm id assigned to it."""
         command = (
             self.sbatch_path.as_posix(),
             "--parsable",
             job_script_path.as_posix(),
         )
 
-        completed_process = self.run_command(command, cwd=self.submission_directory, capture_output=True, text=True)
+        completed_process = self.subprocess_handler.run(
+            command, cwd=self.submission_directory, capture_output=True, text=True
+        )
 
         if match := self.sbatch_output_parser.match(completed_process.stdout):
             slurm_id = int(match.group("id"))
             logger.debug(f"Submission succeeded with {slurm_id=}")
             return slurm_id
         message = f"Failed to parse slurm job id from {completed_process.stdout}"
         logger.error(message)
@@ -141,15 +143,15 @@
     def copy_file_to_submission_directory(self, source_file: Path) -> Path:
         """Copies the job file to the submission directory as the user."""
         # Reference: https://stackoverflow.com/a/71589233
         destination_file = self.submission_directory / source_file.name
         command = ("tee", destination_file.as_posix())
         try:
             with source_file.open("rb") as source:
-                self.run_command(
+                self.subprocess_handler.run(
                     command,
                     stdin=source,
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.PIPE,
                     text=True,
                 )
         except IOError as e:
```

### Comparing `jobbergate_core-5.0.0a2/pyproject.toml` & `jobbergate_core-5.1.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-core"
-version = "5.0.0a2"
+version = "5.1.0a0"
 description = "Jobbergate Core"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_core-5.0.0a2/PKG-INFO` & `jobbergate_core-5.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-core
-Version: 5.0.0a2
+Version: 5.1.0a0
 Summary: Jobbergate Core
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

