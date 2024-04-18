# Comparing `tmp/codestarter-0.0.0.tar.gz` & `tmp/codestarter-0.0.1.tar.gz`

## Comparing `codestarter-0.0.0.tar` & `codestarter-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/__init__.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/cli.py
--rw-r--r--   0        0        0    10479 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/executor.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/utils.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/dependency_resolvers/__init__.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/dependency_resolvers/requirements_resolver.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/dependency_resolvers/utils.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/file/__init__.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/file/local.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 codestarter-0.0.0/src/codestarter/file/utils.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 codestarter-0.0.0/.gitignore
--rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 codestarter-0.0.0/LICENSE
--rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 codestarter-0.0.0/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 codestarter-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 codestarter-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/__init__.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/cli.py
+-rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/executor.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/utils.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/dependency_resolvers/__init__.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/dependency_resolvers/requirements_resolver.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/dependency_resolvers/utils.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/file/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/file/local.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 codestarter-0.0.1/src/codestarter/file/utils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 codestarter-0.0.1/.gitignore
+-rw-r--r--   0        0        0    10932 2020-02-02 00:00:00.000000 codestarter-0.0.1/LICENSE
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 codestarter-0.0.1/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 codestarter-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 codestarter-0.0.1/PKG-INFO
```

### Comparing `codestarter-0.0.0/src/codestarter/cli.py` & `codestarter-0.0.1/src/codestarter/cli.py`

 * *Files identical despite different names*

### Comparing `codestarter-0.0.0/src/codestarter/executor.py` & `codestarter-0.0.1/src/codestarter/executor.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,42 +66,54 @@
 
 
 class ResourceSettings(BaseModel):
     auto_overwrite: bool
 
 
 class ResourceConfig(BaseModel):
+    model_config = ConfigDict(extra="forbid")
     input_path: str
     dependencies: dict[DependencyKey, list[DependencyValue]] = Field(
         default_factory=dict
     )
     replace_configs: list[ReplaceConfig] = Field(default_factory=list)
     output_path: str
+    exclude_patterns: list[str] = Field(default_factory=list)
+    include_patterns: list[str] = Field(default_factory=list)
     auto_overwrite: Optional[bool] = None
+    maintain_directory_structure: Optional[bool] = None
 
     def resolve_settings(self, auto_overwrite: bool) -> ResourceSettings:
         return ResourceSettings(
             auto_overwrite=(
                 auto_overwrite
                 if self.auto_overwrite is None
                 else self.auto_overwrite
             )
         )
 
     def _get_output_path(
         self,
         input_file_path: str,
+        input_base_path: str,
         input_file_type: FileType,
         output_file_path: str,
         output_file_type: FileType,
+        maintain_directory_structure: bool,
     ) -> str:
         if input_file_type == FileType.directory:
             assert output_file_type == FileType.directory
-            input_filename = input_file_path.split("/")[-1]
-            return os.path.join(output_file_path, input_filename)
+            if maintain_directory_structure:
+                relative_path = os.path.relpath(
+                    input_file_path, input_base_path
+                )
+                return os.path.join(output_file_path, relative_path)
+            else:
+                input_filename = input_file_path.split("/")[-1]
+                return os.path.join(output_file_path, input_filename)
         elif input_file_type == FileType.file:
             if output_file_type == FileType.directory:
                 input_filename = input_file_path.split("/")[-1]
                 return os.path.join(output_file_path, input_filename)
             elif output_file_type == FileType.file:
                 return output_file_path
             else:
@@ -138,47 +150,65 @@
                 "Output path does not match input path and does not end with extension, assuming output path is a directory"
             )
             return FileType.directory
 
     async def process_resource(
         self,
         global_auto_overwrite: bool,
+        global_maintain_directory_structure: bool,
         global_variables: dict[str, str],
+        global_replace_configs: list[ReplaceConfig],
     ) -> StatusCounter:
         status_counter = StatusCounter()
         file_client = get_file_client(self.input_path)
 
         try:
             input_file_type = await file_client.validate_file(self.input_path)
         except FileNotFoundError:
             logger.error(f"ERROR: Input path {self.input_path} not found")
             status_counter.fail += 1
             return status_counter
 
         output_file_type = self._determine_output_file_type(
-            self.input_path, input_file_type, self.output_path
+            self.input_path,
+            input_file_type,
+            self.output_path,
         )
 
         if input_file_type == FileType.directory:
-            files = await file_client.get_all_files(self.input_path)
+            files = await file_client.get_all_files(
+                self.input_path,
+                self.include_patterns,
+                self.exclude_patterns,
+            )
         else:
             files = [self.input_path]
 
         settings_to_use = self.resolve_settings(
             auto_overwrite=global_auto_overwrite
         )
         replace_configs_to_use = [
-            config.resolve(global_variables) for config in self.replace_configs
+            config.resolve(global_variables)
+            for config in [*self.replace_configs, *global_replace_configs]
         ]
 
         file_to_process: list[tuple[str, str]] = [
             (
                 file,
                 self._get_output_path(
-                    file, input_file_type, self.output_path, output_file_type
+                    file,
+                    self.input_path,
+                    input_file_type,
+                    self.output_path,
+                    output_file_type,
+                    (
+                        self.maintain_directory_structure
+                        if self.maintain_directory_structure is not None
+                        else global_maintain_directory_structure
+                    ),
                 ),
             )
             for file in files
         ]
         process_coros = [
             file_client.copy_file(
                 input_file_path,
@@ -194,15 +224,17 @@
 
         return status_counter
 
 
 class CodeStarterConfig(BaseModel):
     model_config = ConfigDict(extra="forbid")
     auto_overwrite: bool = False
+    maintain_directory_structure: bool = True
     global_variables: dict[str, str] = Field(default_factory=dict)
+    global_replace_configs: list[ReplaceConfig] = Field(default_factory=list)
     dependency_configs: DependencyConfigs = Field(
         default_factory=DependencyConfigs
     )
     resource_configs: list[ResourceConfig] = Field(default_factory=list)
     commands: list[Command] = Field(default_factory=list)
 
     async def process_dependency(
@@ -256,15 +288,18 @@
 
 async def execute_codestarter(
     config: CodeStarterConfig, skip_commands: bool
 ) -> tuple[StatusCounter, list[tuple[str, int]], StatusCounter]:
     # process all files
     coros = [
         resource_config.process_resource(
-            config.auto_overwrite, config.global_variables
+            config.auto_overwrite,
+            config.maintain_directory_structure,
+            config.global_variables,
+            config.global_replace_configs,
         )
         for resource_config in config.resource_configs
     ]
     status_counters = await asyncio.gather(*coros)
     total_status_counter = StatusCounter.aggregate(status_counters)
 
     # gather dependencies
```

### Comparing `codestarter-0.0.0/src/codestarter/dependency_resolvers/__init__.py` & `codestarter-0.0.1/src/codestarter/dependency_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `codestarter-0.0.0/src/codestarter/dependency_resolvers/requirements_resolver.py` & `codestarter-0.0.1/src/codestarter/dependency_resolvers/requirements_resolver.py`

 * *Files identical despite different names*

### Comparing `codestarter-0.0.0/src/codestarter/file/__init__.py` & `codestarter-0.0.1/src/codestarter/file/__init__.py`

 * *Files identical despite different names*

### Comparing `codestarter-0.0.0/src/codestarter/file/local.py` & `codestarter-0.0.1/src/codestarter/file/local.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+from fnmatch import fnmatch
 
 import aiofiles
 
 from .utils import FileClient, FileType
 
 logger = logging.getLogger(__name__)
 
@@ -25,19 +26,33 @@
         if os.path.isfile(path):
             return FileType.file
         elif os.path.isdir(path):
             return FileType.directory
         else:
             raise FileNotFoundError(f"No file or directory found at {path}")
 
-    async def get_all_files(self, directory: str) -> list[str]:
+    async def get_all_files(
+        self,
+        directory: str,
+        include_patterns: list[str],
+        exclude_patterns: list[str],
+    ) -> list[str]:
         all_files = []
         for root, _, files in os.walk(directory):
             for file in files:
-                all_files.append(os.path.join(root, file))
+                full_path = os.path.join(root, file)
+                if any(
+                    fnmatch(full_path, pattern) for pattern in exclude_patterns
+                ):
+                    continue
+                if len(include_patterns) > 0 and not any(
+                    fnmatch(full_path, pattern) for pattern in include_patterns
+                ):
+                    continue
+                all_files.append(full_path)
         return all_files
 
     async def file_exists(self, path: str) -> bool:
         return os.path.exists(path)
 
     async def directory_exists(self, path: str) -> bool:
         return os.path.isdir(os.path.dirname(path))
```

### Comparing `codestarter-0.0.0/src/codestarter/file/utils.py` & `codestarter-0.0.1/src/codestarter/file/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,20 @@
         raise NotImplementedError()
 
     @abstractmethod
     async def validate_file(self, path: str) -> FileType:
         raise NotImplementedError()
 
     @abstractmethod
-    async def get_all_files(self, directory: str) -> list[str]:
+    async def get_all_files(
+        self,
+        directory: str,
+        include_patterns: list[str],
+        exclude_patterns: list[str],
+    ) -> list[str]:
         raise NotImplementedError()
 
     async def copy_file(
         self,
         input_file_path: str,
         output_file_path: str,
         output_file_type: FileType,
```

### Comparing `codestarter-0.0.0/LICENSE` & `codestarter-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codestarter-0.0.0/README.md` & `codestarter-0.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.3
+Name: codestarter
+Version: 0.0.1
+Summary: A tool for assembling a repo using copy/paste
+Project-URL: Homepage, https://github.com/pateli18/codestarter
+Project-URL: Issues, https://github.com/pateli18/codestarter/issues
+Author: Ihsaan Patel
+License-File: LICENSE
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Requires-Dist: pydantic
+Requires-Dist: pydantic-settings
+Provides-Extra: cli
+Requires-Dist: typer; extra == 'cli'
+Provides-Extra: local
+Requires-Dist: aiofiles; extra == 'local'
+Provides-Extra: pythondep
+Requires-Dist: packaging; extra == 'pythondep'
+Description-Content-Type: text/markdown
+
 # CodeStarter
 
 CodeStarter is a tool for assembling a repo using copy/paste. Inspired by the installation of components with [shadcn/ui](https://ui.shadcn.com/), CodeStarter allows you to easily bring in code and alter it without having to worry about assembling internal packages.
 
 ![Run](./images/run.gif)
 
 ## Contents
@@ -23,37 +45,48 @@
 
 ### Create a Config
 
 Add a `codestarter.json` config to your project (we recommend the root of your project, but you can technically put it anywhere).
 
 ```json
 {
-  "auto_overwrite": false, // If true, the output file will be overwritten if it already exists. If false, the system will not overwrite the existing file. This can be overridden by the auto_overwrite flag in the resource_configs. Default is Fa
+  "auto_overwrite": false, // If true, the output file will be overwritten if it already exists. If false, the system will not overwrite the existing file. This can be overridden by the auto_overwrite flag in the resource_configs. Default is False
+  "maintain_directory_structure": true, // If true, the directory structure from the input path will be maintained. If false, the directory structure will be flattened and only the filenames will be used. Default is True
   "global_variables": {
     "$new_project_name": "codestarter" // global variables can be referenced within the resource_configs. The key must start with $.
   },
+  "global_replace_configs": [
+    // global replace configs will be run for every resource after the resource_configs.
+    {
+      "original_value": "old_repo", // the value to be replaced within the file, can reference global variables.
+      "new_value": "$new_project_name" // the value to replace the original value with, can reference global variables.
+    }
+  ],
   "dependency_configs": {
     "requirements_config": {
       // The key is the name of the dependency config that will be referenced in the resource_configs.
       "type": "requirements.txt", // The type of the dependency resolver.
       "output_file": "./requirements.txt" // The actual path to the file that contains the dependency
     }
   },
   "resource_configs": [
     {
       "input_path": "../old_repo/.vscode/", // path to the file or directory that will be copied. if it's a directory, the entire directory will be copied.
       "output_path": "./.vscode/", // path to the file or directory that the input will be copied to. If it's a directory, the input filenames will be used
+      "include_patterns": ["*.py"], // [OPTIONAL] The file patterns to include. If not provided, all files will be included.
+      "exclude_patterns": ["*.pyc"], // [OPTIONAL] The file patterns to exclude. If not provided, no files will be excluded.
       "replace_configs": [
         {
           "original_value": "old_repo", // the value to be replaced within the file, can reference global variables.
           "new_value": "$new_project_name" // the value to replace the original value with, can reference global variables.
         }
       ],
       "dependencies": { "requirements_config": ["pandas>=1.0", "httpx"] }, // The dependencies to be installed. The key is the name of the dependency config that will be referenced in the resource_configs.
-      "auto_overwrite": false // [OPTIONAL] If true, the output file will be overwritten if it already exists. If false, the system will prompt or skip the overwrite. If not provided, the value of "auto_overwrite" at the top level will be used.
+      "auto_overwrite": false, // [OPTIONAL] If true, the output file will be overwritten if it already exists. If false, the system will prompt or skip the overwrite. If not provided, the value of "auto_overwrite" at the top level will be used.
+      "maintain_directory_structure": false // [OPTIONAL] If true, the directory structure from the input path will be maintained. If false, the directory structure will be flattened and only the filenames will be used. If not provided, the value of "maintain_directory_structure" at the top level will be used.
     }
   ],
   "commands": [
     {
       "command": "uv venv", // The command to run.
       "not_run_check": "[[ -d .venv ]] && exit 1 || exit 0" // The command to run to check if the command should be run. If the command returns 0, the command will be run. If the command returns any other value, the command will not be run.
     }
```

### Comparing `codestarter-0.0.0/pyproject.toml` & `codestarter-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "codestarter"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name="Ihsaan Patel" },
 ]
 description = "A tool for assembling a repo using copy/paste"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `codestarter-0.0.0/PKG-INFO` & `codestarter-0.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.3
-Name: codestarter
-Version: 0.0.0
-Summary: A tool for assembling a repo using copy/paste
-Project-URL: Homepage, https://github.com/pateli18/codestarter
-Project-URL: Issues, https://github.com/pateli18/codestarter/issues
-Author: Ihsaan Patel
-License-File: LICENSE
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Requires-Dist: pydantic
-Requires-Dist: pydantic-settings
-Provides-Extra: cli
-Requires-Dist: typer; extra == 'cli'
-Provides-Extra: local
-Requires-Dist: aiofiles; extra == 'local'
-Provides-Extra: pythondep
-Requires-Dist: packaging; extra == 'pythondep'
-Description-Content-Type: text/markdown
-
 # CodeStarter
 
 CodeStarter is a tool for assembling a repo using copy/paste. Inspired by the installation of components with [shadcn/ui](https://ui.shadcn.com/), CodeStarter allows you to easily bring in code and alter it without having to worry about assembling internal packages.
 
 ![Run](./images/run.gif)
 
 ## Contents
@@ -45,37 +23,48 @@
 
 ### Create a Config
 
 Add a `codestarter.json` config to your project (we recommend the root of your project, but you can technically put it anywhere).
 
 ```json
 {
-  "auto_overwrite": false, // If true, the output file will be overwritten if it already exists. If false, the system will not overwrite the existing file. This can be overridden by the auto_overwrite flag in the resource_configs. Default is Fa
+  "auto_overwrite": false, // If true, the output file will be overwritten if it already exists. If false, the system will not overwrite the existing file. This can be overridden by the auto_overwrite flag in the resource_configs. Default is False
+  "maintain_directory_structure": true, // If true, the directory structure from the input path will be maintained. If false, the directory structure will be flattened and only the filenames will be used. Default is True
   "global_variables": {
     "$new_project_name": "codestarter" // global variables can be referenced within the resource_configs. The key must start with $.
   },
+  "global_replace_configs": [
+    // global replace configs will be run for every resource after the resource_configs.
+    {
+      "original_value": "old_repo", // the value to be replaced within the file, can reference global variables.
+      "new_value": "$new_project_name" // the value to replace the original value with, can reference global variables.
+    }
+  ],
   "dependency_configs": {
     "requirements_config": {
       // The key is the name of the dependency config that will be referenced in the resource_configs.
       "type": "requirements.txt", // The type of the dependency resolver.
       "output_file": "./requirements.txt" // The actual path to the file that contains the dependency
     }
   },
   "resource_configs": [
     {
       "input_path": "../old_repo/.vscode/", // path to the file or directory that will be copied. if it's a directory, the entire directory will be copied.
       "output_path": "./.vscode/", // path to the file or directory that the input will be copied to. If it's a directory, the input filenames will be used
+      "include_patterns": ["*.py"], // [OPTIONAL] The file patterns to include. If not provided, all files will be included.
+      "exclude_patterns": ["*.pyc"], // [OPTIONAL] The file patterns to exclude. If not provided, no files will be excluded.
       "replace_configs": [
         {
           "original_value": "old_repo", // the value to be replaced within the file, can reference global variables.
           "new_value": "$new_project_name" // the value to replace the original value with, can reference global variables.
         }
       ],
       "dependencies": { "requirements_config": ["pandas>=1.0", "httpx"] }, // The dependencies to be installed. The key is the name of the dependency config that will be referenced in the resource_configs.
-      "auto_overwrite": false // [OPTIONAL] If true, the output file will be overwritten if it already exists. If false, the system will prompt or skip the overwrite. If not provided, the value of "auto_overwrite" at the top level will be used.
+      "auto_overwrite": false, // [OPTIONAL] If true, the output file will be overwritten if it already exists. If false, the system will prompt or skip the overwrite. If not provided, the value of "auto_overwrite" at the top level will be used.
+      "maintain_directory_structure": false // [OPTIONAL] If true, the directory structure from the input path will be maintained. If false, the directory structure will be flattened and only the filenames will be used. If not provided, the value of "maintain_directory_structure" at the top level will be used.
     }
   ],
   "commands": [
     {
       "command": "uv venv", // The command to run.
       "not_run_check": "[[ -d .venv ]] && exit 1 || exit 0" // The command to run to check if the command should be run. If the command returns 0, the command will be run. If the command returns any other value, the command will not be run.
     }
```

