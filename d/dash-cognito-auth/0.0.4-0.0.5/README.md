# Comparing `tmp/dash-cognito-auth-0.0.4.tar.gz` & `tmp/dash_cognito_auth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-cognito-auth-0.0.4.tar", last modified: Wed Apr  3 14:52:27 2024, max compression
+gzip compressed data, was "dash_cognito_auth-0.0.5.tar", last modified: Fri Apr 19 13:28:50 2024, max compression
```

## Comparing `dash-cognito-auth-0.0.4.tar` & `dash_cognito_auth-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.550729 dash-cognito-auth-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.554729 dash-cognito-auth-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1792 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.554729 dash-cognito-auth-0.0.4/dash_cognito_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/dash_cognito_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/dash_cognito_auth/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/dash_cognito_auth/cognito.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/dash_cognito_auth/cognito_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 14:52:27.000000 dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/example/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/example/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/example/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/example/aws_resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27275 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/example/image.png
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1120 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.558729 dash-cognito-auth-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/test_auth_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/test_end_to_end_with_path_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 14:52:22.000000 dash-cognito-auth-0.0.4/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:28:50.389073 dash_cognito_auth-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:28:50.381073 dash_cognito_auth-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:28:50.385073 dash_cognito_auth-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-19 13:28:50.389073 dash_cognito_auth-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1792 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:28:50.385073 dash_cognito_auth-0.0.5/dash_cognito_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/dash_cognito_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/dash_cognito_auth/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/dash_cognito_auth/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/dash_cognito_auth/cognito_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:28:50.389073 dash_cognito_auth-0.0.5/dash_cognito_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-19 13:28:50.000000 dash_cognito_auth-0.0.5/dash_cognito_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-19 13:28:50.000000 dash_cognito_auth-0.0.5/dash_cognito_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:28:50.000000 dash_cognito_auth-0.0.5/dash_cognito_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:28:50.000000 dash_cognito_auth-0.0.5/dash_cognito_auth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-19 13:28:50.000000 dash_cognito_auth-0.0.5/dash_cognito_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 13:28:50.000000 dash_cognito_auth-0.0.5/dash_cognito_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:28:50.385073 dash_cognito_auth-0.0.5/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/example/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/example/aws_resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27275 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/example/image.png
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 13:28:50.389073 dash_cognito_auth-0.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1120 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:28:50.385073 dash_cognito_auth-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/tests/test_auth_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/tests/test_end_to_end_with_path_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-19 13:28:45.000000 dash_cognito_auth-0.0.5/tests/test_import.py
```

### Comparing `dash-cognito-auth-0.0.4/.github/workflows/build.yml` & `dash_cognito_auth-0.0.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/.github/workflows/python-publish.yml` & `dash_cognito_auth-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/.gitignore` & `dash_cognito_auth-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/LICENSE.md` & `dash_cognito_auth-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/PKG-INFO` & `dash_cognito_auth-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-cognito-auth
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dash Cognito Auth
 Home-page: https://github.com/fspijkerman/dash-cognito-auth
 Author: Frank Spijkerman
 Author-email: frank@jeito.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -28,14 +28,20 @@
 
 This Library uses [Flask Dance](https://github.com/singingwolfboy/flask-dance)
 and a modified version of Plotly's own [dash auth](https://github.com/plotly/dash-auth)
 for authentication.
 
 This Library is heavily inspired by [dash-google-oauth](https://github.com/lchapo/dash-google-auth) created by Lucas Chapin
 
+## Installation
+
+```bash
+$ pip install dash-cognito-auth
+```
+
 ## Basic Use
 
 Authentication can be added to your Dash application using the `CognitoOAuth`
 class, i.e.
 
 ```python
 from dash import Dash
```

### Comparing `dash-cognito-auth-0.0.4/README.md` & `dash_cognito_auth-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 
 This Library uses [Flask Dance](https://github.com/singingwolfboy/flask-dance)
 and a modified version of Plotly's own [dash auth](https://github.com/plotly/dash-auth)
 for authentication.
 
 This Library is heavily inspired by [dash-google-oauth](https://github.com/lchapo/dash-google-auth) created by Lucas Chapin
 
+## Installation
+
+```bash
+$ pip install dash-cognito-auth
+```
+
 ## Basic Use
 
 Authentication can be added to your Dash application using the `CognitoOAuth`
 class, i.e.
 
 ```python
 from dash import Dash
```

### Comparing `dash-cognito-auth-0.0.4/app.py` & `dash_cognito_auth-0.0.5/app.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/dash_cognito_auth/auth.py` & `dash_cognito_auth-0.0.5/dash_cognito_auth/auth.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/dash_cognito_auth/cognito.py` & `dash_cognito_auth-0.0.5/dash_cognito_auth/cognito.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/dash_cognito_auth/cognito_oauth.py` & `dash_cognito_auth-0.0.5/dash_cognito_auth/cognito_oauth.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     def __init__(
         self,
         app: Dash,
         domain: str,
         region=None,
         additional_scopes=None,
         logout_url: str = None,
+        user_info_to_session_attr_mapping: dict[str, str] = None,
     ):
         """
         Wrap a Dash App with Cognito authentication.
 
         The app needs two configuration options to work:
 
         COGNITO_OAUTH_CLIENT_ID -> Client-ID of the Cognito App Client
@@ -56,17 +57,32 @@
             By default openid, email, and profile are requested - default value: None
         logout_url : str, optional
             Add a URL to the app that logs out the user when accessed via HTTP GET.
             The URL automatically respects path prefixes, i.e. if your app is hosted
             at example.com/some/prefix and you set logout_url to "logout", the actual
             URL will be example.com/some/prefix/logout. By default, no logout URL is
             added and you will have to create your own.
+        user_info_to_session_attr_mapping : dict[str, str], optional
+            Determines which information from the Cognito user info endpoint will be
+            placed into the session, by default the "email" attribute will be added
+            as "email" into the session. If you overwrite this with the following:
+
+                {"sub": "user_id", "email": "email", "username": "username"}
+
+            it will take the subscriber-ID (sub) and add it as user_id to the session
+            and additionally add the email and username.
         """
         super().__init__(app)
 
+        self.user_info_to_session_attr_mapping = (
+            {"email": "email"}
+            if user_info_to_session_attr_mapping is None
+            else user_info_to_session_attr_mapping
+        )
+
         dash_base_path = app.get_relative_path("")
 
         cognito_bp = make_cognito_blueprint(
             domain=domain,
             region=region,
             redirect_url=dash_base_path,
             scope=[
@@ -112,15 +128,20 @@
             # send to cognito login
             return False
 
         try:
             resp = cognito.get("/oauth2/userInfo")
             assert resp.ok, resp.text
 
-            session["email"] = resp.json().get("email")
+            for (
+                user_info_attr,
+                session_attr,
+            ) in self.user_info_to_session_attr_mapping.items():
+                session[session_attr] = resp.json()[user_info_attr]
+
             return True
         except (InvalidGrantError, TokenExpiredError):
             return self.login_request()
 
     def login_request(self):
         # send to cognito auth page
         return redirect(url_for("cognito.login"))
```

### Comparing `dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/PKG-INFO` & `dash_cognito_auth-0.0.5/dash_cognito_auth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-cognito-auth
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dash Cognito Auth
 Home-page: https://github.com/fspijkerman/dash-cognito-auth
 Author: Frank Spijkerman
 Author-email: frank@jeito.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -28,14 +28,20 @@
 
 This Library uses [Flask Dance](https://github.com/singingwolfboy/flask-dance)
 and a modified version of Plotly's own [dash auth](https://github.com/plotly/dash-auth)
 for authentication.
 
 This Library is heavily inspired by [dash-google-oauth](https://github.com/lchapo/dash-google-auth) created by Lucas Chapin
 
+## Installation
+
+```bash
+$ pip install dash-cognito-auth
+```
+
 ## Basic Use
 
 Authentication can be added to your Dash application using the `CognitoOAuth`
 class, i.e.
 
 ```python
 from dash import Dash
```

### Comparing `dash-cognito-auth-0.0.4/dash_cognito_auth.egg-info/SOURCES.txt` & `dash_cognito_auth-0.0.5/dash_cognito_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/example/README.md` & `dash_cognito_auth-0.0.5/example/README.md`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/example/app.py` & `dash_cognito_auth-0.0.5/example/app.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/example/aws_resources.yaml` & `dash_cognito_auth-0.0.5/example/aws_resources.yaml`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/example/image.png` & `dash_cognito_auth-0.0.5/example/image.png`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/setup.py` & `dash_cognito_auth-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/tests/conftest.py` & `dash_cognito_auth-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/tests/test_auth_flows.py` & `dash_cognito_auth-0.0.5/tests/test_auth_flows.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/tests/test_end_to_end.py` & `dash_cognito_auth-0.0.5/tests/test_end_to_end.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,25 +42,27 @@
     dash_app.server.secret_key = "just_a_test"
 
     auth = CognitoOAuth(
         dash_app,
         domain=os.environ["COGNITO_DOMAIN"],
         region=os.environ["COGNITO_REGION"],
         logout_url="logout",
+        user_info_to_session_attr_mapping={"email": "email", "sub": "user_id"},
     )
     auth.app.server.config["COGNITO_OAUTH_CLIENT_ID"] = os.environ[
         "COGNITO_OAUTH_CLIENT_ID"
     ]
     auth.app.server.config["COGNITO_OAUTH_CLIENT_SECRET"] = os.environ[
         "COGNITO_OAUTH_CLIENT_SECRET"
     ]
 
     @dash_app.server.route("/session-info")
     def session_info():
-        return {"email": session["email"]}
+        session_attributes = {"email", "user_id"}
+        return {attr: session[attr] for attr in session_attributes}
 
     return auth
 
 
 def test_end_to_end(end_to_end_app: CognitoOAuth):
     """
     - Request the local webapp
@@ -120,14 +122,15 @@
     # We should now be redirected to the home page which will be displayed
     home_page_with_auth = client.get(post_cognito_auth_redirect.location)
     assert home_page_with_auth.status_code == HTTPStatus.OK
 
     # Verify that the logged in users' email matches the one from the env
     session_info_response = client.get("/session-info")
     assert session_info_response.json["email"] == os.environ["COGNITO_EMAIL"]
+    assert "user_id" in session_info_response.json
 
     # Log out
     logout_response = client.get("/logout")
     assert logout_response.status_code == HTTPStatus.FOUND
     assert "/logout" in logout_response.location
 
     # Since we're not longer logged in, we should be redirected to the local
```

### Comparing `dash-cognito-auth-0.0.4/tests/test_end_to_end_with_path_prefix.py` & `dash_cognito_auth-0.0.5/tests/test_end_to_end_with_path_prefix.py`

 * *Files identical despite different names*

### Comparing `dash-cognito-auth-0.0.4/tests/test_import.py` & `dash_cognito_auth-0.0.5/tests/test_import.py`

 * *Files identical despite different names*

