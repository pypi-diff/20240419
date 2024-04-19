# Comparing `tmp/motionphoto-0.1.0.tar.gz` & `tmp/motionphoto-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motionphoto-0.1.0.tar", last modified: Fri Apr 19 19:02:10 2024, max compression
+gzip compressed data, was "motionphoto-0.1.1.tar", last modified: Fri Apr 19 19:24:33 2024, max compression
```

## Comparing `motionphoto-0.1.0.tar` & `motionphoto-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 doodspav   (501) staff       (20)        0 2024-04-19 19:02:10.243453 motionphoto-0.1.0/
--rw-r--r--   0 doodspav   (501) staff       (20)     5963 2024-04-19 19:02:10.243391 motionphoto-0.1.0/PKG-INFO
--rw-r--r--   0 doodspav   (501) staff       (20)     4781 2024-04-19 18:30:34.000000 motionphoto-0.1.0/README.md
-drwxr-xr-x   0 doodspav   (501) staff       (20)        0 2024-04-19 19:02:10.242277 motionphoto-0.1.0/motionphoto/
--rw-r--r--   0 doodspav   (501) staff       (20)       87 2024-04-19 18:53:57.000000 motionphoto-0.1.0/motionphoto/__init__.py
--rw-r--r--   0 doodspav   (501) staff       (20)       70 2024-04-19 18:56:16.000000 motionphoto-0.1.0/motionphoto/__main__.py
--rw-r--r--   0 doodspav   (501) staff       (20)     3041 2024-04-19 18:56:16.000000 motionphoto-0.1.0/motionphoto/cli.py
--rw-r--r--   0 doodspav   (501) staff       (20)      962 2024-04-19 15:53:29.000000 motionphoto-0.1.0/motionphoto/exiftool.py
--rw-r--r--   0 doodspav   (501) staff       (20)     1002 2024-04-19 15:57:01.000000 motionphoto-0.1.0/motionphoto/google.py
--rw-r--r--   0 doodspav   (501) staff       (20)     2899 2024-04-19 16:07:17.000000 motionphoto-0.1.0/motionphoto/motion.py
--rw-r--r--   0 doodspav   (501) staff       (20)     3241 2024-04-19 17:59:38.000000 motionphoto-0.1.0/motionphoto/samsung.py
-drwxr-xr-x   0 doodspav   (501) staff       (20)        0 2024-04-19 19:02:10.243190 motionphoto-0.1.0/motionphoto.egg-info/
--rw-r--r--   0 doodspav   (501) staff       (20)     5963 2024-04-19 19:02:10.000000 motionphoto-0.1.0/motionphoto.egg-info/PKG-INFO
--rw-r--r--   0 doodspav   (501) staff       (20)      421 2024-04-19 19:02:10.000000 motionphoto-0.1.0/motionphoto.egg-info/SOURCES.txt
--rw-r--r--   0 doodspav   (501) staff       (20)        1 2024-04-19 19:02:10.000000 motionphoto-0.1.0/motionphoto.egg-info/dependency_links.txt
--rw-r--r--   0 doodspav   (501) staff       (20)       57 2024-04-19 19:02:10.000000 motionphoto-0.1.0/motionphoto.egg-info/entry_points.txt
--rw-r--r--   0 doodspav   (501) staff       (20)       29 2024-04-19 19:02:10.000000 motionphoto-0.1.0/motionphoto.egg-info/requires.txt
--rw-r--r--   0 doodspav   (501) staff       (20)       12 2024-04-19 19:02:10.000000 motionphoto-0.1.0/motionphoto.egg-info/top_level.txt
--rw-r--r--   0 doodspav   (501) staff       (20)       81 2024-04-19 18:49:59.000000 motionphoto-0.1.0/pyproject.toml
--rw-r--r--   0 doodspav   (501) staff       (20)       28 2024-04-19 18:35:43.000000 motionphoto-0.1.0/requirements.txt
--rw-r--r--   0 doodspav   (501) staff       (20)     1272 2024-04-19 19:02:10.243701 motionphoto-0.1.0/setup.cfg
+drwxr-xr-x   0 doodspav   (501) staff       (20)        0 2024-04-19 19:24:33.586393 motionphoto-0.1.1/
+-rw-r--r--   0 doodspav   (501) staff       (20)     6002 2024-04-19 19:24:33.586319 motionphoto-0.1.1/PKG-INFO
+-rw-r--r--   0 doodspav   (501) staff       (20)     4820 2024-04-19 19:14:37.000000 motionphoto-0.1.1/README.md
+drwxr-xr-x   0 doodspav   (501) staff       (20)        0 2024-04-19 19:24:33.585055 motionphoto-0.1.1/motionphoto/
+-rw-r--r--   0 doodspav   (501) staff       (20)       87 2024-04-19 19:22:51.000000 motionphoto-0.1.1/motionphoto/__init__.py
+-rw-r--r--   0 doodspav   (501) staff       (20)       70 2024-04-19 18:56:16.000000 motionphoto-0.1.1/motionphoto/__main__.py
+-rw-r--r--   0 doodspav   (501) staff       (20)     3041 2024-04-19 18:56:16.000000 motionphoto-0.1.1/motionphoto/cli.py
+-rw-r--r--   0 doodspav   (501) staff       (20)      962 2024-04-19 15:53:29.000000 motionphoto-0.1.1/motionphoto/exiftool.py
+-rw-r--r--   0 doodspav   (501) staff       (20)     1002 2024-04-19 15:57:01.000000 motionphoto-0.1.1/motionphoto/google.py
+-rw-r--r--   0 doodspav   (501) staff       (20)     2899 2024-04-19 16:07:17.000000 motionphoto-0.1.1/motionphoto/motion.py
+-rw-r--r--   0 doodspav   (501) staff       (20)     3241 2024-04-19 17:59:38.000000 motionphoto-0.1.1/motionphoto/samsung.py
+drwxr-xr-x   0 doodspav   (501) staff       (20)        0 2024-04-19 19:24:33.586093 motionphoto-0.1.1/motionphoto.egg-info/
+-rw-r--r--   0 doodspav   (501) staff       (20)     6002 2024-04-19 19:24:33.000000 motionphoto-0.1.1/motionphoto.egg-info/PKG-INFO
+-rw-r--r--   0 doodspav   (501) staff       (20)      421 2024-04-19 19:24:33.000000 motionphoto-0.1.1/motionphoto.egg-info/SOURCES.txt
+-rw-r--r--   0 doodspav   (501) staff       (20)        1 2024-04-19 19:24:33.000000 motionphoto-0.1.1/motionphoto.egg-info/dependency_links.txt
+-rw-r--r--   0 doodspav   (501) staff       (20)       57 2024-04-19 19:24:33.000000 motionphoto-0.1.1/motionphoto.egg-info/entry_points.txt
+-rw-r--r--   0 doodspav   (501) staff       (20)       29 2024-04-19 19:24:33.000000 motionphoto-0.1.1/motionphoto.egg-info/requires.txt
+-rw-r--r--   0 doodspav   (501) staff       (20)       12 2024-04-19 19:24:33.000000 motionphoto-0.1.1/motionphoto.egg-info/top_level.txt
+-rw-r--r--   0 doodspav   (501) staff       (20)       81 2024-04-19 18:49:59.000000 motionphoto-0.1.1/pyproject.toml
+-rw-r--r--   0 doodspav   (501) staff       (20)       28 2024-04-19 18:35:43.000000 motionphoto-0.1.1/requirements.txt
+-rw-r--r--   0 doodspav   (501) staff       (20)     1272 2024-04-19 19:24:33.586649 motionphoto-0.1.1/setup.cfg
```

### Comparing `motionphoto-0.1.0/PKG-INFO` & `motionphoto-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionphoto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for creating Google and Samsung compatible Motion Photos
 Home-page: https://github.com/doodspav/motionphoto
 Download-URL: https://github.com/doodspav/motionphoto
 Author: doodspav
 Project-URL: Source, https://github.com/doodspav/motionphoto
 Keywords: livephoto,LivePhoto,motionphoto,MotionPhoto
 Platform: any
@@ -51,25 +51,26 @@
 ```
 
 Windows:
 ```shell
 $ py -m pip install motionphoto
 ```
 
-This library has a dependency on `exiftool`.  
+This library has a dependency on `exiftool`.
+
 Instructions for installing it can be found [here](https://exiftool.org/install.html) and it must be available on
 `PATH`, or it can be installed with a package manager.
 
 ## Usage
 
 `motionphoto -i <imagePath> -v <videoPath> -m <outputPath> [-t_us <keyFrameOffset> --overwrite]`
 
 Notes:
-- `-i` image format must be JPEG
-- `-t_us` is in microseconds, from the start of the video file
+- `<imagePath>` image format must be JPEG
+- `<keyFrameOffset>` is where the image is, in microseconds, from the start of the video file
 - `--overwrite` flag allows overwriting an existing file instead of returning an error
 
 ## Motion Photo Format
 This section will cover the requirements to make a valid Motion Photo.  
 Since each application/vendor has their own implementation, they also have separate requirements.
 
 The image format should be JPEG, not HEIC. HEIC occassionally works, but is not reliable.
```

### Comparing `motionphoto-0.1.0/README.md` & `motionphoto-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 ```
 
 Windows:
 ```shell
 $ py -m pip install motionphoto
 ```
 
-This library has a dependency on `exiftool`.  
+This library has a dependency on `exiftool`.
+
 Instructions for installing it can be found [here](https://exiftool.org/install.html) and it must be available on
 `PATH`, or it can be installed with a package manager.
 
 ## Usage
 
 `motionphoto -i <imagePath> -v <videoPath> -m <outputPath> [-t_us <keyFrameOffset> --overwrite]`
 
 Notes:
-- `-i` image format must be JPEG
-- `-t_us` is in microseconds, from the start of the video file
+- `<imagePath>` image format must be JPEG
+- `<keyFrameOffset>` is where the image is, in microseconds, from the start of the video file
 - `--overwrite` flag allows overwriting an existing file instead of returning an error
 
 ## Motion Photo Format
 This section will cover the requirements to make a valid Motion Photo.  
 Since each application/vendor has their own implementation, they also have separate requirements.
 
 The image format should be JPEG, not HEIC. HEIC occassionally works, but is not reliable.
```

### Comparing `motionphoto-0.1.0/motionphoto/cli.py` & `motionphoto-0.1.1/motionphoto/cli.py`

 * *Files identical despite different names*

### Comparing `motionphoto-0.1.0/motionphoto/exiftool.py` & `motionphoto-0.1.1/motionphoto/exiftool.py`

 * *Files identical despite different names*

### Comparing `motionphoto-0.1.0/motionphoto/google.py` & `motionphoto-0.1.1/motionphoto/google.py`

 * *Files identical despite different names*

### Comparing `motionphoto-0.1.0/motionphoto/motion.py` & `motionphoto-0.1.1/motionphoto/motion.py`

 * *Files identical despite different names*

### Comparing `motionphoto-0.1.0/motionphoto/samsung.py` & `motionphoto-0.1.1/motionphoto/samsung.py`

 * *Files identical despite different names*

### Comparing `motionphoto-0.1.0/motionphoto.egg-info/PKG-INFO` & `motionphoto-0.1.1/motionphoto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionphoto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for creating Google and Samsung compatible Motion Photos
 Home-page: https://github.com/doodspav/motionphoto
 Download-URL: https://github.com/doodspav/motionphoto
 Author: doodspav
 Project-URL: Source, https://github.com/doodspav/motionphoto
 Keywords: livephoto,LivePhoto,motionphoto,MotionPhoto
 Platform: any
@@ -51,25 +51,26 @@
 ```
 
 Windows:
 ```shell
 $ py -m pip install motionphoto
 ```
 
-This library has a dependency on `exiftool`.  
+This library has a dependency on `exiftool`.
+
 Instructions for installing it can be found [here](https://exiftool.org/install.html) and it must be available on
 `PATH`, or it can be installed with a package manager.
 
 ## Usage
 
 `motionphoto -i <imagePath> -v <videoPath> -m <outputPath> [-t_us <keyFrameOffset> --overwrite]`
 
 Notes:
-- `-i` image format must be JPEG
-- `-t_us` is in microseconds, from the start of the video file
+- `<imagePath>` image format must be JPEG
+- `<keyFrameOffset>` is where the image is, in microseconds, from the start of the video file
 - `--overwrite` flag allows overwriting an existing file instead of returning an error
 
 ## Motion Photo Format
 This section will cover the requirements to make a valid Motion Photo.  
 Since each application/vendor has their own implementation, they also have separate requirements.
 
 The image format should be JPEG, not HEIC. HEIC occassionally works, but is not reliable.
```

### Comparing `motionphoto-0.1.0/setup.cfg` & `motionphoto-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = motionphoto
-version = 0.1.0
+version = 0.1.1
 description = Python library for creating Google and Samsung compatible Motion Photos
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = livephoto, LivePhoto, motionphoto, MotionPhoto
 url = https://github.com/doodspav/motionphoto
 author = doodspav
 autor_email = doodspav@gmail.com
@@ -30,13 +30,13 @@
 
 [options]
 python_requires = >=3.8, <4
 install_requires = file: requirements.txt
 
 [options.entry_points]
 console_scripts = 
-	motionphoto=motionphoto.cli.cli_file
+	motionphoto=motionphoto.cli:cli_file
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

