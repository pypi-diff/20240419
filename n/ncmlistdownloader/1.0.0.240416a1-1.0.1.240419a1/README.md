# Comparing `tmp/ncmlistdownloader-1.0.0.240416a1.tar.gz` & `tmp/ncmlistdownloader-1.0.1.240419a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.0.240416a1.tar", last modified: Tue Apr 16 14:58:22 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.1.240419a1.tar", last modified: Fri Apr 19 14:58:02 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.0.240416a1.tar` & `ncmlistdownloader-1.0.1.240419a1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.168530 ncmlistdownloader-1.0.0.240416a1/
--rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240416a1/LICENSE
--rw-rw-rw-   0        0        0     1399 2024-04-16 14:58:22.164530 ncmlistdownloader-1.0.0.240416a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.106611 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1263 2024-04-14 14:42:21.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.129037 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     2373 2024-04-16 14:56:43.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/cmd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.142589 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2859 2024-04-10 14:43:02.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-14 14:36:25.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2184 2024-04-14 14:42:02.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.145610 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.151568 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.155554 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2145 2024-04-16 14:56:43.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.158556 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     7481 2024-04-12 15:08:55.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:58:22.162541 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1399 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      640 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-16 14:58:22.000000 ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 14:58:22.169519 ncmlistdownloader-1.0.0.240416a1/setup.cfg
--rw-rw-rw-   0        0        0     1758 2024-04-16 14:58:11.000000 ncmlistdownloader-1.0.0.240416a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.086654 ncmlistdownloader-1.0.1.240419a1/
+-rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.1.240419a1/LICENSE
+-rw-rw-rw-   0        0        0     1399 2024-04-19 14:58:02.084662 ncmlistdownloader-1.0.1.240419a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.032582 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1263 2024-04-14 14:42:21.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.051532 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0     3177 2024-04-19 14:57:23.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/cmd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.065494 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2859 2024-04-10 14:43:02.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-14 14:36:25.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2184 2024-04-14 14:42:02.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.070496 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.073474 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.076684 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     2323 2024-04-19 07:04:10.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.079674 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     7481 2024-04-12 15:08:55.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:58:02.083663 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1399 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2024-04-19 14:58:02.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-19 14:58:01.000000 ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 14:58:02.086654 ncmlistdownloader-1.0.1.240419a1/setup.cfg
+-rw-rw-rw-   0        0        0     1758 2024-04-19 14:42:22.000000 ncmlistdownloader-1.0.1.240419a1/setup.py
```

### Comparing `ncmlistdownloader-1.0.0.240416a1/LICENSE` & `ncmlistdownloader-1.0.1.240419a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/PKG-INFO` & `ncmlistdownloader-1.0.1.240419a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240416a1
+Version: 1.0.1.240419a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/cmd/__init__.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/cmd/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/cmd/__init__.py
-Core.Ver.1.0.0.240416a1
+Core.Ver.1.0.1.240419a1
 Author: CooooldWind_
 '''
 import time
 from ncmlistdownloader.song import *
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.common.global_args import *
 
@@ -37,38 +37,54 @@
     now = None
     id = str(input_func("Press the id/Url "))
     if choice == 1:
         now = Song(id)
         now.get_info()
     elif choice == 2:
         now = Playlist(id)
-        if now.auto_get_info(cookies = cookies) == -1:
+        if now.get_info(cookies = cookies) == -1:
             print(format_output("You don't have the currect cookies to get the info of this Playlist.", type = "Error"))
-        
-
+        now.multiprocessing_get_detail()
+        wait_time = 0
+        while now.done_sum() != now.track_count:
+            count = now.done_sum()
+            wait_time += 1
+            least = -1
+            if count != 0:
+                least = int(wait_time / count * (now.track_count - count))
+            print(format_output(f"Done: {count}/{now.track_count}, still need: {least} seconds", type = "Info"))
+            time.sleep(1)
+        for i in range(0, len(now.track)):
+            j = now.track[i]
+            print(format_output(f"Song #{i + 1}: {j.title} - {j.artist_str}", type = "Info"))
 
 def main():
     global cookies
     for i in CMD_START_WORDS:
         print(format_output(raw = i, type = "Info"))
     cookies = {'MUSIC_U': input_func("Please input your cookies (ONLY MUSIC_U) (if you don't have, just press enter) ")}
     if cookies["MUSIC_U"] == '':
         cookies = None
-    FUNC_CHOICE = [
-        "Find Playlist/Song by ID/Url",
-        "Load from json file",
-        "Search",
-    ]
-    for i in range(0, len(FUNC_CHOICE)):
-        if not(i == 2 and cookies == None): print(format_output(f"[{i + 1}] -> {FUNC_CHOICE[i]}", type = "Info"))
-        else: print(format_output(f"[X] -> {FUNC_CHOICE[i]}", type = "Info"))
-    choice = None
-    while True:    
-        choice = int(input_func("Press the number of the function "))
-        if choice >= 1 and choice <= len(FUNC_CHOICE):
+    while True:
+        FUNC_CHOICE = [
+            "Find Playlist/Song by ID/Url",
+            "Load from json file",
+            "Search",
+            "Exit",
+        ]
+        for i in range(0, len(FUNC_CHOICE)):
+            if not(i == 2 and cookies == None): print(format_output(f"[{i + 1}] -> {FUNC_CHOICE[i]}", type = "Info"))
+            else: print(format_output(f"[X] -> {FUNC_CHOICE[i]}", type = "Info"))
+        choice = None
+        while True:    
+            choice = int(input_func("Press the number of the function "))
+            if choice >= 1 and choice <= len(FUNC_CHOICE):
+                break
+        if choice == 1:
+            find_from_id()
+        if choice == 4:
             break
-    if choice == 1:
-        find_from_id()
+        print(format_output(raw = "Byebye~", type = "Info"))
 
 if __name__ == "__main__":
     main()
```

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/global_args.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/playlist/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/playlist/__init__.py
-Core.Ver.1.0.0.240416a1
+Core.Ver.1.0.1.240419a1
 Author: CooooldWind_
 '''
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.global_args import *
 from ncmlistdownloader.song import *
 import threading
@@ -42,19 +42,25 @@
     
     def get_detail_info(self):
         threads: list[threading.Thread] = []
         for i in self.track:
             thread = threading.Thread(target = i.multi_get_info)
             thread.start()
             threads.append(thread)
+        for i in threads:
+            i.join()
 
     def auto_get_info(self, cookies = dict()):
         if self.get_info(cookies = cookies) != -1:
             self.get_detail_info()
         else: return -1
 
     def done_sum(self):
         count = 0
         for i in self.track:
             if i.is_get == True:
                 count += 1
-        return count
+        return count
+    
+    def multiprocessing_get_detail(self):
+        p = threading.Thread(target = self.get_detail_info)
+        p.start()
```

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader/song/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240416a1
+Version: 1.0.1.240419a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-1.0.0.240416a1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.1.240419a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240416a1/setup.py` & `ncmlistdownloader-1.0.1.240419a1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.0.240416a1",
+    version = "1.0.1.240419a1",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
     install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

