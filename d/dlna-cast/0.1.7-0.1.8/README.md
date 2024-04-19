# Comparing `tmp/dlna_cast-0.1.7.tar.gz` & `tmp/dlna_cast-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlna_cast-0.1.7.tar", max compression
+gzip compressed data, was "dlna_cast-0.1.8.tar", max compression
```

## Comparing `dlna_cast-0.1.7.tar` & `dlna_cast-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2022-11-15 00:44:40.333276 dlna_cast-0.1.7/LICENSE
--rw-r--r--   0        0        0     3823 2023-12-13 03:15:41.831158 dlna_cast-0.1.7/README.md
--rw-r--r--   0        0        0        0 2022-11-15 00:44:40.333276 dlna_cast-0.1.7/dlna_cast/__init__.py
--rw-r--r--   0        0        0     5502 2023-12-13 01:21:39.293104 dlna_cast-0.1.7/dlna_cast/main.py
--rw-r--r--   0        0        0     3263 2023-12-13 14:09:03.736714 dlna_cast-0.1.7/dlna_cast/ssdp.py
--rw-r--r--   0        0        0      838 2023-12-13 14:09:03.736714 dlna_cast-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4784 1970-01-01 00:00:00.000000 dlna_cast-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-11-12 14:20:51.347519 dlna_cast-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3823 2023-12-13 13:59:58.344790 dlna_cast-0.1.8/README.md
+-rwxr-xr-x   0        0        0        0 2022-11-12 15:48:16.599675 dlna_cast-0.1.8/dlna_cast/__init__.py
+-rwxr-xr-x   0        0        0     5515 2024-04-19 12:49:12.866593 dlna_cast-0.1.8/dlna_cast/main.py
+-rwxr-xr-x   0        0        0     3263 2023-12-13 14:06:00.747319 dlna_cast-0.1.8/dlna_cast/ssdp.py
+-rw-r--r--   0        0        0      838 2024-04-19 12:49:34.081185 dlna_cast-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4835 1970-01-01 00:00:00.000000 dlna_cast-0.1.8/PKG-INFO
```

### Comparing `dlna_cast-0.1.7/LICENSE` & `dlna_cast-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dlna_cast-0.1.7/README.md` & `dlna_cast-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dlna_cast-0.1.7/dlna_cast/main.py` & `dlna_cast-0.1.8/dlna_cast/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             '-keyint_min:v 1 -force_key_frames:v "expr:gte(t,n_forced*{segment_size})" '
             '-f hls -hls_time {segment_size} -hls_list_size 10 -hls_flags delete_segments'
         ).format(segment_size=segment_size, crf=crf)
 
         cmd = [
             self.ffmpeg_bin, '-framerate', str(framerate),
             input_opts, enc_opts,
-            join(self.dlna_cast_dir, 'index.m3u8'),
+            shlex.quote(join(self.dlna_cast_dir, 'index.m3u8')),
         ]
         cmd = ' '.join(cmd)
         print('run command: ', cmd)
         self._ffmpeg_process = sp.Popen(shlex.split(cmd))
         atexit.register(lambda: self._ffmpeg_process.kill())
 
     def __init__(self):
```

### Comparing `dlna_cast-0.1.7/dlna_cast/ssdp.py` & `dlna_cast-0.1.8/dlna_cast/ssdp.py`

 * *Files identical despite different names*

### Comparing `dlna_cast-0.1.7/pyproject.toml` & `dlna_cast-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlna-cast"
-version = "0.1.7"
+version = "0.1.8"
 description = "A cross-platform command-line tool that casts screen and media file to remote DLNA device."
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 packages = [{include = "dlna_cast"}]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 keywords = ["DLNA", "ffmpeg", "media", "smart-tv", "screen-cast", "uPnP"]
 include = [
```

### Comparing `dlna_cast-0.1.7/PKG-INFO` & `dlna_cast-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlna-cast
-Version: 0.1.7
+Version: 0.1.8
 Summary: A cross-platform command-line tool that casts screen and media file to remote DLNA device.
 License: GPL-3.0-or-later
 Keywords: DLNA,ffmpeg,media,smart-tv,screen-cast,uPnP
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fire (>=0.4.0,<0.5.0)
 Requires-Dist: python-dotenv[cli] (>=0.21.0,<0.22.0)
 Requires-Dist: upnpclient (>=1.0.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # dlna-cast
 [![PyPI version](https://badge.fury.io/py/dlna-cast.svg)](https://badge.fury.io/py/dlna-cast)
```

