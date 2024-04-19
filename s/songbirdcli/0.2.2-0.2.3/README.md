# Comparing `tmp/songbirdcli-0.2.2.tar.gz` & `tmp/songbirdcli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songbirdcli-0.2.2.tar", last modified: Thu Apr 18 19:38:34 2024, max compression
+gzip compressed data, was "songbirdcli-0.2.3.tar", last modified: Thu Apr 18 22:47:25 2024, max compression
```

## Comparing `songbirdcli-0.2.2.tar` & `songbirdcli-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.875332 songbirdcli-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.867333 songbirdcli-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-18 19:38:34.875332 songbirdcli-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/docs/songbirdcli/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/docs/songbirdcli/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/docs/songbirdcli/helpers.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/docs/songbirdcli/settings.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:38:34.875332 songbirdcli-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/songbirdcli/
--rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/requirements.txt.blank
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.875332 songbirdcli-0.2.2/songbirdcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.867333 songbirdcli-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/tests/unit/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.661662 songbirdcli-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.665663 songbirdcli-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.665663 songbirdcli-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.665663 songbirdcli-0.2.3/docs/songbirdcli/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/docs/songbirdcli/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/docs/songbirdcli/helpers.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/docs/songbirdcli/settings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/songbirdcli/
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/requirements.txt.blank
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/songbirdcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.665663 songbirdcli-0.2.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/tests/unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/tests/unit/test_helpers.py
```

### Comparing `songbirdcli-0.2.2/.github/workflows/docker.yml` & `songbirdcli-0.2.3/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/.github/workflows/pages.yaml` & `songbirdcli-0.2.3/.github/workflows/pages.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/.github/workflows/pypi-publish.yaml` & `songbirdcli-0.2.3/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/.github/workflows/tests.yaml` & `songbirdcli-0.2.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/Dockerfile` & `songbirdcli-0.2.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/LICENSE` & `songbirdcli-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/Makefile` & `songbirdcli-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/PKG-INFO` & `songbirdcli-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcli
-Version: 0.2.2
+Version: 0.2.3
 Summary: Songbird's cli.
 Author: Christian Boin
 Project-URL: Documentation, https://cboin1996.github.io/songbird/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
```

### Comparing `songbirdcli-0.2.2/README.md` & `songbirdcli-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/mkdocs.yml` & `songbirdcli-0.2.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/pyproject.toml` & `songbirdcli-0.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "songbirdcli"
 authors = [
     {name = "Christian Boin"},
 ]
-version = "0.2.2"
+version = "0.2.3"
 description = "Songbird's cli."
 readme = "README.md"
 requires-python = ">=3.11"
 dynamic = ["dependencies"]
 
 [project.urls]
 Documentation = "https://cboin1996.github.io/songbird/"
```

### Comparing `songbirdcli-0.2.2/songbirdcli/cli.py` & `songbirdcli-0.2.3/songbirdcli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
                     break
                 mode = resolve_mode(album_name, current_mode=current_mode)
                 # detect mode change and return to main menu
                 if mode is not None:
                     current_mode = mode
                     continue
 
-                album_song_properties = launch_album_mode(album_name)
+                album_song_properties = helpers.launch_album_mode(album_name)
                 if album_song_properties is None:
                     break
 
                 songs = [song.trackName for song in album_song_properties]
             elif current_mode == modes.Modes.SONG:
                 songs = helpers.get_input_list(
                     "Please input song(s), separated by ';'. E.g. song1; song2; song3.",
```

### Comparing `songbirdcli-0.2.2/songbirdcli/helpers.py` & `songbirdcli-0.2.3/songbirdcli/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,16 @@
         if choices is not None:
             built_prompt += f" , choices=({choices})"
         built_prompt += " ['q' quits]: "
         inp = input(built_prompt)
         if inp == quit_str:
             return None
 
+        # initialize type to be empty by default
+        typed = None
         if out_type is not None:
             try:
                 typed = out_type(inp)
 
             except ValueError as e:
                 logger.error(
                     "Invalid type received. Try again, inputting an '{out_type}'"
@@ -179,16 +181,16 @@
     while True:
         inp = input(prompt + f" ['{quit_str}' quits]: ")
         if inp == quit_str:
             return None
 
         str_list = inp.split(sep)
         typed_list = []
-        # by default pass type check
-        type_check_passed = True
+        # by default fail type check
+        type_check_passed = False
         for item in str_list:
             type_check_passed = True
             try:
                 typed_inp = out_type(item)
             except ValueError as e:
                 logger.error(
                     f"Invalid input {inp} recieved, expected list with types: {out_type}, separated by '{sep}'"
```

### Comparing `songbirdcli-0.2.2/songbirdcli/requirements.txt` & `songbirdcli-0.2.3/songbirdcli/requirements.txt`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/songbirdcli/settings.py` & `songbirdcli-0.2.3/songbirdcli/settings.py`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/songbirdcli.egg-info/PKG-INFO` & `songbirdcli-0.2.3/songbirdcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcli
-Version: 0.2.2
+Version: 0.2.3
 Summary: Songbird's cli.
 Author: Christian Boin
 Project-URL: Documentation, https://cboin1996.github.io/songbird/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
```

### Comparing `songbirdcli-0.2.2/songbirdcli.egg-info/SOURCES.txt` & `songbirdcli-0.2.3/songbirdcli.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 songbirdcli/settings.py
 songbirdcli/version.py
 songbirdcli.egg-info/PKG-INFO
 songbirdcli.egg-info/SOURCES.txt
 songbirdcli.egg-info/dependency_links.txt
 songbirdcli.egg-info/requires.txt
 songbirdcli.egg-info/top_level.txt
-tests/unit/test_cli.py
+tests/unit/test_cli.py
+tests/unit/test_helpers.py
```

### Comparing `songbirdcli-0.2.2/songbirdcli.egg-info/requires.txt` & `songbirdcli-0.2.3/songbirdcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.2/tests/unit/test_cli.py` & `songbirdcli-0.2.3/tests/unit/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,25 @@
         "billy joel",  # user enters billy joel
         "-1",  # user selects continue without properties
         "",  # user opts to search youtube
         "0",  # user selects first song
         "l",  # user selects  save locally
         "q",  # user quits
     ],
+    [
+        "john mayer",  # user enters john mayer
+        "",  # user hits enter by accident
+        "0",  # user continues by selecting property 0
+        "",  # user opts to search youtube
+        "",  # user hits enter by accident
+        "800",  # user enters invalid input
+        "0",  # user selects first song
+        "l",  # user selects  save locally
+        "q",  # user quits
+    ],
 ]
 
 
 @pytest.fixture
 def create_test_folder():
     tests_data_folder = os.path.join(sys.path[0], "tests-output")
     if not os.path.exists(tests_data_folder):
```

