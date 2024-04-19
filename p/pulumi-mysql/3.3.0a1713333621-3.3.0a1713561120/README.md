# Comparing `tmp/pulumi_mysql-3.3.0a1713333621.tar.gz` & `tmp/pulumi_mysql-3.3.0a1713561120.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mysql-3.3.0a1713333621.tar", last modified: Wed Apr 17 06:14:06 2024, max compression
+gzip compressed data, was "pulumi_mysql-3.3.0a1713561120.tar", last modified: Fri Apr 19 21:18:17 2024, max compression
```

## Comparing `pulumi_mysql-3.3.0a1713333621.tar` & `pulumi_mysql-3.3.0a1713561120.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:14:06.590693 pulumi_mysql-3.3.0a1713333621/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-17 06:14:06.590693 pulumi_mysql-3.3.0a1713333621/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:14:06.586693 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:14:06.590693 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    17580 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    27364 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/grant.py
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    23843 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql/user_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:14:06.590693 pulumi_mysql-3.3.0a1713333621/pulumi_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-17 06:14:06.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-17 06:14:06.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:14:06.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 06:14:06.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 06:14:06.000000 pulumi_mysql-3.3.0a1713333621/pulumi_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-17 06:14:00.000000 pulumi_mysql-3.3.0a1713333621/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:14:06.590693 pulumi_mysql-3.3.0a1713333621/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27312 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23843 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/user_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/setup.cfg
```

### Comparing `pulumi_mysql-3.3.0a1713333621/PKG-INFO` & `pulumi_mysql-3.3.0a1713561120/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mysql
-Version: 3.3.0a1713333621
+Version: 3.3.0a1713561120
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi,mysql
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.3.0a1713333621/README.md` & `pulumi_mysql-3.3.0a1713561120/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/__init__.py` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/_utilities.py` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/config/__init__.pyi` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/config/vars.py` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/database.py` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        app = mysql.Database("app")
+        app = mysql.Database("app", name="my_awesome_app")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Databases can be imported using their name, e.g.
 
@@ -244,15 +244,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        app = mysql.Database("app")
+        app = mysql.Database("app", name="my_awesome_app")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         Databases can be imported using their name, e.g.
```

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/grant.py` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/grant.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,64 +338,64 @@
         ### Granting Privileges to a User
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        jdoe_user = mysql.User("jdoeUser",
+        jdoe = mysql.User("jdoe",
+            user="jdoe",
             host="example.com",
-            plaintext_password="password",
-            user="jdoe")
-        jdoe_grant = mysql.Grant("jdoeGrant",
+            plaintext_password="password")
+        jdoe_grant = mysql.Grant("jdoe",
+            user=jdoe.user,
+            host=jdoe.host,
             database="app",
-            host=jdoe_user.host,
             privileges=[
                 "SELECT",
                 "UPDATE",
-            ],
-            user=jdoe_user.user)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Granting Privileges to a Role
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        developer_role = mysql.Role("developerRole")
-        developer_grant = mysql.Grant("developerGrant",
+        developer = mysql.Role("developer", name="developer")
+        developer_grant = mysql.Grant("developer",
+            role=developer.name,
             database="app",
             privileges=[
                 "SELECT",
                 "UPDATE",
-            ],
-            role=developer_role.name)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Adding a Role to a User
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
+            user="jdoe",
             host="example.com",
-            plaintext_password="password",
-            user="jdoe")
-        developer_role = mysql.Role("developerRole")
-        developer_grant = mysql.Grant("developerGrant",
-            database="app",
+            plaintext_password="password")
+        developer = mysql.Role("developer", name="developer")
+        developer_grant = mysql.Grant("developer",
+            user=jdoe.user,
             host=jdoe.host,
-            roles=[developer_role.name],
-            user=jdoe.user)
+            database="app",
+            roles=[developer.name])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] database: The database to grant privileges on.
         :param pulumi.Input[bool] grant: Whether to also give the user privileges to grant the same privileges to other users.
@@ -422,64 +422,64 @@
         ### Granting Privileges to a User
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        jdoe_user = mysql.User("jdoeUser",
+        jdoe = mysql.User("jdoe",
+            user="jdoe",
             host="example.com",
-            plaintext_password="password",
-            user="jdoe")
-        jdoe_grant = mysql.Grant("jdoeGrant",
+            plaintext_password="password")
+        jdoe_grant = mysql.Grant("jdoe",
+            user=jdoe.user,
+            host=jdoe.host,
             database="app",
-            host=jdoe_user.host,
             privileges=[
                 "SELECT",
                 "UPDATE",
-            ],
-            user=jdoe_user.user)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Granting Privileges to a Role
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        developer_role = mysql.Role("developerRole")
-        developer_grant = mysql.Grant("developerGrant",
+        developer = mysql.Role("developer", name="developer")
+        developer_grant = mysql.Grant("developer",
+            role=developer.name,
             database="app",
             privileges=[
                 "SELECT",
                 "UPDATE",
-            ],
-            role=developer_role.name)
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         ### Adding a Role to a User
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
+            user="jdoe",
             host="example.com",
-            plaintext_password="password",
-            user="jdoe")
-        developer_role = mysql.Role("developerRole")
-        developer_grant = mysql.Grant("developerGrant",
-            database="app",
+            plaintext_password="password")
+        developer = mysql.Role("developer", name="developer")
+        developer_grant = mysql.Grant("developer",
+            user=jdoe.user,
             host=jdoe.host,
-            roles=[developer_role.name],
-            user=jdoe.user)
+            database="app",
+            roles=[developer.name])
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param GrantArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/provider.py` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/role.py` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        developer = mysql.Role("developer")
+        developer = mysql.Role("developer", name="developer")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of the role.
         """
@@ -102,15 +102,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        developer = mysql.Role("developer")
+        developer = mysql.Role("developer", name="developer")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param RoleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/user.py` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,31 +260,31 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
+            user="jdoe",
             host="example.com",
-            plaintext_password="password",
-            user="jdoe")
+            plaintext_password="password")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage with an Authentication Plugin
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         nologin = mysql.User("nologin",
-            auth_plugin="mysql_no_login",
+            user="nologin",
             host="example.com",
-            user="nologin")
+            auth_plugin="mysql_no_login")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] auth_plugin: Use an [authentication plugin][ref-auth-plugins] to authenticate the user instead of using password authentication.  Description of the fields allowed in the block below. Conflicts with `password` and `plaintext_password`.
         :param pulumi.Input[str] host: The source host of the user. Defaults to "localhost".
@@ -311,31 +311,31 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
+            user="jdoe",
             host="example.com",
-            plaintext_password="password",
-            user="jdoe")
+            plaintext_password="password")
         ```
         <!--End PulumiCodeChooser -->
 
         ### Example Usage with an Authentication Plugin
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         nologin = mysql.User("nologin",
-            auth_plugin="mysql_no_login",
+            user="nologin",
             host="example.com",
-            user="nologin")
+            auth_plugin="mysql_no_login")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql/user_password.py` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/user_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,18 +176,18 @@
         ## Example Usage
 
          <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        jdoe_user = mysql.User("jdoeUser", user="jdoe")
-        jdoe_user_password = mysql.UserPassword("jdoeUserPassword",
-            pgp_key="keybase:joestump",
-            user=jdoe_user.user)
+        jdoe = mysql.User("jdoe", user="jdoe")
+        jdoe_user_password = mysql.UserPassword("jdoe",
+            user=jdoe.user,
+            pgp_key="keybase:joestump")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] host: The source host of the user. Defaults to `localhost`.
         :param pulumi.Input[str] pgp_key: Either a base-64 encoded PGP public key, or a keybase username in the form `keybase:some_person_that_exists`.
@@ -213,18 +213,18 @@
         ## Example Usage
 
          <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
-        jdoe_user = mysql.User("jdoeUser", user="jdoe")
-        jdoe_user_password = mysql.UserPassword("jdoeUserPassword",
-            pgp_key="keybase:joestump",
-            user=jdoe_user.user)
+        jdoe = mysql.User("jdoe", user="jdoe")
+        jdoe_user_password = mysql.UserPassword("jdoe",
+            user=jdoe.user,
+            pgp_key="keybase:joestump")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param UserPasswordArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
```

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql.egg-info/PKG-INFO` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mysql
-Version: 3.3.0a1713333621
+Version: 3.3.0a1713561120
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi,mysql
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.3.0a1713333621/pulumi_mysql.egg-info/SOURCES.txt` & `pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713333621/pyproject.toml` & `pulumi_mysql-3.3.0a1713561120/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_mysql"
   description = "A Pulumi package for creating and managing mysql cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0a1,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "mysql"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.3.0a1713333621"
+  version = "3.3.0a1713561120"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-mysql"
 
 [build-system]
```

