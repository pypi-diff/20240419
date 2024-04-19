# Comparing `tmp/simpleworkspace-1.2.184.tar.gz` & `tmp/simpleworkspace-1.2.185.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworkspace-1.2.184.tar", last modified: Sat Mar 30 18:55:43 2024, max compression
+gzip compressed data, was "simpleworkspace-1.2.185.tar", last modified: Fri Apr 19 16:31:13 2024, max compression
```

## Comparing `simpleworkspace-1.2.184.tar` & `simpleworkspace-1.2.185.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.548162 simpleworkspace-1.2.184/
--rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.184/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2024-03-30 18:55:43.538162 simpleworkspace-1.2.184/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-03-30 18:53:09.000000 simpleworkspace-1.2.184/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 18:55:43.549726 simpleworkspace-1.2.184/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:42.746563 simpleworkspace-1.2.184/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:42.879640 simpleworkspace-1.2.184/src/simpleworkspace/
--rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.184/src/simpleworkspace/__init__.py
--rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.184/src/simpleworkspace/__lazyimporter__.py
--rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.184/src/simpleworkspace/app.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:42.966761 simpleworkspace-1.2.184/src/simpleworkspace/assets/
--rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:42.983844 simpleworkspace-1.2.184/src/simpleworkspace/assets/__pycache__/
--rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:42.758343 simpleworkspace-1.2.184/src/simpleworkspace/assets/audio/
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:42.991987 simpleworkspace-1.2.184/src/simpleworkspace/assets/audio/alarms/
--rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/audio/alarms/Siren.wav
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.016094 simpleworkspace-1.2.184/src/simpleworkspace/assets/audio/notifications/
--rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/audio/notifications/Completed.wav
--rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/audio/notifications/Error.wav
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.089172 simpleworkspace-1.2.184/src/simpleworkspace/assets/icons/
--rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/icons/ErrorCircle.png
--rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/icons/InfoCircle.png
--rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/icons/QuestionCircle.png
--rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.184/src/simpleworkspace/assets/icons/WarningCircle.png
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.109559 simpleworkspace-1.2.184/src/simpleworkspace/collections/
--rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/collections/__init__.py
--rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/collections/loader.py
--rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.184/src/simpleworkspace/collections/observables.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.137922 simpleworkspace-1.2.184/src/simpleworkspace/db/
--rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.184/src/simpleworkspace/db/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.184/src/simpleworkspace/db/dbfactory.py
--rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.184/src/simpleworkspace/db/fluentsqlbuilder.py
--rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/db/loader.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.178638 simpleworkspace-1.2.184/src/simpleworkspace/gui/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.184/src/simpleworkspace/gui/__init__.py
--rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.184/src/simpleworkspace/gui/dialogs.py
--rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.184/src/simpleworkspace/gui/loader.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.233491 simpleworkspace-1.2.184/src/simpleworkspace/io/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/__init__.py
--rw-rw-rw-   0        0        0     9009 2024-02-25 18:43:27.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/archive.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.258529 simpleworkspace-1.2.184/src/simpleworkspace/io/audio/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/audio/__init__.py
--rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/audio/loader.py
--rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/audio/play.py
--rw-rw-rw-   0        0        0     5574 2024-02-28 16:08:09.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/directory.py
--rw-rw-rw-   0        0        0     2962 2024-02-07 20:22:40.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/file.py
--rw-rw-rw-   0        0        0      705 2024-02-23 06:39:35.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/loader.py
--rw-rw-rw-   0        0        0     6058 2024-02-21 21:38:25.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/path.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.290076 simpleworkspace-1.2.184/src/simpleworkspace/io/readers/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/readers/__init__.py
--rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/readers/csvreader.py
--rw-rw-rw-   0        0        0      321 2023-12-11 19:38:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/readers/loader.py
--rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.184/src/simpleworkspace/io/readers/logreader.py
--rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.184/src/simpleworkspace/loader.py
--rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.184/src/simpleworkspace/logproviders.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:42.835030 simpleworkspace-1.2.184/src/simpleworkspace/packages/
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.292108 simpleworkspace-1.2.184/src/simpleworkspace/packages/debug/
--rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/debug/profiler.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:42.821099 simpleworkspace-1.2.184/src/simpleworkspace/packages/network/
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.302042 simpleworkspace-1.2.184/src/simpleworkspace/packages/network/servers/
--rw-rw-rw-   0        0        0    10843 2024-02-04 13:59:24.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/network/servers/basicserver.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.308591 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.313981 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/
--rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.334407 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
--rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
--rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
--rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
--rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
--rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
--rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.340188 simpleworkspace-1.2.184/src/simpleworkspace/packages/taskscheduler/
--rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/taskscheduler/__init__.py
--rw-rw-rw-   0        0        0     8961 2024-02-25 08:04:38.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/taskscheduler/manager.py
--rw-rw-rw-   0        0        0     4389 2024-02-04 17:20:14.000000 simpleworkspace-1.2.184/src/simpleworkspace/packages/taskscheduler/model.py
--rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.184/src/simpleworkspace/settingsproviders.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.405597 simpleworkspace-1.2.184/src/simpleworkspace/types/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.184/src/simpleworkspace/types/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.184/src/simpleworkspace/types/byte.py
--rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/types/iunit.py
--rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/types/loader.py
--rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/types/measurement.py
--rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.184/src/simpleworkspace/types/os.py
--rw-rw-rw-   0        0        0     8243 2023-09-27 18:18:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/types/time.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.528917 simpleworkspace-1.2.184/src/simpleworkspace/utility/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/__init__.py
--rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/bytes.py
--rw-rw-rw-   0        0        0     1915 2023-12-12 18:58:31.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/cache.py
--rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/console.py
--rw-rw-rw-   0        0        0    14495 2024-02-14 19:32:38.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/linq.py
--rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/loader.py
--rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/module.py
--rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/parallel.py
--rw-rw-rw-   0        0        0    11207 2024-03-18 16:44:18.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/progressbar.py
--rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/regex.py
--rw-rw-rw-   0        0        0     1865 2024-02-07 19:12:33.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/strings.py
--rw-rw-rw-   0        0        0     6758 2024-03-02 16:36:06.000000 simpleworkspace-1.2.184/src/simpleworkspace/utility/time.py
-drwxrwxrwx   0        0        0        0 2024-03-30 18:55:43.538162 simpleworkspace-1.2.184/src/simpleworkspace.egg-info/
--rw-rw-rw-   0        0        0      148 2024-03-30 18:55:42.000000 simpleworkspace-1.2.184/src/simpleworkspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3310 2024-03-30 18:55:42.000000 simpleworkspace-1.2.184/src/simpleworkspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 18:55:42.000000 simpleworkspace-1.2.184/src/simpleworkspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-30 18:55:42.000000 simpleworkspace-1.2.184/src/simpleworkspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-30 18:55:42.000000 simpleworkspace-1.2.184/src/simpleworkspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:13.615781 simpleworkspace-1.2.185/
+-rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.185/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2024-04-19 16:31:13.610229 simpleworkspace-1.2.185/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-04-19 16:28:55.000000 simpleworkspace-1.2.185/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 16:31:13.615781 simpleworkspace-1.2.185/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.259435 simpleworkspace-1.2.185/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.667587 simpleworkspace-1.2.185/src/simpleworkspace/
+-rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.185/src/simpleworkspace/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.185/src/simpleworkspace/__lazyimporter__.py
+-rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.185/src/simpleworkspace/app.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.783424 simpleworkspace-1.2.185/src/simpleworkspace/assets/
+-rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.805411 simpleworkspace-1.2.185/src/simpleworkspace/assets/__pycache__/
+-rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.282005 simpleworkspace-1.2.185/src/simpleworkspace/assets/audio/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.828720 simpleworkspace-1.2.185/src/simpleworkspace/assets/audio/alarms/
+-rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/audio/alarms/Siren.wav
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.864502 simpleworkspace-1.2.185/src/simpleworkspace/assets/audio/notifications/
+-rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/audio/notifications/Completed.wav
+-rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/audio/notifications/Error.wav
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.922954 simpleworkspace-1.2.185/src/simpleworkspace/assets/icons/
+-rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/icons/ErrorCircle.png
+-rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/icons/InfoCircle.png
+-rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/icons/QuestionCircle.png
+-rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.185/src/simpleworkspace/assets/icons/WarningCircle.png
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.964804 simpleworkspace-1.2.185/src/simpleworkspace/collections/
+-rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/collections/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/collections/loader.py
+-rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.185/src/simpleworkspace/collections/observables.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.056623 simpleworkspace-1.2.185/src/simpleworkspace/db/
+-rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.185/src/simpleworkspace/db/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.185/src/simpleworkspace/db/dbfactory.py
+-rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.185/src/simpleworkspace/db/fluentsqlbuilder.py
+-rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/db/loader.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.113958 simpleworkspace-1.2.185/src/simpleworkspace/gui/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.185/src/simpleworkspace/gui/__init__.py
+-rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.185/src/simpleworkspace/gui/dialogs.py
+-rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.185/src/simpleworkspace/gui/loader.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.360414 simpleworkspace-1.2.185/src/simpleworkspace/io/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/__init__.py
+-rw-rw-rw-   0        0        0     9009 2024-02-25 18:43:27.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/archive.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.384927 simpleworkspace-1.2.185/src/simpleworkspace/io/audio/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/audio/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/audio/loader.py
+-rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/audio/play.py
+-rw-rw-rw-   0        0        0     5574 2024-02-28 16:08:09.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/directory.py
+-rw-rw-rw-   0        0        0     2962 2024-02-07 20:22:40.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/file.py
+-rw-rw-rw-   0        0        0      705 2024-02-23 06:39:35.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/loader.py
+-rw-rw-rw-   0        0        0     6058 2024-02-21 21:38:25.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/path.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.476775 simpleworkspace-1.2.185/src/simpleworkspace/io/readers/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/readers/__init__.py
+-rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/readers/csvreader.py
+-rw-rw-rw-   0        0        0      321 2023-12-11 19:38:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/readers/loader.py
+-rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.185/src/simpleworkspace/io/readers/logreader.py
+-rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.185/src/simpleworkspace/loader.py
+-rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.185/src/simpleworkspace/logproviders.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.399027 simpleworkspace-1.2.185/src/simpleworkspace/packages/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.499380 simpleworkspace-1.2.185/src/simpleworkspace/packages/debug/
+-rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/debug/profiler.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:11.374753 simpleworkspace-1.2.185/src/simpleworkspace/packages/network/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.541264 simpleworkspace-1.2.185/src/simpleworkspace/packages/network/servers/
+-rw-rw-rw-   0        0        0    10843 2024-02-04 13:59:24.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/network/servers/basicserver.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.586868 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.596770 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/
+-rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.804032 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
+-rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
+-rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
+-rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
+-rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
+-rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
+-rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:12.840646 simpleworkspace-1.2.185/src/simpleworkspace/packages/taskscheduler/
+-rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/taskscheduler/__init__.py
+-rw-rw-rw-   0        0        0     8953 2024-04-19 16:09:12.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/taskscheduler/manager.py
+-rw-rw-rw-   0        0        0     5122 2024-04-19 16:21:13.000000 simpleworkspace-1.2.185/src/simpleworkspace/packages/taskscheduler/model.py
+-rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.185/src/simpleworkspace/settingsproviders.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:13.146955 simpleworkspace-1.2.185/src/simpleworkspace/types/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.185/src/simpleworkspace/types/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.185/src/simpleworkspace/types/byte.py
+-rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/types/iunit.py
+-rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/types/loader.py
+-rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/types/measurement.py
+-rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.185/src/simpleworkspace/types/os.py
+-rw-rw-rw-   0        0        0     8243 2023-09-27 18:18:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/types/time.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:13.563472 simpleworkspace-1.2.185/src/simpleworkspace/utility/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/bytes.py
+-rw-rw-rw-   0        0        0     1915 2023-12-12 18:58:31.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/cache.py
+-rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/console.py
+-rw-rw-rw-   0        0        0    14495 2024-02-14 19:32:38.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/linq.py
+-rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/loader.py
+-rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/module.py
+-rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/parallel.py
+-rw-rw-rw-   0        0        0    11207 2024-03-18 16:44:18.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/progressbar.py
+-rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/regex.py
+-rw-rw-rw-   0        0        0     1865 2024-02-07 19:12:33.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/strings.py
+-rw-rw-rw-   0        0        0     6758 2024-03-02 16:36:06.000000 simpleworkspace-1.2.185/src/simpleworkspace/utility/time.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:31:13.571487 simpleworkspace-1.2.185/src/simpleworkspace.egg-info/
+-rw-rw-rw-   0        0        0      148 2024-04-19 16:31:10.000000 simpleworkspace-1.2.185/src/simpleworkspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3310 2024-04-19 16:31:11.000000 simpleworkspace-1.2.185/src/simpleworkspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 16:31:10.000000 simpleworkspace-1.2.185/src/simpleworkspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 16:31:10.000000 simpleworkspace-1.2.185/src/simpleworkspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 16:31:10.000000 simpleworkspace-1.2.185/src/simpleworkspace.egg-info/top_level.txt
```

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/app.py` & `simpleworkspace-1.2.185/src/simpleworkspace/app.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/__init__.py` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/audio/alarms/Siren.wav` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/audio/alarms/Siren.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/audio/notifications/Completed.wav` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/audio/notifications/Completed.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/audio/notifications/Error.wav` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/audio/notifications/Error.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/icons/ErrorCircle.png` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/icons/ErrorCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/icons/InfoCircle.png` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/icons/InfoCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/icons/QuestionCircle.png` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/icons/QuestionCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/assets/icons/WarningCircle.png` & `simpleworkspace-1.2.185/src/simpleworkspace/assets/icons/WarningCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/collections/observables.py` & `simpleworkspace-1.2.185/src/simpleworkspace/collections/observables.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/db/dbfactory.py` & `simpleworkspace-1.2.185/src/simpleworkspace/db/dbfactory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/db/fluentsqlbuilder.py` & `simpleworkspace-1.2.185/src/simpleworkspace/db/fluentsqlbuilder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/gui/dialogs.py` & `simpleworkspace-1.2.185/src/simpleworkspace/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/io/archive.py` & `simpleworkspace-1.2.185/src/simpleworkspace/io/archive.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/io/audio/play.py` & `simpleworkspace-1.2.185/src/simpleworkspace/io/audio/play.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/io/directory.py` & `simpleworkspace-1.2.185/src/simpleworkspace/io/directory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/io/file.py` & `simpleworkspace-1.2.185/src/simpleworkspace/io/file.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/io/loader.py` & `simpleworkspace-1.2.185/src/simpleworkspace/io/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/io/path.py` & `simpleworkspace-1.2.185/src/simpleworkspace/io/path.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/io/readers/csvreader.py` & `simpleworkspace-1.2.185/src/simpleworkspace/io/readers/csvreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/io/readers/logreader.py` & `simpleworkspace-1.2.185/src/simpleworkspace/io/readers/logreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/loader.py` & `simpleworkspace-1.2.185/src/simpleworkspace/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/logproviders.py` & `simpleworkspace-1.2.185/src/simpleworkspace/logproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/packages/debug/profiler.py` & `simpleworkspace-1.2.185/src/simpleworkspace/packages/debug/profiler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/packages/network/servers/basicserver.py` & `simpleworkspace-1.2.185/src/simpleworkspace/packages/network/servers/basicserver.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py` & `simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py` & `simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py` & `simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py` & `simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py` & `simpleworkspace-1.2.185/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/packages/taskscheduler/manager.py` & `simpleworkspace-1.2.185/src/simpleworkspace/packages/taskscheduler/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             #skip tasks without schedules, eg no interval or custom nextschedule handler
             if(not task._HasEvent_Schedule):
                 continue
 
             scheduleName = ""
             if(task.task_interval is not None):
                 scheduleName += str(task.task_interval.InSeconds())
-            if(task.NextSchedule.__func__ is not ITask.NextSchedule):
+            if (task._HasImplementedFunc(task.NextSchedule)):
                 scheduleName += f"FN"
 
             if(task._task_id not in taskSettings) or (taskSettings[task._task_id]["scheduleName"] != scheduleName):
                 taskSettings[task._task_id] = {
                     "scheduleName": scheduleName,
                     "lastRunDate": None
                 }
```

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/packages/taskscheduler/model.py` & `simpleworkspace-1.2.185/src/simpleworkspace/packages/taskscheduler/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC
 from datetime import datetime
 from simpleworkspace.types.time import TimeSpan
 from datetime import datetime, timedelta
+import types
 
 class ITask(ABC):
     '''
     Tasks needs to implement this interface to be loaded into task scheduler
 
     Implementation:
         * To have scheduled tasks implement: On_Schedule() together with either task_interval OR NextSchedule()
@@ -55,57 +56,71 @@
         nextRunDate = previousRunDate + timedelta(seconds=self.task_interval.InSeconds())
         if(datetime.now() > nextRunDate):
             return True
         return False
     
     @property 
     def _HasEvent_Schedule(self):
-        if(self.task_interval is None) and (self.NextSchedule.__func__ is ITask.NextSchedule): # no scheduler used, therefore would never be triggered
+        if(self.task_interval is None) and not (self._HasImplementedFunc(self.NextSchedule)): # no scheduler used, therefore would never be triggered
             return False
-        if(self.On_Schedule.__func__ is ITask.On_Schedule): #schedule function is not implemented, therefore no actions to perform
+        if not (self._HasImplementedFunc(self.On_Schedule)): #schedule function is not implemented, therefore no actions to perform
             return False
         return True
 
     @property
     def _HasEvent_StartUp(self):
-        if(self.On_StartUp.__func__ is ITask.On_StartUp): #startup function is not implemented
+        if not(self._HasImplementedFunc(self.On_StartUp)): #startup function is not implemented
             return False
         return True
 
+    def _HasImplementedFunc(self, func: types.FunctionType|types.MethodType):
+        #a methodtype is a class method, a functiontype on other hand is lamdba or local function etc
+
+        if(isinstance(func, types.MethodType)) and ( func.__func__ is getattr(ITask, func.__name__)): #still original method
+            return False
+        return True
+    
     def __new__(cls, *args, **kwargs):
         '''Gives possibility to ensure logic always run even if __init__ is left out. __init__ runs after this method has ran to completion'''
         instance = super().__new__(cls)
         instance._task_id = cls.__module__ + "." + cls.__name__
         return instance
     
 
 class CommandTask(ITask):
     '''Premade task for running a simple command'''
-    def __init__(self, interval:TimeSpan, command:str|list[str]) -> None:
+    def __init__(self, command:str|list[str], schedule_interval:TimeSpan=None, schedule_startup=False) -> None:
         from hashlib import md5
         import shlex
 
         super().__init__()
 
-        self.task_interval = interval
-        if type(interval) is not TimeSpan:
-            raise TypeError(f"interval must be of type {type(TimeSpan)}")
+        if(schedule_interval is None) and not (schedule_startup):
+            raise ValueError("No schedules specified for command, use interval or startup")
+        
+        if(schedule_interval is not None):
+            if type(schedule_interval) is not TimeSpan:
+                raise TypeError(f"interval must be of type {type(TimeSpan)}")
+            self.task_interval = schedule_interval
+        if schedule_startup:
+            def On_StartUp():
+                return self.On_Schedule()
+            self.On_StartUp = On_StartUp
+            
         if isinstance(command, str):
             command = shlex.split(command)
         self.command = command
         commandStringRepresentation = ' '.join(command)
         self.task_description = commandStringRepresentation
 
         #adjust taskid since normal retrieved task id would not be unique per command
         self._task_id = md5(commandStringRepresentation.encode()).hexdigest()[:16]
 
-    
     def On_Schedule(self):
         import subprocess
-        from simpleworkspace.types.os import OperatingSystemEnum
 
         result = subprocess.run(self.command, text=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         message = ""
         if(result.returncode != 0): #something went bad
             stderr = ""
             if(result.stderr is not None):
                 stderr = result.stderr.rstrip()
```

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/settingsproviders.py` & `simpleworkspace-1.2.185/src/simpleworkspace/settingsproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/types/byte.py` & `simpleworkspace-1.2.185/src/simpleworkspace/types/byte.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/types/iunit.py` & `simpleworkspace-1.2.185/src/simpleworkspace/types/iunit.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/types/measurement.py` & `simpleworkspace-1.2.185/src/simpleworkspace/types/measurement.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/types/os.py` & `simpleworkspace-1.2.185/src/simpleworkspace/types/os.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/types/time.py` & `simpleworkspace-1.2.185/src/simpleworkspace/types/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/cache.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/cache.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/console.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/console.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/linq.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/linq.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/loader.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/module.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/module.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/parallel.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/parallel.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/progressbar.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/progressbar.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/regex.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/regex.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/strings.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/strings.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace/utility/time.py` & `simpleworkspace-1.2.185/src/simpleworkspace/utility/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.184/src/simpleworkspace.egg-info/SOURCES.txt` & `simpleworkspace-1.2.185/src/simpleworkspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

