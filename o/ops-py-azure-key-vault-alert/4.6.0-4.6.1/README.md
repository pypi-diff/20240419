# Comparing `tmp/ops_py_azure_key_vault_alert-4.6.0.tar.gz` & `tmp/ops_py_azure_key_vault_alert-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_py_azure_key_vault_alert-4.6.0.tar", last modified: Wed Apr 17 09:30:04 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_alert-4.6.1.tar", last modified: Fri Apr 19 14:13:24 2024, max compression
```

## Comparing `ops_py_azure_key_vault_alert-4.6.0.tar` & `ops_py_azure_key_vault_alert-4.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:04.327673 ops_py_azure_key_vault_alert-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-17 09:30:02.000000 ops_py_azure_key_vault_alert-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-17 09:30:04.327673 ops_py_azure_key_vault_alert-4.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:04.323673 ops_py_azure_key_vault_alert-4.6.0/azure_key_vault_alert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-17 09:29:59.000000 ops_py_azure_key_vault_alert-4.6.0/azure_key_vault_alert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8913 2024-04-17 09:29:59.000000 ops_py_azure_key_vault_alert-4.6.0/azure_key_vault_alert/azure_key_vault_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1648 2024-04-17 09:29:59.000000 ops_py_azure_key_vault_alert-4.6.0/azure_key_vault_alert/slack_post.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-17 09:29:59.000000 ops_py_azure_key_vault_alert-4.6.0/azure_key_vault_alert/teams_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:04.323673 ops_py_azure_key_vault_alert-4.6.0/ops_py_azure_key_vault_alert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-17 09:30:04.000000 ops_py_azure_key_vault_alert-4.6.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 09:30:04.000000 ops_py_azure_key_vault_alert-4.6.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:30:04.000000 ops_py_azure_key_vault_alert-4.6.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 09:30:04.000000 ops_py_azure_key_vault_alert-4.6.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 09:30:04.000000 ops_py_azure_key_vault_alert-4.6.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 09:30:02.000000 ops_py_azure_key_vault_alert-4.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-17 09:30:02.000000 ops_py_azure_key_vault_alert-4.6.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 09:29:59.000000 ops_py_azure_key_vault_alert-4.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:30:04.327673 ops_py_azure_key_vault_alert-4.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 09:30:02.000000 ops_py_azure_key_vault_alert-4.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:13:24.503633 ops_py_azure_key_vault_alert-4.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-19 14:13:21.000000 ops_py_azure_key_vault_alert-4.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-19 14:13:24.503633 ops_py_azure_key_vault_alert-4.6.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:13:24.499633 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8903 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/azure_key_vault_alert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1648 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/slack_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/teams_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:13:24.503633 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 14:13:24.000000 ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-19 14:13:21.000000 ops_py_azure_key_vault_alert-4.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-19 14:13:21.000000 ops_py_azure_key_vault_alert-4.6.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-19 14:13:15.000000 ops_py_azure_key_vault_alert-4.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:13:24.503633 ops_py_azure_key_vault_alert-4.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 14:13:21.000000 ops_py_azure_key_vault_alert-4.6.1/setup.py
```

### Comparing `ops_py_azure_key_vault_alert-4.6.0/LICENSE` & `ops_py_azure_key_vault_alert-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.6.0/PKG-INFO` & `ops_py_azure_key_vault_alert-4.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.6.0
+Version: 4.6.1
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,15 +37,15 @@
 Requires-Dist: jaraco.context==5.3.0
 Requires-Dist: jaraco.functools==4.0.0
 Requires-Dist: keyring==25.1.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: nh3==0.2.17
-Requires-Dist: ops-py-azure-key-vault-report==5.0.2
+Requires-Dist: ops-py-azure-key-vault-report==5.0.3
 Requires-Dist: ops-py-generate-pyproject==2.2.3
 Requires-Dist: ops-py-message-handler==1.0.3
 Requires-Dist: packaging==24.0
 Requires-Dist: pip==24.0
 Requires-Dist: pkginfo==1.10.0
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: pyproject_hooks==1.0.0
```

### Comparing `ops_py_azure_key_vault_alert-4.6.0/azure_key_vault_alert/azure_key_vault_alert.py` & `ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/azure_key_vault_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,22 +151,23 @@
 
     if teams_output and not success:
         success = teams_alert(title, kv_report, teams_max_chars, stdout_only=stdout_only, msg_handler=msg_handler)
 
     if msg_handler and not teams_output and not success:
         if slack_app and not success:
             if not isinstance(critical_threshold, int):
-                payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, md=False)
-            else:
                 payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars)
+            else:
+                payloads = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, md=True)
+
             if payloads:
                 success = slack_post(msg_handler, payloads=payloads)
 
         if not slack_app and not isinstance(critical_threshold, int) and not success:
-            posts = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, app=False, md=False)
+            posts = kv_report.get_slack_payloads(title, max_chars=slack_split_chars, app=False)
             if posts:
                 success = slack_post(msg_handler, posts=posts)
 
         if isinstance(critical_threshold, int) and not slack_app and not success:
             error_msg = "Posting individual critical messages to Slack Workflow is not supported."
             logging.error(error_msg)
             success = slack_post(msg_handler, posts=[(f"ERROR - {title}", error_msg)])
```

### Comparing `ops_py_azure_key_vault_alert-4.6.0/azure_key_vault_alert/slack_post.py` & `ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/slack_post.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.6.0/azure_key_vault_alert/teams_alert.py` & `ops_py_azure_key_vault_alert-4.6.1/azure_key_vault_alert/teams_alert.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.6.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO` & `ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.6.0
+Version: 4.6.1
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,15 +37,15 @@
 Requires-Dist: jaraco.context==5.3.0
 Requires-Dist: jaraco.functools==4.0.0
 Requires-Dist: keyring==25.1.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: nh3==0.2.17
-Requires-Dist: ops-py-azure-key-vault-report==5.0.2
+Requires-Dist: ops-py-azure-key-vault-report==5.0.3
 Requires-Dist: ops-py-generate-pyproject==2.2.3
 Requires-Dist: ops-py-message-handler==1.0.3
 Requires-Dist: packaging==24.0
 Requires-Dist: pip==24.0
 Requires-Dist: pkginfo==1.10.0
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: pyproject_hooks==1.0.0
```

### Comparing `ops_py_azure_key_vault_alert-4.6.0/ops_py_azure_key_vault_alert.egg-info/requires.txt` & `ops_py_azure_key_vault_alert-4.6.1/ops_py_azure_key_vault_alert.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jaraco.context==5.3.0
 jaraco.functools==4.0.0
 keyring==25.1.0
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
-ops-py-azure-key-vault-report==5.0.2
+ops-py-azure-key-vault-report==5.0.3
 ops-py-generate-pyproject==2.2.3
 ops-py-message-handler==1.0.3
 packaging==24.0
 pip==24.0
 pkginfo==1.10.0
 Pygments==2.17.2
 pyproject_hooks==1.0.0
```

### Comparing `ops_py_azure_key_vault_alert-4.6.0/readme.md` & `ops_py_azure_key_vault_alert-4.6.1/readme.md`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_alert-4.6.0/requirements.txt` & `ops_py_azure_key_vault_alert-4.6.1/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jaraco.context==5.3.0
 jaraco.functools==4.0.0
 keyring==25.1.0
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
-ops-py-azure-key-vault-report==5.0.2
+ops-py-azure-key-vault-report==5.0.3
 ops-py-generate-pyproject==2.2.3
 ops-py-message-handler==1.0.3
 packaging==24.0
 pip==24.0
 pkginfo==1.10.0
 Pygments==2.17.2
 pyproject_hooks==1.0.0
```

