# Comparing `tmp/pytorrentdl-1.0.2.tar.gz` & `tmp/pytorrentdl-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorrentdl-1.0.2.tar", last modified: Thu Apr 18 13:25:26 2024, max compression
+gzip compressed data, was "pytorrentdl-2.0.0.tar", last modified: Fri Apr 19 10:39:46 2024, max compression
```

## Comparing `pytorrentdl-1.0.2.tar` & `pytorrentdl-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 13:25:25.980951 pytorrentdl-1.0.2/
--rw-rw-rw-   0        0        0    12179 2024-04-18 14:36:08.000000 pytorrentdl-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     5121 2024-04-18 13:25:25.978951 pytorrentdl-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3982 2024-04-18 14:36:08.000000 pytorrentdl-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 13:25:25.920947 pytorrentdl-1.0.2/pytorrentdl/
--rw-rw-rw-   0        0        0      578 2024-04-18 13:23:15.000000 pytorrentdl-1.0.2/pytorrentdl/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-18 14:36:08.000000 pytorrentdl-1.0.2/pytorrentdl/cli.py
--rw-rw-rw-   0        0        0     3874 2024-04-18 13:22:54.000000 pytorrentdl-1.0.2/pytorrentdl/downloader.py
--rw-rw-rw-   0        0        0     1204 2024-04-18 14:36:08.000000 pytorrentdl-1.0.2/pytorrentdl/session.py
--rw-rw-rw-   0        0        0     1972 2024-04-18 11:53:32.000000 pytorrentdl-1.0.2/pytorrentdl/torrent_downloader.py
--rw-rw-rw-   0        0        0      470 2024-04-18 12:10:21.000000 pytorrentdl-1.0.2/pytorrentdl/torrent_info.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:25:25.971950 pytorrentdl-1.0.2/pytorrentdl.egg-info/
--rw-rw-rw-   0        0        0     5121 2024-04-18 13:25:24.000000 pytorrentdl-1.0.2/pytorrentdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-04-18 13:25:24.000000 pytorrentdl-1.0.2/pytorrentdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 13:25:24.000000 pytorrentdl-1.0.2/pytorrentdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-18 13:25:24.000000 pytorrentdl-1.0.2/pytorrentdl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-04-18 13:25:24.000000 pytorrentdl-1.0.2/pytorrentdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-18 13:25:24.000000 pytorrentdl-1.0.2/pytorrentdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 13:25:25.982951 pytorrentdl-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1733 2024-04-18 11:17:10.000000 pytorrentdl-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:39:46.487618 pytorrentdl-2.0.0/
+-rw-rw-rw-   0        0        0    12179 2024-04-18 14:36:08.000000 pytorrentdl-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     5121 2024-04-19 10:39:46.484618 pytorrentdl-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3982 2024-04-18 14:36:08.000000 pytorrentdl-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 10:39:46.429615 pytorrentdl-2.0.0/pytorrentdl/
+-rw-rw-rw-   0        0        0      578 2024-04-19 10:38:51.000000 pytorrentdl-2.0.0/pytorrentdl/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-18 14:36:08.000000 pytorrentdl-2.0.0/pytorrentdl/cli.py
+-rw-rw-rw-   0        0        0     3737 2024-04-19 10:38:19.000000 pytorrentdl-2.0.0/pytorrentdl/downloader.py
+-rw-rw-rw-   0        0        0     1204 2024-04-18 14:36:08.000000 pytorrentdl-2.0.0/pytorrentdl/session.py
+-rw-rw-rw-   0        0        0     1972 2024-04-18 11:53:32.000000 pytorrentdl-2.0.0/pytorrentdl/torrent_downloader.py
+-rw-rw-rw-   0        0        0      470 2024-04-18 12:10:21.000000 pytorrentdl-2.0.0/pytorrentdl/torrent_info.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:39:46.464617 pytorrentdl-2.0.0/pytorrentdl.egg-info/
+-rw-rw-rw-   0        0        0     5121 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 10:39:46.489618 pytorrentdl-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1733 2024-04-18 11:17:10.000000 pytorrentdl-2.0.0/setup.py
```

### Comparing `pytorrentdl-1.0.2/LICENSE` & `pytorrentdl-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorrentdl-1.0.2/PKG-INFO` & `pytorrentdl-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorrentdl
-Version: 1.0.2
+Version: 2.0.0
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytorrentdl-1.0.2/README.md` & `pytorrentdl-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pytorrentdl-1.0.2/pytorrentdl/__init__.py` & `pytorrentdl-2.0.0/pytorrentdl/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 A great wrapped library for downloading from torrent.
 """
 from .torrent_downloader import TorrentDownloader
 from .torrent_info import TorrentInfo
 from .downloader import Downloader
 from .session import Session
 
-__version__ = "1.0.2"
+__version__ = "2.0.0"
 __author__ = 'Nima Akbarzade'
 __author_email__ = "iw4p@protonmail.com"
 __license__ = "BSD 2-clause"
 __url__ = "https://github.com/iw4p/torrentp"
 
 PYPI_SIMPLE_ENDPOINT: str = "https://pypi.org/project/torrentp"
```

### Comparing `pytorrentdl-1.0.2/pytorrentdl/cli.py` & `pytorrentdl-2.0.0/pytorrentdl/cli.py`

 * *Files identical despite different names*

### Comparing `pytorrentdl-1.0.2/pytorrentdl/downloader.py` & `pytorrentdl-2.0.0/pytorrentdl/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,21 +39,20 @@
     async def download(self,callback=None):
         self._callback = callback
         self.get_size_info(self.status().total_wanted)
 
         while not self._status.is_seeding:
             if not self._paused:
                 if self._callback:
-                    await self._callback(self._torrent_info, self._save_path,self.status(),self.name, self._status.progress, self._status.download_rate,finalizado=False)
+                    await self._callback(self._save_path,self.status())
                 else:
                     self._get_status_progress(self.status())
                     sys.stdout.flush()
 
-            await asyncio.sleep(1)
-        self._callback(finalizado=True)
+            #await asyncio.sleep(1)
 
     def _get_status_progress(self, s):
         _percentage = s.progress * 100
         _download_speed = s.download_rate / 1000
         _upload_speed = s.upload_rate / 1000
 
         counting = math.ceil(_percentage / 5)
```

### Comparing `pytorrentdl-1.0.2/pytorrentdl/session.py` & `pytorrentdl-2.0.0/pytorrentdl/session.py`

 * *Files identical despite different names*

### Comparing `pytorrentdl-1.0.2/pytorrentdl/torrent_downloader.py` & `pytorrentdl-2.0.0/pytorrentdl/torrent_downloader.py`

 * *Files identical despite different names*

### Comparing `pytorrentdl-1.0.2/pytorrentdl.egg-info/PKG-INFO` & `pytorrentdl-2.0.0/pytorrentdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorrentdl
-Version: 1.0.2
+Version: 2.0.0
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytorrentdl-1.0.2/setup.py` & `pytorrentdl-2.0.0/setup.py`

 * *Files identical despite different names*

