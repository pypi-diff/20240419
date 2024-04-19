# Comparing `tmp/pypianotune-0.1.2.tar.gz` & `tmp/pypianotune-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypianotune-0.1.2.tar", last modified: Fri Apr 19 06:10:30 2024, max compression
+gzip compressed data, was "pypianotune-0.1.3.tar", last modified: Fri Apr 19 07:38:31 2024, max compression
```

## Comparing `pypianotune-0.1.2.tar` & `pypianotune-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kelvinxu   (501) staff       (20)        0 2024-04-19 06:10:30.129843 pypianotune-0.1.2/
--rw-r--r--   0 kelvinxu   (501) staff       (20)     1069 2024-04-19 05:36:54.000000 pypianotune-0.1.2/LICENSE
--rw-r--r--   0 kelvinxu   (501) staff       (20)     1165 2024-04-19 06:10:30.129465 pypianotune-0.1.2/PKG-INFO
--rw-r--r--   0 kelvinxu   (501) staff       (20)      646 2024-04-19 06:08:40.000000 pypianotune-0.1.2/README.md
--rw-r--r--   0 kelvinxu   (501) staff       (20)      500 2024-04-19 06:10:06.000000 pypianotune-0.1.2/pyproject.toml
--rw-r--r--   0 kelvinxu   (501) staff       (20)       38 2024-04-19 06:10:30.129913 pypianotune-0.1.2/setup.cfg
-drwxr-xr-x   0 kelvinxu   (501) staff       (20)        0 2024-04-19 06:10:30.126886 pypianotune-0.1.2/src/
-drwxr-xr-x   0 kelvinxu   (501) staff       (20)        0 2024-04-19 06:10:30.129235 pypianotune-0.1.2/src/PyPianoTune.egg-info/
--rw-r--r--   0 kelvinxu   (501) staff       (20)     1165 2024-04-19 06:10:30.000000 pypianotune-0.1.2/src/PyPianoTune.egg-info/PKG-INFO
--rw-r--r--   0 kelvinxu   (501) staff       (20)      247 2024-04-19 06:10:30.000000 pypianotune-0.1.2/src/PyPianoTune.egg-info/SOURCES.txt
--rw-r--r--   0 kelvinxu   (501) staff       (20)        1 2024-04-19 06:10:30.000000 pypianotune-0.1.2/src/PyPianoTune.egg-info/dependency_links.txt
--rw-r--r--   0 kelvinxu   (501) staff       (20)       12 2024-04-19 06:10:30.000000 pypianotune-0.1.2/src/PyPianoTune.egg-info/top_level.txt
-drwxr-xr-x   0 kelvinxu   (501) staff       (20)        0 2024-04-19 06:10:30.128694 pypianotune-0.1.2/src/pypianotune/
--rw-rw-r--   0 kelvinxu   (501) staff       (20)       49 2024-04-19 01:37:22.000000 pypianotune-0.1.2/src/pypianotune/__init__.py
--rw-r--r--   0 kelvinxu   (501) staff       (20)    11343 2024-04-19 03:51:24.000000 pypianotune-0.1.2/src/pypianotune/pypianotune.py
+drwxr-xr-x   0 kelvinxu   (501) staff       (20)        0 2024-04-19 07:38:31.467049 pypianotune-0.1.3/
+-rw-r--r--   0 kelvinxu   (501) staff       (20)     1069 2024-04-19 05:36:54.000000 pypianotune-0.1.3/LICENSE
+-rw-r--r--   0 kelvinxu   (501) staff       (20)     1215 2024-04-19 07:38:31.466822 pypianotune-0.1.3/PKG-INFO
+-rw-r--r--   0 kelvinxu   (501) staff       (20)      696 2024-04-19 06:21:30.000000 pypianotune-0.1.3/README.md
+-rw-r--r--   0 kelvinxu   (501) staff       (20)      500 2024-04-19 07:37:45.000000 pypianotune-0.1.3/pyproject.toml
+-rw-r--r--   0 kelvinxu   (501) staff       (20)       38 2024-04-19 07:38:31.467091 pypianotune-0.1.3/setup.cfg
+drwxr-xr-x   0 kelvinxu   (501) staff       (20)        0 2024-04-19 07:38:31.464461 pypianotune-0.1.3/src/
+drwxr-xr-x   0 kelvinxu   (501) staff       (20)        0 2024-04-19 07:38:31.466607 pypianotune-0.1.3/src/PyPianoTune.egg-info/
+-rw-r--r--   0 kelvinxu   (501) staff       (20)     1215 2024-04-19 07:38:31.000000 pypianotune-0.1.3/src/PyPianoTune.egg-info/PKG-INFO
+-rw-r--r--   0 kelvinxu   (501) staff       (20)      247 2024-04-19 07:38:31.000000 pypianotune-0.1.3/src/PyPianoTune.egg-info/SOURCES.txt
+-rw-r--r--   0 kelvinxu   (501) staff       (20)        1 2024-04-19 07:38:31.000000 pypianotune-0.1.3/src/PyPianoTune.egg-info/dependency_links.txt
+-rw-r--r--   0 kelvinxu   (501) staff       (20)       12 2024-04-19 07:38:31.000000 pypianotune-0.1.3/src/PyPianoTune.egg-info/top_level.txt
+drwxr-xr-x   0 kelvinxu   (501) staff       (20)        0 2024-04-19 07:38:31.466271 pypianotune-0.1.3/src/pypianotune/
+-rw-rw-r--   0 kelvinxu   (501) staff       (20)       49 2024-04-19 01:37:22.000000 pypianotune-0.1.3/src/pypianotune/__init__.py
+-rw-r--r--   0 kelvinxu   (501) staff       (20)    11337 2024-04-19 07:37:32.000000 pypianotune-0.1.3/src/pypianotune/pypianotune.py
```

### Comparing `pypianotune-0.1.2/LICENSE` & `pypianotune-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypianotune-0.1.2/PKG-INFO` & `pypianotune-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPianoTune
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python module to convert music notes into piano tune.
 Author-email: Kelvin Xu <xxk59@hotmail.com>
 Project-URL: Homepage, https://github.com/xxk59/piano_tune
 Project-URL: Issues, https://github.com/xxk59/piano_tune/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyPianoTune
 
 A Python module to convert music notes into piano tune
 
+## Installation
+
+```
+pip install PyPianoTune
+```
+
 ## Import module
 
 ```python
 from pypianotune import PyPianoTune
 ```
 
 ## Sample
```

### Comparing `pypianotune-0.1.2/README.md` & `pypianotune-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # PyPianoTune
 
 A Python module to convert music notes into piano tune
 
+## Installation
+
+```
+pip install PyPianoTune
+```
+
 ## Import module
 
 ```python
 from pypianotune import PyPianoTune
 ```
 
 ## Sample
```

### Comparing `pypianotune-0.1.2/src/PyPianoTune.egg-info/PKG-INFO` & `pypianotune-0.1.3/src/PyPianoTune.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPianoTune
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python module to convert music notes into piano tune.
 Author-email: Kelvin Xu <xxk59@hotmail.com>
 Project-URL: Homepage, https://github.com/xxk59/piano_tune
 Project-URL: Issues, https://github.com/xxk59/piano_tune/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyPianoTune
 
 A Python module to convert music notes into piano tune
 
+## Installation
+
+```
+pip install PyPianoTune
+```
+
 ## Import module
 
 ```python
 from pypianotune import PyPianoTune
 ```
 
 ## Sample
```

### Comparing `pypianotune-0.1.2/src/pypianotune/pypianotune.py` & `pypianotune-0.1.3/src/pypianotune/pypianotune.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
                                         decay, sustain_level)
                 song[start_idx[i]:end_idx[i]] += this_note*weights
 
         song = song*(amplitude/np.max(song))
         return song
 
     # Combine one or more song data for Audio readiness
-    def getAudioFromSongData(self, *args):
+    def appendSongData(self, *args):
         # Check if all arguments are ndarrays
         if not all(isinstance(arr, np.ndarray) for arr in args):
             raise ValueError("All arguments must be NumPy ndarrays")
 
         max_length = max(arr.shape[0] for arr in args)
         combined_array = np.zeros(max_length, dtype=args[0].dtype)
         for arr in args:
```

