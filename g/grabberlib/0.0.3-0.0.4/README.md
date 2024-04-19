# Comparing `tmp/grabberlib-0.0.3.tar.gz` & `tmp/grabberlib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.0.3.tar", max compression
+gzip compressed data, was "grabberlib-0.0.4.tar", max compression
```

## Comparing `grabberlib-0.0.3.tar` & `grabberlib-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0        0 2024-04-18 15:32:29.439621 grabberlib-0.0.3/README.md
--rw-r--r--   0        0        0     6140 2024-04-18 21:16:51.421239 grabberlib-0.0.3/assets/pages.txt
--rw-r--r--   0        0        0        0 2024-04-15 17:38:47.146959 grabberlib-0.0.3/grabber/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-18 21:14:28.281973 grabberlib-0.0.3/grabber/__main__.py
--rw-r--r--   0        0        0        0 2024-04-18 20:26:25.002814 grabberlib-0.0.3/grabber/controllers/__init__.py
--rw-r--r--   0        0        0     2831 2024-04-18 21:14:28.281125 grabberlib-0.0.3/grabber/controllers/base.py
--rw-r--r--   0        0        0        0 2024-04-18 20:26:36.846498 grabberlib-0.0.3/grabber/core/__init__.py
--rw-r--r--   0        0        0       65 2024-04-18 21:14:28.281820 grabberlib-0.0.3/grabber/core/exc.py
--rw-r--r--   0        0        0      181 2024-04-17 22:05:44.064553 grabberlib-0.0.3/grabber/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-18 20:50:40.150458 grabberlib-0.0.3/grabber/core/sources/__init__.py
--rw-r--r--   0        0        0     3545 2024-04-18 21:14:28.282154 grabberlib-0.0.3/grabber/core/sources/graph.py
--rw-r--r--   0        0        0     4083 2024-04-18 21:14:28.282411 grabberlib-0.0.3/grabber/core/sources/khd.py
--rw-r--r--   0        0        0     3671 2024-04-18 21:14:28.282077 grabberlib-0.0.3/grabber/core/sources/xasiat.py
--rw-r--r--   0        0        0     1721 2024-04-18 21:14:28.281979 grabberlib-0.0.3/grabber/core/sources/yellow.py
--rw-r--r--   0        0        0     9248 2024-04-18 21:14:28.282016 grabberlib-0.0.3/grabber/core/utils.py
--rw-r--r--   0        0        0      175 2024-04-18 21:14:28.281457 grabberlib-0.0.3/grabber/core/version.py
--rw-r--r--   0        0        0        0 2024-04-18 20:28:10.854369 grabberlib-0.0.3/grabber/templates/__init__.py
--rw-r--r--   0        0        0     1017 2024-04-18 21:17:12.932509 grabberlib-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 15:32:29.439621 grabberlib-0.0.4/README.md
+-rw-r--r--   0        0        0     6702 2024-04-18 21:25:26.788330 grabberlib-0.0.4/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-15 17:38:47.146959 grabberlib-0.0.4/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-18 21:14:28.281973 grabberlib-0.0.4/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:26:25.002814 grabberlib-0.0.4/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     2844 2024-04-19 13:19:11.652567 grabberlib-0.0.4/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:26:36.846498 grabberlib-0.0.4/grabber/core/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-18 21:14:28.281820 grabberlib-0.0.4/grabber/core/exc.py
+-rw-r--r--   0        0        0      181 2024-04-17 22:05:44.064553 grabberlib-0.0.4/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:50:40.150458 grabberlib-0.0.4/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:18:21.758961 grabberlib-0.0.4/grabber/core/sources/common.py
+-rw-r--r--   0        0        0     3545 2024-04-18 21:14:28.282154 grabberlib-0.0.4/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     4083 2024-04-18 21:14:28.282411 grabberlib-0.0.4/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3671 2024-04-18 21:14:28.282077 grabberlib-0.0.4/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     1721 2024-04-18 21:14:28.281979 grabberlib-0.0.4/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0    10587 2024-04-19 12:51:10.359256 grabberlib-0.0.4/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-04-19 13:19:25.126511 grabberlib-0.0.4/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:28:10.854369 grabberlib-0.0.4/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1017 2024-04-19 13:19:16.677717 grabberlib-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.4/PKG-INFO
```

### Comparing `grabberlib-0.0.3/assets/pages.txt` & `grabberlib-0.0.4/assets/pages.txt`

 * *Files 7% similar despite different names*

```diff
@@ -70,7 +70,12 @@
 
 Xingyan星颜社Vol: https://telegra.ph/Xingyan星颜社Vol-04-18
 
 
 01 Yuuhui玉汇 No.019 间谍过家家 约尔·福杰[402Mb 44Photos] : https://telegra.ph/01-Yuuhui玉汇-No019-间谍过家家-约尔福杰402Mb-44Photos-04-18
 02 Yuuhui玉汇 No.018 圣女の史莱姆修行计划(986Mb)(106Photos) : https://telegra.ph/02-Yuuhui玉汇-No018-圣女の史莱姆修行计划986Mb106Photos-04-18
 03 Yuuhui玉汇 No.017 熊猫女仆(510Mb)(30Photos) : https://telegra.ph/03-Yuuhui玉汇-No017-熊猫女仆510Mb30Photos-04-18
+01 女主K 快递员[139Mb 100Photos] : https://telegra.ph/01-女主K-快递员139Mb-100Photos-04-18
+02 女主K   性感水手服妹妹[58Mb 23Photos] : https://telegra.ph/02-女主K-性感水手服妹妹58Mb-23Photos-04-18
+03 Cosplay 女主K – 白双子[263Mb 75Photos] : https://telegra.ph/03-Cosplay-女主K--白双子263Mb-75Photos-04-18
+04 女主K 性感一夏[237Mb 97Photos] : https://telegra.ph/04-女主K-性感一夏237Mb-97Photos-04-18
+05 女主K   可爱的制服[322Mb 99Photos] : https://telegra.ph/05-女主K-可爱的制服322Mb-99Photos-04-18
```

### Comparing `grabberlib-0.0.3/grabber/__main__.py` & `grabberlib-0.0.4/grabber/__main__.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.3/grabber/controllers/base.py` & `grabberlib-0.0.4/grabber/controllers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,14 @@
             "4khd": get_sources_for_4khd,
             "telegraph": get_for_telegraph,
         }
 
         if upload:
             upload_folders_to_telegraph(folder_name=folder)
         else:
-            getter_images = getter_mapping.get(entity, None)
+            getter_images = getter_mapping.get(entity, get_for_telegraph)
             getter_images(
                 sources=sources,
                 entity=entity,
                 final_dest=folder,
                 save_to_telegraph=publish,
             )
```

### Comparing `grabberlib-0.0.3/grabber/core/sources/graph.py` & `grabberlib-0.0.4/grabber/core/sources/graph.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.3/grabber/core/sources/khd.py` & `grabberlib-0.0.4/grabber/core/sources/khd.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.3/grabber/core/sources/xasiat.py` & `grabberlib-0.0.4/grabber/core/sources/xasiat.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.3/grabber/core/sources/yellow.py` & `grabberlib-0.0.4/grabber/core/sources/yellow.py`

 * *Files identical despite different names*

### Comparing `grabberlib-0.0.3/grabber/core/utils.py` & `grabberlib-0.0.4/grabber/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,30 @@
 import pathlib
 import shutil
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 from bs4 import BeautifulSoup, Tag
 from casefy.casefy import snakecase
+from lxml import etree
 from PIL import Image
 from telegraph import Telegraph
 from telegraph.exceptions import TelegraphException
 from tenacity import retry, wait_chain, wait_fixed
 from tqdm import tqdm
 
 from grabber.core.settings import MEDIA_ROOT
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
+PAGINATION_QUERY = "div.jeg_navigation.jeg_pagination"
+PAGINATION_PAGES_COUNT_QUERY = f"{PAGINATION_QUERY} span.page_info"
+PAGINATION_BASE_URL_QUERY = "div.jeg_navigation.jeg_pagination a.page_number"
+POSTS_QUERY_XPATH = "/html/body/div[2]/div[5]/div/div[1]/div/div/div[2]/div/div/div[2]/div/div[1]/div/div/div/article/div/div/a"
+
+
 first_query = "div.content-inner img"
 
 
 query_mapping = {
     "xiuren": ("div.content-inner img", "src"),
     "nudebird": ("div.thecontent a", "href"),
     "nudecosplay": ("div.content-inner img", "src"),
@@ -270,7 +277,38 @@
                     folders = root_folders
 
     for folder in folders:
         upload_to_telegraph(folder)
 
     with open("assets/pages.txt", "a") as f:
         f.write("\n\n\n")
+
+
+def get_pages_from_pagination(url: str) -> List[str]:
+    source_urls = []
+    soup = get_soup(url)
+    dom = etree.HTML(str(soup))
+    pagination = soup.select(PAGINATION_PAGES_COUNT_QUERY)[0]
+    pagination_text = pagination.text
+    first, last = pagination_text.split("Page")[-1].strip().split("of")
+    first_page, last_page = int(first), int(last)
+
+    first_link_pagination = soup.select(PAGINATION_BASE_URL_QUERY)[0]
+    href = first_link_pagination.attrs["href"]
+    base_pagination_url = href.rsplit("/", 2)[0]
+
+    for a_tag in dom.xpath(POSTS_QUERY_XPATH):
+        source_urls.append(a_tag.attrib["href"])
+
+    for index in range(first_page, last_page + 1):
+        if index == 1:
+            continue
+
+        target_url = f"{base_pagination_url}/{index}/"
+
+        soup = get_soup(target_url)
+        dom = etree.HTML(str(soup))
+        source_urls.extend(
+            [a_tag.attrib["href"] for a_tag in dom.xpath(POSTS_QUERY_XPATH)]
+        )
+
+    return source_urls
```

### Comparing `grabberlib-0.0.3/pyproject.toml` & `grabberlib-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
     { include = "assets/pages.txt" },
 ]
```

### Comparing `grabberlib-0.0.3/PKG-INFO` & `grabberlib-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

