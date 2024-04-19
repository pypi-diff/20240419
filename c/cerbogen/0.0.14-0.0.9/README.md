# Comparing `tmp/cerbogen-0.0.14.tar.gz` & `tmp/cerbogen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbogen-0.0.14.tar", last modified: Fri Apr 19 13:40:43 2024, max compression
+gzip compressed data, was "cerbogen-0.0.9.tar", last modified: Fri Apr 19 08:07:30 2024, max compression
```

## Comparing `cerbogen-0.0.14.tar` & `cerbogen-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 13:40:43.375497 cerbogen-0.0.14/
--rw-rw-rw-   0        0        0      725 2024-04-19 13:40:43.374503 cerbogen-0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.14/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 13:40:43.288447 cerbogen-0.0.14/cerbogen/
--rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.14/cerbogen/__init__.py
--rw-rw-rw-   0        0        0     8856 2024-04-19 07:05:53.000000 cerbogen-0.0.14/cerbogen/cerbogen.py
--rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.14/cerbogen/check.py
-drwxrwxrwx   0        0        0        0 2024-04-19 13:40:43.281447 cerbogen-0.0.14/cerbogen/data/
-drwxrwxrwx   0        0        0        0 2024-04-19 13:40:43.355482 cerbogen-0.0.14/cerbogen/data/img/
--rw-rw-rw-   0        0        0   188454 2024-04-19 11:49:03.000000 cerbogen-0.0.14/cerbogen/data/img/logo.ico
--rw-rw-rw-   0        0        0     5115 2024-04-19 11:47:44.000000 cerbogen-0.0.14/cerbogen/data/img/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-19 13:40:43.372489 cerbogen-0.0.14/cerbogen/ffmpeg/
--rw-rw-rw-   0        0        0    35147 2023-12-31 08:04:26.000000 cerbogen-0.0.14/cerbogen/ffmpeg/LICENSE
--rw-rw-rw-   0        0        0    42234 2023-12-31 08:04:27.000000 cerbogen-0.0.14/cerbogen/ffmpeg/README.txt
--rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.14/cerbogen/plot.py
--rw-rw-rw-   0        0        0     2145 2024-04-19 13:40:10.000000 cerbogen-0.0.14/cerbogen/setup.py
--rw-rw-rw-   0        0        0     9334 2024-04-19 11:58:11.000000 cerbogen-0.0.14/cerbogen/ui.py
-drwxrwxrwx   0        0        0        0 2024-04-19 13:40:43.373501 cerbogen-0.0.14/cerbogen.egg-info/
--rw-rw-rw-   0        0        0      725 2024-04-19 13:40:43.000000 cerbogen-0.0.14/cerbogen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-04-19 13:40:43.000000 cerbogen-0.0.14/cerbogen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 13:40:43.000000 cerbogen-0.0.14/cerbogen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-19 13:40:43.000000 cerbogen-0.0.14/cerbogen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-19 13:40:43.000000 cerbogen-0.0.14/cerbogen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 13:40:43.375497 cerbogen-0.0.14/setup.cfg
--rw-rw-rw-   0        0        0     1358 2024-04-19 13:40:42.000000 cerbogen-0.0.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:07:30.389639 cerbogen-0.0.9/
+-rw-rw-rw-   0        0        0      700 2024-04-19 08:07:30.388636 cerbogen-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:11:50.000000 cerbogen-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 08:07:30.367637 cerbogen-0.0.9/cerbogen/
+-rw-rw-rw-   0        0        0        0 2024-04-19 06:04:16.000000 cerbogen-0.0.9/cerbogen/__init__.py
+-rw-rw-rw-   0        0        0     8856 2024-04-19 07:05:53.000000 cerbogen-0.0.9/cerbogen/cerbogen.py
+-rw-rw-rw-   0        0        0     1078 2024-04-19 06:03:12.000000 cerbogen-0.0.9/cerbogen/check.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:07:30.387652 cerbogen-0.0.9/cerbogen/ffmpeg/
+-rw-rw-rw-   0        0        0    35147 2023-12-31 08:04:26.000000 cerbogen-0.0.9/cerbogen/ffmpeg/LICENSE
+-rw-rw-rw-   0        0        0    42234 2023-12-31 08:04:27.000000 cerbogen-0.0.9/cerbogen/ffmpeg/README.txt
+-rw-rw-rw-   0        0        0     2348 2024-04-10 13:05:15.000000 cerbogen-0.0.9/cerbogen/plot.py
+-rw-rw-rw-   0        0        0     8965 2024-04-19 08:05:35.000000 cerbogen-0.0.9/cerbogen/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:07:30.388636 cerbogen-0.0.9/cerbogen.egg-info/
+-rw-rw-rw-   0        0        0      700 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 08:07:30.000000 cerbogen-0.0.9/cerbogen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:07:30.389639 cerbogen-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      909 2024-04-19 08:07:29.000000 cerbogen-0.0.9/setup.py
```

### Comparing `cerbogen-0.0.14/PKG-INFO` & `cerbogen-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.14
+Version: 0.0.9
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -14,8 +14,7 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib
 Requires-Dist: pydub
 Requires-Dist: numpy
 Requires-Dist: wave
 Requires-Dist: librosa
-Requires-Dist: pywin32
```

### Comparing `cerbogen-0.0.14/cerbogen/cerbogen.py` & `cerbogen-0.0.9/cerbogen/cerbogen.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.14/cerbogen/check.py` & `cerbogen-0.0.9/cerbogen/check.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.14/cerbogen/ffmpeg/LICENSE` & `cerbogen-0.0.9/cerbogen/ffmpeg/LICENSE`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.14/cerbogen/ffmpeg/README.txt` & `cerbogen-0.0.9/cerbogen/ffmpeg/README.txt`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.14/cerbogen/plot.py` & `cerbogen-0.0.9/cerbogen/plot.py`

 * *Files identical despite different names*

### Comparing `cerbogen-0.0.14/cerbogen/ui.py` & `cerbogen-0.0.9/cerbogen/ui.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,33 +61,16 @@
 
 def update():
     pass
 
 
 # Main window
 root = tk.Tk()
-root.title("CerboGen")
-
-# RESOLUTION
-root.geometry("340x700")  # Set initial window size
-
-# Get the screen width and height
-screen_width = root.winfo_screenwidth()
-screen_height = root.winfo_screenheight()
-
-# Calculate the position to place the window on the left side, touching the top
-x_pos = 0
-y_pos = 0
-
-# Set the position of the window
-root.geometry("+{}+{}".format(x_pos, y_pos))
-
-
-# Set the icon for the window
-root.iconbitmap("./data/img/logo.ico")
+root.title("Binaural Beats and Power Nap Generator")
+root.geometry("340x670")  # Set initial window size
 
 # Lock window resizing
 root.resizable(False, False)
 
 # Theremin-style background
 background_color = "#2c3e50"
 root.configure(bg=background_color)
```

### Comparing `cerbogen-0.0.14/cerbogen.egg-info/PKG-INFO` & `cerbogen-0.0.9/cerbogen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerbogen
-Version: 0.0.14
+Version: 0.0.9
 Summary: A Python package for CerboTech
 Home-page: https://github.com/clarenceparmar/cerbogen
 Author: Clarence Parmar
 Author-email: git.clarence@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -14,8 +14,7 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib
 Requires-Dist: pydub
 Requires-Dist: numpy
 Requires-Dist: wave
 Requires-Dist: librosa
-Requires-Dist: pywin32
```
