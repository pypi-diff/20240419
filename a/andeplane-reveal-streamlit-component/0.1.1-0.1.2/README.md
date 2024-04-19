# Comparing `tmp/andeplane_reveal_streamlit_component-0.1.1.tar.gz` & `tmp/andeplane_reveal_streamlit_component-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andeplane_reveal_streamlit_component-0.1.1.tar", last modified: Fri Apr 19 12:42:52 2024, max compression
+gzip compressed data, was "andeplane_reveal_streamlit_component-0.1.2.tar", last modified: Fri Apr 19 13:10:00 2024, max compression
```

## Comparing `andeplane_reveal_streamlit_component-0.1.1.tar` & `andeplane_reveal_streamlit_component-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 12:42:52.487405 andeplane_reveal_streamlit_component-0.1.1/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2506 2024-04-19 12:42:52.487092 andeplane_reveal_streamlit_component-0.1.1/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1845 2024-04-19 11:37:29.000000 andeplane_reveal_streamlit_component-0.1.1/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 12:42:52.486363 andeplane_reveal_streamlit_component-0.1.1/andeplane_reveal_streamlit_component.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     2506 2024-04-19 12:42:52.000000 andeplane_reveal_streamlit_component-0.1.1/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1688 2024-04-19 12:42:52.000000 andeplane_reveal_streamlit_component-0.1.1/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-19 12:42:52.000000 andeplane_reveal_streamlit_component-0.1.1/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-19 12:42:52.000000 andeplane_reveal_streamlit_component-0.1.1/andeplane_reveal_streamlit_component.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-04-19 12:42:52.000000 andeplane_reveal_streamlit_component-0.1.1/andeplane_reveal_streamlit_component.egg-info/top_level.txt
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 12:42:52.462900 andeplane_reveal_streamlit_component-0.1.1/reveal/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3699 2024-04-19 12:40:38.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/__init__.py
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 12:42:52.461123 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 12:42:52.463588 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1693 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/asset-manifest.json
--rw-r--r--   0 kvakkefly   (501) staff       (20)   197459 2024-04-19 12:40:42.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/bootstrap.min.css
--rw-r--r--   0 kvakkefly   (501) staff       (20)      553 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/index.html
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 12:42:52.461513 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 12:42:52.464232 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/css/
--rw-r--r--   0 kvakkefly   (501) staff       (20)   331112 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/css/main.c81cb3cf.css
--rw-r--r--   0 kvakkefly   (501) staff       (20)   461776 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/css/main.c81cb3cf.css.map
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 12:42:52.472347 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3941 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/114.e0ebff55.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3959 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/142.e332c9ad.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     5176 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/211.ee14119e.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3976 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/413.5c9588ac.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     4033 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/463.ad8fb302.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3940 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/690.16ab8bc4.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     4753 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/797.fb53d4d2.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     4270 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/809.14863d52.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3589 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/82.2b5d6c2f.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3822 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/913.b1b6282c.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3882 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/974.691b1718.chunk.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)  5724912 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/main.84078e82.js
--rw-r--r--   0 kvakkefly   (501) staff       (20)     5906 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/main.84078e82.js.LICENSE.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20) 16427889 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/main.84078e82.js.map
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 12:42:52.486034 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/
--rw-r--r--   0 kvakkefly   (501) staff       (20)   106140 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)   104332 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)   105924 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)    98868 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)   105804 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-19 12:42:52.487455 andeplane_reveal_streamlit_component-0.1.1/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1140 2024-04-19 12:42:47.000000 andeplane_reveal_streamlit_component-0.1.1/setup.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 13:10:00.509569 andeplane_reveal_streamlit_component-0.1.2/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2506 2024-04-19 13:10:00.509269 andeplane_reveal_streamlit_component-0.1.2/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1845 2024-04-19 11:37:29.000000 andeplane_reveal_streamlit_component-0.1.2/README.md
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 13:10:00.508538 andeplane_reveal_streamlit_component-0.1.2/andeplane_reveal_streamlit_component.egg-info/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     2506 2024-04-19 13:10:00.000000 andeplane_reveal_streamlit_component-0.1.2/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1688 2024-04-19 13:10:00.000000 andeplane_reveal_streamlit_component-0.1.2/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-19 13:10:00.000000 andeplane_reveal_streamlit_component-0.1.2/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-19 13:10:00.000000 andeplane_reveal_streamlit_component-0.1.2/andeplane_reveal_streamlit_component.egg-info/requires.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        7 2024-04-19 13:10:00.000000 andeplane_reveal_streamlit_component-0.1.2/andeplane_reveal_streamlit_component.egg-info/top_level.txt
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 13:10:00.480399 andeplane_reveal_streamlit_component-0.1.2/reveal/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3699 2024-04-19 13:09:39.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/__init__.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 13:10:00.477549 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 13:10:00.481887 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1693 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/asset-manifest.json
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   197459 2024-04-19 12:40:42.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/bootstrap.min.css
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      553 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/index.html
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 13:10:00.478033 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 13:10:00.483209 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/css/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   331112 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/css/main.c81cb3cf.css
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   461776 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/css/main.c81cb3cf.css.map
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 13:10:00.492508 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3941 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/114.e0ebff55.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3959 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/142.e332c9ad.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     5176 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/211.ee14119e.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3976 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/413.5c9588ac.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4033 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/463.ad8fb302.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3940 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/690.16ab8bc4.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4753 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/797.fb53d4d2.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     4270 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/809.14863d52.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3589 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/82.2b5d6c2f.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3822 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/913.b1b6282c.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3882 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/974.691b1718.chunk.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)  5724912 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/main.84078e82.js
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     5906 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/main.84078e82.js.LICENSE.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20) 16427889 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/main.84078e82.js.map
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-19 13:10:00.508082 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   106140 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   104332 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   105924 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)    98868 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)   105804 2024-04-19 12:41:09.000000 andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-19 13:10:00.509618 andeplane_reveal_streamlit_component-0.1.2/setup.cfg
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1140 2024-04-19 13:09:49.000000 andeplane_reveal_streamlit_component-0.1.2/setup.py
```

### Comparing `andeplane_reveal_streamlit_component-0.1.1/PKG-INFO` & `andeplane_reveal_streamlit_component-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.1.1
+Version: 0.1.2
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
```

### Comparing `andeplane_reveal_streamlit_component-0.1.1/README.md` & `andeplane_reveal_streamlit_component-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/andeplane_reveal_streamlit_component.egg-info/PKG-INFO` & `andeplane_reveal_streamlit_component-0.1.2/andeplane_reveal_streamlit_component.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.1.1
+Version: 0.1.2
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
```

### Comparing `andeplane_reveal_streamlit_component-0.1.1/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt` & `andeplane_reveal_streamlit_component-0.1.2/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/__init__.py` & `andeplane_reveal_streamlit_component-0.1.2/reveal/__init__.py`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/asset-manifest.json` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/bootstrap.min.css` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/index.html` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/css/main.c81cb3cf.css` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/css/main.c81cb3cf.css`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/css/main.c81cb3cf.css.map` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/css/main.c81cb3cf.css.map`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/114.e0ebff55.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/114.e0ebff55.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/142.e332c9ad.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/142.e332c9ad.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/211.ee14119e.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/211.ee14119e.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/413.5c9588ac.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/413.5c9588ac.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/463.ad8fb302.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/463.ad8fb302.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/690.16ab8bc4.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/690.16ab8bc4.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/797.fb53d4d2.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/797.fb53d4d2.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/809.14863d52.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/809.14863d52.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/82.2b5d6c2f.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/82.2b5d6c2f.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/913.b1b6282c.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/913.b1b6282c.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/974.691b1718.chunk.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/974.691b1718.chunk.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/main.84078e82.js` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/main.84078e82.js`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/main.84078e82.js.LICENSE.txt` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/main.84078e82.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/js/main.84078e82.js.map` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/js/main.84078e82.js.map`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/reveal/frontend/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2` & `andeplane_reveal_streamlit_component-0.1.2/reveal/frontend/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.1.1/setup.py` & `andeplane_reveal_streamlit_component-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="andeplane_reveal_streamlit_component",
-    version="0.1.1",
+    version="0.1.2",
     author="John Smith",
     author_email="john@example.com",
     description="Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

