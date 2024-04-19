# Comparing `tmp/grabberlib-0.0.4.tar.gz` & `tmp/grabberlib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.0.4.tar", max compression
+gzip compressed data, was "grabberlib-0.0.5.tar", max compression
```

## Comparing `grabberlib-0.0.4.tar` & `grabberlib-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2024-04-18 15:32:29.439621 grabberlib-0.0.4/README.md
--rw-r--r--   0        0        0     6702 2024-04-18 21:25:26.788330 grabberlib-0.0.4/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-15 17:38:47.146959 grabberlib-0.0.4/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-18 21:14:28.281973 grabberlib-0.0.4/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-18 20:26:25.002814 grabberlib-0.0.4/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     2844 2024-04-19 13:19:11.652567 grabberlib-0.0.4/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-18 20:26:36.846498 grabberlib-0.0.4/grabber/core/__init__.py
--rw-r--r--   0        0        0       65 2024-04-18 21:14:28.281820 grabberlib-0.0.4/grabber/core/exc.py
--rw-r--r--   0        0        0      181 2024-04-17 22:05:44.064553 grabberlib-0.0.4/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-18 20:50:40.150458 grabberlib-0.0.4/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 13:18:21.758961 grabberlib-0.0.4/grabber/core/sources/common.py
--rw-r--r--   0        0        0     3545 2024-04-18 21:14:28.282154 grabberlib-0.0.4/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     4083 2024-04-18 21:14:28.282411 grabberlib-0.0.4/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3671 2024-04-18 21:14:28.282077 grabberlib-0.0.4/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     1721 2024-04-18 21:14:28.281979 grabberlib-0.0.4/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0    10587 2024-04-19 12:51:10.359256 grabberlib-0.0.4/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-04-19 13:19:25.126511 grabberlib-0.0.4/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-18 20:28:10.854369 grabberlib-0.0.4/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1017 2024-04-19 13:19:16.677717 grabberlib-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.061439 grabberlib-0.0.5/README.md
+-rw-r--r--   0        0        0        1 2024-04-19 21:08:54.051660 grabberlib-0.0.5/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.031593 grabberlib-0.0.5/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-19 16:44:36.314458 grabberlib-0.0.5/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.314537 grabberlib-0.0.5/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     3798 2024-04-19 21:11:49.668721 grabberlib-0.0.5/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.315102 grabberlib-0.0.5/grabber/core/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-19 16:44:36.315699 grabberlib-0.0.5/grabber/core/exc.py
+-rw-r--r--   0        0        0      188 2024-04-19 16:50:32.400947 grabberlib-0.0.5/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.316024 grabberlib-0.0.5/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3378 2024-04-19 17:11:11.625028 grabberlib-0.0.5/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     3986 2024-04-19 17:48:30.254982 grabberlib-0.0.5/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3588 2024-04-19 17:11:18.798709 grabberlib-0.0.5/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     3717 2024-04-19 17:10:44.092619 grabberlib-0.0.5/grabber/core/sources/xiuren.py
+-rw-r--r--   0        0        0        1 2024-04-19 16:44:36.392872 grabberlib-0.0.5/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    12856 2024-04-19 21:01:29.273811 grabberlib-0.0.5/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-04-19 21:09:53.350881 grabberlib-0.0.5/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:44:36.318014 grabberlib-0.0.5/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1017 2024-04-19 21:09:44.516801 grabberlib-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.5/PKG-INFO
```

### Comparing `grabberlib-0.0.4/grabber/__main__.py` & `grabberlib-0.0.5/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.4/grabber/controllers/base.py` & `grabberlib-0.0.5/grabber/controllers/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from cement import Controller, ex
 from cement.utils.version import get_version_banner
 
 from grabber.core.sources.graph import get_for_telegraph
 from grabber.core.sources.khd import get_sources_for_4khd
+from grabber.core.sources.xiuren import get_sources_for_xiuren
 from grabber.core.utils import upload_folders_to_telegraph
 
 from ..core.version import get_version
 
 VERSION_BANNER = """
-MyApp Does Amazing Things! %s
+A beautiful CLI utility to download images from the web! %s
 %s
 """ % (get_version(), get_version_banner())
 
 
 class Base(Controller):
     class Meta:
         label = "base"
 
         # text displayed at the top of --help output
-        description = "MyApp Does Amazing Things!"
+        description = "A beautiful CLI utility to download images from the web"
 
         # text displayed at the bottom of --help output
-        epilog = "Usage: test command1 --foo bar"
+        epilog = "Usage: grabber --entity 4khd --folder 4khd --publish --sources <list of links>"
 
         # controller level arguments. ex: 'test --version'
         arguments = [
             ### add a version banner
             (
                 ["-e", "--entity"],
                 {
@@ -49,14 +50,23 @@
                     "dest": "folder",
                     "default": "",
                     "type": str,
                     "help": "Folder where to save",
                 },
             ),
             (
+                ["-l", "--limit"],
+                {
+                    "dest": "limit",
+                    "type": int,
+                    "help": "Limit the amount of posts retrieved (used altogether with --tag)",
+                    "default": 0,
+                },
+            ),
+            (
                 ["-p", "--publish"],
                 {
                     "dest": "publish",
                     "action": "store_true",
                     "help": "Publish page to telegraph",
                 },
             ),
@@ -64,34 +74,47 @@
                 ["-u", "--upload"],
                 {
                     "dest": "upload",
                     "action": "store_true",
                     "help": "Upload and publish folders to telegraph",
                 },
             ),
+            (
+                ["-t", "--tag"],
+                {
+                    "dest": "is_tag",
+                    "action": "store_true",
+                    "help": "Indicates that the link(s) passed is a tag in which the posts are paginated",
+                },
+            ),
         ]
 
     @ex(hide=True)
     def _default(self):
         """Default action if no sub-command is passed."""
 
         entity = self.app.pargs.entity
         sources = self.app.pargs.sources
         folder = self.app.pargs.folder
         publish = self.app.pargs.publish
         upload = self.app.pargs.upload
+        is_tag = self.app.pargs.is_tag
+        limit = self.app.pargs.limit
 
         getter_mapping = {
             "4khd": get_sources_for_4khd,
             "telegraph": get_for_telegraph,
+            "xiuren": get_sources_for_xiuren,
         }
 
         if upload:
-            upload_folders_to_telegraph(folder_name=folder)
+            upload_folders_to_telegraph(folder_name=folder, limit=limit)
         else:
             getter_images = getter_mapping.get(entity, get_for_telegraph)
             getter_images(
                 sources=sources,
                 entity=entity,
                 final_dest=folder,
                 save_to_telegraph=publish,
+                is_tag=is_tag,
+                limit=limit,
             )
```

### Comparing `grabberlib-0.0.4/grabber/core/sources/graph.py` & `grabberlib-0.0.5/grabber/core/sources/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 def get_for_telegraph(
     sources: List[str],
     entity: str,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
+    **kwargs,
 ) -> None:
     titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
     )
     query, src_attr = query_mapping[entity]
@@ -39,26 +40,23 @@
         final_dest_folder = MEDIA_ROOT / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
-        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
         tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
         title_tag = soup.select("title")[0]  # type: ignore
         folder_name = title_tag.get_text().strip().rstrip()
-        image_index = f"{idx + 1}".zfill(2)
         title = folder_name
-        folder_name = f"{image_index}-{folder_name}"
         titles.add(title)
         titles_and_folders.add((title, folder_name))
 
         if final_dest:
             new_folder = MEDIA_ROOT / final_dest / folder_name
         else:
             new_folder = MEDIA_ROOT / folder_name
```

### Comparing `grabberlib-0.0.4/grabber/core/sources/khd.py` & `grabberlib-0.0.5/grabber/core/sources/xasiat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,118 @@
 import multiprocessing
 import pathlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
-from typing import List, Optional
+from typing import List
 
 from tqdm import tqdm
 
 from grabber.core.settings import MEDIA_ROOT
 from grabber.core.utils import (
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
-page_nav_query = "div.page-link-box li a.page-numbers"
 
 
-def get_pages_from_pagination(url: str, headers: Optional[dict] = None) -> List[str]:
-    tags, _ = get_tags(url, headers=headers, query=page_nav_query)
-    return [a.attrs["href"] for a in tags if tags]
-
-
-def get_sources_for_4khd(
+def get_for_xasiat(
     sources: List[str],
     entity: str,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
+    **kwargs,
 ) -> None:
     titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
-        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     folders = set()
     titles_and_folders = set()
     title_folder_mapping = {}
 
     if final_dest:
-        final_dest_folder = MEDIA_ROOT / pathlib.Path(final_dest)
+        final_dest_folder = MEDIA_ROOT / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
-        current_folder = None
-        current_title = None
         folder_name = ""
-        urls = [source_url, *get_pages_from_pagination(url=source_url, headers=headers)]
-        image_tags = []
-
-        for index, url in enumerate(urls):
-            tags, soup = get_tags(
-                url,
-                headers=headers,
-                query=query,
-            )
-            image_tags.extend(tags or [])
-
-            if index == 0:
-                folder_name = soup.select("title")[0].get_text()  # type: ignore
-                title = folder_name.strip().rstrip()
-                titles.add(title)
-                image_index = f"{idx + 1}".zfill(2)
-                folder_name = f"{image_index}-{folder_name}"
-                titles_and_folders.add((title, folder_name))
-                current_title = title
-
-        image_index = f"{idx + 1}".zfill(2)
-        folder_name = f"{image_index}-{folder_name}"
+        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
+        tags, soup = get_tags(
+            source_url,
+            headers=headers,
+            query=query,
+        )
+
+        title_tag = soup.select("title")[0]  # type: ignore
+        folder_name = title_tag.get_text().strip().rstrip()
+        title = folder_name
+        titles.add(title)
+        titles_and_folders.add((title, folder_name))
 
         if final_dest:
             new_folder = MEDIA_ROOT / final_dest / folder_name
         else:
             new_folder = MEDIA_ROOT / folder_name
 
         if not new_folder.exists():
             new_folder.mkdir(parents=True, exist_ok=True)
 
-        current_folder = new_folder
-        folders.add(current_folder)
+        folders.add(new_folder)
         unique_img_urls = set()
 
-        for idx, img_tag in enumerate(image_tags):
+        for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
-            img_name: str = img_src.split("/")[-1].split("?")[0]
-            img_name = img_name.strip().rstrip()
-            unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
-        title_folder_mapping[current_title] = (unique_img_urls, new_folder)
+
+            if "xasiat" in img_src:
+                img_name: str = img_src.split("/")[-2]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
+            else:
+                img_name: str = img_src.split("/")[-1]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
+
+            unique_img_urls.add(
+                (title, f"{idx + 1}.{img_extension}", img_src),
+            )
+
+        title_folder_mapping[title] = (unique_img_urls, new_folder)
 
     futures = []
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
         for title, (images_set, folder_dest) in title_folder_mapping.items():
             partial_download = partial(
                 download_images,
                 new_folder=folder_dest,
                 headers=headers,
                 title=title,
             )
-            future = executor.submit(partial_download, images_set)
+            future = executor.submit(partial_download, images_set, title=title)
             futures.append(future)
 
     for future in tqdm(
         futures,
         total=len(futures),
         desc="Finishing download...",
     ):
         future.result()
 
     if save_to_telegraph:
-        for title, (_, folder_dest) in title_folder_mapping.items():
-            upload_to_telegraph(folder_dest, page_title=title)
+        for folder in folders:
+            print(f"Uploading to telegraph {folder}")
+            upload_to_telegraph(folder)
 
     albums_message = "".join([f"- {title}\n" for title in titles])
     message = f"""
     All images have been downloaded and saved to the specified folder.
     Albums saved are the following:
         {albums_message}
     """
```

### Comparing `grabberlib-0.0.4/grabber/core/sources/xasiat.py` & `grabberlib-0.0.5/grabber/core/sources/xiuren.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,34 +4,39 @@
 from functools import partial
 from typing import List
 
 from tqdm import tqdm
 
 from grabber.core.settings import MEDIA_ROOT
 from grabber.core.utils import (
+    get_pages_from_pagination,
     query_mapping,
     headers_mapping,
     get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 
 
-def get_for_xasiat(
+def get_sources_for_xiuren(
     sources: List[str],
     entity: str,
     final_dest: str | pathlib.Path = "",
     save_to_telegraph: bool | None = False,
+    **kwargs,
 ) -> None:
     titles = set()
+    is_tag: bool = kwargs.get("is_tag", False)
+    limit: int = kwargs.get("limit", 0)
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
+        desc="Retrieving URLs...",
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
     folders = set()
     titles_and_folders = set()
     title_folder_mapping = {}
 
@@ -39,26 +44,34 @@
         final_dest_folder = MEDIA_ROOT / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
         folder_name = ""
-        tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
         tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
+        if is_tag:
+            urls = get_pages_from_pagination(url=source_url, target="xiuren")
+            targets = urls[:limit] if limit else urls
+            return get_sources_for_xiuren(
+                sources=targets,
+                entity=entity,
+                final_dest=final_dest,
+                save_to_telegraph=save_to_telegraph,
+                is_tag=False,
+            )
+
         title_tag = soup.select("title")[0]  # type: ignore
         folder_name = title_tag.get_text().strip().rstrip()
-        image_index = f"{idx + 1}".zfill(2)
         title = folder_name
-        folder_name = f"{image_index}-{folder_name}"
         titles.add(title)
         titles_and_folders.add((title, folder_name))
 
         if final_dest:
             new_folder = MEDIA_ROOT / final_dest / folder_name
         else:
             new_folder = MEDIA_ROOT / folder_name
@@ -67,53 +80,42 @@
             new_folder.mkdir(parents=True, exist_ok=True)
 
         folders.add(new_folder)
         unique_img_urls = set()
 
         for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
-
-            if "xasiat" in img_src:
-                img_name: str = img_src.split("/")[-2]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
-            else:
-                img_name: str = img_src.split("/")[-1]
-                img_name = img_name.strip().rstrip()
-                img_extension: str = img_name.split(".")[-1]
-
-            unique_img_urls.add(
-                (title, f"{idx + 1}.{img_extension}", img_src),
-            )
+            img_name: str = img_src.split("/")[-1]
+            img_name = img_name.strip().rstrip()
+            unique_img_urls.add((f"{idx + 1}-{img_name}", img_src))
 
         title_folder_mapping[title] = (unique_img_urls, new_folder)
 
     futures = []
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
         for title, (images_set, folder_dest) in title_folder_mapping.items():
             partial_download = partial(
                 download_images,
                 new_folder=folder_dest,
                 headers=headers,
                 title=title,
             )
-            future = executor.submit(partial_download, images_set, title=title)
+            future = executor.submit(partial_download, images_set)
             futures.append(future)
 
     for future in tqdm(
         futures,
         total=len(futures),
         desc="Finishing download...",
     ):
         future.result()
 
     if save_to_telegraph:
-        for folder in folders:
-            print(f"Uploading to telegraph {folder}")
-            upload_to_telegraph(folder)
+        for title, (_, folder_dest) in title_folder_mapping.items():
+            upload_to_telegraph(folder_dest, page_title=title)
 
     albums_message = "".join([f"- {title}\n" for title in titles])
     message = f"""
     All images have been downloaded and saved to the specified folder.
     Albums saved are the following:
         {albums_message}
     """
```

### Comparing `grabberlib-0.0.4/pyproject.toml` & `grabberlib-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.0.4/PKG-INFO` & `grabberlib-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

