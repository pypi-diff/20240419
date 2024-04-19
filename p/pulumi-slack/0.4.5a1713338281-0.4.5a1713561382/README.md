# Comparing `tmp/pulumi_slack-0.4.5a1713338281.tar.gz` & `tmp/pulumi_slack-0.4.5a1713561382.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_slack-0.4.5a1713338281.tar", last modified: Wed Apr 17 07:40:32 2024, max compression
+gzip compressed data, was "pulumi_slack-0.4.5a1713561382.tar", last modified: Fri Apr 19 21:24:32 2024, max compression
```

## Comparing `pulumi_slack-0.4.5a1713338281.tar` & `pulumi_slack-0.4.5a1713561382.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:40:32.140221 pulumi_slack-0.4.5a1713338281/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-17 07:40:32.140221 pulumi_slack-0.4.5a1713338281/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:40:32.140221 pulumi_slack-0.4.5a1713338281/pulumi_slack/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:40:32.140221 pulumi_slack-0.4.5a1713338281/pulumi_slack/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    39532 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/get_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/get_usergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18298 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack/usergroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:40:32.140221 pulumi_slack-0.4.5a1713338281/pulumi_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-17 07:40:32.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-17 07:40:32.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:40:32.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 07:40:32.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 07:40:32.000000 pulumi_slack-0.4.5a1713338281/pulumi_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-17 07:40:25.000000 pulumi_slack-0.4.5a1713338281/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:40:32.140221 pulumi_slack-0.4.5a1713338281/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:24:32.228590 pulumi_slack-0.4.5a1713561382/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-19 21:24:32.228590 pulumi_slack-0.4.5a1713561382/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:24:32.228590 pulumi_slack-0.4.5a1713561382/pulumi_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:24:32.228590 pulumi_slack-0.4.5a1713561382/pulumi_slack/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39726 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/get_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/get_usergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack/usergroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:24:32.228590 pulumi_slack-0.4.5a1713561382/pulumi_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-19 21:24:32.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-19 21:24:32.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:24:32.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:24:32.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 21:24:32.000000 pulumi_slack-0.4.5a1713561382/pulumi_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-19 21:24:26.000000 pulumi_slack-0.4.5a1713561382/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:24:32.228590 pulumi_slack-0.4.5a1713561382/setup.cfg
```

### Comparing `pulumi_slack-0.4.5a1713338281/PKG-INFO` & `pulumi_slack-0.4.5a1713561382/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.5a1713338281
+Version: 0.4.5a1713561382
 Summary: A Pulumi package for managing Slack workspaces.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi,slack,category/utility
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_slack-0.4.5a1713338281/README.md` & `pulumi_slack-0.4.5a1713561382/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack/__init__.py` & `pulumi_slack-0.4.5a1713561382/pulumi_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack/_utilities.py` & `pulumi_slack-0.4.5a1713561382/pulumi_slack/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack/config/vars.py` & `pulumi_slack-0.4.5a1713561382/pulumi_slack/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack/conversation.py` & `pulumi_slack-0.4.5a1713561382/pulumi_slack/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,43 +499,46 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         test = slack.Conversation("test",
-            is_private=True,
+            name="my-channel",
+            topic="The topic for my channel",
             permanent_members=[],
-            topic="The topic for my channel")
+            is_private=True)
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         nonadmin = slack.Conversation("nonadmin",
-            action_on_destroy="none",
-            is_private=True,
+            name="my-channel01",
+            topic="The channel won't be archived on destroy",
             permanent_members=[],
-            topic="The channel won't be archived on destroy")
+            is_private=True,
+            action_on_destroy="none")
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         adopted = slack.Conversation("adopted",
-            action_on_update_permanent_members="none",
-            adopt_existing_channel=True,
+            name="my-channel02",
+            topic="Adopt existing, don't kick members",
             permanent_members=[],
-            topic="Adopt existing, don't kick members")
+            adopt_existing_channel=True,
+            action_on_update_permanent_members="none")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         `slack_conversation` can be imported using the ID of the conversation/channel, e.g.
 
@@ -615,43 +618,46 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         test = slack.Conversation("test",
-            is_private=True,
+            name="my-channel",
+            topic="The topic for my channel",
             permanent_members=[],
-            topic="The topic for my channel")
+            is_private=True)
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         nonadmin = slack.Conversation("nonadmin",
-            action_on_destroy="none",
-            is_private=True,
+            name="my-channel01",
+            topic="The channel won't be archived on destroy",
             permanent_members=[],
-            topic="The channel won't be archived on destroy")
+            is_private=True,
+            action_on_destroy="none")
         ```
         <!--End PulumiCodeChooser -->
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         adopted = slack.Conversation("adopted",
-            action_on_update_permanent_members="none",
-            adopt_existing_channel=True,
+            name="my-channel02",
+            topic="Adopt existing, don't kick members",
             permanent_members=[],
-            topic="Adopt existing, don't kick members")
+            adopt_existing_channel=True,
+            action_on_update_permanent_members="none")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         `slack_conversation` can be imported using the ID of the conversation/channel, e.g.
```

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack/get_conversation.py` & `pulumi_slack-0.4.5a1713561382/pulumi_slack/get_conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack/get_user.py` & `pulumi_slack-0.4.5a1713561382/pulumi_slack/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack/get_usergroup.py` & `pulumi_slack-0.4.5a1713561382/pulumi_slack/get_usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack/provider.py` & `pulumi_slack-0.4.5a1713561382/pulumi_slack/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack/usergroup.py` & `pulumi_slack-0.4.5a1713561382/pulumi_slack/usergroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,36 +231,39 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
-        my_group = slack.Usergroup("myGroup",
-            channels=["CHANNEL00"],
-            description="Test user group",
+        my_group = slack.Usergroup("my_group",
+            name="TestGroup",
             handle="test",
-            users=["USER00"])
+            description="Test user group",
+            users=["USER00"],
+            channels=["CHANNEL00"])
         ```
         <!--End PulumiCodeChooser -->
 
         Note that if a channel is removed from the `channels` list users are
         **not** removed from the channel. In order to keep the users in the
         groups and in the channel in sync set `permanent_users` in the channel:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
-        my_group = slack.Usergroup("myGroup",
+        my_group = slack.Usergroup("my_group",
+            name="TestGroup",
             handle="test",
             description="Test user group",
             users=["USER00"])
         test = slack.Conversation("test",
+            name="my-channel",
             topic="The topic for my channel",
             permanent_members=my_group.users,
             is_private=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
@@ -312,36 +315,39 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
-        my_group = slack.Usergroup("myGroup",
-            channels=["CHANNEL00"],
-            description="Test user group",
+        my_group = slack.Usergroup("my_group",
+            name="TestGroup",
             handle="test",
-            users=["USER00"])
+            description="Test user group",
+            users=["USER00"],
+            channels=["CHANNEL00"])
         ```
         <!--End PulumiCodeChooser -->
 
         Note that if a channel is removed from the `channels` list users are
         **not** removed from the channel. In order to keep the users in the
         groups and in the channel in sync set `permanent_users` in the channel:
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
-        my_group = slack.Usergroup("myGroup",
+        my_group = slack.Usergroup("my_group",
+            name="TestGroup",
             handle="test",
             description="Test user group",
             users=["USER00"])
         test = slack.Conversation("test",
+            name="my-channel",
             topic="The topic for my channel",
             permanent_members=my_group.users,
             is_private=True)
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
```

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack.egg-info/PKG-INFO` & `pulumi_slack-0.4.5a1713561382/pulumi_slack.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.5a1713338281
+Version: 0.4.5a1713561382
 Summary: A Pulumi package for managing Slack workspaces.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi,slack,category/utility
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_slack-0.4.5a1713338281/pulumi_slack.egg-info/SOURCES.txt` & `pulumi_slack-0.4.5a1713561382/pulumi_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713338281/pyproject.toml` & `pulumi_slack-0.4.5a1713561382/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_slack"
   description = "A Pulumi package for managing Slack workspaces."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "slack", "category/utility"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.4.5a1713338281"
+  version = "0.4.5a1713561382"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-slack"
 
 [build-system]
```

