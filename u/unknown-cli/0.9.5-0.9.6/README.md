# Comparing `tmp/unknown-cli-0.9.5.tar.gz` & `tmp/unknown-cli-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unknown-cli-0.9.5.tar", last modified: Tue Apr  9 23:08:56 2024, max compression
+gzip compressed data, was "unknown-cli-0.9.6.tar", last modified: Fri Apr 19 17:29:43 2024, max compression
```

## Comparing `unknown-cli-0.9.5.tar` & `unknown-cli-0.9.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-09 23:08:56.563310 unknown-cli-0.9.5/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-04-09 23:08:56.562309 unknown-cli-0.9.5/PKG-INFO
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       30 2023-09-08 21:53:36.000000 unknown-cli-0.9.5/README.md
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       38 2024-04-09 23:08:56.564308 unknown-cli-0.9.5/setup.cfg
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2695 2024-03-13 22:40:13.000000 unknown-cli-0.9.5/setup.py
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-09 23:08:56.429118 unknown-cli-0.9.5/unknown_cli.egg-info/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-04-09 23:08:56.000000 unknown-cli-0.9.5/unknown_cli.egg-info/PKG-INFO
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      561 2024-04-09 23:08:56.000000 unknown-cli-0.9.5/unknown_cli.egg-info/SOURCES.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        1 2024-04-09 23:08:56.000000 unknown-cli-0.9.5/unknown_cli.egg-info/dependency_links.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       83 2024-04-09 23:08:56.000000 unknown-cli-0.9.5/unknown_cli.egg-info/entry_points.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      130 2024-04-09 23:08:56.000000 unknown-cli-0.9.5/unknown_cli.egg-info/requires.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       11 2024-04-09 23:08:56.000000 unknown-cli-0.9.5/unknown_cli.egg-info/top_level.txt
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-09 23:08:56.481936 unknown-cli-0.9.5/unknowncli/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        5 2024-04-09 23:08:56.000000 unknown-cli-0.9.5/unknowncli/VERSION
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      407 2024-03-11 22:54:16.000000 unknown-cli-0.9.5/unknowncli/__init__.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1815 2024-04-09 23:06:38.000000 unknown-cli-0.9.5/unknowncli/__main__.py
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-09 23:08:56.539760 unknown-cli-0.9.5/unknowncli/commands/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2023-09-08 21:53:36.000000 unknown-cli-0.9.5/unknowncli/commands/__init__.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    34140 2024-03-22 11:18:20.000000 unknown-cli-0.9.5/unknowncli/commands/preflight.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    19661 2024-04-09 22:21:41.000000 unknown-cli-0.9.5/unknowncli/commands/project.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    18631 2024-04-09 23:06:24.000000 unknown-cli-0.9.5/unknowncli/commands/task.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2436 2023-09-08 21:53:36.000000 unknown-cli-0.9.5/unknowncli/commands/unreal.py
-drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-09 23:08:56.551760 unknown-cli-0.9.5/unknowncli/data/
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     3560 2023-09-08 21:53:36.000000 unknown-cli-0.9.5/unknowncli/data/.p4ignore.txt
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      840 2023-12-07 23:07:53.000000 unknown-cli-0.9.5/unknowncli/set_registry_keys.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1005 2023-12-07 23:07:53.000000 unknown-cli-0.9.5/unknowncli/set_url_handler.py
--rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    11460 2024-04-09 23:06:38.000000 unknown-cli-0.9.5/unknowncli/utils.py
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-19 17:29:43.119444 unknown-cli-0.9.6/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-04-19 17:29:43.118443 unknown-cli-0.9.6/PKG-INFO
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       30 2023-09-08 21:53:36.000000 unknown-cli-0.9.6/README.md
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       38 2024-04-19 17:29:43.120443 unknown-cli-0.9.6/setup.cfg
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2695 2024-03-13 22:40:13.000000 unknown-cli-0.9.6/setup.py
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-19 17:29:42.986444 unknown-cli-0.9.6/unknown_cli.egg-info/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      474 2024-04-19 17:29:42.000000 unknown-cli-0.9.6/unknown_cli.egg-info/PKG-INFO
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      561 2024-04-19 17:29:42.000000 unknown-cli-0.9.6/unknown_cli.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        1 2024-04-19 17:29:42.000000 unknown-cli-0.9.6/unknown_cli.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       83 2024-04-19 17:29:42.000000 unknown-cli-0.9.6/unknown_cli.egg-info/entry_points.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      130 2024-04-19 17:29:42.000000 unknown-cli-0.9.6/unknown_cli.egg-info/requires.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)       11 2024-04-19 17:29:42.000000 unknown-cli-0.9.6/unknown_cli.egg-info/top_level.txt
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-19 17:29:43.038443 unknown-cli-0.9.6/unknowncli/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        5 2024-04-19 17:29:42.000000 unknown-cli-0.9.6/unknowncli/VERSION
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      407 2024-03-11 22:54:16.000000 unknown-cli-0.9.6/unknowncli/__init__.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1815 2024-04-19 17:07:31.000000 unknown-cli-0.9.6/unknowncli/__main__.py
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-19 17:29:43.096444 unknown-cli-0.9.6/unknowncli/commands/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2023-09-08 21:53:36.000000 unknown-cli-0.9.6/unknowncli/commands/__init__.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    34140 2024-03-22 11:18:20.000000 unknown-cli-0.9.6/unknowncli/commands/preflight.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    19697 2024-04-19 17:07:36.000000 unknown-cli-0.9.6/unknowncli/commands/project.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    19908 2024-04-19 17:07:36.000000 unknown-cli-0.9.6/unknowncli/commands/task.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     2436 2023-09-08 21:53:36.000000 unknown-cli-0.9.6/unknowncli/commands/unreal.py
+drwxrwxrwx   0 nixonk    (1000) nixonk    (1000)        0 2024-04-19 17:29:43.107445 unknown-cli-0.9.6/unknowncli/data/
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     3560 2023-09-08 21:53:36.000000 unknown-cli-0.9.6/unknowncli/data/.p4ignore.txt
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)      840 2023-12-07 23:07:53.000000 unknown-cli-0.9.6/unknowncli/set_registry_keys.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)     1005 2023-12-07 23:07:53.000000 unknown-cli-0.9.6/unknowncli/set_url_handler.py
+-rwxrwxrwx   0 nixonk    (1000) nixonk    (1000)    11460 2024-04-19 17:07:31.000000 unknown-cli-0.9.6/unknowncli/utils.py
```

### Comparing `unknown-cli-0.9.5/setup.py` & `unknown-cli-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.5/unknown_cli.egg-info/SOURCES.txt` & `unknown-cli-0.9.6/unknown_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.5/unknowncli/__main__.py` & `unknown-cli-0.9.6/unknowncli/__main__.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.5/unknowncli/commands/preflight.py` & `unknown-cli-0.9.6/unknowncli/commands/preflight.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.5/unknowncli/commands/project.py` & `unknown-cli-0.9.6/unknowncli/commands/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from typer import Context, launch, echo, secho, Option, Typer, confirm, prompt, style, progressbar
 
 app = Typer()
 
 hostname = socket.gethostname().lower()
 SUBST_DRIVE = "S:"
+BASE_STREAM = "//Project/SN2-Main"
 STREAMS = {
     "sn2-main": "//project/sn2-main-ue"
 }
 SUB_STREAMS = {
     "//project/sn2-main": {
         "Project"               : "//project/sn2-main-ue",
         "Project+RawRecommended": "//project/sn2-main-ue-raw-content",
```

### Comparing `unknown-cli-0.9.5/unknowncli/commands/task.py` & `unknown-cli-0.9.6/unknowncli/commands/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import datetime
 import logging
 import socket
 import sys
 from ..utils import abort
-from .project import SUB_STREAMS
+from .project import BASE_STREAM, SUB_STREAMS
 from P4 import P4, P4Exception
 from typing import Optional
 from subprocess import check_call
 
 log = logging.getLogger(__name__)
 
 from typer import echo, secho, Option, Typer, confirm, prompt
 from rich.progress import Progress, MofNCompleteColumn, TimeRemainingColumn, BarColumn, SpinnerColumn, TextColumn
 
 app = Typer()
 
 hostname = socket.gethostname().lower()
 SUBST_DRIVE = "S:"
 path = f"{SUBST_DRIVE}\\sn2-main\\"
-BASE_STREAM = "//Project/SN2-Main"
 STREAM_LIST_LOWER = [s.lower() for s in list(list(SUB_STREAMS.values())[0].values())]
 STREAM_LIST_STRING = "\n\t" + "\n\t".join(STREAM_LIST_LOWER)
 
 p4 = None
 
 
 def connect_p4():
@@ -59,16 +58,17 @@
         abort(
             f"To use this tool you must be working in a valid stream but your workspace is set to {stream_name}." +
             "\nPlease change to a relevant workspace with 'p4 set p4client=<your_valid_workspace>'" +
             "\nOr set up a workspace with 'unk project setup'."
         )
 
 
-def get_task_streams(owner):
-    lst = p4.run_streams("-F", f"Owner={owner} Type=task baseParent={BASE_STREAM}")
+def get_task_streams(owner: str=""):
+    streams_filter = f"Type=task baseParent={BASE_STREAM}" + ( f" Owner={owner}" if owner else "" )
+    lst = p4.run_streams("-F", streams_filter)
     return lst
 
 
 def get_current_stream():
     try:
         ret = p4.run_stream("-o")[0]
     except P4Exception as e:
@@ -198,42 +198,49 @@
     # update the server without syncing
     ret = p4.run_sync("-q", "-k", f"{root_path}\...")
 
     secho(f"You are now working in task stream {stream_name} from parent {parent}", bold=True, fg="green")
 
 
 @app.command()
-def switch():
+def switch(owned: Optional[bool] = Option(True, help="See only owned task streams")):
     """
     Lists your current task streams and lets you switch between them
     """
     stream = get_current_stream()
     old_stream_name = stream["Stream"]
     client = p4.run_client("-o")[0]
-    client_owner = client["Owner"]
-    task_streams = get_task_streams(client_owner)
+    task_streams = get_task_streams(client["Owner"] if owned else "")
+    if owned and not task_streams:
+        secho("You have no owned task streams. You can create one with the 'create' command.", bold=True)
+        if confirm("\nDo you want to instead see other streams that you don't own?"):
+            switch(owned=False)
+        abort("")
     parent = None
     if stream["Type"] == "task":
         parent = stream["Parent"]
     for i, t in enumerate(task_streams):
         secho(f"{i+1} : {t['Stream']}")
     if parent:
-        secho(f"0 : {parent}")
+        secho(f"0 : (Parent stream) {parent}")
+    if owned:
+        secho(f"99 : <See other streams, including task streams that you don't own>")
 
-    if not task_streams:
-        abort("You have no task streams. You can create one with the 'create' command")
     n = prompt("\nSelect a stream to work in")
     if n is None:
         abort("No stream selected")
     try:
         n = int(n)
     except:
         abort("Aborted.")
-    if n == 0:
+    if parent and n == 0:
         new_stream = parent
+    elif owned and n == 99:
+        switch(owned=False)
+        abort("")
     else:
         try:
             new_stream = task_streams[n - 1]["Stream"]
         except:
             abort("Aborted.")
 
     secho(f"\nSwitching to stream {new_stream}", bold=True)
@@ -422,15 +429,15 @@
     else:
         echo(
             f"Your merge changelist is now ready for submitting. Use this description: 'Automatically merge {parent_stream} to {stream_name}. {mr}"
         )
 
 
 @app.command()
-def copyup():
+def copyup(force: Optional[bool] = Option(False, help="Use p4 copy force arguments: -f -F")):
     """
     Finish the task and copy into the parent stream
     """
     ret = p4.run_opened()
     if ret:
         abort("There are unsubmitted files in your workspace")
 
@@ -441,24 +448,36 @@
     if ret["Type"] != "task":
         abort(f"Current stream {stream_name} is not a task stream")
 
     secho(f"Switching to parent stream {parent} ...", fg="blue")
     p4.run_client("-s", "-S", parent)
 
     p4.run_sync("-q")
-    echo(f"Performing copy from {stream_name} to {ret['baseParent']}/...")
+    copy_target = f"{ret['baseParent']}/..."
+    echo(f"Performing copy from {stream_name} to {copy_target}")
+    copy_args = [ "-Af", "-S", stream_name, copy_target ]
+    force_copy_args = [ "-f", "-F" ]
     try:
-        copy_ret = p4.run_copy("-Af", "-S", stream_name, ret["baseParent"] + "/...")
+        copy_ret = p4.run_copy(*(force_copy_args if force else []), *copy_args)
     except P4Exception as e:
         if "up-to-date" in str(e):
             secho(f"Nothing to do. Parent {parent} is identical to task stream {stream_name}", fg="green")
             return
         elif "No such file(s)" in str(e):
             secho(f"Nothing to do. No changes were made yet in task stream {stream_name}", fg="green")
             return
+        elif not force and "cannot 'copy' over outstanding 'merge' changes" in str(e):
+            # Occurs when mergedown is not complete but it can be the case when P4 has issues
+            # merging rename/move+edit and the fix is to force merge which causes "outstanding...".
+            secho(f"\n{str(e)}", fg="yellow")
+            if confirm("Try a force copy? (Do this if you're sure that you're done with mergedowns)"):
+                copy_ret = p4.run_copy(*force_copy_args, *copy_args)
+            else:
+                secho("No action taken.")
+                return
         else:
             raise
     else:
         echo("Adding files...")
         for r in copy_ret:
             echo(f"  {r['fromFile']} -> {r['depotFile']}")
```

### Comparing `unknown-cli-0.9.5/unknowncli/commands/unreal.py` & `unknown-cli-0.9.6/unknowncli/commands/unreal.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.5/unknowncli/data/.p4ignore.txt` & `unknown-cli-0.9.6/unknowncli/data/.p4ignore.txt`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.5/unknowncli/set_registry_keys.py` & `unknown-cli-0.9.6/unknowncli/set_registry_keys.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.5/unknowncli/set_url_handler.py` & `unknown-cli-0.9.6/unknowncli/set_url_handler.py`

 * *Files identical despite different names*

### Comparing `unknown-cli-0.9.5/unknowncli/utils.py` & `unknown-cli-0.9.6/unknowncli/utils.py`

 * *Files identical despite different names*

