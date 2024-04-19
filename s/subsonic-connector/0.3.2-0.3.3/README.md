# Comparing `tmp/subsonic_connector-0.3.2.tar.gz` & `tmp/subsonic_connector-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsonic_connector-0.3.2.tar", max compression
+gzip compressed data, was "subsonic_connector-0.3.3.tar", max compression
```

## Comparing `subsonic_connector-0.3.2.tar` & `subsonic_connector-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1071 2023-06-05 17:56:34.461154 subsonic_connector-0.3.2/LICENSE
--rw-r--r--   0        0        0     1015 2023-06-05 17:56:34.465154 subsonic_connector-0.3.2/README.md
--rw-r--r--   0        0        0      908 2024-02-05 18:22:38.839149 subsonic_connector-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 17:56:34.465154 subsonic_connector-0.3.2/subsonic_connector/__init__.py
--rw-r--r--   0        0        0     3153 2024-02-05 18:22:38.839149 subsonic_connector-0.3.2/subsonic_connector/album.py
--rw-r--r--   0        0        0      297 2023-11-06 18:53:44.080455 subsonic_connector-0.3.2/subsonic_connector/album_list.py
--rw-r--r--   0        0        0     1246 2023-11-24 18:19:04.084670 subsonic_connector-0.3.2/subsonic_connector/artist.py
--rw-r--r--   0        0        0      449 2023-11-06 18:53:44.080455 subsonic_connector-0.3.2/subsonic_connector/artist_cover.py
--rw-r--r--   0        0        0     1448 2023-11-24 18:19:04.084670 subsonic_connector-0.3.2/subsonic_connector/artist_info.py
--rw-r--r--   0        0        0      575 2023-11-24 18:19:04.084670 subsonic_connector-0.3.2/subsonic_connector/artist_list_item.py
--rw-r--r--   0        0        0      389 2023-11-24 18:19:04.084670 subsonic_connector-0.3.2/subsonic_connector/artists.py
--rw-r--r--   0        0        0      460 2023-11-24 18:19:04.084670 subsonic_connector-0.3.2/subsonic_connector/artists_initial.py
--rw-r--r--   0        0        0     1256 2023-11-19 11:57:02.427483 subsonic_connector-0.3.2/subsonic_connector/configuration.py
--rw-r--r--   0        0        0    10725 2023-12-06 14:56:36.310212 subsonic_connector-0.3.2/subsonic_connector/connector.py
--rw-r--r--   0        0        0     1215 2023-11-19 11:57:02.431483 subsonic_connector-0.3.2/subsonic_connector/default_config.py
--rw-r--r--   0        0        0      408 2023-11-24 18:19:04.084670 subsonic_connector-0.3.2/subsonic_connector/genre.py
--rw-r--r--   0        0        0      338 2023-11-24 18:19:04.084670 subsonic_connector-0.3.2/subsonic_connector/genres.py
--rw-r--r--   0        0        0      496 2023-11-24 18:19:04.084670 subsonic_connector-0.3.2/subsonic_connector/internet_radio_station.py
--rw-r--r--   0        0        0      447 2023-11-24 18:19:04.084670 subsonic_connector-0.3.2/subsonic_connector/internet_radio_stations.py
--rw-r--r--   0        0        0     1686 2024-02-05 18:22:38.839149 subsonic_connector-0.3.2/subsonic_connector/item.py
--rw-r--r--   0        0        0      521 2023-06-05 17:56:34.465154 subsonic_connector-0.3.2/subsonic_connector/list_type.py
--rw-r--r--   0        0        0      590 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/multi_value.py
--rw-r--r--   0        0        0     1681 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/playlist.py
--rw-r--r--   0        0        0     1776 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/playlist_entry.py
--rw-r--r--   0        0        0      362 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/playlists.py
--rw-r--r--   0        0        0      342 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/random_songs.py
--rw-r--r--   0        0        0      542 2023-06-07 15:30:45.107952 subsonic_connector-0.3.2/subsonic_connector/response.py
--rw-r--r--   0        0        0      806 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/search_result.py
--rw-r--r--   0        0        0      316 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/similar_artist.py
--rw-r--r--   0        0        0      345 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/similar_songs.py
--rw-r--r--   0        0        0     2609 2023-11-29 17:25:26.128264 subsonic_connector-0.3.2/subsonic_connector/song.py
--rw-r--r--   0        0        0      707 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/starred.py
--rw-r--r--   0        0        0      336 2023-11-24 18:19:04.088670 subsonic_connector-0.3.2/subsonic_connector/top_songs.py
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 subsonic_connector-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 17:56:34.461154 subsonic_connector-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1015 2023-06-05 17:56:34.465154 subsonic_connector-0.3.3/README.md
+-rw-r--r--   0        0        0      907 2024-04-19 13:10:49.667352 subsonic_connector-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 17:56:34.465154 subsonic_connector-0.3.3/subsonic_connector/__init__.py
+-rw-r--r--   0        0        0     3153 2024-02-05 18:22:38.839149 subsonic_connector-0.3.3/subsonic_connector/album.py
+-rw-r--r--   0        0        0      297 2023-11-06 18:53:44.080455 subsonic_connector-0.3.3/subsonic_connector/album_list.py
+-rw-r--r--   0        0        0     1246 2023-11-24 18:19:04.084670 subsonic_connector-0.3.3/subsonic_connector/artist.py
+-rw-r--r--   0        0        0      449 2023-11-06 18:53:44.080455 subsonic_connector-0.3.3/subsonic_connector/artist_cover.py
+-rw-r--r--   0        0        0     1448 2023-11-24 18:19:04.084670 subsonic_connector-0.3.3/subsonic_connector/artist_info.py
+-rw-r--r--   0        0        0      575 2023-11-24 18:19:04.084670 subsonic_connector-0.3.3/subsonic_connector/artist_list_item.py
+-rw-r--r--   0        0        0      389 2023-11-24 18:19:04.084670 subsonic_connector-0.3.3/subsonic_connector/artists.py
+-rw-r--r--   0        0        0      460 2023-11-24 18:19:04.084670 subsonic_connector-0.3.3/subsonic_connector/artists_initial.py
+-rw-r--r--   0        0        0     1256 2023-11-19 11:57:02.427483 subsonic_connector-0.3.3/subsonic_connector/configuration.py
+-rw-r--r--   0        0        0    10725 2023-12-06 14:56:36.310212 subsonic_connector-0.3.3/subsonic_connector/connector.py
+-rw-r--r--   0        0        0     1215 2023-11-19 11:57:02.431483 subsonic_connector-0.3.3/subsonic_connector/default_config.py
+-rw-r--r--   0        0        0      408 2023-11-24 18:19:04.084670 subsonic_connector-0.3.3/subsonic_connector/genre.py
+-rw-r--r--   0        0        0      338 2023-11-24 18:19:04.084670 subsonic_connector-0.3.3/subsonic_connector/genres.py
+-rw-r--r--   0        0        0      496 2023-11-24 18:19:04.084670 subsonic_connector-0.3.3/subsonic_connector/internet_radio_station.py
+-rw-r--r--   0        0        0      447 2023-11-24 18:19:04.084670 subsonic_connector-0.3.3/subsonic_connector/internet_radio_stations.py
+-rw-r--r--   0        0        0     1686 2024-02-05 18:22:38.839149 subsonic_connector-0.3.3/subsonic_connector/item.py
+-rw-r--r--   0        0        0      521 2023-06-05 17:56:34.465154 subsonic_connector-0.3.3/subsonic_connector/list_type.py
+-rw-r--r--   0        0        0      590 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/multi_value.py
+-rw-r--r--   0        0        0     1681 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/playlist.py
+-rw-r--r--   0        0        0     1776 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/playlist_entry.py
+-rw-r--r--   0        0        0      362 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/playlists.py
+-rw-r--r--   0        0        0      342 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/random_songs.py
+-rw-r--r--   0        0        0      542 2023-06-07 15:30:45.107952 subsonic_connector-0.3.3/subsonic_connector/response.py
+-rw-r--r--   0        0        0      806 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/search_result.py
+-rw-r--r--   0        0        0      316 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/similar_artist.py
+-rw-r--r--   0        0        0      345 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/similar_songs.py
+-rw-r--r--   0        0        0     2609 2023-11-29 17:25:26.128264 subsonic_connector-0.3.3/subsonic_connector/song.py
+-rw-r--r--   0        0        0      707 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/starred.py
+-rw-r--r--   0        0        0      336 2023-11-24 18:19:04.088670 subsonic_connector-0.3.3/subsonic_connector/top_songs.py
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 subsonic_connector-0.3.3/PKG-INFO
```

### Comparing `subsonic_connector-0.3.2/LICENSE` & `subsonic_connector-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/README.md` & `subsonic_connector-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/pyproject.toml` & `subsonic_connector-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 [project.urls]
 "Homepage" = "https://github.com/GioF71/subsonic-connector"
 "Bug Tracker" = "https://github.com/GioF71/subsonic-connector/issues"
 
 [tool.poetry]
 name = "subsonic-connector"
-version = "0.3.2"
+version = "0.3.3"
 description = "SubSonic Connector based on py-sonic"
 authors = ["GioF71 <giovanni.fulco@gmail.com>"]
 readme = "README.md"
 packages = [{include = "subsonic_connector"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-py-sonic = "^1.0.0"
+py-sonic = "1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `subsonic_connector-0.3.2/subsonic_connector/album.py` & `subsonic_connector-0.3.3/subsonic_connector/album.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/artist.py` & `subsonic_connector-0.3.3/subsonic_connector/artist.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/artist_info.py` & `subsonic_connector-0.3.3/subsonic_connector/artist_info.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/artist_list_item.py` & `subsonic_connector-0.3.3/subsonic_connector/artist_list_item.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/configuration.py` & `subsonic_connector-0.3.3/subsonic_connector/configuration.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/connector.py` & `subsonic_connector-0.3.3/subsonic_connector/connector.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/default_config.py` & `subsonic_connector-0.3.3/subsonic_connector/default_config.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/item.py` & `subsonic_connector-0.3.3/subsonic_connector/item.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/list_type.py` & `subsonic_connector-0.3.3/subsonic_connector/list_type.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/multi_value.py` & `subsonic_connector-0.3.3/subsonic_connector/multi_value.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/playlist.py` & `subsonic_connector-0.3.3/subsonic_connector/playlist.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/playlist_entry.py` & `subsonic_connector-0.3.3/subsonic_connector/playlist_entry.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/response.py` & `subsonic_connector-0.3.3/subsonic_connector/response.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/search_result.py` & `subsonic_connector-0.3.3/subsonic_connector/search_result.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/song.py` & `subsonic_connector-0.3.3/subsonic_connector/song.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/subsonic_connector/starred.py` & `subsonic_connector-0.3.3/subsonic_connector/starred.py`

 * *Files identical despite different names*

### Comparing `subsonic_connector-0.3.2/PKG-INFO` & `subsonic_connector-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: subsonic-connector
-Version: 0.3.2
+Version: 0.3.3
 Summary: SubSonic Connector based on py-sonic
 Author: GioF71
 Author-email: giovanni.fulco@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: py-sonic (>=1.0.0,<2.0.0)
+Requires-Dist: py-sonic (==1.0.0)
 Description-Content-Type: text/markdown
 
 # Subsonic Connector
 
 ## Reference
 
 This library relies on the [py-sonic](https://github.com/crustymonkey/py-sonic) project.
```

