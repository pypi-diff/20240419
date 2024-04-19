# Comparing `tmp/instagram-dlpy-1.1.0.tar.gz` & `tmp/instagram-dlpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram-dlpy-1.1.0.tar", last modified: Tue Apr  9 22:16:57 2024, max compression
+gzip compressed data, was "instagram-dlpy-1.2.0.tar", last modified: Fri Apr 19 09:06:11 2024, max compression
```

## Comparing `instagram-dlpy-1.1.0.tar` & `instagram-dlpy-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-09 22:16:57.180484 instagram-dlpy-1.1.0/
--rw-r--r--   0 becky      (501) staff       (20)    34888 2024-03-28 00:53:11.000000 instagram-dlpy-1.1.0/LICENSE
--rw-r--r--   0 becky      (501) staff       (20)     1347 2024-04-09 22:16:57.180411 instagram-dlpy-1.1.0/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      617 2024-03-28 00:54:03.000000 instagram-dlpy-1.1.0/README.md
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-09 22:16:57.180229 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/
--rw-r--r--   0 becky      (501) staff       (20)     1347 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      331 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/SOURCES.txt
--rw-r--r--   0 becky      (501) staff       (20)        1 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/dependency_links.txt
--rw-r--r--   0 becky      (501) staff       (20)        9 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/requires.txt
--rw-r--r--   0 becky      (501) staff       (20)       12 2024-04-09 22:16:57.000000 instagram-dlpy-1.1.0/instagram_dlpy.egg-info/top_level.txt
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-09 22:16:57.179922 instagram-dlpy-1.1.0/instagramdl/
--rw-r--r--   0 becky      (501) staff       (20)        0 2023-06-21 12:21:02.000000 instagram-dlpy-1.1.0/instagramdl/__init__.py
--rw-r--r--   0 becky      (501) staff       (20)     2473 2024-03-28 00:53:11.000000 instagram-dlpy-1.1.0/instagramdl/api.py
--rw-r--r--   0 becky      (501) staff       (20)     3723 2024-04-09 22:14:48.000000 instagram-dlpy-1.1.0/instagramdl/models.py
--rw-r--r--   0 becky      (501) staff       (20)     6974 2024-03-28 00:53:11.000000 instagram-dlpy-1.1.0/instagramdl/parser.py
--rw-r--r--   0 becky      (501) staff       (20)       79 2024-04-09 22:16:57.180662 instagram-dlpy-1.1.0/setup.cfg
--rw-r--r--   0 becky      (501) staff       (20)     1022 2024-04-09 22:15:34.000000 instagram-dlpy-1.1.0/setup.py
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-09 22:16:57.180053 instagram-dlpy-1.1.0/tests/
--rw-r--r--   0 becky      (501) staff       (20)     3740 2024-03-28 00:53:11.000000 instagram-dlpy-1.1.0/tests/test_urls.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-19 09:06:11.651701 instagram-dlpy-1.2.0/
+-rw-r--r--   0 becky      (501) staff       (20)    34888 2024-03-28 00:53:11.000000 instagram-dlpy-1.2.0/LICENSE
+-rw-r--r--   0 becky      (501) staff       (20)     1446 2024-04-19 09:06:11.651629 instagram-dlpy-1.2.0/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      617 2024-03-28 00:54:03.000000 instagram-dlpy-1.2.0/README.md
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-19 09:06:11.651380 instagram-dlpy-1.2.0/instagram_dlpy.egg-info/
+-rw-r--r--   0 becky      (501) staff       (20)     1446 2024-04-19 09:06:11.000000 instagram-dlpy-1.2.0/instagram_dlpy.egg-info/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      331 2024-04-19 09:06:11.000000 instagram-dlpy-1.2.0/instagram_dlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 becky      (501) staff       (20)        1 2024-04-19 09:06:11.000000 instagram-dlpy-1.2.0/instagram_dlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 becky      (501) staff       (20)       45 2024-04-19 09:06:11.000000 instagram-dlpy-1.2.0/instagram_dlpy.egg-info/requires.txt
+-rw-r--r--   0 becky      (501) staff       (20)       12 2024-04-19 09:06:11.000000 instagram-dlpy-1.2.0/instagram_dlpy.egg-info/top_level.txt
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-19 09:06:11.650876 instagram-dlpy-1.2.0/instagramdl/
+-rw-r--r--   0 becky      (501) staff       (20)        0 2023-06-21 12:21:02.000000 instagram-dlpy-1.2.0/instagramdl/__init__.py
+-rw-r--r--   0 becky      (501) staff       (20)     2567 2024-04-17 10:38:59.000000 instagram-dlpy-1.2.0/instagramdl/api.py
+-rw-r--r--   0 becky      (501) staff       (20)     3802 2024-04-17 11:04:37.000000 instagram-dlpy-1.2.0/instagramdl/models.py
+-rw-r--r--   0 becky      (501) staff       (20)     7024 2024-04-17 10:41:19.000000 instagram-dlpy-1.2.0/instagramdl/parser.py
+-rw-r--r--   0 becky      (501) staff       (20)       79 2024-04-19 09:06:11.651910 instagram-dlpy-1.2.0/setup.cfg
+-rw-r--r--   0 becky      (501) staff       (20)     1172 2024-04-17 11:01:30.000000 instagram-dlpy-1.2.0/setup.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2024-04-19 09:06:11.651197 instagram-dlpy-1.2.0/tests/
+-rw-r--r--   0 becky      (501) staff       (20)     3740 2024-03-28 00:53:11.000000 instagram-dlpy-1.2.0/tests/test_urls.py
```

### Comparing `instagram-dlpy-1.1.0/LICENSE` & `instagram-dlpy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `instagram-dlpy-1.1.0/PKG-INFO` & `instagram-dlpy-1.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: instagram-dlpy
-Version: 1.1.0
+Version: 1.2.0
 Summary: A python package to download Instagram posts by URL without needing to login
 Home-page: https://github.com/Fluxticks/InstagramDL
-Download-URL: https://github.com/Fluxticks/InstagramDL/archive/v1.1.0.tar.gz
+Download-URL: https://github.com/Fluxticks/InstagramDL/archive/v1.2.0.tar.gz
 Author: Fluxticks
 Keywords: instagram,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: StrEnum; python_version < "3.11"
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/instagram-dlpy)
 
 # InstagramDL
 
 A python package to download Instagram posts by URL without needing to login.
```

### Comparing `instagram-dlpy-1.1.0/README.md` & `instagram-dlpy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `instagram-dlpy-1.1.0/instagram_dlpy.egg-info/PKG-INFO` & `instagram-dlpy-1.2.0/instagram_dlpy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: instagram-dlpy
-Version: 1.1.0
+Version: 1.2.0
 Summary: A python package to download Instagram posts by URL without needing to login
 Home-page: https://github.com/Fluxticks/InstagramDL
-Download-URL: https://github.com/Fluxticks/InstagramDL/archive/v1.1.0.tar.gz
+Download-URL: https://github.com/Fluxticks/InstagramDL/archive/v1.2.0.tar.gz
 Author: Fluxticks
 Keywords: instagram,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: StrEnum; python_version < "3.11"
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/instagram-dlpy)
 
 # InstagramDL
 
 A python package to download Instagram posts by URL without needing to login.
```

### Comparing `instagram-dlpy-1.1.0/instagramdl/api.py` & `instagram-dlpy-1.2.0/instagramdl/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,26 +30,29 @@
 
     Args:
         post_url (str): The URL to get the data from.
 
     Returns:
         Dict: The raw data returned from the API request.
     """
+    parsed_url = urlparse(post_url)
+    url = f"{parsed_url.scheme}://{parsed_url.netloc}{parsed_url.path}"
+
     headers = {
         "User-Agent": make_random_string(10),
         "Accept": "*/*",
         "Accept-Language": "en-US,en;q=0.5",
-        "Referer": post_url,
+        "Referer": url,
         "Content-Type": "application/x-www-form-urlencoded",
         "Origin": "https://www.instagram.com",
         "Sec-Fetch-Site": "same-origin",
     }
 
-    parts = post_url.split("/")
-    if post_url.endswith("/"):
+    parts = url.split("/")
+    if url.endswith("/"):
         short_code = parts[-2]
     else:
         short_code = parts[-1]
 
     data = f"__hs={make_random_string(10)}&lsd={make_random_string(11)}&variables=%7B%22shortcode%22:%22{short_code}%22%7D&doc_id={MAGIC_DOC_NUMBER}"
 
     response = requests.post(
```

### Comparing `instagram-dlpy-1.1.0/instagramdl/models.py` & `instagram-dlpy-1.2.0/instagramdl/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 from dataclasses import dataclass
-from enum import StrEnum
+
+try:
+    from enum import StrEnum
+except ImportError:
+    from strenum import StrEnum  # type: ignore
+
 from typing import List, Optional, Union
 
 from instagramdl.api import download_file
 
 
 @dataclass()
 class User:
```

### Comparing `instagram-dlpy-1.1.0/instagramdl/parser.py` & `instagram-dlpy-1.2.0/instagramdl/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,20 +150,19 @@
     width = dimensions.get("width")
     height = dimensions.get("height")
 
     # Get post interactions
     comment_count = api_response.get("edge_media_to_comment").get("count")
     like_count = api_response.get("edge_media_preview_like").get("count")
 
-    post_caption = (
-        api_response.get("edge_media_to_caption")
-        .get("edges")[0]
-        .get("node")
-        .get("text")
-    )
+    caption_data = api_response.get("edge_media_to_caption").get("edges")
+    if caption_data:
+        post_caption = caption_data[0].get("node").get("text")
+    else:
+        post_caption = ""
 
     timestamp = api_response.get("taken_at_timestamp")
 
     owner = parse_user(api_response)
 
     return Post(
         id=post_id,
```

### Comparing `instagram-dlpy-1.1.0/setup.py` & `instagram-dlpy-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,32 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="instagram-dlpy",
-    version="1.1.0",
+    version="1.2.0",
     url="https://github.com/Fluxticks/InstagramDL",
-    download_url="https://github.com/Fluxticks/InstagramDL/archive/v1.1.0.tar.gz",
+    download_url="https://github.com/Fluxticks/InstagramDL/archive/v1.2.0.tar.gz",
     author="Fluxticks",
     packages=find_packages(),
     install_requires=["requests"],
+    extras_require={
+        ':python_version < "3.11"': [
+            "StrEnum",
+        ],
+    },
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="A python package to download Instagram posts by URL without needing to login",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords=["instagram", "api"],
 )
```

### Comparing `instagram-dlpy-1.1.0/tests/test_urls.py` & `instagram-dlpy-1.2.0/tests/test_urls.py`

 * *Files identical despite different names*

