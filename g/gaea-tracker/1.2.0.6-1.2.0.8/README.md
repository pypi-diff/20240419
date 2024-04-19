# Comparing `tmp/gaea_tracker-1.2.0.6-py3-none-any.whl.zip` & `tmp/gaea_tracker-1.2.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5898 bytes, number of entries: 8
--rw-r--r--  2.0 unx      213 b- defN 24-Apr-16 05:40 gaea_tracker/__init__.py
--rw-r--r--  2.0 unx     1654 b- defN 24-Apr-16 05:40 gaea_tracker/aim_tracker.py
--rw-r--r--  2.0 unx     7736 b- defN 24-Apr-16 05:40 gaea_tracker/experiment_tracker.py
--rw-r--r--  2.0 unx     1459 b- defN 24-Apr-16 05:40 gaea_tracker/mlflow_tracker.py
--rw-r--r--  2.0 unx     1770 b- defN 24-Apr-16 05:40 gaea_tracker-1.2.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 05:40 gaea_tracker-1.2.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-16 05:40 gaea_tracker-1.2.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      668 b- defN 24-Apr-16 05:40 gaea_tracker-1.2.0.6.dist-info/RECORD
-8 files, 13605 bytes uncompressed, 4726 bytes compressed:  65.3%
+Zip file size: 5952 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      213 b- defN 24-Apr-19 05:25 gaea_tracker/__init__.py
+-rw-r--r--  2.0 unx     1654 b- defN 24-Apr-19 05:25 gaea_tracker/aim_tracker.py
+-rw-r--r--  2.0 unx     8046 b- defN 24-Apr-19 05:25 gaea_tracker/experiment_tracker.py
+-rw-r--r--  2.0 unx     1459 b- defN 24-Apr-19 05:25 gaea_tracker/mlflow_tracker.py
+-rw-r--r--  2.0 unx     1770 b- defN 24-Apr-19 05:26 gaea_tracker-1.2.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 05:26 gaea_tracker-1.2.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-19 05:26 gaea_tracker-1.2.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      668 b- defN 24-Apr-19 05:26 gaea_tracker-1.2.0.8.dist-info/RECORD
+8 files, 13915 bytes uncompressed, 4780 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gaea_tracker/experiment_tracker.py
 Comment: 
 
 Filename: gaea_tracker/mlflow_tracker.py
 Comment: 
 
-Filename: gaea_tracker-1.2.0.6.dist-info/METADATA
+Filename: gaea_tracker-1.2.0.8.dist-info/METADATA
 Comment: 
 
-Filename: gaea_tracker-1.2.0.6.dist-info/WHEEL
+Filename: gaea_tracker-1.2.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: gaea_tracker-1.2.0.6.dist-info/top_level.txt
+Filename: gaea_tracker-1.2.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: gaea_tracker-1.2.0.6.dist-info/RECORD
+Filename: gaea_tracker-1.2.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gaea_tracker/experiment_tracker.py

```diff
@@ -140,19 +140,23 @@
                                                 project_name=project_name,
                                                 local_name=local_name)
         experiment_runs = response.experimentRuns
         if experiment_runs is None:
             experiment_runs = {}
         bcelogger.info(f"Job kind is {self.job_kind} and run id is {run_id}")
         experiment_runs.update({self.job_kind: run_id})
-        self.windmill_client.update_job(workspace_id=workspace_id,
-                                        project_name=project_name,
-                                        display_name=response.displayName,
-                                        local_name=local_name,
-                                        experiment_runs=experiment_runs)
+        response = self.windmill_client.update_job(workspace_id=workspace_id,
+                                                   project_name=project_name,
+                                                   display_name=response.displayName,
+                                                   local_name=local_name,
+                                                   experiment_runs=experiment_runs)
+        bcelogger.info(f"Update job workspace id {workspace_id} "
+                       f"project name {project_name}"
+                       f"local name {local_name}"
+                       f"experiment runs to {experiment_runs}, response {response}")
         bcelogger.info(f"Update job {name} run id to {run_id}")
 
     def _get_windmill_job(self):
         """
         Get windmill job.
         """
         bcelogger.info(f"Project name is {self.project_name}")
```

## Comparing `gaea_tracker-1.2.0.6.dist-info/METADATA` & `gaea_tracker-1.2.0.8.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaea-tracker
-Version: 1.2.0.6
+Version: 1.2.0.8
 Summary: A common tracker library.
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/mlops/gaea-operator/tree/master
 Author: liuyawen03
 Author-email: liuyawen03@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gaea_tracker-1.2.0.6.dist-info/RECORD` & `gaea_tracker-1.2.0.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gaea_tracker/__init__.py,sha256=W_LJdwsPO-i_I_labqmA9UtINpc16H_xrUMtH3BgJrg,213
 gaea_tracker/aim_tracker.py,sha256=B8WcwJPQC6hKy-NMeZOYY6rQ4-cER_2j0zrxdPcNlxQ,1654
-gaea_tracker/experiment_tracker.py,sha256=zXPRhsH4lfPh_lscxHmEYRkV0LCSeBs55N06Kx9SuG4,7736
+gaea_tracker/experiment_tracker.py,sha256=jncI36sm4JEg6nXE8nMwZCz9ZZJzyQ4LhsRjvbFDpNU,8046
 gaea_tracker/mlflow_tracker.py,sha256=iSHBX25D1K5Ss1Jnhyq_2q9KAeizhOz_LTXIVcU3OXE,1459
-gaea_tracker-1.2.0.6.dist-info/METADATA,sha256=fSfqE1Fgx-uDqwCAcctI-Qx9TDnEFkiKMqx8dGeRwSo,1770
-gaea_tracker-1.2.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-gaea_tracker-1.2.0.6.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
-gaea_tracker-1.2.0.6.dist-info/RECORD,,
+gaea_tracker-1.2.0.8.dist-info/METADATA,sha256=bJS7o_wEQdbrPdm73aTUEno_spE4GbreV6zmpNSXGRg,1770
+gaea_tracker-1.2.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+gaea_tracker-1.2.0.8.dist-info/top_level.txt,sha256=puBG5QOAqx9ZaALXFt41yG0oBynhWzrKEJOMgH__hYw,13
+gaea_tracker-1.2.0.8.dist-info/RECORD,,
```

