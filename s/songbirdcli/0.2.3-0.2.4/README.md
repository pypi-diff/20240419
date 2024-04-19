# Comparing `tmp/songbirdcli-0.2.3.tar.gz` & `tmp/songbirdcli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songbirdcli-0.2.3.tar", last modified: Thu Apr 18 22:47:25 2024, max compression
+gzip compressed data, was "songbirdcli-0.2.4.tar", last modified: Fri Apr 19 16:43:02 2024, max compression
```

## Comparing `songbirdcli-0.2.3.tar` & `songbirdcli-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.661662 songbirdcli-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.665663 songbirdcli-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.665663 songbirdcli-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.665663 songbirdcli-0.2.3/docs/songbirdcli/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/docs/songbirdcli/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/docs/songbirdcli/helpers.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/docs/songbirdcli/settings.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/songbirdcli/
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/requirements.txt.blank
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/songbirdcli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/songbirdcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 22:47:25.000000 songbirdcli-0.2.3/songbirdcli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.665663 songbirdcli-0.2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:47:25.669663 songbirdcli-0.2.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/tests/unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-18 22:47:21.000000 songbirdcli-0.2.3/tests/unit/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:43:02.333353 songbirdcli-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:43:02.325353 songbirdcli-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:43:02.329353 songbirdcli-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/.github/workflows/pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-19 16:43:02.333353 songbirdcli-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:43:02.329353 songbirdcli-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:43:02.329353 songbirdcli-0.2.4/docs/songbirdcli/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/docs/songbirdcli/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/docs/songbirdcli/helpers.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/docs/songbirdcli/settings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 16:43:02.333353 songbirdcli-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:43:02.329353 songbirdcli-0.2.4/songbirdcli/
+-rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/songbirdcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/songbirdcli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/songbirdcli/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/songbirdcli/requirements.txt.blank
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/songbirdcli/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/songbirdcli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:43:02.329353 songbirdcli-0.2.4/songbirdcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-04-19 16:43:02.000000 songbirdcli-0.2.4/songbirdcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-19 16:43:02.000000 songbirdcli-0.2.4/songbirdcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:43:02.000000 songbirdcli-0.2.4/songbirdcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-19 16:43:02.000000 songbirdcli-0.2.4/songbirdcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 16:43:02.000000 songbirdcli-0.2.4/songbirdcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:43:02.325353 songbirdcli-0.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:43:02.329353 songbirdcli-0.2.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/tests/unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-19 16:42:58.000000 songbirdcli-0.2.4/tests/unit/test_helpers.py
```

### Comparing `songbirdcli-0.2.3/.github/workflows/docker.yml` & `songbirdcli-0.2.4/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/.github/workflows/pages.yaml` & `songbirdcli-0.2.4/.github/workflows/pages.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/.github/workflows/pypi-publish.yaml` & `songbirdcli-0.2.4/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/.github/workflows/tests.yaml` & `songbirdcli-0.2.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/Dockerfile` & `songbirdcli-0.2.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/LICENSE` & `songbirdcli-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/Makefile` & `songbirdcli-0.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/PKG-INFO` & `songbirdcli-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcli
-Version: 0.2.3
+Version: 0.2.4
 Summary: Songbird's cli.
 Author: Christian Boin
 Project-URL: Documentation, https://cboin1996.github.io/songbird/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
```

### Comparing `songbirdcli-0.2.3/README.md` & `songbirdcli-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/mkdocs.yml` & `songbirdcli-0.2.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/pyproject.toml` & `songbirdcli-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "songbirdcli"
 authors = [
     {name = "Christian Boin"},
 ]
-version = "0.2.3"
+version = "0.2.4"
 description = "Songbird's cli."
 readme = "README.md"
 requires-python = ">=3.11"
 dynamic = ["dependencies"]
 
 [project.urls]
 Documentation = "https://cboin1996.github.io/songbird/"
@@ -38,8 +38,11 @@
 ]
 package = [
     "build",
     "twine"
 ]
 
 [tool.setuptools.packages.find]
-exclude = ["app", "junit"]
+exclude = ["app", "junit"]
+
+[tool.pytest.ini_options]
+log_cli_level="INFO"
```

### Comparing `songbirdcli-0.2.3/songbirdcli/cli.py` & `songbirdcli-0.2.4/songbirdcli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import datetime
 from enum import Enum
-from typing import Optional, List
+from typing import Optional, List, Union
+import requests
 import os, sys, shutil
 
 from songbirdcli import settings
 from songbirdcli import helpers
 from songbirdcli import version
 
 from songbirdcore.models import modes, itunes_api
@@ -110,14 +111,15 @@
     youtube_search_url: str,
     youtube_query_payload: dict,
     file_format: str,
     render_timeout: int,
     render_wait: float,
     render_retries: int,
     render_sleep: int,
+    quit_str: str = "q",
 ) -> str:
     """Download a song from youtube.
 
     Args:
         file_path_no_format (str): the absolute path of where to save the file (excluding file format)
         youtube_home_url (str): the url to youtube's home page
         youtube_search_url (str): the search url for youtube
@@ -125,26 +127,48 @@
         file_format (str): desired file format
         render_timeout (int): amount of time before abandoning a render
         render_wait (float): the amount of time before attempting a render
         render_retries (int): the number of retries for a render
         render_sleep (int): the amount of time to wait after rendering
 
     Returns:
-        str: the path on disk that the file was saved to. None if the download fails.
+        str: the path on disk that the file was saved to, None if failure occured, quit_str if user quit
     """
-    # obtain video selection from user
-    video_url = helpers.get_input(
-        prompt=f"Enter a URL, or hit enter to use '{youtube_query_payload}' as a query to youtube: ",
-        out_type=str,
-    )
+    is_valid_url = False
+    while not is_valid_url:
+        # obtain video selection from user
+        video_url = helpers.get_input(
+            prompt=f"Enter a URL, or hit enter to use '{youtube_query_payload}' as a query to youtube: ",
+            out_type=str,
+            quit_str=quit_str,
+        )
+        # if user hits enter, bypass url checks
+        if video_url == "":
+            break
 
-    if video_url is None:
-        return None
+        if video_url == quit_str:
+            return quit_str
 
-    # empty str (enter) query youtube
+        if video_url is None:
+            return None
+        try:
+            response = requests.get(video_url)
+        except Exception as e:
+            logger.error(f"exception occured testing your url: {e}")
+            continue
+
+        # only continue if url was valid
+        if response.status_code == 200:
+            is_valid_url = True
+        else:
+            logger.error(
+                f"URL is valid, but could not receive 200 status from {video_url}, is internet down?"
+            )
+
+        # empty str (enter) query youtube
     if video_url == "":
         link_list, links = youtube.get_video_links(
             youtube_home_url,
             youtube_search_url,
             youtube_query_payload,
             render_timeout,
             render_wait,
@@ -160,33 +184,40 @@
 
         video_selection_idx = helpers.select_items_from_list(
             "Select the song you wish to download!",
             link_list,
             1,
             return_value=False,
         )
+        if video_selection_idx == quit_str:
+            return quit_str
+
         if video_selection_idx is None or len(video_selection_idx) == 0:
             return None
 
         video_url = youtube_home_url + links[video_selection_idx[0]].attrs["href"]
     # Process the download, and save locally
     return youtube.run_download(video_url, file_path_no_format, file_format)
 
 
 def run_for_song(
     config: settings.SongbirdCliConfig,
     song_name: str,
     song_properties: Optional[itunes_api.ItunesApiSongModel],
-):
+    quit_str: str = "q",
+) -> Union[bool, None, str]:
     """Run a cycle of the application given a song.
 
     Args:
         config (settings.SongbirdConfig): the songbird config
         song_name (str): the name of the song to run the app for
         song_properties (Optional[itunes_api.ItunesApiSongModel]): optionally include song properties. Including these skips the itunes api parser.
+
+    Returns:
+        Union[bool, None, str]: returns boolean indicating success/failure. None indicated error occurred, quit_str indicates user quit
     """
     logger.info(f"Searching for: {song_name}")
     file_itunes = []
     file_gdrive = []
     # itunes craves m4a formatted files. Otherwise we use mp3s, as were civilized people.
     file_format = config.file_format if not config.itunes_enabled else "m4a"
     # check if song exists locally in dump folder
@@ -203,23 +234,26 @@
     files = file_local + file_itunes + file_gdrive
     if len(files) > 0:
         logger.info("Found the following similar files:")
         common.pretty_lst_printer(files)
         inp = helpers.get_input(
             "Do you want to proceed with download anyway?", choices=["y", "n"]
         )
+        # user quits or selects no
+        if inp == quit_str or inp == "n":
+            return quit_str
 
-        if inp is None or inp == "n":
+        if inp is None:
             return
 
     if song_properties is None:
         song_properties = helpers.parse_itunes_search_api(song_name, modes.Modes.SONG)
 
-    if song_properties is None:
-        return
+    if song_properties == quit_str:
+        return quit_str
 
     file_path_no_format = os.path.join(config.get_local_folder_path(), song_name)
     file_path = file_path_no_format + "." + file_format
     downloaded_file_path = None
     # make sure file doesnt already exist
     duped_filepath = common.fname_duper(file_path, config.fname_dup_limit, 1, "_dup")
     if duped_filepath is None:
@@ -247,19 +281,29 @@
             youtube_search_url=config.youtube_search_url,
             youtube_query_payload=payload,
             file_format=file_format,
             render_timeout=config.youtube_render_timeout,
             render_wait=config.youtube_render_wait,
             render_retries=config.youtube_render_retries,
             render_sleep=config.youtube_render_sleep,
+            quit_str=quit_str,
         )
+    if downloaded_file_path == quit_str:
+        return quit_str
 
     if downloaded_file_path is None:
         return
 
+    # perform sanity check in case no file exists and yt-dlp didnt throw an error
+    if not os.path.exists(downloaded_file_path):
+        logger.error(
+            f"yt-dlp reported no error downloading file, but file does not exist. Cannot proceed with tagging as no file exists."
+        )
+        return
+
     if song_properties != False:
         # tag file if user specified song properties
         tag_successful = False
         if file_format == "mp3":
             tag_successful = itunes.mp3ID3Tagger(downloaded_file_path, song_properties)
         elif file_format == "m4a":
             tag_successful = itunes.m4a_tagger(downloaded_file_path, song_properties)
@@ -290,14 +334,16 @@
             out_type=str,
             choices=["g", "l"],
         )
 
     if not config.itunes_enabled and not config.gdrive_enabled:
         inp = "l"
 
+    if inp == quit_str:
+        return quit_str
     if inp is None:
         return
 
     if inp == "i":
         msg = "Saved to itunes"
         itunes_dest_path = common.fname_duper(
             os.path.join(
@@ -342,21 +388,70 @@
     else:
         msg = "Saved locally."
 
     logger.info(msg)
     return True
 
 
+def get_songs_from_user(
+    current_mode: modes.Modes, quit_str: str = "q"
+) -> Optional[Union[str, List[str]]]:
+    # launch album mode to collect songs
+    if current_mode == modes.Modes.ALBUM:
+        album_name = helpers.get_input(
+            f"Enter an album name.", out_type=str, quit_str=quit_str
+        )
+        # quit condition
+        if album_name == quit_str:
+            return quit_str
+        if album_name is None:
+            return None
+
+        mode = resolve_mode(album_name, current_mode=current_mode)
+        # detect mode change and return to main menu
+        if mode is not None:
+            return mode
+
+        album_song_properties = helpers.launch_album_mode(album_name)
+        # quit iteration to main menu
+        if album_song_properties == quit_str:
+            return quit_str
+        if album_song_properties is None:
+            return None
+        return [song.trackName for song in album_song_properties]
+
+    # launch song mode to collect songs
+    elif current_mode == modes.Modes.SONG:
+        songs = helpers.get_input_list(
+            "Please input song(s), separated by ';'. E.g. song1; song2; song3.",
+            out_type=str,
+            sep="; ",
+        )
+        # quit iteration to main menu
+        if songs == quit_str:
+            return quit_str
+        if songs is None:
+            return None
+
+        mode = resolve_mode(songs[0], current_mode=current_mode)
+        # detect mode change and return to main menu
+        if mode is not None:
+            return mode
+        return songs
+
+
 def run(config: settings.SongbirdCliConfig):
     """main entrypoint for songbirdcli. Expects the songbirdcli config object.
 
     Args:
         config (settings.SongbirdCliConfig): songbirdcli settings pydantic model
 
     """
+    # setup quit str for user
+    quit_str = "q"
     try:
         common.set_logger_config_globally(log_level=config.log_level)
         common.name_plate(entries=[f"--cli {config.version}"])
         # only need folders on OS if we are running locally. Otherwise user is expected to provied folders
         # via bind mounts
         if config.run_local:
             initialize_dirs(
@@ -372,51 +467,62 @@
             return None
         current_mode = modes.Modes.SONG
         while True:
             logger.info(f"---Songbird Main Menu v{config.version}🐦---")
 
             song_properties = None
             album_song_properties = None
-            # launch album mode to collect songs
-            if current_mode == modes.Modes.ALBUM:
-                album_name = helpers.get_input(f"Enter an album name.", out_type=str)
-                # quit condition
-                if album_name is None:
-                    break
-                mode = resolve_mode(album_name, current_mode=current_mode)
-                # detect mode change and return to main menu
-                if mode is not None:
-                    current_mode = mode
-                    continue
-
-                album_song_properties = helpers.launch_album_mode(album_name)
-                if album_song_properties is None:
-                    break
-
-                songs = [song.trackName for song in album_song_properties]
-            elif current_mode == modes.Modes.SONG:
-                songs = helpers.get_input_list(
-                    "Please input song(s), separated by ';'. E.g. song1; song2; song3.",
+            result = get_songs_from_user(current_mode=current_mode, quit_str=quit_str)
+            # user quits
+            if result == quit_str:
+                return_to_menu = helpers.get_input(
+                    prompt=f"Are you sure you want to quit?",
+                    choices=["y", "n"],
                     out_type=str,
-                    sep="; ",
+                    quit_str=quit_str,
                 )
-                # quit condition
-                if songs is None:
-                    break
-                mode = resolve_mode(songs[0], current_mode=current_mode)
-                # detect mode change and return to main menu
-                if mode is not None:
-                    current_mode = mode
+                # allow user to return to main menu before
+                # full shutdown
+                if return_to_menu == "n":
                     continue
 
+                return quit_str
+
+            # user changed mode
+            if isinstance(result, modes.Modes):
+                current_mode = result
+                continue
+
+            # error occurred
+            if result is None:
+                continue
+            # set songs to result and continue otherwise
+            songs = result
             logger.info(f"Searching for songs: {songs}")
             for i, song in enumerate(songs):
                 if album_song_properties is not None:
                     song_properties = album_song_properties[i]
-                success = run_for_song(config, song, song_properties)
+                success = run_for_song(config, song, song_properties, quit_str)
+
+                # detect if more songs are queued, and asks if user wants to continue with other songs
+                if (success == quit_str or success == None) and i + 1 < len(songs):
+                    songs_remaining = songs[i + 1 :]
+                    common.pretty_lst_printer(songs_remaining)
+                    return_to_menu = helpers.get_input(
+                        prompt=f"You have {len(songs_remaining)} songs (above) in queue. Would you like to continue?",
+                        choices=["y", "n"],
+                        out_type=str,
+                        quit_str=quit_str,
+                    )
+                    # only return to main menu if user opts to, otherwise enter next iteration
+                    # to preserve list of selections
+                    if return_to_menu == "n" or return_to_menu == quit_str:
+                        break
+                    if return_to_menu == "y":
+                        continue
 
     except KeyboardInterrupt as e:
         logger.info("\nReceived keyboard interrupt :o")
 
     logger.info("Shutting down!")
```

### Comparing `songbirdcli-0.2.3/songbirdcli/helpers.py` & `songbirdcli-0.2.4/songbirdcli/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,94 +6,120 @@
 from songbirdcore import common, itunes
 from songbirdcore.models import modes, itunes_api
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-def launch_album_mode(artist_album_string=""):
+def launch_album_mode(artist_album_string="", quit_str="q"):
     """
     Args:
         artist_album_string (str): the album/artist to search for.
 
-    Returns: the list of song properties gathered from the search.
+    Returns: the list of song properties gathered from the search, None if error occured, quit_str if user quit
 
     """
     while True:
         album_props = parse_itunes_search_api(
-            search_variable=artist_album_string, mode=modes.Modes.ALBUM, lookup=False
+            search_variable=artist_album_string,
+            mode=modes.Modes.ALBUM,
+            lookup=False,
+            # disable no selection here, user must select album properties.
+            no_selection_value=None,
         )
         # check if user quit
+        if album_props == quit_str:
+            return quit_str
+
         if album_props is None:
             return None
 
         # get the song matching the album metadata
         songs_in_album_props = itunes.query_api(
             search_variable=album_props.collectionId,  # get list of songs for chosen album
             limit=album_props.trackCount,
             mode=modes.Modes.SONG,
             lookup=True,
         )
+        # api error occurred
         if songs_in_album_props == None:
-            logger.error("Sorry. Cant seem to find any details for this album!")
+            return None
+        # no songs found for album
+        if len(songs_in_album_props) == 0:
+            logger.error(
+                "Sorry. Cant seem to find any details for this album in itunes api! Please select a different album."
+            )
+            return None
 
         songs_in_album_props = remove_songs_selected(
-            song_properties_list=songs_in_album_props
+            song_properties_list=songs_in_album_props, quit_str=quit_str
         )
+        if songs_in_album_props == quit_str:
+            return quit_str
         if songs_in_album_props is None:
             return None
 
         return songs_in_album_props
 
 
 # entity is usually song for searching songs
 def parse_itunes_search_api(
-    search_variable: str, mode: modes.Modes, limit: int = 20, lookup: bool = False
-) -> Optional[Union[bool, itunes_api.ItunesApiSongModel]]:
+    search_variable: str,
+    mode: modes.Modes,
+    limit: int = 20,
+    lookup: bool = False,
+    no_selection_value: Optional[int] = -1,
+    quit_str: str = "q",
+) -> Optional[
+    Union[bool, itunes_api.ItunesApiSongModel, itunes_api.ItunesApiAlbumKeys]
+]:
     """perform a query of the items api, allowing user to select
     an item from the returned list of options
 
     Args:
         search_variable (str): the value for the query
         mode (modes.Modes): the mode to run
         limit (int, optional): number of results. Defaults to 20.
         lookup (bool, optional): whether to enable 'lookup' mode in itunes api. Defaults to False.
+        no_selection_value (int, optional): whether to set an option for 'no selection' from stdin
+        quit_str (str, optional): str value used to determine whether to quit the song selection process
 
     Returns:
-        Optional[Union[itunes_api.ItunesApiSongModel]]: returns the selected song properties, a bool=False if use continues without selection, or None if the user quits or an error occurred.
+        Optional[Union[itunes_api.ItunesApiSongModel]]: returns the selected song properties, a bool=False if use continues without selection, None if error occurred, or quit_str if user quit.
     """
     parsed_results_list = itunes.query_api(search_variable, limit, mode, lookup=lookup)
 
     # Present results to user
     common.pretty_list_of_basemodel_printer(parsed_results_list)
     logger.info("Searched for: %s" % (search_variable))
     # Only one item can be selected
     user_selection = select_items_from_list(
-        "Select the number for the properties you want",
-        parsed_results_list,
-        1,
-        no_selection_value=-1,
+        prompt="Select the number for the properties you want",
+        lyst=parsed_results_list,
+        n_choices=1,
+        quit_str=quit_str,
+        no_selection_value=no_selection_value,
     )
 
     # user has quit
-    if user_selection is None:
+    if user_selection == quit_str:
         logger.info("Quitting.")
-        return
+        return quit_str
     if len(user_selection) == 0:
         logger.info("Continuing without properties.")
         return False
 
     print(f"Selected item: ")
     for k, v in user_selection[0].model_dump().items():
         print(" - %s : %s" % (k, v))
 
     return user_selection[0]
 
 
-def remove_songs_selected(song_properties_list) -> Optional[List]:
+def remove_songs_selected(song_properties_list, quit_str: str = "q") -> Optional[List]:
     """Given a list of songs properties, allow the user to remove
     via stdio
 
     Args:
         song_properties_list (Any): the list of song properties
 
     Returns:
@@ -102,18 +128,21 @@
     common.pretty_list_of_basemodel_printer(song_properties_list)
     input_string = "Enter song id's (1 4 5 etc.) you dont want from this album"
     user_input = select_items_from_list(
         input_string,
         song_properties_list,
         n_choices=len(song_properties_list) - 1,
         sep=" ",
+        quit_str=quit_str,
         opposite=True,
         no_selection_value=-1,
     )
     # user has quit
+    if user_input == quit_str:
+        return quit_str
     if user_input == None:
         return None
     # user selects all songs
     if user_input == []:
         return song_properties_list
     # otherwise, user gets the processed list with their items removed
     return user_input
@@ -127,24 +156,24 @@
     Args:
         prompt (str): the prompt to use
         out_type (type, optional): expected type for input. Defaults to None.
         quit_str (str, optional): a character to signify quitting from the input gatherer. Defaults to "q".
         choices (Optional[List], optional): valid character options to parse as input. Defaults to None.
 
     Returns:
-        Optional[Any]: the typed user input, or None if quit or invalid type received.
+        Optional[Any]: the typed user input, None if error occured, quit_str if use quit
     """
     while True:
         built_prompt = prompt
         if choices is not None:
             built_prompt += f" , choices=({choices})"
         built_prompt += " ['q' quits]: "
         inp = input(built_prompt)
         if inp == quit_str:
-            return None
+            return quit_str
 
         # initialize type to be empty by default
         typed = None
         if out_type is not None:
             try:
                 typed = out_type(inp)
 
@@ -172,20 +201,20 @@
         sep (str): the expected separator in the input list
         out_type (_type_, optional): The expected data type. Defaults to int.
 
     Raises:
         ValueError: If the input does not match the given type.
 
     Returns:
-        Optional[List[int]]: the typed list, or None if user quit
+        Optional[List[int]]: the typed list, or the quit_str value if user quits
     """
     while True:
         inp = input(prompt + f" ['{quit_str}' quits]: ")
         if inp == quit_str:
-            return None
+            return quit_str
 
         str_list = inp.split(sep)
         typed_list = []
         # by default fail type check
         type_check_passed = False
         for item in str_list:
             type_check_passed = True
@@ -209,31 +238,31 @@
 def select_items_from_list(
     prompt: str,
     lyst: List,
     n_choices: int,
     sep: Optional[str] = None,
     quit_str: str = "q",
     opposite: bool = False,
-    no_selection_value=None,
+    no_selection_value: int = None,
     return_value: bool = True,
 ) -> List:
     """Input validation against a list.
 
     Args:
         prompt (str): prompt to display to user
         sep    (str): the separator for the input
         lyst (List): the list to perform input validation against
         n_choices (int): the number of choices allowed
         quit_str (str): The string to cancel validation and exit. Defaults to "q".
         opposite (bool): return everything BUT the user selection
-        no_selection_value (any): value to indicate no selection wanted from the user
+        no_selection_value (int, optional): value to indicate no selection wanted from the user
         return_value (bool): if true, return the value, otherwise return the indicies of selections
 
     Returns:
-        Optiona[List]: None if user quits, [] if user selects nothing, otherwise a list of the users selections are returned.
+        Optiona[List]: quit_str if user quits, [] if user selects nothing, otherwise a list of the users selections are returned.
     """
     tries = 0
     low = 0
     high = len(lyst) - 1
     # provide useful ranges to user
     if high == -1:
         range_display = ""
@@ -256,18 +285,20 @@
         tries += 1
         if tries > 5:
             logger.info(f"Wtf man. {tries} tries so far? Just get it right!")
         # get user input
         inp = get_input_list(
             prompt + f"{range_display} {no_selection_prompt}",
             sep,
+            quit_str=quit_str,
             out_type=int,
         )
-        if inp is None:
-            return None
+        if inp == quit_str:
+            return quit_str
+
         if len(inp) == 0:
             logger.info("You selected nothing.")
             return []
         # verify if the value of the input is the selection value
         if inp[0] == no_selection_value:
             return []
         # if user has entered too many choices, try again!!
```

### Comparing `songbirdcli-0.2.3/songbirdcli/requirements.txt` & `songbirdcli-0.2.4/songbirdcli/requirements.txt`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/songbirdcli/settings.py` & `songbirdcli-0.2.4/songbirdcli/settings.py`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/songbirdcli.egg-info/PKG-INFO` & `songbirdcli-0.2.4/songbirdcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcli
-Version: 0.2.3
+Version: 0.2.4
 Summary: Songbird's cli.
 Author: Christian Boin
 Project-URL: Documentation, https://cboin1996.github.io/songbird/
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
```

### Comparing `songbirdcli-0.2.3/songbirdcli.egg-info/SOURCES.txt` & `songbirdcli-0.2.4/songbirdcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/songbirdcli.egg-info/requires.txt` & `songbirdcli-0.2.4/songbirdcli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `songbirdcli-0.2.3/tests/unit/test_cli.py` & `songbirdcli-0.2.4/tests/unit/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,74 @@
 from songbirdcli import cli
 from songbirdcli import settings
 from songbirdcli import version
 from io import StringIO
 import os, sys, shutil
 import pytest
 
+# cli_inputs defined vectors that a user would
+# input as they navigate through the app
 cli_inputs = [
     [
         "jolene",  # user enters jolene
         "0",  # user selects first song
         "",  # user opts to search youtube
         "0",  # user selects first song
         "i",  # save to local itunes folder
         "q",  # user quits
+        "y",  # user quits via y/n selection
     ],
     [
         "jolene",  # user enters jolene
         "0",  # user selects first song
+        "https://s"  # user enter invalid download url
         "https://www.youtube.com/watch?v=Ixrje2rXLMA",  # user opts to direct download
         "l",  # save locally
         "q",  # user quits
-    ],
-    [
-        "billy joel",  # user enters billy joel
-        "-1",  # user selects continue without properties
-        "",  # user opts to search youtube
+        "n",  # user selects to continue
+        "billy",  # user searches billy
         "0",  # user selects first song
-        "l",  # user selects  save locally
-        "q",  # user quits
+        "q",  # user quits to main menu
+        "q",  # user quits app
+        "q",  # user confirms quit
     ],
     [
-        "john mayer",  # user enters john mayer
-        "",  # user hits enter by accident
-        "0",  # user continues by selecting property 0
+        "billy joel; john lennon",  # user enters billy joel and john lennon
+        "-1",  # user selects continue without properties
         "",  # user opts to search youtube
         "",  # user hits enter by accident
         "800",  # user enters invalid input
         "0",  # user selects first song
         "l",  # user selects  save locally
-        "q",  # user quits
+        "q",  # user accidentally quits
+        "y",  # user selects to resume
+        "0",  # user selects property 0
+        "q",  # user quits to main menu
+        "q",  # user quits app
+        "y",  # user quits app
+    ],
+    [
+        "album",  # user enters album mode
+        "billy joel the stranger",  # user enters billy joel
+        "",  # validation for empty input
+        "-5",  # user enters invalid value
+        "0",  # user selects album 0
+        "-1",  # user selects keep all songs
+        "-5",  # user enters invalid input
+        "0",  # user selects song property 0 for first song
+        "",  # user hits enter to search youtube
+        "0",  # user selects song 0
+        "l",  # save locally
+        "q",  # select quit
+        "y",  # continue with queued songs
+        "0",  # select property 0
+        "q",  # quit queued songs
+        "n",  # do not continue queue
+        "q",  # quit application
+        "y",  # set yes to are you sure message
     ],
 ]
 
 
 @pytest.fixture
 def create_test_folder():
     tests_data_folder = os.path.join(sys.path[0], "tests-output")
```

