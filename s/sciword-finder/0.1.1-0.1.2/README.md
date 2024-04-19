# Comparing `tmp/sciword_finder-0.1.1.tar.gz` & `tmp/sciword_finder-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciword_finder-0.1.1.tar", last modified: Fri Apr 19 06:34:25 2024, max compression
+gzip compressed data, was "sciword_finder-0.1.2.tar", last modified: Fri Apr 19 20:44:50 2024, max compression
```

## Comparing `sciword_finder-0.1.1.tar` & `sciword_finder-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 06:34:25.931896 sciword_finder-0.1.1/
--rw-rw-rw-   0        0        0      373 2024-04-19 06:34:25.927325 sciword_finder-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 06:34:25.917489 sciword_finder-0.1.1/sciword-finder/
--rw-rw-rw-   0        0        0      974 2024-04-18 17:31:41.000000 sciword_finder-0.1.1/sciword-finder/__init__.py
--rw-rw-rw-   0        0        0     1925 2024-04-19 06:12:47.000000 sciword_finder-0.1.1/sciword-finder/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:34:25.927325 sciword_finder-0.1.1/sciword_finder.egg-info/
--rw-rw-rw-   0        0        0      373 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-19 06:34:25.000000 sciword_finder-0.1.1/sciword_finder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 06:34:25.931896 sciword_finder-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      618 2024-04-19 06:32:22.000000 sciword_finder-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:44:50.228261 sciword_finder-0.1.2/
+-rw-rw-rw-   0        0        0      373 2024-04-19 20:44:50.227263 sciword_finder-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 20:44:50.218316 sciword_finder-0.1.2/sciword-finder/
+-rw-rw-rw-   0        0        0      974 2024-04-18 17:31:41.000000 sciword_finder-0.1.2/sciword-finder/__init__.py
+-rw-rw-rw-   0        0        0     1860 2024-04-19 06:37:21.000000 sciword_finder-0.1.2/sciword-finder/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:44:50.226261 sciword_finder-0.1.2/sciword_finder.egg-info/
+-rw-rw-rw-   0        0        0      373 2024-04-19 20:44:50.000000 sciword_finder-0.1.2/sciword_finder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-19 20:44:50.000000 sciword_finder-0.1.2/sciword_finder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 20:44:50.000000 sciword_finder-0.1.2/sciword_finder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-19 20:44:50.000000 sciword_finder-0.1.2/sciword_finder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-19 20:44:50.000000 sciword_finder-0.1.2/sciword_finder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 20:44:50.229298 sciword_finder-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      618 2024-04-19 20:44:45.000000 sciword_finder-0.1.2/setup.py
```

### Comparing `sciword_finder-0.1.1/sciword-finder/__init__.py` & `sciword_finder-0.1.2/sciword-finder/__init__.py`

 * *Files identical despite different names*

### Comparing `sciword_finder-0.1.1/sciword-finder/__main__.py` & `sciword_finder-0.1.2/sciword-finder/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
     if args.action == "start":
         directory_path = r"C:\Users\user\AppData\Local\sciword-finder"
         if not os.path.exists(directory_path):
             nltk.download("words")
             with open("eng_words.dat", "wb") as f:
                 pickle.dump(words, f)
-            with open("eng_words.dat", "rb") as f:
-                WORDS = pickle.load(f)
+            WORDS = words
             init_dir("eng_words.dat", pw="antidisestablishmentarianism_pi3.14159265")
         start()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sciword_finder-0.1.1/setup.py` & `sciword_finder-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="sciword-finder",
-    version="0.1.1",
+    version="0.1.2",
     author="Torrez",
     author_email="that1.stinkyarmpits@gmail.com",
     description="A user interface for finding scientific names for a specified word.",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

