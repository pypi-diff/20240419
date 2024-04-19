# Comparing `tmp/pytorrentdl-2.0.0.tar.gz` & `tmp/pytorrentdl-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorrentdl-2.0.0.tar", last modified: Fri Apr 19 10:39:46 2024, max compression
+gzip compressed data, was "pytorrentdl-2.0.1.tar", last modified: Fri Apr 19 11:19:55 2024, max compression
```

## Comparing `pytorrentdl-2.0.0.tar` & `pytorrentdl-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 10:39:46.487618 pytorrentdl-2.0.0/
--rw-rw-rw-   0        0        0    12179 2024-04-18 14:36:08.000000 pytorrentdl-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     5121 2024-04-19 10:39:46.484618 pytorrentdl-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3982 2024-04-18 14:36:08.000000 pytorrentdl-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 10:39:46.429615 pytorrentdl-2.0.0/pytorrentdl/
--rw-rw-rw-   0        0        0      578 2024-04-19 10:38:51.000000 pytorrentdl-2.0.0/pytorrentdl/__init__.py
--rw-rw-rw-   0        0        0     1812 2024-04-18 14:36:08.000000 pytorrentdl-2.0.0/pytorrentdl/cli.py
--rw-rw-rw-   0        0        0     3737 2024-04-19 10:38:19.000000 pytorrentdl-2.0.0/pytorrentdl/downloader.py
--rw-rw-rw-   0        0        0     1204 2024-04-18 14:36:08.000000 pytorrentdl-2.0.0/pytorrentdl/session.py
--rw-rw-rw-   0        0        0     1972 2024-04-18 11:53:32.000000 pytorrentdl-2.0.0/pytorrentdl/torrent_downloader.py
--rw-rw-rw-   0        0        0      470 2024-04-18 12:10:21.000000 pytorrentdl-2.0.0/pytorrentdl/torrent_info.py
-drwxrwxrwx   0        0        0        0 2024-04-19 10:39:46.464617 pytorrentdl-2.0.0/pytorrentdl.egg-info/
--rw-rw-rw-   0        0        0     5121 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-19 10:39:44.000000 pytorrentdl-2.0.0/pytorrentdl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 10:39:46.489618 pytorrentdl-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1733 2024-04-18 11:17:10.000000 pytorrentdl-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:19:54.946541 pytorrentdl-2.0.1/
+-rw-rw-rw-   0        0        0    12179 2024-04-18 14:36:08.000000 pytorrentdl-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5121 2024-04-19 11:19:54.910539 pytorrentdl-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3982 2024-04-18 14:36:08.000000 pytorrentdl-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 11:19:54.857536 pytorrentdl-2.0.1/pytorrentdl/
+-rw-rw-rw-   0        0        0      578 2024-04-19 11:19:18.000000 pytorrentdl-2.0.1/pytorrentdl/__init__.py
+-rw-rw-rw-   0        0        0     1812 2024-04-18 14:36:08.000000 pytorrentdl-2.0.1/pytorrentdl/cli.py
+-rw-rw-rw-   0        0        0     3173 2024-04-19 11:18:58.000000 pytorrentdl-2.0.1/pytorrentdl/downloader.py
+-rw-rw-rw-   0        0        0     1204 2024-04-18 14:36:08.000000 pytorrentdl-2.0.1/pytorrentdl/session.py
+-rw-rw-rw-   0        0        0     1972 2024-04-18 11:53:32.000000 pytorrentdl-2.0.1/pytorrentdl/torrent_downloader.py
+-rw-rw-rw-   0        0        0      470 2024-04-18 12:10:21.000000 pytorrentdl-2.0.1/pytorrentdl/torrent_info.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:19:54.904538 pytorrentdl-2.0.1/pytorrentdl.egg-info/
+-rw-rw-rw-   0        0        0     5121 2024-04-19 11:19:52.000000 pytorrentdl-2.0.1/pytorrentdl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2024-04-19 11:19:53.000000 pytorrentdl-2.0.1/pytorrentdl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:19:52.000000 pytorrentdl-2.0.1/pytorrentdl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 11:19:52.000000 pytorrentdl-2.0.1/pytorrentdl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2024-04-19 11:19:52.000000 pytorrentdl-2.0.1/pytorrentdl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-19 11:19:52.000000 pytorrentdl-2.0.1/pytorrentdl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 11:19:54.947541 pytorrentdl-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1733 2024-04-18 11:17:10.000000 pytorrentdl-2.0.1/setup.py
```

### Comparing `pytorrentdl-2.0.0/LICENSE` & `pytorrentdl-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorrentdl-2.0.0/PKG-INFO` & `pytorrentdl-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorrentdl
-Version: 2.0.0
+Version: 2.0.1
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytorrentdl-2.0.0/README.md` & `pytorrentdl-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytorrentdl-2.0.0/pytorrentdl/__init__.py` & `pytorrentdl-2.0.1/pytorrentdl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 A great wrapped library for downloading from torrent.
 """
 from .torrent_downloader import TorrentDownloader
 from .torrent_info import TorrentInfo
 from .downloader import Downloader
 from .session import Session
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __author__ = 'Nima Akbarzade'
 __author_email__ = "iw4p@protonmail.com"
 __license__ = "BSD 2-clause"
 __url__ = "https://github.com/iw4p/torrentp"
 
 PYPI_SIMPLE_ENDPOINT: str = "https://pypi.org/project/torrentp"
```

### Comparing `pytorrentdl-2.0.0/pytorrentdl/cli.py` & `pytorrentdl-2.0.1/pytorrentdl/cli.py`

 * *Files identical despite different names*

### Comparing `pytorrentdl-2.0.0/pytorrentdl/downloader.py` & `pytorrentdl-2.0.1/pytorrentdl/downloader.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             if not self._paused:
                 if self._callback:
                     await self._callback(self._save_path,self.status())
                 else:
                     self._get_status_progress(self.status())
                     sys.stdout.flush()
 
-            #await asyncio.sleep(1)
+            await asyncio.sleep(1)
 
     def _get_status_progress(self, s):
         _percentage = s.progress * 100
         _download_speed = s.download_rate / 1000
         _upload_speed = s.upload_rate / 1000
 
         counting = math.ceil(_percentage / 5)
@@ -67,42 +67,28 @@
             _size_info += 'MB' if _file_size > 1000 else 'KB'
             print('\033[95m' + _size_info  + '\033[0m')
 
         if self.status().name:
             print('\033[95m' + f'Saving as: {self.status().name}' + '\033[0m')
 
     def pause(self):
-        print("Pausing download...")
         if self._file:
             self._file.pause()
             self._paused = True
-            print("Download paused successfully.")
-        else:
-            print("Download file instance not found.")
 
     def resume(self):
-        print("Resuming download...")
         if self._file:
             if self._paused:
                 self._file.resume()
                 self._paused = False
-                print("Download resumed successfully.")
-            else:
-                print("Download is not paused. No action taken.")
-        else:
-            print("Download file instance not found.")
 
     def stop(self):
-        print("Stopping download...")
         if self._file:
             self._session.remove_torrent(self._file)
             self._file = None
-            print("Download stopped successfully.")
-        else:
-            print("Download file instance not found.")
 
     def is_paused(self):
         return self._paused
 
     def __str__(self):
         pass
```

### Comparing `pytorrentdl-2.0.0/pytorrentdl/session.py` & `pytorrentdl-2.0.1/pytorrentdl/session.py`

 * *Files identical despite different names*

### Comparing `pytorrentdl-2.0.0/pytorrentdl/torrent_downloader.py` & `pytorrentdl-2.0.1/pytorrentdl/torrent_downloader.py`

 * *Files identical despite different names*

### Comparing `pytorrentdl-2.0.0/pytorrentdl.egg-info/PKG-INFO` & `pytorrentdl-2.0.1/pytorrentdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorrentdl
-Version: 2.0.0
+Version: 2.0.1
 Summary: Download from torrent with magnet link or .torrent file
 Home-page: https://github.com/iw4p/torrentp
 Author: Nima Akbarzade
 Author-email: iw4p@protonmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pytorrentdl-2.0.0/setup.py` & `pytorrentdl-2.0.1/setup.py`

 * *Files identical despite different names*

