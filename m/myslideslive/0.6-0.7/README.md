# Comparing `tmp/myslideslive-0.6.tar.gz` & `tmp/myslideslive-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/myslideslive-0.6.tar", last modified: Mon Feb 26 22:01:33 2024, max compression
+gzip compressed data, was "dist/myslideslive-0.7.tar", last modified: Fri Apr 19 13:29:35 2024, max compression
```

## Comparing `myslideslive-0.6.tar` & `myslideslive-0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 22:01:33.000000 myslideslive-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-26 22:01:30.000000 myslideslive-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-26 22:01:30.000000 myslideslive-0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-02-26 22:01:33.000000 myslideslive-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-02-26 22:01:30.000000 myslideslive-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 22:01:33.000000 myslideslive-0.6/myslideslive/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-26 22:01:30.000000 myslideslive-0.6/myslideslive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-26 22:01:30.000000 myslideslive-0.6/myslideslive/_nbdev.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-02-26 22:01:30.000000 myslideslive-0.6/myslideslive/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    28844 2024-02-26 22:01:30.000000 myslideslive-0.6/myslideslive/slideslive.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-26 22:01:30.000000 myslideslive-0.6/myslideslive/test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 22:01:33.000000 myslideslive-0.6/myslideslive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-02-26 22:01:33.000000 myslideslive-0.6/myslideslive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-26 22:01:33.000000 myslideslive-0.6/myslideslive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 22:01:33.000000 myslideslive-0.6/myslideslive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-26 22:01:33.000000 myslideslive-0.6/myslideslive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 22:01:33.000000 myslideslive-0.6/myslideslive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-26 22:01:33.000000 myslideslive-0.6/myslideslive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-26 22:01:33.000000 myslideslive-0.6/myslideslive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-26 22:01:30.000000 myslideslive-0.6/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 22:01:33.000000 myslideslive-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-26 22:01:30.000000 myslideslive-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:29:35.000000 myslideslive-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-19 13:29:32.000000 myslideslive-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-19 13:29:32.000000 myslideslive-0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-19 13:29:35.000000 myslideslive-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-19 13:29:32.000000 myslideslive-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:29:35.000000 myslideslive-0.7/myslideslive/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 13:29:32.000000 myslideslive-0.7/myslideslive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-19 13:29:32.000000 myslideslive-0.7/myslideslive/_nbdev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-19 13:29:32.000000 myslideslive-0.7/myslideslive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30314 2024-04-19 13:29:32.000000 myslideslive-0.7/myslideslive/slideslive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 13:29:32.000000 myslideslive-0.7/myslideslive/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:29:35.000000 myslideslive-0.7/myslideslive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-19 13:29:34.000000 myslideslive-0.7/myslideslive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-19 13:29:34.000000 myslideslive-0.7/myslideslive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:29:34.000000 myslideslive-0.7/myslideslive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 13:29:34.000000 myslideslive-0.7/myslideslive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:29:34.000000 myslideslive-0.7/myslideslive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 13:29:34.000000 myslideslive-0.7/myslideslive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 13:29:34.000000 myslideslive-0.7/myslideslive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-19 13:29:32.000000 myslideslive-0.7/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:29:35.000000 myslideslive-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-19 13:29:32.000000 myslideslive-0.7/setup.py
```

### Comparing `myslideslive-0.6/LICENSE` & `myslideslive-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `myslideslive-0.6/PKG-INFO` & `myslideslive-0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myslideslive
-Version: 0.6
+Version: 0.7
 Summary: Download the (video) slides of your SlidesLive talk
 Home-page: https://github.com/So-Cool/myslideslive/tree/master/
 Author: Kacper Sokol
 Author-email: dev@kcpr.me
 License: BSD License
 Description: # mySlidesLive
         > ...helps you to extract your SlidesLive presentation.
@@ -51,15 +51,15 @@
         Directly from terminal:
         ```bash
         msl --slide 1074 1075 \
         https://slideslive.com/38956531/beyond-static-papers-rethinking-how-we-share-scientific-understanding-in-ml
         ```
         
         ## Development
-        - To develop this package you need [nbdev] v1 (`pip install "nbdev<2"`).
+        - To develop this package you need [nbdev] v1 and [unidecode] (`pip install "nbdev<2" unidecode`).
         - The library (and `Makefile`) is built with `nbdev_build_lib`.
         - `nbdev_update_lib` updates the notebooks based on changes in the library.
         - The `README.md` is regenerated with `nbdev_build_docs`.
         - The git hooks are set up with `nbdev_install_git_hooks`.
         - `jupyter nbconvert --clear-output --inplace notebook.ipynb` clears all output cells of a notebook.
         
         Before committing code changes make sure to run:
@@ -68,14 +68,15 @@
         nbdev_build_lib && \
         nbdev_build_docs && \
         nbdev_clean_nbs --clear_all True && \
         nbdev_test_nbs
         ```
         
         [nbdev]: https://nbdev.fast.ai/
+        [unidecode]: https://github.com/avian2/unidecode
         
         ## What about the SlidesLive video recording?
         If you want to get the video recording of your SlidesLive presentation as well,
         [youtube-dl] can take care of that.
         
         ## Cutting the video
         Then you can cut the video with:
```

### Comparing `myslideslive-0.6/README.md` & `myslideslive-0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 Directly from terminal:
 ```bash
 msl --slide 1074 1075 \
 https://slideslive.com/38956531/beyond-static-papers-rethinking-how-we-share-scientific-understanding-in-ml
 ```
 
 ## Development
-- To develop this package you need [nbdev] v1 (`pip install "nbdev<2"`).
+- To develop this package you need [nbdev] v1 and [unidecode] (`pip install "nbdev<2" unidecode`).
 - The library (and `Makefile`) is built with `nbdev_build_lib`.
 - `nbdev_update_lib` updates the notebooks based on changes in the library.
 - The `README.md` is regenerated with `nbdev_build_docs`.
 - The git hooks are set up with `nbdev_install_git_hooks`.
 - `jupyter nbconvert --clear-output --inplace notebook.ipynb` clears all output cells of a notebook.
 
 Before committing code changes make sure to run:
@@ -60,14 +60,15 @@
 nbdev_build_lib && \
 nbdev_build_docs && \
 nbdev_clean_nbs --clear_all True && \
 nbdev_test_nbs
 ```
 
 [nbdev]: https://nbdev.fast.ai/
+[unidecode]: https://github.com/avian2/unidecode
 
 ## What about the SlidesLive video recording?
 If you want to get the video recording of your SlidesLive presentation as well,
 [youtube-dl] can take care of that.
 
 ## Cutting the video
 Then you can cut the video with:
```

### Comparing `myslideslive-0.6/myslideslive/_nbdev.py` & `myslideslive-0.7/myslideslive/_nbdev.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
          "YODA_CDN": "slideslive.ipynb",
          "RS_CDN": "slideslive.ipynb",
          "SIZE_MAP": "slideslive.ipynb",
          "url2id": "slideslive.ipynb",
          "get_sl_info": "slideslive.ipynb",
          "parse_slide_xml": "slideslive.ipynb",
          "get_slide_metadata": "slideslive.ipynb",
+         "prune_video_chunks": "slideslive.ipynb",
          "get_urls": "slideslive.ipynb",
          "download_slides": "slideslive.ipynb",
          "ffmpeg_concat_script": "slideslive.ipynb",
          "compose_ffmpeg_video": "slideslive.ipynb",
          "SlidesLive": "slideslive.ipynb"}
 
 modules = ["cli.py",
```

### Comparing `myslideslive-0.6/myslideslive/cli.py` & `myslideslive-0.7/myslideslive/cli.py`

 * *Files identical despite different names*

### Comparing `myslideslive-0.6/myslideslive/slideslive.py` & `myslideslive-0.7/myslideslive/slideslive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: src/slideslive.ipynb (unless otherwise specified).
 
 __all__ = ['SL_REGEX', 'SL_INFO', 'SL_HTML', 'SL_CDN', 'YODA_CDN', 'RS_CDN', 'SIZE_MAP', 'url2id', 'get_sl_info',
-           'parse_slide_xml', 'get_slide_metadata', 'get_urls', 'download_slides', 'ffmpeg_concat_script',
-           'compose_ffmpeg_video', 'SlidesLive']
+           'parse_slide_xml', 'get_slide_metadata', 'prune_video_chunks', 'get_urls', 'download_slides',
+           'ffmpeg_concat_script', 'compose_ffmpeg_video', 'SlidesLive']
 
 # Cell
 #export
 import json
 import os
 import re
 import requests
@@ -159,14 +159,52 @@
                                           'image': {'name': d['slideName']}}
                       for d in meta_data_}
         meta_data = {'slides': [meta_data_[i] for i in sorted(meta_data_.keys())]}
 
     return meta_data
 
 # Cell
+def prune_video_chunks(meta_data):
+    """
+    Replace video chunks in the slide metadata with static images.
+    """
+    pruned_meta_data = dict(meta_data)
+    slides = list(pruned_meta_data['slides'])
+    pruned_slides = []
+
+    time = None
+    for s in slides:
+        slide_type = s.get('type')
+        # catch the first video in a sequence
+        if slide_type == 'video' and time is None:
+            # memorise time
+            time = s['time']
+        # catch the n-th video in a sequence
+        elif slide_type == 'video' and time is not None:
+            # we already have the starting time so we can continue
+            continue
+        # catch first image after a video chunk
+        elif slide_type != 'video' and time is not None:
+            # override the start time with the time of the first video chunk
+            s_ = dict(s)
+            s_['time'] = time
+            time = None
+            pruned_slides.append(s_)
+        else:
+            assert time is None
+            pruned_slides.append(s)
+
+    if time is not None:
+        raise RuntimeError('A video chunk cannot be last '
+                           '(i.e., without an image that follows)')
+
+    pruned_meta_data['slides'] = pruned_slides
+    return pruned_meta_data
+
+# Cell
 def get_urls(video_id, slide_meta, slide_type='xlarge', slide_format='png',
              slide=(None, None), time=(None, None)):
     """
     Composes a list of URLs for slides of a given SlidesLive presentation.
 
     `video_id` specifies the ID of a SlidesLive presentation.
     `slide_meta` is the metadata of a SlidesLive presentation
@@ -593,15 +631,19 @@
         else:
             try_json = False
 
         # raise an error if both failed
         if not try_xml and not try_json:
             raise RuntimeError('Failed to retrieve XML or JSON slides metadata')
 
-        self.video_metadata = meta
+        # prune video chunks in the slides
+        # TODO: use the video chunks instead of replacing them with static images
+        meta_image_only = prune_video_chunks(meta)
+
+        self.video_metadata = meta_image_only
 
     def get_slide_urls(self, slide_type='xlarge', slide=None, time=None):
         """Returns a list of slide URLs -- see `get_urls` for more details."""
         if self.slide is None and slide is None:
             self.slide = (None, None)
         elif self.slide is None and slide is not None:
             self.slide = slide
```

### Comparing `myslideslive-0.6/myslideslive.egg-info/PKG-INFO` & `myslideslive-0.7/myslideslive.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myslideslive
-Version: 0.6
+Version: 0.7
 Summary: Download the (video) slides of your SlidesLive talk
 Home-page: https://github.com/So-Cool/myslideslive/tree/master/
 Author: Kacper Sokol
 Author-email: dev@kcpr.me
 License: BSD License
 Description: # mySlidesLive
         > ...helps you to extract your SlidesLive presentation.
@@ -51,15 +51,15 @@
         Directly from terminal:
         ```bash
         msl --slide 1074 1075 \
         https://slideslive.com/38956531/beyond-static-papers-rethinking-how-we-share-scientific-understanding-in-ml
         ```
         
         ## Development
-        - To develop this package you need [nbdev] v1 (`pip install "nbdev<2"`).
+        - To develop this package you need [nbdev] v1 and [unidecode] (`pip install "nbdev<2" unidecode`).
         - The library (and `Makefile`) is built with `nbdev_build_lib`.
         - `nbdev_update_lib` updates the notebooks based on changes in the library.
         - The `README.md` is regenerated with `nbdev_build_docs`.
         - The git hooks are set up with `nbdev_install_git_hooks`.
         - `jupyter nbconvert --clear-output --inplace notebook.ipynb` clears all output cells of a notebook.
         
         Before committing code changes make sure to run:
@@ -68,14 +68,15 @@
         nbdev_build_lib && \
         nbdev_build_docs && \
         nbdev_clean_nbs --clear_all True && \
         nbdev_test_nbs
         ```
         
         [nbdev]: https://nbdev.fast.ai/
+        [unidecode]: https://github.com/avian2/unidecode
         
         ## What about the SlidesLive video recording?
         If you want to get the video recording of your SlidesLive presentation as well,
         [youtube-dl] can take care of that.
         
         ## Cutting the video
         Then you can cut the video with:
```

### Comparing `myslideslive-0.6/settings.ini` & `myslideslive-0.7/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 lib_name = myslideslive
 
 user = So-Cool
 description = Download the (video) slides of your SlidesLive talk
 keywords = SlidesLive
 author = Kacper Sokol
 author_email = dev@kcpr.me
-copyright = %(author)s 2021 (%(license)s)
+copyright = %(author)s 2024 (%(license)s)
 branch = master
-version = 0.6
+version = 0.7
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = BSD3
```

### Comparing `myslideslive-0.6/setup.py` & `myslideslive-0.7/setup.py`

 * *Files identical despite different names*

