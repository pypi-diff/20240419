# Comparing `tmp/pulumi_opsgenie-1.4.0a1713336015.tar.gz` & `tmp/pulumi_opsgenie-1.4.0a1713561317.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opsgenie-1.4.0a1713336015.tar", last modified: Wed Apr 17 07:02:17 2024, max compression
+gzip compressed data, was "pulumi_opsgenie-1.4.0a1713561317.tar", last modified: Fri Apr 19 21:22:41 2024, max compression
```

## Comparing `pulumi_opsgenie-1.4.0a1713336015.tar` & `pulumi_opsgenie-1.4.0a1713561317.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:02:17.577229 pulumi_opsgenie-1.4.0a1713336015/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-17 07:02:17.577229 pulumi_opsgenie-1.4.0a1713336015/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:02:17.573229 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   180603 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    58224 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    33812 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:02:17.577229 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/custom_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    23238 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/email_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23996 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    23857 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/incident_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15598 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/integration_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    36145 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    30636 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)   161038 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    25443 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/schedule_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/service_incident_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    19623 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    28130 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/team_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/user_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:02:17.577229 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-17 07:02:17.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-17 07:02:17.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:02:17.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 07:02:17.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 07:02:17.000000 pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 07:02:11.000000 pulumi_opsgenie-1.4.0a1713336015/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:02:17.577229 pulumi_opsgenie-1.4.0a1713336015/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:41.455259 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   180603 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58334 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30384 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19644 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/email_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20208 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24070 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24073 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/incident_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28522 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/integration_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36241 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30668 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)   161038 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25481 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/schedule_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/service_incident_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19745 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28280 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/team_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/user_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/setup.cfg
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/PKG-INFO` & `pulumi_opsgenie-1.4.0a1713561317/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.4.0a1713336015
+Version: 1.4.0a1713561317
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi,opsgenie
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/README.md` & `pulumi_opsgenie-1.4.0a1713561317/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/__init__.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/_inputs.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/_utilities.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/alert_policy.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/alert_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -700,20 +700,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_alert_policy = opsgenie.AlertPolicy("testAlertPolicy",
-            team_id=test_team.id,
+        test = opsgenie.Team("test",
+            name="example team",
+            description="This team deals with all the things")
+        test_alert_policy = opsgenie.AlertPolicy("test",
+            filters=[opsgenie.AlertPolicyFilterArgs()],
+            name="example policy",
+            team_id=test.id,
             policy_description="This is sample policy",
             message="{{message}}",
-            filters=[opsgenie.AlertPolicyFilterArgs()],
             time_restrictions=[opsgenie.AlertPolicyTimeRestrictionArgs(
                 type="weekday-and-time-of-day",
                 restriction_list=[
                     opsgenie.AlertPolicyTimeRestrictionRestrictionListArgs(
                         end_day="monday",
                         end_hour=7,
                         end_min=0,
@@ -783,20 +786,23 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_alert_policy = opsgenie.AlertPolicy("testAlertPolicy",
-            team_id=test_team.id,
+        test = opsgenie.Team("test",
+            name="example team",
+            description="This team deals with all the things")
+        test_alert_policy = opsgenie.AlertPolicy("test",
+            filters=[opsgenie.AlertPolicyFilterArgs()],
+            name="example policy",
+            team_id=test.id,
             policy_description="This is sample policy",
             message="{{message}}",
-            filters=[opsgenie.AlertPolicyFilterArgs()],
             time_restrictions=[opsgenie.AlertPolicyTimeRestrictionArgs(
                 type="weekday-and-time-of-day",
                 restriction_list=[
                     opsgenie.AlertPolicyTimeRestrictionRestrictionListArgs(
                         end_day="monday",
                         end_hour=7,
                         end_min=0,
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/api_integration.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/api_integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -372,60 +372,14 @@
                  suppress_notifications: Optional[pulumi.Input[bool]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  webhook_url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages an API Integration within Opsgenie.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_opsgenie as opsgenie
-
-        example_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationApiIntegration",
-            type="API",
-            responders=[
-                opsgenie.ApiIntegrationResponderArgs(
-                    type="user",
-                    id=opsgenie_user["user"]["id"],
-                ),
-                opsgenie.ApiIntegrationResponderArgs(
-                    type="user",
-                    id=opsgenie_user["fahri"]["id"],
-                ),
-            ])
-        example_api_integration_index_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationIndex/apiIntegrationApiIntegration",
-            type="Prometheus",
-            responders=[opsgenie.ApiIntegrationResponderArgs(
-                type="user",
-                id=opsgenie_user["user"]["id"],
-            )],
-            enabled=False,
-            allow_write_access=False,
-            ignore_responders_from_payload=True,
-            suppress_notifications=True,
-            owner_team_id=opsgenie_team["team"]["id"])
-        test3 = opsgenie.ApiIntegration("test3",
-            type="Webhook",
-            responders=[opsgenie.ApiIntegrationResponderArgs(
-                type="user",
-                id=opsgenie_user["user"]["id"],
-            )],
-            enabled=False,
-            allow_write_access=False,
-            suppress_notifications=True,
-            webhook_url="https://api.example.com/v1",
-            headers={
-                "header1": value1,
-            })
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         API Integrations can be imported using the `integration_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/apiIntegration:ApiIntegration this integration_id`
         ```
@@ -447,60 +401,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ApiIntegrationArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages an API Integration within Opsgenie.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_opsgenie as opsgenie
-
-        example_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationApiIntegration",
-            type="API",
-            responders=[
-                opsgenie.ApiIntegrationResponderArgs(
-                    type="user",
-                    id=opsgenie_user["user"]["id"],
-                ),
-                opsgenie.ApiIntegrationResponderArgs(
-                    type="user",
-                    id=opsgenie_user["fahri"]["id"],
-                ),
-            ])
-        example_api_integration_index_api_integration_api_integration = opsgenie.ApiIntegration("example-api-integrationIndex/apiIntegrationApiIntegration",
-            type="Prometheus",
-            responders=[opsgenie.ApiIntegrationResponderArgs(
-                type="user",
-                id=opsgenie_user["user"]["id"],
-            )],
-            enabled=False,
-            allow_write_access=False,
-            ignore_responders_from_payload=True,
-            suppress_notifications=True,
-            owner_team_id=opsgenie_team["team"]["id"])
-        test3 = opsgenie.ApiIntegration("test3",
-            type="Webhook",
-            responders=[opsgenie.ApiIntegrationResponderArgs(
-                type="user",
-                id=opsgenie_user["user"]["id"],
-            )],
-            enabled=False,
-            allow_write_access=False,
-            suppress_notifications=True,
-            webhook_url="https://api.example.com/v1",
-            headers={
-                "header1": value1,
-            })
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         API Integrations can be imported using the `integration_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/apiIntegration:ApiIntegration this integration_id`
         ```
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/config/vars.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/custom_role.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/custom_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,21 +171,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.CustomRole("test",
+            role_name="genierole",
+            extended_role="user",
+            granted_rights=["alert-delete"],
             disallowed_rights=[
                 "profile-edit",
                 "contacts-edit",
-            ],
-            extended_role="user",
-            granted_rights=["alert-delete"],
-            role_name="genierole")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disallowed_rights: The rights this role cannot have. For allowed values please refer [User Right Prerequisites](https://docs.opsgenie.com/docs/custom-user-role-api#section-user-right-prerequisites)
         :param pulumi.Input[str] extended_role: The role from which this role has been derived. Allowed Values: "user", "observer", "stakeholder".
@@ -205,21 +205,21 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.CustomRole("test",
+            role_name="genierole",
+            extended_role="user",
+            granted_rights=["alert-delete"],
             disallowed_rights=[
                 "profile-edit",
                 "contacts-edit",
-            ],
-            extended_role="user",
-            granted_rights=["alert-delete"],
-            role_name="genierole")
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param CustomRoleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/email_integration.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/email_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -256,58 +256,14 @@
                  owner_team_id: Optional[pulumi.Input[str]] = None,
                  responders: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EmailIntegrationResponderArgs']]]]] = None,
                  suppress_notifications: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Manages an Email Integration within Opsgenie.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_opsgenie as opsgenie
-
-        test_email_integration = opsgenie.EmailIntegration("testEmailIntegration", email_username="fahri")
-        test_index_email_integration_email_integration = opsgenie.EmailIntegration("testIndex/emailIntegrationEmailIntegration",
-            responders=[
-                opsgenie.EmailIntegrationResponderArgs(
-                    type="user",
-                    id=opsgenie_user["test"]["id"],
-                ),
-                opsgenie.EmailIntegrationResponderArgs(
-                    type="schedule",
-                    id=opsgenie_schedule["test"]["id"],
-                ),
-                opsgenie.EmailIntegrationResponderArgs(
-                    type="escalation",
-                    id=opsgenie_escalation["test"]["id"],
-                ),
-                opsgenie.EmailIntegrationResponderArgs(
-                    type="team",
-                    id=opsgenie_team["test2"]["id"],
-                ),
-            ],
-            email_username="test",
-            enabled=True,
-            ignore_responders_from_payload=True,
-            suppress_notifications=True)
-        test_opsgenie_index_email_integration_email_integration = opsgenie.EmailIntegration("testOpsgenieIndex/emailIntegrationEmailIntegration",
-            responders=[opsgenie.EmailIntegrationResponderArgs(
-                type="user",
-                id=opsgenie_user["test"]["id"],
-            )],
-            email_username="test",
-            enabled=True,
-            ignore_responders_from_payload=True,
-            suppress_notifications=True,
-            owner_team_id=opsgenie_team_genies["id"])
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         Email Integrations can be imported using the `id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/emailIntegration:EmailIntegration test id`
         ```
@@ -326,58 +282,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: EmailIntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages an Email Integration within Opsgenie.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_opsgenie as opsgenie
-
-        test_email_integration = opsgenie.EmailIntegration("testEmailIntegration", email_username="fahri")
-        test_index_email_integration_email_integration = opsgenie.EmailIntegration("testIndex/emailIntegrationEmailIntegration",
-            responders=[
-                opsgenie.EmailIntegrationResponderArgs(
-                    type="user",
-                    id=opsgenie_user["test"]["id"],
-                ),
-                opsgenie.EmailIntegrationResponderArgs(
-                    type="schedule",
-                    id=opsgenie_schedule["test"]["id"],
-                ),
-                opsgenie.EmailIntegrationResponderArgs(
-                    type="escalation",
-                    id=opsgenie_escalation["test"]["id"],
-                ),
-                opsgenie.EmailIntegrationResponderArgs(
-                    type="team",
-                    id=opsgenie_team["test2"]["id"],
-                ),
-            ],
-            email_username="test",
-            enabled=True,
-            ignore_responders_from_payload=True,
-            suppress_notifications=True)
-        test_opsgenie_index_email_integration_email_integration = opsgenie.EmailIntegration("testOpsgenieIndex/emailIntegrationEmailIntegration",
-            responders=[opsgenie.EmailIntegrationResponderArgs(
-                type="user",
-                id=opsgenie_user["test"]["id"],
-            )],
-            email_username="test",
-            enabled=True,
-            ignore_responders_from_payload=True,
-            suppress_notifications=True,
-            owner_team_id=opsgenie_team_genies["id"])
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         Email Integrations can be imported using the `id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/emailIntegration:EmailIntegration test id`
         ```
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/escalation.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/escalation.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,62 +207,65 @@
         An escalation with a single rule
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        default = opsgenie.Escalation("default", rules=[opsgenie.EscalationRuleArgs(
-            condition="if-not-acked",
-            notify_type="default",
-            delay=1,
-            recipients=[opsgenie.EscalationRuleRecipientArgs(
-                type="user",
-                id=opsgenie_user["test"]["id"],
-            )],
-        )])
+        default = opsgenie.Escalation("default",
+            name="genieescalation",
+            rules=[opsgenie.EscalationRuleArgs(
+                condition="if-not-acked",
+                notify_type="default",
+                delay=1,
+                recipients=[opsgenie.EscalationRuleRecipientArgs(
+                    type="user",
+                    id=test["id"],
+                )],
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         An escalation with a multiple rules
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         default = opsgenie.Escalation("default",
+            name="genieescalation",
             description="test",
-            owner_team_id=opsgenie_team["test"]["id"],
+            owner_team_id=test_opsgenie_team["id"],
             rules=[
                 opsgenie.EscalationRuleArgs(
                     condition="if-not-acked",
                     notify_type="default",
                     delay=1,
                     recipients=[opsgenie.EscalationRuleRecipientArgs(
                         type="user",
-                        id=opsgenie_user["test"]["id"],
+                        id=test["id"],
                     )],
                 ),
                 opsgenie.EscalationRuleArgs(
                     condition="if-not-acked",
                     notify_type="default",
                     delay=1,
                     recipients=[opsgenie.EscalationRuleRecipientArgs(
                         type="team",
-                        id=opsgenie_team["test"]["id"],
+                        id=test_opsgenie_team["id"],
                     )],
                 ),
                 opsgenie.EscalationRuleArgs(
                     condition="if-not-acked",
                     notify_type="default",
                     delay=1,
                     recipients=[opsgenie.EscalationRuleRecipientArgs(
                         type="schedule",
-                        id=opsgenie_schedule["test"]["id"],
+                        id=test_opsgenie_schedule["id"],
                     )],
                 ),
             ],
             repeats=[opsgenie.EscalationRepeatArgs(
                 wait_interval=10,
                 count=1,
                 reset_recipient_states=True,
@@ -301,62 +304,65 @@
         An escalation with a single rule
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        default = opsgenie.Escalation("default", rules=[opsgenie.EscalationRuleArgs(
-            condition="if-not-acked",
-            notify_type="default",
-            delay=1,
-            recipients=[opsgenie.EscalationRuleRecipientArgs(
-                type="user",
-                id=opsgenie_user["test"]["id"],
-            )],
-        )])
+        default = opsgenie.Escalation("default",
+            name="genieescalation",
+            rules=[opsgenie.EscalationRuleArgs(
+                condition="if-not-acked",
+                notify_type="default",
+                delay=1,
+                recipients=[opsgenie.EscalationRuleRecipientArgs(
+                    type="user",
+                    id=test["id"],
+                )],
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         An escalation with a multiple rules
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         default = opsgenie.Escalation("default",
+            name="genieescalation",
             description="test",
-            owner_team_id=opsgenie_team["test"]["id"],
+            owner_team_id=test_opsgenie_team["id"],
             rules=[
                 opsgenie.EscalationRuleArgs(
                     condition="if-not-acked",
                     notify_type="default",
                     delay=1,
                     recipients=[opsgenie.EscalationRuleRecipientArgs(
                         type="user",
-                        id=opsgenie_user["test"]["id"],
+                        id=test["id"],
                     )],
                 ),
                 opsgenie.EscalationRuleArgs(
                     condition="if-not-acked",
                     notify_type="default",
                     delay=1,
                     recipients=[opsgenie.EscalationRuleRecipientArgs(
                         type="team",
-                        id=opsgenie_team["test"]["id"],
+                        id=test_opsgenie_team["id"],
                     )],
                 ),
                 opsgenie.EscalationRuleArgs(
                     condition="if-not-acked",
                     notify_type="default",
                     delay=1,
                     recipients=[opsgenie.EscalationRuleRecipientArgs(
                         type="schedule",
-                        id=opsgenie_schedule["test"]["id"],
+                        id=test_opsgenie_schedule["id"],
                     )],
                 ),
             ],
             repeats=[opsgenie.EscalationRepeatArgs(
                 wait_interval=10,
                 count=1,
                 reset_recipient_states=True,
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_escalation.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_heartbeat.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_schedule.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_service.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_team.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/get_user.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/heartbeat.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/heartbeat.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,25 +334,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Heartbeat("test",
+            name="genieheartbeat-test",
+            description="test opsgenie heartbeat terraform",
+            interval_unit="minutes",
+            interval=10,
+            enabled=False,
             alert_message="Test",
             alert_priority="P3",
             alert_tags=[
                 "test",
                 "fahri",
             ],
-            description="test opsgenie heartbeat terraform",
-            enabled=False,
-            interval=10,
-            interval_unit="minutes",
-            owner_team_id=opsgenie_team["test"]["id"])
+            owner_team_id=test_opsgenie_team["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Heartbeat Integrations can be imported using the `name`, e.g.
 
@@ -385,25 +386,26 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Heartbeat("test",
+            name="genieheartbeat-test",
+            description="test opsgenie heartbeat terraform",
+            interval_unit="minutes",
+            interval=10,
+            enabled=False,
             alert_message="Test",
             alert_priority="P3",
             alert_tags=[
                 "test",
                 "fahri",
             ],
-            description="test opsgenie heartbeat terraform",
-            enabled=False,
-            interval=10,
-            interval_unit="minutes",
-            owner_team_id=opsgenie_team["test"]["id"])
+            owner_team_id=test_opsgenie_team["id"])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Heartbeat Integrations can be imported using the `name`, e.g.
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/incident_template.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/incident_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,17 +286,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_service = opsgenie.Service("testService", team_id=test_team.id)
-        test_incident_template = opsgenie.IncidentTemplate("testIncidentTemplate",
+        test = opsgenie.Team("test",
+            name="genietest-team",
+            description="This team deals with all the things")
+        test_service = opsgenie.Service("test",
+            name="genietest-service",
+            team_id=test.id)
+        test_incident_template = opsgenie.IncidentTemplate("test",
+            name="genietest-incident-template",
             message="Incident Message",
             priority="P2",
             stakeholder_properties=[opsgenie.IncidentTemplateStakeholderPropertyArgs(
                 enable=True,
                 message="Stakeholder Message",
                 description="Stakeholder Description",
             )],
@@ -342,17 +347,22 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_service = opsgenie.Service("testService", team_id=test_team.id)
-        test_incident_template = opsgenie.IncidentTemplate("testIncidentTemplate",
+        test = opsgenie.Team("test",
+            name="genietest-team",
+            description="This team deals with all the things")
+        test_service = opsgenie.Service("test",
+            name="genietest-service",
+            team_id=test.id)
+        test_incident_template = opsgenie.IncidentTemplate("test",
+            name="genietest-incident-template",
             message="Incident Message",
             priority="P2",
             stakeholder_properties=[opsgenie.IncidentTemplateStakeholderPropertyArgs(
                 enable=True,
                 message="Stakeholder Message",
                 description="Stakeholder Description",
             )],
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/integration_action.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/service.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,333 +4,332 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
-from . import outputs
-from ._inputs import *
 
-__all__ = ['IntegrationActionArgs', 'IntegrationAction']
+__all__ = ['ServiceArgs', 'Service']
 
 @pulumi.input_type
-class IntegrationActionArgs:
+class ServiceArgs:
     def __init__(__self__, *,
-                 integration_id: pulumi.Input[str],
-                 acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]] = None,
-                 add_notes: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]] = None,
-                 closes: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]] = None,
-                 creates: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]] = None,
-                 ignores: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]] = None):
-        """
-        The set of arguments for constructing a IntegrationAction resource.
-        :param pulumi.Input[str] integration_id: ID of the parent integration resource to bind to.
-        """
-        pulumi.set(__self__, "integration_id", integration_id)
-        if acknowledges is not None:
-            pulumi.set(__self__, "acknowledges", acknowledges)
-        if add_notes is not None:
-            pulumi.set(__self__, "add_notes", add_notes)
-        if closes is not None:
-            pulumi.set(__self__, "closes", closes)
-        if creates is not None:
-            pulumi.set(__self__, "creates", creates)
-        if ignores is not None:
-            pulumi.set(__self__, "ignores", ignores)
-
-    @property
-    @pulumi.getter(name="integrationId")
-    def integration_id(self) -> pulumi.Input[str]:
-        """
-        ID of the parent integration resource to bind to.
-        """
-        return pulumi.get(self, "integration_id")
-
-    @integration_id.setter
-    def integration_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "integration_id", value)
-
-    @property
-    @pulumi.getter
-    def acknowledges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]]:
-        return pulumi.get(self, "acknowledges")
-
-    @acknowledges.setter
-    def acknowledges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]]):
-        pulumi.set(self, "acknowledges", value)
+                 team_id: pulumi.Input[str],
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        The set of arguments for constructing a Service resource.
+        :param pulumi.Input[str] team_id: Team id of the service. This field must not be longer than 512 characters.
+        :param pulumi.Input[str] description: Description field of the service that is generally used to provide a detailed information about the service.
+        :param pulumi.Input[str] name: Name of the service. This field must not be longer than 100 characters.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags for the service, with a maximum of 20 tags per service.
+        """
+        pulumi.set(__self__, "team_id", team_id)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
 
     @property
-    @pulumi.getter(name="addNotes")
-    def add_notes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]]:
-        return pulumi.get(self, "add_notes")
+    @pulumi.getter(name="teamId")
+    def team_id(self) -> pulumi.Input[str]:
+        """
+        Team id of the service. This field must not be longer than 512 characters.
+        """
+        return pulumi.get(self, "team_id")
 
-    @add_notes.setter
-    def add_notes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]]):
-        pulumi.set(self, "add_notes", value)
+    @team_id.setter
+    def team_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "team_id", value)
 
     @property
     @pulumi.getter
-    def closes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]]:
-        return pulumi.get(self, "closes")
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        Description field of the service that is generally used to provide a detailed information about the service.
+        """
+        return pulumi.get(self, "description")
 
-    @closes.setter
-    def closes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]]):
-        pulumi.set(self, "closes", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def creates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]]:
-        return pulumi.get(self, "creates")
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the service. This field must not be longer than 100 characters.
+        """
+        return pulumi.get(self, "name")
 
-    @creates.setter
-    def creates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]]):
-        pulumi.set(self, "creates", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def ignores(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]]:
-        return pulumi.get(self, "ignores")
+    def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Tags for the service, with a maximum of 20 tags per service.
+        """
+        return pulumi.get(self, "tags")
 
-    @ignores.setter
-    def ignores(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]]):
-        pulumi.set(self, "ignores", value)
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
 
 
 @pulumi.input_type
-class _IntegrationActionState:
+class _ServiceState:
     def __init__(__self__, *,
-                 acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]] = None,
-                 add_notes: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]] = None,
-                 closes: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]] = None,
-                 creates: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]] = None,
-                 ignores: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]] = None,
-                 integration_id: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering IntegrationAction resources.
-        :param pulumi.Input[str] integration_id: ID of the parent integration resource to bind to.
-        """
-        if acknowledges is not None:
-            pulumi.set(__self__, "acknowledges", acknowledges)
-        if add_notes is not None:
-            pulumi.set(__self__, "add_notes", add_notes)
-        if closes is not None:
-            pulumi.set(__self__, "closes", closes)
-        if creates is not None:
-            pulumi.set(__self__, "creates", creates)
-        if ignores is not None:
-            pulumi.set(__self__, "ignores", ignores)
-        if integration_id is not None:
-            pulumi.set(__self__, "integration_id", integration_id)
-
-    @property
-    @pulumi.getter
-    def acknowledges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]]:
-        return pulumi.get(self, "acknowledges")
-
-    @acknowledges.setter
-    def acknowledges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeArgs']]]]):
-        pulumi.set(self, "acknowledges", value)
-
-    @property
-    @pulumi.getter(name="addNotes")
-    def add_notes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]]:
-        return pulumi.get(self, "add_notes")
-
-    @add_notes.setter
-    def add_notes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteArgs']]]]):
-        pulumi.set(self, "add_notes", value)
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 team_id: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering Service resources.
+        :param pulumi.Input[str] description: Description field of the service that is generally used to provide a detailed information about the service.
+        :param pulumi.Input[str] name: Name of the service. This field must not be longer than 100 characters.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags for the service, with a maximum of 20 tags per service.
+        :param pulumi.Input[str] team_id: Team id of the service. This field must not be longer than 512 characters.
+        """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if team_id is not None:
+            pulumi.set(__self__, "team_id", team_id)
 
     @property
     @pulumi.getter
-    def closes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]]:
-        return pulumi.get(self, "closes")
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        Description field of the service that is generally used to provide a detailed information about the service.
+        """
+        return pulumi.get(self, "description")
 
-    @closes.setter
-    def closes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseArgs']]]]):
-        pulumi.set(self, "closes", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def creates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]]:
-        return pulumi.get(self, "creates")
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the service. This field must not be longer than 100 characters.
+        """
+        return pulumi.get(self, "name")
 
-    @creates.setter
-    def creates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateArgs']]]]):
-        pulumi.set(self, "creates", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def ignores(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]]:
-        return pulumi.get(self, "ignores")
+    def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Tags for the service, with a maximum of 20 tags per service.
+        """
+        return pulumi.get(self, "tags")
 
-    @ignores.setter
-    def ignores(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreArgs']]]]):
-        pulumi.set(self, "ignores", value)
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
 
     @property
-    @pulumi.getter(name="integrationId")
-    def integration_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="teamId")
+    def team_id(self) -> Optional[pulumi.Input[str]]:
         """
-        ID of the parent integration resource to bind to.
+        Team id of the service. This field must not be longer than 512 characters.
         """
-        return pulumi.get(self, "integration_id")
+        return pulumi.get(self, "team_id")
 
-    @integration_id.setter
-    def integration_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "integration_id", value)
+    @team_id.setter
+    def team_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "team_id", value)
 
 
-class IntegrationAction(pulumi.CustomResource):
+class Service(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAcknowledgeArgs']]]]] = None,
-                 add_notes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAddNoteArgs']]]]] = None,
-                 closes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCloseArgs']]]]] = None,
-                 creates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCreateArgs']]]]] = None,
-                 ignores: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionIgnoreArgs']]]]] = None,
-                 integration_id: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 team_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manages advanced actions for Integrations within Opsgenie. This applies for the following resources:
-        * `ApiIntegration`
-        * `EmailIntegration`
-
-        The actions that are supported are:
-        * `create`
-        * `close`
-        * `acknowledge`
-        * `add_note`
-        * `ignore`
+        Manages a Service within Opsgenie.
+
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_opsgenie as opsgenie
+
+        payment = opsgenie.Team("payment",
+            name="example",
+            description="This team deals with all the things")
+        this = opsgenie.Service("this",
+            name="Payment",
+            team_id="$opsgenie_team.payment.id")
+        ```
+        <!--End PulumiCodeChooser -->
+
+        ## Import
+
+        Teams can be imported using the `service_id`, e.g.
+
+        ```sh
+        $ pulumi import opsgenie:index/service:Service this service_id`
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] integration_id: ID of the parent integration resource to bind to.
+        :param pulumi.Input[str] description: Description field of the service that is generally used to provide a detailed information about the service.
+        :param pulumi.Input[str] name: Name of the service. This field must not be longer than 100 characters.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags for the service, with a maximum of 20 tags per service.
+        :param pulumi.Input[str] team_id: Team id of the service. This field must not be longer than 512 characters.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: IntegrationActionArgs,
+                 args: ServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manages advanced actions for Integrations within Opsgenie. This applies for the following resources:
-        * `ApiIntegration`
-        * `EmailIntegration`
-
-        The actions that are supported are:
-        * `create`
-        * `close`
-        * `acknowledge`
-        * `add_note`
-        * `ignore`
+        Manages a Service within Opsgenie.
+
+        ## Example Usage
+
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_opsgenie as opsgenie
+
+        payment = opsgenie.Team("payment",
+            name="example",
+            description="This team deals with all the things")
+        this = opsgenie.Service("this",
+            name="Payment",
+            team_id="$opsgenie_team.payment.id")
+        ```
+        <!--End PulumiCodeChooser -->
+
+        ## Import
+
+        Teams can be imported using the `service_id`, e.g.
+
+        ```sh
+        $ pulumi import opsgenie:index/service:Service this service_id`
+        ```
 
         :param str resource_name: The name of the resource.
-        :param IntegrationActionArgs args: The arguments to use to populate this resource's properties.
+        :param ServiceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(IntegrationActionArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAcknowledgeArgs']]]]] = None,
-                 add_notes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAddNoteArgs']]]]] = None,
-                 closes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCloseArgs']]]]] = None,
-                 creates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCreateArgs']]]]] = None,
-                 ignores: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionIgnoreArgs']]]]] = None,
-                 integration_id: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 team_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = IntegrationActionArgs.__new__(IntegrationActionArgs)
+            __props__ = ServiceArgs.__new__(ServiceArgs)
 
-            __props__.__dict__["acknowledges"] = acknowledges
-            __props__.__dict__["add_notes"] = add_notes
-            __props__.__dict__["closes"] = closes
-            __props__.__dict__["creates"] = creates
-            __props__.__dict__["ignores"] = ignores
-            if integration_id is None and not opts.urn:
-                raise TypeError("Missing required property 'integration_id'")
-            __props__.__dict__["integration_id"] = integration_id
-        super(IntegrationAction, __self__).__init__(
-            'opsgenie:index/integrationAction:IntegrationAction',
+            __props__.__dict__["description"] = description
+            __props__.__dict__["name"] = name
+            __props__.__dict__["tags"] = tags
+            if team_id is None and not opts.urn:
+                raise TypeError("Missing required property 'team_id'")
+            __props__.__dict__["team_id"] = team_id
+        super(Service, __self__).__init__(
+            'opsgenie:index/service:Service',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            acknowledges: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAcknowledgeArgs']]]]] = None,
-            add_notes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionAddNoteArgs']]]]] = None,
-            closes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCloseArgs']]]]] = None,
-            creates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionCreateArgs']]]]] = None,
-            ignores: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationActionIgnoreArgs']]]]] = None,
-            integration_id: Optional[pulumi.Input[str]] = None) -> 'IntegrationAction':
+            description: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            team_id: Optional[pulumi.Input[str]] = None) -> 'Service':
         """
-        Get an existing IntegrationAction resource's state with the given name, id, and optional extra
+        Get an existing Service resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] integration_id: ID of the parent integration resource to bind to.
+        :param pulumi.Input[str] description: Description field of the service that is generally used to provide a detailed information about the service.
+        :param pulumi.Input[str] name: Name of the service. This field must not be longer than 100 characters.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags for the service, with a maximum of 20 tags per service.
+        :param pulumi.Input[str] team_id: Team id of the service. This field must not be longer than 512 characters.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _IntegrationActionState.__new__(_IntegrationActionState)
+        __props__ = _ServiceState.__new__(_ServiceState)
 
-        __props__.__dict__["acknowledges"] = acknowledges
-        __props__.__dict__["add_notes"] = add_notes
-        __props__.__dict__["closes"] = closes
-        __props__.__dict__["creates"] = creates
-        __props__.__dict__["ignores"] = ignores
-        __props__.__dict__["integration_id"] = integration_id
-        return IntegrationAction(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["description"] = description
+        __props__.__dict__["name"] = name
+        __props__.__dict__["tags"] = tags
+        __props__.__dict__["team_id"] = team_id
+        return Service(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def acknowledges(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionAcknowledge']]]:
-        return pulumi.get(self, "acknowledges")
-
-    @property
-    @pulumi.getter(name="addNotes")
-    def add_notes(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionAddNote']]]:
-        return pulumi.get(self, "add_notes")
-
-    @property
-    @pulumi.getter
-    def closes(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionClose']]]:
-        return pulumi.get(self, "closes")
+    def description(self) -> pulumi.Output[Optional[str]]:
+        """
+        Description field of the service that is generally used to provide a detailed information about the service.
+        """
+        return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def creates(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionCreate']]]:
-        return pulumi.get(self, "creates")
+    def name(self) -> pulumi.Output[str]:
+        """
+        Name of the service. This field must not be longer than 100 characters.
+        """
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def ignores(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationActionIgnore']]]:
-        return pulumi.get(self, "ignores")
+    def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        Tags for the service, with a maximum of 20 tags per service.
+        """
+        return pulumi.get(self, "tags")
 
     @property
-    @pulumi.getter(name="integrationId")
-    def integration_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="teamId")
+    def team_id(self) -> pulumi.Output[str]:
         """
-        ID of the parent integration resource to bind to.
+        Team id of the service. This field must not be longer than 512 characters.
         """
-        return pulumi.get(self, "integration_id")
+        return pulumi.get(self, "team_id")
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/maintenance.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/maintenance.py`

 * *Files 13% similar despite different names*

```diff
@@ -131,38 +131,14 @@
                  description: Optional[pulumi.Input[str]] = None,
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MaintenanceRuleArgs']]]]] = None,
                  times: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MaintenanceTimeArgs']]]]] = None,
                  __props__=None):
         """
         Manages a Maintenance within Opsgenie.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_opsgenie as opsgenie
-
-        test = opsgenie.Maintenance("test",
-            description="geniemaintenance-%s",
-            rules=[opsgenie.MaintenanceRuleArgs(
-                entities=[opsgenie.MaintenanceRuleEntityArgs(
-                    id=opsgenie_email_integration["test"]["id"],
-                    type="integration",
-                )],
-                state="enabled",
-            )],
-            times=[opsgenie.MaintenanceTimeArgs(
-                end_date="2019-06-%dT17:50:00Z",
-                start_date="2019-06-20T17:45:00Z",
-                type="schedule",
-            )])
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         Maintenance policies can be imported using the `policy_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/maintenance:Maintenance test policy_id`
         ```
@@ -178,38 +154,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: MaintenanceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Maintenance within Opsgenie.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_opsgenie as opsgenie
-
-        test = opsgenie.Maintenance("test",
-            description="geniemaintenance-%s",
-            rules=[opsgenie.MaintenanceRuleArgs(
-                entities=[opsgenie.MaintenanceRuleEntityArgs(
-                    id=opsgenie_email_integration["test"]["id"],
-                    type="integration",
-                )],
-                state="enabled",
-            )],
-            times=[opsgenie.MaintenanceTimeArgs(
-                end_date="2019-06-%dT17:50:00Z",
-                start_date="2019-06-20T17:45:00Z",
-                type="schedule",
-            )])
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         Maintenance policies can be imported using the `policy_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/maintenance:Maintenance test policy_id`
         ```
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/notification_policy.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/notification_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,24 +402,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_notification_policy = opsgenie.NotificationPolicy("testNotificationPolicy",
-            team_id=test_team.id,
+        test = opsgenie.Team("test",
+            name="example team",
+            description="This team deals with all the things")
+        test_notification_policy = opsgenie.NotificationPolicy("test",
+            filters=[opsgenie.NotificationPolicyFilterArgs()],
+            name="example policy",
+            team_id=test.id,
             policy_description="This policy has a delay action",
             delay_actions=[opsgenie.NotificationPolicyDelayActionArgs(
                 delay_option="next-time",
                 until_minute=1,
                 until_hour=9,
-            )],
-            filters=[opsgenie.NotificationPolicyFilterArgs()])
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Notification policies can be imported using the `team_id` and `notification_policy_id`, e.g.
 
@@ -453,24 +456,27 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_notification_policy = opsgenie.NotificationPolicy("testNotificationPolicy",
-            team_id=test_team.id,
+        test = opsgenie.Team("test",
+            name="example team",
+            description="This team deals with all the things")
+        test_notification_policy = opsgenie.NotificationPolicy("test",
+            filters=[opsgenie.NotificationPolicyFilterArgs()],
+            name="example policy",
+            team_id=test.id,
             policy_description="This policy has a delay action",
             delay_actions=[opsgenie.NotificationPolicyDelayActionArgs(
                 delay_option="next-time",
                 until_minute=1,
                 until_hour=9,
-            )],
-            filters=[opsgenie.NotificationPolicyFilterArgs()])
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Notification policies can be imported using the `team_id` and `notification_policy_id`, e.g.
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/notification_rule.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/notification_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,20 +370,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_user = opsgenie.User("testUser",
+        test = opsgenie.User("test",
             username="Example user",
             full_name="Name Lastname",
             role="User")
-        test_notification_rule = opsgenie.NotificationRule("testNotificationRule",
-            username=test_user.username,
+        test_notification_rule = opsgenie.NotificationRule("test",
+            name="Example notification rule",
+            username=test.username,
             action_type="schedule-end",
             notification_times=[
                 "just-before",
                 "15-minutes-ago",
             ],
             steps=[opsgenie.NotificationRuleStepArgs(
                 contacts=[opsgenie.NotificationRuleStepContactArgs(
@@ -424,20 +425,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_user = opsgenie.User("testUser",
+        test = opsgenie.User("test",
             username="Example user",
             full_name="Name Lastname",
             role="User")
-        test_notification_rule = opsgenie.NotificationRule("testNotificationRule",
-            username=test_user.username,
+        test_notification_rule = opsgenie.NotificationRule("test",
+            name="Example notification rule",
+            username=test.username,
             action_type="schedule-end",
             notification_times=[
                 "just-before",
                 "15-minutes-ago",
             ],
             steps=[opsgenie.NotificationRuleStepArgs(
                 contacts=[opsgenie.NotificationRuleStepContactArgs(
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/outputs.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/provider.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/schedule.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/schedule.py`

 * *Files 8% similar despite different names*

```diff
@@ -197,29 +197,14 @@
                  name: Optional[pulumi.Input[str]] = None,
                  owner_team_id: Optional[pulumi.Input[str]] = None,
                  timezone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Schedule within Opsgenie.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_opsgenie as opsgenie
-
-        test = opsgenie.Schedule("test",
-            description="schedule test",
-            enabled=False,
-            owner_team_id=opsgenie_team["test"]["id"],
-            timezone="Europe/Rome")
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         Schedule can be imported using the `schedule_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/schedule:Schedule test schedule_id`
         ```
@@ -237,29 +222,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ScheduleArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Schedule within Opsgenie.
 
-        ## Example Usage
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        import pulumi_opsgenie as opsgenie
-
-        test = opsgenie.Schedule("test",
-            description="schedule test",
-            enabled=False,
-            owner_team_id=opsgenie_team["test"]["id"],
-            timezone="Europe/Rome")
-        ```
-        <!--End PulumiCodeChooser -->
-
         ## Import
 
         Schedule can be imported using the `schedule_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/schedule:Schedule test schedule_id`
         ```
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/schedule_rotation.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/schedule_rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,32 +294,33 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.ScheduleRotation("test",
+            schedule_id=test_opsgenie_schedule["id"],
+            name="test",
+            start_date="2019-06-18T17:00:00Z",
             end_date="2019-06-20T17:30:00Z",
+            type="hourly",
             length=6,
             participants=[opsgenie.ScheduleRotationParticipantArgs(
-                id=opsgenie_user["test"]["id"],
                 type="user",
+                id=test_opsgenie_user["id"],
             )],
-            schedule_id=opsgenie_schedule["test"]["id"],
-            start_date="2019-06-18T17:00:00Z",
             time_restrictions=[opsgenie.ScheduleRotationTimeRestrictionArgs(
+                type="time-of-day",
                 restriction=[opsgenie.ScheduleRotationTimeRestrictionRestrictionArgs(
-                    end_hour=10,
-                    end_min=1,
                     start_hour=1,
                     start_min=1,
+                    end_hour=10,
+                    end_min=1,
                 )],
-                type="time-of-day",
-            )],
-            type="hourly")
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Schedule Rotations can be imported using the `schedule_id/rotation_id`, e.g.
 
@@ -350,32 +351,33 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.ScheduleRotation("test",
+            schedule_id=test_opsgenie_schedule["id"],
+            name="test",
+            start_date="2019-06-18T17:00:00Z",
             end_date="2019-06-20T17:30:00Z",
+            type="hourly",
             length=6,
             participants=[opsgenie.ScheduleRotationParticipantArgs(
-                id=opsgenie_user["test"]["id"],
                 type="user",
+                id=test_opsgenie_user["id"],
             )],
-            schedule_id=opsgenie_schedule["test"]["id"],
-            start_date="2019-06-18T17:00:00Z",
             time_restrictions=[opsgenie.ScheduleRotationTimeRestrictionArgs(
+                type="time-of-day",
                 restriction=[opsgenie.ScheduleRotationTimeRestrictionRestrictionArgs(
-                    end_hour=10,
-                    end_min=1,
                     start_hour=1,
                     start_min=1,
+                    end_hour=10,
+                    end_min=1,
                 )],
-                type="time-of-day",
-            )],
-            type="hourly")
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Schedule Rotations can be imported using the `schedule_id/rotation_id`, e.g.
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/service.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/user_contact.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,323 +5,345 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['ServiceArgs', 'Service']
+__all__ = ['UserContactArgs', 'UserContact']
 
 @pulumi.input_type
-class ServiceArgs:
+class UserContactArgs:
     def __init__(__self__, *,
-                 team_id: pulumi.Input[str],
-                 description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        The set of arguments for constructing a Service resource.
-        :param pulumi.Input[str] team_id: Team id of the service. This field must not be longer than 512 characters.
-        :param pulumi.Input[str] description: Description field of the service that is generally used to provide a detailed information about the service.
-        :param pulumi.Input[str] name: Name of the service. This field must not be longer than 100 characters.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags for the service, with a maximum of 20 tags per service.
-        """
-        pulumi.set(__self__, "team_id", team_id)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if tags is not None:
-            pulumi.set(__self__, "tags", tags)
+                 method: pulumi.Input[str],
+                 to: pulumi.Input[str],
+                 username: pulumi.Input[str],
+                 enabled: Optional[pulumi.Input[bool]] = None):
+        """
+        The set of arguments for constructing a UserContact resource.
+        :param pulumi.Input[str] method: This parameter is the contact method of user and should be one of email, sms or voice. Please note that adding mobile is not supported from API.
+        :param pulumi.Input[str] to: to field is the address of given method.
+        :param pulumi.Input[str] username: The username for contact.(reference)
+        :param pulumi.Input[bool] enabled: Enable contact of the user in OpsGenie. Default value is true.
+        """
+        pulumi.set(__self__, "method", method)
+        pulumi.set(__self__, "to", to)
+        pulumi.set(__self__, "username", username)
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
 
     @property
-    @pulumi.getter(name="teamId")
-    def team_id(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def method(self) -> pulumi.Input[str]:
         """
-        Team id of the service. This field must not be longer than 512 characters.
+        This parameter is the contact method of user and should be one of email, sms or voice. Please note that adding mobile is not supported from API.
         """
-        return pulumi.get(self, "team_id")
+        return pulumi.get(self, "method")
 
-    @team_id.setter
-    def team_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "team_id", value)
+    @method.setter
+    def method(self, value: pulumi.Input[str]):
+        pulumi.set(self, "method", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    def to(self) -> pulumi.Input[str]:
         """
-        Description field of the service that is generally used to provide a detailed information about the service.
+        to field is the address of given method.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "to")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @to.setter
+    def to(self, value: pulumi.Input[str]):
+        pulumi.set(self, "to", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def username(self) -> pulumi.Input[str]:
         """
-        Name of the service. This field must not be longer than 100 characters.
+        The username for contact.(reference)
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "username")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
 
     @property
     @pulumi.getter
-    def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Tags for the service, with a maximum of 20 tags per service.
+        Enable contact of the user in OpsGenie. Default value is true.
         """
-        return pulumi.get(self, "tags")
+        return pulumi.get(self, "enabled")
 
-    @tags.setter
-    def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "tags", value)
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
 
 
 @pulumi.input_type
-class _ServiceState:
+class _UserContactState:
     def __init__(__self__, *,
-                 description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 team_id: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering Service resources.
-        :param pulumi.Input[str] description: Description field of the service that is generally used to provide a detailed information about the service.
-        :param pulumi.Input[str] name: Name of the service. This field must not be longer than 100 characters.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags for the service, with a maximum of 20 tags per service.
-        :param pulumi.Input[str] team_id: Team id of the service. This field must not be longer than 512 characters.
-        """
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if tags is not None:
-            pulumi.set(__self__, "tags", tags)
-        if team_id is not None:
-            pulumi.set(__self__, "team_id", team_id)
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 method: Optional[pulumi.Input[str]] = None,
+                 to: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering UserContact resources.
+        :param pulumi.Input[bool] enabled: Enable contact of the user in OpsGenie. Default value is true.
+        :param pulumi.Input[str] method: This parameter is the contact method of user and should be one of email, sms or voice. Please note that adding mobile is not supported from API.
+        :param pulumi.Input[str] to: to field is the address of given method.
+        :param pulumi.Input[str] username: The username for contact.(reference)
+        """
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if method is not None:
+            pulumi.set(__self__, "method", method)
+        if to is not None:
+            pulumi.set(__self__, "to", to)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Description field of the service that is generally used to provide a detailed information about the service.
+        Enable contact of the user in OpsGenie. Default value is true.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "enabled")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def method(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the service. This field must not be longer than 100 characters.
+        This parameter is the contact method of user and should be one of email, sms or voice. Please note that adding mobile is not supported from API.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "method")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @method.setter
+    def method(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "method", value)
 
     @property
     @pulumi.getter
-    def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def to(self) -> Optional[pulumi.Input[str]]:
         """
-        Tags for the service, with a maximum of 20 tags per service.
+        to field is the address of given method.
         """
-        return pulumi.get(self, "tags")
+        return pulumi.get(self, "to")
 
-    @tags.setter
-    def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "tags", value)
+    @to.setter
+    def to(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "to", value)
 
     @property
-    @pulumi.getter(name="teamId")
-    def team_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def username(self) -> Optional[pulumi.Input[str]]:
         """
-        Team id of the service. This field must not be longer than 512 characters.
+        The username for contact.(reference)
         """
-        return pulumi.get(self, "team_id")
+        return pulumi.get(self, "username")
 
-    @team_id.setter
-    def team_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "team_id", value)
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
 
 
-class Service(pulumi.CustomResource):
+class UserContact(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 team_id: Optional[pulumi.Input[str]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 method: Optional[pulumi.Input[str]] = None,
+                 to: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manages a Service within Opsgenie.
+        Manages a User Contact.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        payment = opsgenie.Team("payment", description="This team deals with all the things")
-        this = opsgenie.Service("this", team_id="$opsgenie_team.payment.id")
+        sms = opsgenie.UserContact("sms",
+            username=exampleuser["username"],
+            to="39-123",
+            method="sms")
+        email = opsgenie.UserContact("email",
+            username=exampleuser["username"],
+            to="fahri@opsgenie.com",
+            method="email")
+        voice = opsgenie.UserContact("voice",
+            username=exampleuser["username"],
+            to="39-123",
+            method="voice")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        Teams can be imported using the `service_id`, e.g.
+        Users can be imported using the `username/contact_id`, e.g.
 
         ```sh
-        $ pulumi import opsgenie:index/service:Service this service_id`
+        $ pulumi import opsgenie:index/userContact:UserContact testcontact username/contact_id`
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: Description field of the service that is generally used to provide a detailed information about the service.
-        :param pulumi.Input[str] name: Name of the service. This field must not be longer than 100 characters.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags for the service, with a maximum of 20 tags per service.
-        :param pulumi.Input[str] team_id: Team id of the service. This field must not be longer than 512 characters.
+        :param pulumi.Input[bool] enabled: Enable contact of the user in OpsGenie. Default value is true.
+        :param pulumi.Input[str] method: This parameter is the contact method of user and should be one of email, sms or voice. Please note that adding mobile is not supported from API.
+        :param pulumi.Input[str] to: to field is the address of given method.
+        :param pulumi.Input[str] username: The username for contact.(reference)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ServiceArgs,
+                 args: UserContactArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manages a Service within Opsgenie.
+        Manages a User Contact.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        payment = opsgenie.Team("payment", description="This team deals with all the things")
-        this = opsgenie.Service("this", team_id="$opsgenie_team.payment.id")
+        sms = opsgenie.UserContact("sms",
+            username=exampleuser["username"],
+            to="39-123",
+            method="sms")
+        email = opsgenie.UserContact("email",
+            username=exampleuser["username"],
+            to="fahri@opsgenie.com",
+            method="email")
+        voice = opsgenie.UserContact("voice",
+            username=exampleuser["username"],
+            to="39-123",
+            method="voice")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        Teams can be imported using the `service_id`, e.g.
+        Users can be imported using the `username/contact_id`, e.g.
 
         ```sh
-        $ pulumi import opsgenie:index/service:Service this service_id`
+        $ pulumi import opsgenie:index/userContact:UserContact testcontact username/contact_id`
         ```
 
         :param str resource_name: The name of the resource.
-        :param ServiceArgs args: The arguments to use to populate this resource's properties.
+        :param UserContactArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserContactArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 team_id: Optional[pulumi.Input[str]] = None,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 method: Optional[pulumi.Input[str]] = None,
+                 to: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ServiceArgs.__new__(ServiceArgs)
+            __props__ = UserContactArgs.__new__(UserContactArgs)
 
-            __props__.__dict__["description"] = description
-            __props__.__dict__["name"] = name
-            __props__.__dict__["tags"] = tags
-            if team_id is None and not opts.urn:
-                raise TypeError("Missing required property 'team_id'")
-            __props__.__dict__["team_id"] = team_id
-        super(Service, __self__).__init__(
-            'opsgenie:index/service:Service',
+            __props__.__dict__["enabled"] = enabled
+            if method is None and not opts.urn:
+                raise TypeError("Missing required property 'method'")
+            __props__.__dict__["method"] = method
+            if to is None and not opts.urn:
+                raise TypeError("Missing required property 'to'")
+            __props__.__dict__["to"] = to
+            if username is None and not opts.urn:
+                raise TypeError("Missing required property 'username'")
+            __props__.__dict__["username"] = username
+        super(UserContact, __self__).__init__(
+            'opsgenie:index/userContact:UserContact',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            team_id: Optional[pulumi.Input[str]] = None) -> 'Service':
+            enabled: Optional[pulumi.Input[bool]] = None,
+            method: Optional[pulumi.Input[str]] = None,
+            to: Optional[pulumi.Input[str]] = None,
+            username: Optional[pulumi.Input[str]] = None) -> 'UserContact':
         """
-        Get an existing Service resource's state with the given name, id, and optional extra
+        Get an existing UserContact resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: Description field of the service that is generally used to provide a detailed information about the service.
-        :param pulumi.Input[str] name: Name of the service. This field must not be longer than 100 characters.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags for the service, with a maximum of 20 tags per service.
-        :param pulumi.Input[str] team_id: Team id of the service. This field must not be longer than 512 characters.
+        :param pulumi.Input[bool] enabled: Enable contact of the user in OpsGenie. Default value is true.
+        :param pulumi.Input[str] method: This parameter is the contact method of user and should be one of email, sms or voice. Please note that adding mobile is not supported from API.
+        :param pulumi.Input[str] to: to field is the address of given method.
+        :param pulumi.Input[str] username: The username for contact.(reference)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ServiceState.__new__(_ServiceState)
+        __props__ = _UserContactState.__new__(_UserContactState)
 
-        __props__.__dict__["description"] = description
-        __props__.__dict__["name"] = name
-        __props__.__dict__["tags"] = tags
-        __props__.__dict__["team_id"] = team_id
-        return Service(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["enabled"] = enabled
+        __props__.__dict__["method"] = method
+        __props__.__dict__["to"] = to
+        __props__.__dict__["username"] = username
+        return UserContact(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    def enabled(self) -> pulumi.Output[Optional[bool]]:
         """
-        Description field of the service that is generally used to provide a detailed information about the service.
+        Enable contact of the user in OpsGenie. Default value is true.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def method(self) -> pulumi.Output[str]:
         """
-        Name of the service. This field must not be longer than 100 characters.
+        This parameter is the contact method of user and should be one of email, sms or voice. Please note that adding mobile is not supported from API.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "method")
 
     @property
     @pulumi.getter
-    def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def to(self) -> pulumi.Output[str]:
         """
-        Tags for the service, with a maximum of 20 tags per service.
+        to field is the address of given method.
         """
-        return pulumi.get(self, "tags")
+        return pulumi.get(self, "to")
 
     @property
-    @pulumi.getter(name="teamId")
-    def team_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def username(self) -> pulumi.Output[str]:
         """
-        Team id of the service. This field must not be longer than 512 characters.
+        The username for contact.(reference)
         """
-        return pulumi.get(self, "team_id")
+        return pulumi.get(self, "username")
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/service_incident_rule.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/service_incident_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,17 +105,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_service = opsgenie.Service("testService", team_id=test_team.id)
-        test_service_incident_rule = opsgenie.ServiceIncidentRule("testServiceIncidentRule",
+        test = opsgenie.Team("test",
+            name="example-team",
+            description="This team deals with all the things")
+        test_service = opsgenie.Service("test",
+            name="example-service",
+            team_id=test.id)
+        test_service_incident_rule = opsgenie.ServiceIncidentRule("test",
             service_id=test_service.id,
             incident_rules=[opsgenie.ServiceIncidentRuleIncidentRuleArgs(
                 condition_match_type="match-any-condition",
                 conditions=[
                     opsgenie.ServiceIncidentRuleIncidentRuleConditionArgs(
                         field="message",
                         not_=False,
@@ -166,17 +170,21 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_service = opsgenie.Service("testService", team_id=test_team.id)
-        test_service_incident_rule = opsgenie.ServiceIncidentRule("testServiceIncidentRule",
+        test = opsgenie.Team("test",
+            name="example-team",
+            description="This team deals with all the things")
+        test_service = opsgenie.Service("test",
+            name="example-service",
+            team_id=test.id)
+        test_service_incident_rule = opsgenie.ServiceIncidentRule("test",
             service_id=test_service.id,
             incident_rules=[opsgenie.ServiceIncidentRuleIncidentRuleArgs(
                 condition_match_type="match-any-condition",
                 conditions=[
                     opsgenie.ServiceIncidentRuleIncidentRuleConditionArgs(
                         field="message",
                         not_=False,
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/team.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,37 +207,39 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         first = opsgenie.User("first",
+            username="user@domain.com",
             full_name="name ",
-            role="User",
-            username="user@domain.com")
+            role="User")
         second = opsgenie.User("second",
+            username="test@domain.com",
             full_name="name ",
-            role="User",
-            username="test@domain.com")
+            role="User")
         test = opsgenie.Team("test",
+            name="example",
             description="This team deals with all the things",
             members=[
                 opsgenie.TeamMemberArgs(
                     id=first.id,
                     role="admin",
                 ),
                 opsgenie.TeamMemberArgs(
                     id=second.id,
                     role="user",
                 ),
             ])
         self_service = opsgenie.Team("self-service",
-            delete_default_resources=True,
+            name="Self Service",
             description="Membership in this team is managed via OpsGenie web UI only",
-            ignore_members=True)
+            ignore_members=True,
+            delete_default_resources=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Teams can be imported using the `team_id`, e.g.
 
@@ -266,37 +268,39 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         first = opsgenie.User("first",
+            username="user@domain.com",
             full_name="name ",
-            role="User",
-            username="user@domain.com")
+            role="User")
         second = opsgenie.User("second",
+            username="test@domain.com",
             full_name="name ",
-            role="User",
-            username="test@domain.com")
+            role="User")
         test = opsgenie.Team("test",
+            name="example",
             description="This team deals with all the things",
             members=[
                 opsgenie.TeamMemberArgs(
                     id=first.id,
                     role="admin",
                 ),
                 opsgenie.TeamMemberArgs(
                     id=second.id,
                     role="user",
                 ),
             ])
         self_service = opsgenie.Team("self-service",
-            delete_default_resources=True,
+            name="Self Service",
             description="Membership in this team is managed via OpsGenie web UI only",
-            ignore_members=True)
+            ignore_members=True,
+            delete_default_resources=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Teams can be imported using the `team_id`, e.g.
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/team_routing_rule.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/team_routing_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,47 +303,51 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_schedule = opsgenie.Schedule("testSchedule",
+        test = opsgenie.Schedule("test",
+            name="genieschedule",
             description="schedule test",
-            enabled=False,
-            timezone="Europe/Rome")
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_team_routing_rule = opsgenie.TeamRoutingRule("testTeamRoutingRule",
+            timezone="Europe/Rome",
+            enabled=False)
+        test_team = opsgenie.Team("test",
+            name="example team",
+            description="This team deals with all the things")
+        test_team_routing_rule = opsgenie.TeamRoutingRule("test",
+            name="routing rule example",
+            team_id=test_team.id,
+            order=0,
+            timezone="America/Los_Angeles",
             criterias=[opsgenie.TeamRoutingRuleCriteriaArgs(
+                type="match-any-condition",
                 conditions=[opsgenie.TeamRoutingRuleCriteriaConditionArgs(
-                    expected_value="expected1",
                     field="message",
-                    not_=False,
                     operation="contains",
+                    expected_value="expected1",
+                    not_=False,
                 )],
-                type="match-any-condition",
-            )],
-            notifies=[opsgenie.TeamRoutingRuleNotifyArgs(
-                name=test_schedule.name,
-                type="schedule",
             )],
-            order=0,
-            team_id=test_team.id,
             time_restrictions=[opsgenie.TeamRoutingRuleTimeRestrictionArgs(
+                type="weekday-and-time-of-day",
                 restriction_list=[opsgenie.TeamRoutingRuleTimeRestrictionRestrictionListArgs(
-                    end_day="tuesday",
-                    end_hour=18,
-                    end_min=30,
                     start_day="monday",
                     start_hour=8,
                     start_min=0,
+                    end_day="tuesday",
+                    end_hour=18,
+                    end_min=30,
                 )],
-                type="weekday-and-time-of-day",
             )],
-            timezone="America/Los_Angeles")
+            notifies=[opsgenie.TeamRoutingRuleNotifyArgs(
+                name=test.name,
+                type="schedule",
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Team Routing Rules can be imported using the `team_id/routing_rule_id`, e.g.
 
@@ -374,47 +378,51 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
-        test_schedule = opsgenie.Schedule("testSchedule",
+        test = opsgenie.Schedule("test",
+            name="genieschedule",
             description="schedule test",
-            enabled=False,
-            timezone="Europe/Rome")
-        test_team = opsgenie.Team("testTeam", description="This team deals with all the things")
-        test_team_routing_rule = opsgenie.TeamRoutingRule("testTeamRoutingRule",
+            timezone="Europe/Rome",
+            enabled=False)
+        test_team = opsgenie.Team("test",
+            name="example team",
+            description="This team deals with all the things")
+        test_team_routing_rule = opsgenie.TeamRoutingRule("test",
+            name="routing rule example",
+            team_id=test_team.id,
+            order=0,
+            timezone="America/Los_Angeles",
             criterias=[opsgenie.TeamRoutingRuleCriteriaArgs(
+                type="match-any-condition",
                 conditions=[opsgenie.TeamRoutingRuleCriteriaConditionArgs(
-                    expected_value="expected1",
                     field="message",
-                    not_=False,
                     operation="contains",
+                    expected_value="expected1",
+                    not_=False,
                 )],
-                type="match-any-condition",
-            )],
-            notifies=[opsgenie.TeamRoutingRuleNotifyArgs(
-                name=test_schedule.name,
-                type="schedule",
             )],
-            order=0,
-            team_id=test_team.id,
             time_restrictions=[opsgenie.TeamRoutingRuleTimeRestrictionArgs(
+                type="weekday-and-time-of-day",
                 restriction_list=[opsgenie.TeamRoutingRuleTimeRestrictionRestrictionListArgs(
-                    end_day="tuesday",
-                    end_hour=18,
-                    end_min=30,
                     start_day="monday",
                     start_hour=8,
                     start_min=0,
+                    end_day="tuesday",
+                    end_hour=18,
+                    end_min=30,
                 )],
-                type="weekday-and-time-of-day",
             )],
-            timezone="America/Los_Angeles")
+            notifies=[opsgenie.TeamRoutingRuleNotifyArgs(
+                name=test.name,
+                type="schedule",
+            )])
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Team Routing Rules can be imported using the `team_id/routing_rule_id`, e.g.
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie/user.py` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,35 +336,35 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.User("test",
+            username="user@domain.com",
             full_name="Test User",
-            locale="en_US",
             role="User",
-            skype_username="skypename",
+            locale="en_US",
+            timezone="America/New_York",
             tags=[
                 "sre",
                 "opsgenie",
             ],
-            timezone="America/New_York",
+            skype_username="skypename",
             user_addresses=[opsgenie.UserUserAddressArgs(
-                city="City",
                 country="Country",
-                line="Line",
                 state="State",
+                city="City",
+                line="Line",
                 zipcode="998877",
             )],
             user_details={
                 "key1": "val1,val2",
                 "key2": "val3,val4",
-            },
-            username="user@domain.com")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the `user_id`, e.g.
 
@@ -397,35 +397,35 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.User("test",
+            username="user@domain.com",
             full_name="Test User",
-            locale="en_US",
             role="User",
-            skype_username="skypename",
+            locale="en_US",
+            timezone="America/New_York",
             tags=[
                 "sre",
                 "opsgenie",
             ],
-            timezone="America/New_York",
+            skype_username="skypename",
             user_addresses=[opsgenie.UserUserAddressArgs(
-                city="City",
                 country="Country",
-                line="Line",
                 state="State",
+                city="City",
+                line="Line",
                 zipcode="998877",
             )],
             user_details={
                 "key1": "val1,val2",
                 "key2": "val3,val4",
-            },
-            username="user@domain.com")
+            })
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the `user_id`, e.g.
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie.egg-info/PKG-INFO` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.4.0a1713336015
+Version: 1.4.0a1713561317
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi,opsgenie
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pulumi_opsgenie.egg-info/SOURCES.txt` & `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713336015/pyproject.toml` & `pulumi_opsgenie-1.4.0a1713561317/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_opsgenie"
   description = "A Pulumi package for creating and managing opsgenie cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "opsgenie"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.4.0a1713336015"
+  version = "1.4.0a1713561317"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-opsgenie"
 
 [build-system]
```

