# Comparing `tmp/git_toprepo-0.1.0rc2.tar.gz` & `tmp/git_toprepo-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_toprepo-0.1.0rc2.tar", max compression
+gzip compressed data, was "git_toprepo-0.1.0rc3.tar", max compression
```

## Comparing `git_toprepo-0.1.0rc2.tar` & `git_toprepo-0.1.0rc3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2024-04-15 20:23:34.977662 git_toprepo-0.1.0rc2/LICENSE
--rw-r--r--   0        0        0     8855 2024-04-15 20:23:34.977662 git_toprepo-0.1.0rc2/README.md
--rwxr-xr-x   0        0        0    94962 2024-04-15 20:23:34.977662 git_toprepo-0.1.0rc2/git_toprepo.py
--rw-r--r--   0        0        0      621 2024-04-15 20:23:40.997640 git_toprepo-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     9590 1970-01-01 00:00:00.000000 git_toprepo-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-19 07:12:26.634820 git_toprepo-0.1.0rc3/LICENSE
+-rw-r--r--   0        0        0     8855 2024-04-19 07:12:26.634820 git_toprepo-0.1.0rc3/README.md
+-rwxr-xr-x   0        0        0    96764 2024-04-19 07:12:26.634820 git_toprepo-0.1.0rc3/git_toprepo.py
+-rw-r--r--   0        0        0      621 2024-04-19 07:12:32.826889 git_toprepo-0.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     9590 1970-01-01 00:00:00.000000 git_toprepo-0.1.0rc3/PKG-INFO
```

### Comparing `git_toprepo-0.1.0rc2/LICENSE` & `git_toprepo-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `git_toprepo-0.1.0rc2/README.md` & `git_toprepo-0.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `git_toprepo-0.1.0rc2/git_toprepo.py` & `git_toprepo-0.1.0rc3/git_toprepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 """git-submodule made easy with git-toprepo
 
 git-toprepo merges subrepositories into a common history, similar to git-subtree.
 """
 import argparse
 import itertools
+import os
 import re
 import shutil
 import subprocess
 import sys
 import textwrap
 from abc import ABC, abstractmethod
 from collections import defaultdict
@@ -237,15 +238,18 @@
     for sep in r"/\:":
         name = name.replace(sep, "-")
     return name
 
 
 def join_submodule_url(parent: Url, other: RawUrl) -> Url:
     if other.startswith("./") or other.startswith("../") or other == ".":
-        scheme, parent = parent.split("://", 1)
+        idx = parent.find("://")
+        scheme_end = idx + 3 if idx != -1 else idx + 1
+        scheme = parent[:scheme_end]
+        parent = parent[scheme_end:]
         parent = parent.rstrip("/")
         while True:
             if other.startswith("/"):
                 # Ignore double slash.
                 other = other[1:]
             elif other.startswith("./"):
                 other = other[2:]
@@ -256,17 +260,17 @@
                 else:
                     # Too many '../', move it from other to parent.
                     parent += "/.."
                 other = other[3:]
             else:
                 break
         if other in ("", "."):
-            ret = f"{scheme}://{parent}"
+            ret = f"{scheme}{parent}"
         else:
-            ret = f"{scheme}://{parent}/{other}"
+            ret = f"{scheme}{parent}/{other}"
     else:
         ret = other
     return ret
 
 
 ANNOTATED_TOP_SUBDIR = b"<top>"
 
@@ -343,19 +347,19 @@
     full_args: List[str]
     if repo is None:
         full_args = ["git"] + args
     else:
         full_args = ["git", "-C", str(repo)] + args
     cmdline = subprocess.list2cmdline(full_args)
     if dry_run:
-        print(f"\rWould run  {cmdline}")
+        print(f"\rWould run  {cmdline}", file=sys.stderr)
         ret = None
     else:
         if log_command:
-            print(f"\rRunning   {cmdline}")
+            print(f"\rRunning   {cmdline}", file=sys.stderr)
         ret = subprocess.run(full_args, check=check, **kwargs)
     return ret
 
 
 def ref_exists(repo: Repo, ref: str):
     result = subprocess.run(
         ["git", "-C", str(repo.path)]
@@ -513,14 +517,15 @@
 
     def __init__(self, repo: Repo):
         self.repo = repo
 
     def git_config_list(self) -> str:
         return subprocess.check_output(
             ["git", "-C", str(self.repo.path), "config", "--list"],
+            env=os.environ,  # To make monkeypatching work for tests.
             text=True,
         )
 
 
 class ContentConfigLoader(ConfigLoader):
     @abstractmethod
     def read_config_file_content(self) -> str:
@@ -572,14 +577,16 @@
         self.local_repo = local_repo
         self.local_ref = local_ref
 
     def fetch_remote_config(self) -> None:
         log_run_git(
             self.local_repo.path,
             ["fetch", "--quiet", self.url, f"+{self.remote_ref}:{self.local_ref}"],
+            stdout=sys.__stderr__.fileno(),
+            stderr=subprocess.STDOUT,
         )
 
     def read_config_file_content(self) -> str:
         return subprocess.check_output(
             ["git", "-C", str(self.local_repo.path)]
             + ["show", f"{self.local_ref}:{self.filename.as_posix()}"],
             text=True,
@@ -1924,14 +1931,15 @@
             new_mono_commit = self._create_mono_commit_from_subrepo_commit(
                 monoref_bytes,
                 subdir,
                 subrepo_commit,
                 subrepo_id_to_converted_id,
             )
             repo_filter.insert(new_mono_commit, direct_insertion=True)
+            subrepo_id_to_converted_id[subrepo_commit.id] = new_mono_commit.id
 
         repo_filter.finish()
 
 
 ParentsList = List[RepoFilterId]
 SubrepoParentsMap = Dict[bytes, ParentsList]
 """Maps from subrepo dir to subrepo parent ids.
@@ -2218,14 +2226,34 @@
         raise
     print(f"Initialization of {monorepo.path} succeeded!")
     print("To start, run:")
     print("  git toprepo fetch && git checkout origin/main")
     return 0
 
 
+def main_config(args) -> int:
+    monorepo = MonoRepo(args.cwd)
+    config_dict = ConfigAccumulator(monorepo, online=args.online).try_load_main_config()
+    if config_dict is None:
+        return 1
+    if args.key is not None:
+        if args.key not in config_dict:
+            print("ERROR: Missing configuration key {args.key}")
+            return 1
+        value = config_dict[args.key][-1]
+        print(value)
+    elif args.list:
+        for key, values in sorted(config_dict.items()):
+            for value in values:
+                print(f"{key}={value}")
+    else:
+        assert False, "Bad args {args}"
+    return 0
+
+
 def main_refilter(args) -> int:
     monorepo = MonoRepo(args.cwd)
     config_dict = ConfigAccumulator(monorepo, args.online).try_load_main_config()
     if config_dict is None:
         return 1
     config = Config.try_create(config_dict)
     if config is None:
@@ -2366,15 +2394,15 @@
 
     # Push per repo
     for repo_name, push_list in repo_to_pushes.items():
         for push in push_list:
             push_rev = push.commit_hash.decode("utf-8")
             log_run_git(
                 push.repo.path,
-                ["push", "--quiet", "--force", push.repo.config.push_url]
+                ["push", "--quiet", push.repo.config.push_url]
                 + [f"{push_rev}:{refspec.remote_ref}"]
                 + push.extra_args,
                 log_command=True,
                 dry_run=args.dry_run,
                 check=False,
             )
     return 0
@@ -2423,14 +2451,42 @@
         type=PurePath,
         nargs="?",
         help="""\
             Where to initialize the repository.
             Defaults to the base name of the repository.""",
     )
 
+    config_parser = subparsers.add_parser(
+        "config",
+        description="""\
+            Reads the mono repository configuration.
+        """,
+    )
+    config_parser.set_defaults(func=main_config)
+    config_parser.add_argument(
+        "--offline",
+        action="store_false",
+        dest="online",
+        help="""\
+            Disallow fetching the configuration remotely,
+            use existing information only.""",
+    )
+    config_key_group = config_parser.add_mutually_exclusive_group(required=True)
+    config_key_group.add_argument(
+        "--list",
+        action="store_true",
+        help="List all configurations.",
+    )
+    config_key_group.add_argument(
+        "key",
+        type=str,
+        nargs="?",
+        help="The name of the configuration to get.",
+    )
+
     refilter_parser = subparsers.add_parser(
         "refilter",
         description="Performes a refiltering of the monorepo.",
     )
     refilter_parser.set_defaults(func=main_refilter)
     refilter_parser.add_argument(
         "--from-scratch",
```

### Comparing `git_toprepo-0.1.0rc2/pyproject.toml` & `git_toprepo-0.1.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-toprepo"
-version = "0.1.0rc2"
+version = "0.1.0rc3"
 description = "git-submodule made easy with git-toprepo"
 keywords = ["git", "submodule", "monorepo", "toprepo", "superrepo"]
 authors = ["Fredrik Medley <fredrik@meroton.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `git_toprepo-0.1.0rc2/PKG-INFO` & `git_toprepo-0.1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-toprepo
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: git-submodule made easy with git-toprepo
 License: GPL-3.0-only
 Keywords: git,submodule,monorepo,toprepo,superrepo
 Author: Fredrik Medley
 Author-email: fredrik@meroton.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

