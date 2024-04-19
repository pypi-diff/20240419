# Comparing `tmp/yusefs_library-0.1.tar.gz` & `tmp/yusefs_library-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yusefs_library-0.1.tar", last modified: Fri Apr 19 04:48:07 2024, max compression
+gzip compressed data, was "yusefs_library-0.2.tar", last modified: Fri Apr 19 04:59:14 2024, max compression
```

## Comparing `yusefs_library-0.1.tar` & `yusefs_library-0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 essawifamily   (501) staff       (20)        0 2024-04-19 04:48:07.341205 yusefs_library-0.1/
--rw-r--r--   0 essawifamily   (501) staff       (20)       56 2024-04-19 04:48:07.341031 yusefs_library-0.1/PKG-INFO
--rw-r--r--   0 essawifamily   (501) staff       (20)        0 2024-04-19 04:40:37.000000 yusefs_library-0.1/README.md
--rw-r--r--   0 essawifamily   (501) staff       (20)       38 2024-04-19 04:48:07.341264 yusefs_library-0.1/setup.cfg
--rw-r--r--   0 essawifamily   (501) staff       (20)      243 2024-04-19 04:47:33.000000 yusefs_library-0.1/setup.py
-drwxr-xr-x   0 essawifamily   (501) staff       (20)        0 2024-04-19 04:48:07.339803 yusefs_library-0.1/yusefs_library/
--rw-r--r--   0 essawifamily   (501) staff       (20)       37 2024-04-19 04:47:03.000000 yusefs_library-0.1/yusefs_library/__init__.py
--rw-r--r--   0 essawifamily   (501) staff       (20)       62 2024-04-19 04:42:44.000000 yusefs_library-0.1/yusefs_library/main.py
-drwxr-xr-x   0 essawifamily   (501) staff       (20)        0 2024-04-19 04:48:07.340788 yusefs_library-0.1/yusefs_library.egg-info/
--rw-r--r--   0 essawifamily   (501) staff       (20)       56 2024-04-19 04:48:07.000000 yusefs_library-0.1/yusefs_library.egg-info/PKG-INFO
--rw-r--r--   0 essawifamily   (501) staff       (20)      257 2024-04-19 04:48:07.000000 yusefs_library-0.1/yusefs_library.egg-info/SOURCES.txt
--rw-r--r--   0 essawifamily   (501) staff       (20)        1 2024-04-19 04:48:07.000000 yusefs_library-0.1/yusefs_library.egg-info/dependency_links.txt
--rw-r--r--   0 essawifamily   (501) staff       (20)       14 2024-04-19 04:48:07.000000 yusefs_library-0.1/yusefs_library.egg-info/requires.txt
--rw-r--r--   0 essawifamily   (501) staff       (20)       15 2024-04-19 04:48:07.000000 yusefs_library-0.1/yusefs_library.egg-info/top_level.txt
+drwxr-xr-x   0 essawifamily   (501) staff       (20)        0 2024-04-19 04:59:14.162761 yusefs_library-0.2/
+-rw-r--r--   0 essawifamily   (501) staff       (20)       56 2024-04-19 04:59:14.162551 yusefs_library-0.2/PKG-INFO
+-rw-r--r--   0 essawifamily   (501) staff       (20)        0 2024-04-19 04:40:37.000000 yusefs_library-0.2/README.md
+-rw-r--r--   0 essawifamily   (501) staff       (20)       38 2024-04-19 04:59:14.162817 yusefs_library-0.2/setup.cfg
+-rw-r--r--   0 essawifamily   (501) staff       (20)      398 2024-04-19 04:58:47.000000 yusefs_library-0.2/setup.py
+drwxr-xr-x   0 essawifamily   (501) staff       (20)        0 2024-04-19 04:59:14.160770 yusefs_library-0.2/yusefs_library/
+-rw-r--r--   0 essawifamily   (501) staff       (20)       37 2024-04-19 04:47:03.000000 yusefs_library-0.2/yusefs_library/__init__.py
+-rw-r--r--   0 essawifamily   (501) staff       (20)       62 2024-04-19 04:42:44.000000 yusefs_library-0.2/yusefs_library/main.py
+drwxr-xr-x   0 essawifamily   (501) staff       (20)        0 2024-04-19 04:59:14.162251 yusefs_library-0.2/yusefs_library.egg-info/
+-rw-r--r--   0 essawifamily   (501) staff       (20)       56 2024-04-19 04:59:14.000000 yusefs_library-0.2/yusefs_library.egg-info/PKG-INFO
+-rw-r--r--   0 essawifamily   (501) staff       (20)      298 2024-04-19 04:59:14.000000 yusefs_library-0.2/yusefs_library.egg-info/SOURCES.txt
+-rw-r--r--   0 essawifamily   (501) staff       (20)        1 2024-04-19 04:59:14.000000 yusefs_library-0.2/yusefs_library.egg-info/dependency_links.txt
+-rw-r--r--   0 essawifamily   (501) staff       (20)       56 2024-04-19 04:59:14.000000 yusefs_library-0.2/yusefs_library.egg-info/entry_points.txt
+-rw-r--r--   0 essawifamily   (501) staff       (20)       14 2024-04-19 04:59:14.000000 yusefs_library-0.2/yusefs_library.egg-info/requires.txt
+-rw-r--r--   0 essawifamily   (501) staff       (20)       15 2024-04-19 04:59:14.000000 yusefs_library-0.2/yusefs_library.egg-info/top_level.txt
```

