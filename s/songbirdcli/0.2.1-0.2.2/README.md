# Comparing `tmp/songbirdcli-0.2.1.tar.gz` & `tmp/songbirdcli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songbirdcli-0.2.1.tar", last modified: Wed Apr 17 21:16:00 2024, max compression
+gzip compressed data, was "songbirdcli-0.2.2.tar", last modified: Thu Apr 18 19:38:34 2024, max compression
```

## Comparing `songbirdcli-0.2.1.tar` & `songbirdcli-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.485056 songbirdcli-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.489055 songbirdcli-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.489055 songbirdcli-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.489055 songbirdcli-0.2.1/docs/songbirdcli/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/docs/songbirdcli/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/docs/songbirdcli/helpers.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/docs/songbirdcli/settings.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/songbirdcli/
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/requirements.txt.blank
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/songbirdcli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/songbirdcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 21:16:00.000000 songbirdcli-0.2.1/songbirdcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.485056 songbirdcli-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:16:00.493055 songbirdcli-0.2.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-17 21:15:51.000000 songbirdcli-0.2.1/tests/unit/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.875332 songbirdcli-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.867333 songbirdcli-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-18 19:38:34.875332 songbirdcli-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/docs/songbirdcli/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/docs/songbirdcli/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/docs/songbirdcli/helpers.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/docs/songbirdcli/settings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:38:34.875332 songbirdcli-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/songbirdcli/
+-rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/requirements.txt.blank
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/songbirdcli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.875332 songbirdcli-0.2.2/songbirdcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 19:38:34.000000 songbirdcli-0.2.2/songbirdcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.867333 songbirdcli-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:38:34.871333 songbirdcli-0.2.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-18 19:38:30.000000 songbirdcli-0.2.2/tests/unit/test_cli.py
```

### Comparing `songbirdcli-0.2.1/.github/workflows/docker.yml` & `songbirdcli-0.2.2/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.1/.github/workflows/pages.yaml` & `songbirdcli-0.2.2/.github/workflows/pages.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.1/.github/workflows/pypi-publish.yaml` & `songbirdcli-0.2.2/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.1/.github/workflows/tests.yaml` & `songbirdcli-0.2.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.1/Dockerfile` & `songbirdcli-0.2.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.1/LICENSE` & `songbirdcli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.1/Makefile` & `songbirdcli-0.2.2/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -122,12 +122,18 @@
 .PHONY: dev
 dev: clean build run
 
 lint:
 	black $(APP_NAME)/.
 	black tests
 
+.PHONY: test-cov
+test-stdout:
+	python -m pytest --cov=songbirdcli tests/unit -v
+
+.PHONY: test
 test:
 	python -m pytest --doctest-modules --junitxml=junit/test-results.xml --cov=songbirdcli --cov-report=xml --cov-report=html tests/unit -v
 
+.PHONY: test-env
 test-env:
 	$(ENV_VARS) python -m pytest --doctest-modules --junitxml=junit/test-results.xml --cov=songbirdcli --cov-report=xml --cov-report=html tests/unit -v
```

### Comparing `songbirdcli-0.2.1/PKG-INFO` & `songbirdcli-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Songbird's cli.
 Author: Christian Boin
 Project-URL: Documentation, https://cboin1996.github.io/songbird/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
@@ -44,18 +44,18 @@
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pydantic_core==2.18.1
 Requires-Dist: pyee==11.1.0
 Requires-Dist: pyparsing==3.1.2
 Requires-Dist: pyquery==2.0.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: requests-htmlc==0.0.6
+Requires-Dist: requests-htmlc==0.0.7
 Requires-Dist: requests-oauthlib==2.0.0
 Requires-Dist: rsa==4.9
-Requires-Dist: songbirdcore==0.0.7
+Requires-Dist: songbirdcore==0.0.9
 Requires-Dist: soupsieve==2.5
 Requires-Dist: toml==0.10.2
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: uritemplate==4.1.1
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: w3lib==2.1.2
 Requires-Dist: websockets==12.0
```

### Comparing `songbirdcli-0.2.1/README.md` & `songbirdcli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.1/mkdocs.yml` & `songbirdcli-0.2.2/mkdocs.yml`

 * *Files 21% similar despite different names*

```diff
@@ -7,19 +7,27 @@
 repo_name: cboin1996/songbird
 repo_url: https://github.com/cboin1996/songbird
 edit_uri: ""
 
 theme:
   name: material
   features:
-    - navigation.sections
-    - navigation.tracking
+    - content.tabs.link
+    - content.code.annotate
+    - content.code.copy
+    - announce.dismiss
     - navigation.tabs
-    - navigation.tabs.sticky
+    - navigation.instant
+    - navigation.instant.prefetch
+    - navigation.instant.preview
+    - navigation.instant.progress
+    - navigation.path
     - navigation.top
+    - navigation.tracking
+    - search.suggest
     - toc.follow
   palette:
     # Palette toggle for dark mode
     - scheme: slate
       primary: blue
       toggle:
         icon: material/weather-night
@@ -35,26 +43,27 @@
 validation:
   omitted_files: warn
   absolute_links: warn
   unrecognized_links: warn
 
 nav:
 - Get Started:
-  - Welcome to songbirdcore: index.md
+  - Welcome to songbirdcli: index.md
 - API Documentation:
-  - songbirdcore:
+  - songbirdcli:
     - cli: songbirdcli/cli.md
     - helpers: songbirdcli/helpers.md
     - settings: songbirdcli/settings.md
 
 extra:
   version:
     provider: mike
 
 plugins:
+- search
 - mkdocstrings:
     enabled: !ENV [ENABLE_MKDOCSTRINGS, true]
     default_handler: python
     handlers:
       python:
         options:
           docstring_style: google
```

### Comparing `songbirdcli-0.2.1/pyproject.toml` & `songbirdcli-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "songbirdcli"
 authors = [
     {name = "Christian Boin"},
 ]
-version = "0.2.1"
+version = "0.2.2"
 description = "Songbird's cli."
 readme = "README.md"
 requires-python = ">=3.11"
 dynamic = ["dependencies"]
 
 [project.urls]
 Documentation = "https://cboin1996.github.io/songbird/"
```

### Comparing `songbirdcli-0.2.1/songbirdcli/cli.py` & `songbirdcli-0.2.2/songbirdcli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,16 @@
             f"Duplicate file(s) already exist for base file {file_path}, so I generated a new filename {duped_filepath}!"
         )
         file_path_no_format = os.path.splitext(duped_filepath)[0]
         file_path = duped_filepath
     # run the youtube downloader
     if config.youtube_dl_enabled:
         payload = config.youtube_searchform_payload
-        if song_properties != []:
+        # if song_properties is False, user selected no properties
+        if song_properties != False:
             payload[config.youtube_search_tag] = (
                 f"{song_properties.artistName} {song_properties.trackName}"
             )
         else:
             payload[config.youtube_search_tag] = song_name
 
         downloaded_file_path = run_download_process(
@@ -250,24 +251,26 @@
             render_wait=config.youtube_render_wait,
             render_retries=config.youtube_render_retries,
             render_sleep=config.youtube_render_sleep,
         )
 
     if downloaded_file_path is None:
         return
-    # tag file
-    tag_successful = False
-    if file_format == "mp3":
-        tag_successful = itunes.mp3ID3Tagger(downloaded_file_path, song_properties)
-    elif file_format == "m4a":
-        tag_successful = itunes.m4a_tagger(downloaded_file_path, song_properties)
-    else:
-        logger.warn(
-            "You've specified a file format that is has no tagger supported yet. Saving file without tags."
-        )
+
+    if song_properties != False:
+        # tag file if user specified song properties
+        tag_successful = False
+        if file_format == "mp3":
+            tag_successful = itunes.mp3ID3Tagger(downloaded_file_path, song_properties)
+        elif file_format == "m4a":
+            tag_successful = itunes.m4a_tagger(downloaded_file_path, song_properties)
+        else:
+            logger.warning(
+                "You've specified a file format that is has no tagger supported yet. Saving file without tags."
+            )
 
     # provide user with choices for where to save their file to.
     save_prompt_base = "Would you like to save your file to"
     if config.itunes_enabled and config.gdrive_enabled:
         inp = helpers.get_input(
             save_prompt_base + " gdrive (g), itunes (i), or locally (l)",
             out_type=str,
```

### Comparing `songbirdcli-0.2.1/songbirdcli/helpers.py` & `songbirdcli-0.2.2/songbirdcli/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     Args:
         search_variable (str): the value for the query
         mode (modes.Modes): the mode to run
         limit (int, optional): number of results. Defaults to 20.
         lookup (bool, optional): whether to enable 'lookup' mode in itunes api. Defaults to False.
 
     Returns:
-        Optional[Union[itunes_api.ItunesApiSongModel]]: returns the selected song properties, an empty list if the user continues without selection, or None if the user quits or an error occurred.
+        Optional[Union[itunes_api.ItunesApiSongModel]]: returns the selected song properties, a bool=False if use continues without selection, or None if the user quits or an error occurred.
     """
     parsed_results_list = itunes.query_api(search_variable, limit, mode, lookup=lookup)
 
     # Present results to user
     common.pretty_list_of_basemodel_printer(parsed_results_list)
     logger.info("Searched for: %s" % (search_variable))
     # Only one item can be selected
@@ -76,15 +76,15 @@
 
     # user has quit
     if user_selection is None:
         logger.info("Quitting.")
         return
     if len(user_selection) == 0:
         logger.info("Continuing without properties.")
-        return True
+        return False
 
     print(f"Selected item: ")
     for k, v in user_selection[0].model_dump().items():
         print(" - %s : %s" % (k, v))
 
     return user_selection[0]
 
@@ -179,14 +179,16 @@
     while True:
         inp = input(prompt + f" ['{quit_str}' quits]: ")
         if inp == quit_str:
             return None
 
         str_list = inp.split(sep)
         typed_list = []
+        # by default pass type check
+        type_check_passed = True
         for item in str_list:
             type_check_passed = True
             try:
                 typed_inp = out_type(item)
             except ValueError as e:
                 logger.error(
                     f"Invalid input {inp} recieved, expected list with types: {out_type}, separated by '{sep}'"
```

### Comparing `songbirdcli-0.2.1/songbirdcli/requirements.txt` & `songbirdcli-0.2.2/songbirdcli/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 pydantic-settings==2.2.1
 pydantic_core==2.18.1
 pyee==11.1.0
 pyparsing==3.1.2
 pyquery==2.0.0
 python-dotenv==1.0.1
 requests==2.31.0
-requests-htmlc==0.0.6
+requests-htmlc==0.0.7
 requests-oauthlib==2.0.0
 rsa==4.9
-songbirdcore==0.0.7
+songbirdcore==0.0.9
 soupsieve==2.5
 toml==0.10.2
 typing_extensions==4.11.0
 uritemplate==4.1.1
 urllib3==2.2.1
 w3lib==2.1.2
 websockets==12.0
```

### Comparing `songbirdcli-0.2.1/songbirdcli/settings.py` & `songbirdcli-0.2.2/songbirdcli/settings.py`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.1/songbirdcli.egg-info/PKG-INFO` & `songbirdcli-0.2.2/songbirdcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Songbird's cli.
 Author: Christian Boin
 Project-URL: Documentation, https://cboin1996.github.io/songbird/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
@@ -44,18 +44,18 @@
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pydantic_core==2.18.1
 Requires-Dist: pyee==11.1.0
 Requires-Dist: pyparsing==3.1.2
 Requires-Dist: pyquery==2.0.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: requests==2.31.0
-Requires-Dist: requests-htmlc==0.0.6
+Requires-Dist: requests-htmlc==0.0.7
 Requires-Dist: requests-oauthlib==2.0.0
 Requires-Dist: rsa==4.9
-Requires-Dist: songbirdcore==0.0.7
+Requires-Dist: songbirdcore==0.0.9
 Requires-Dist: soupsieve==2.5
 Requires-Dist: toml==0.10.2
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: uritemplate==4.1.1
 Requires-Dist: urllib3==2.2.1
 Requires-Dist: w3lib==2.1.2
 Requires-Dist: websockets==12.0
```

### Comparing `songbirdcli-0.2.1/songbirdcli.egg-info/SOURCES.txt` & `songbirdcli-0.2.2/songbirdcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.1/songbirdcli.egg-info/requires.txt` & `songbirdcli-0.2.2/songbirdcli.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 pydantic-settings==2.2.1
 pydantic_core==2.18.1
 pyee==11.1.0
 pyparsing==3.1.2
 pyquery==2.0.0
 python-dotenv==1.0.1
 requests==2.31.0
-requests-htmlc==0.0.6
+requests-htmlc==0.0.7
 requests-oauthlib==2.0.0
 rsa==4.9
-songbirdcore==0.0.7
+songbirdcore==0.0.9
 soupsieve==2.5
 toml==0.10.2
 typing_extensions==4.11.0
 uritemplate==4.1.1
 urllib3==2.2.1
 w3lib==2.1.2
 websockets==12.0
```

