# Comparing `tmp/whyis-activitystreams-0.0.4.tar.gz` & `tmp/whyis_activitystreams-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyis-activitystreams-0.0.4.tar", last modified: Tue Jan 30 16:30:53 2024, max compression
+gzip compressed data, was "whyis_activitystreams-0.0.5.tar", last modified: Fri Apr 19 06:52:31 2024, max compression
```

## Comparing `whyis-activitystreams-0.0.4.tar` & `whyis_activitystreams-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-01-30 16:30:53.480670 whyis-activitystreams-0.0.4/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)    11357 2024-01-28 07:20:34.000000 whyis-activitystreams-0.0.4/LICENSE
--rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-01-30 16:30:53.480670 whyis-activitystreams-0.0.4/PKG-INFO
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       23 2024-01-28 07:20:34.000000 whyis-activitystreams-0.0.4/README.md
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      516 2024-01-30 16:30:25.000000 whyis-activitystreams-0.0.4/pyproject.toml
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       38 2024-01-30 16:30:53.480670 whyis-activitystreams-0.0.4/setup.cfg
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-01-30 16:30:53.476670 whyis-activitystreams-0.0.4/whyis_activitystreams/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       22 2024-01-28 07:33:16.000000 whyis-activitystreams-0.0.4/whyis_activitystreams/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-01-29 08:29:08.000000 whyis-activitystreams-0.0.4/whyis_activitystreams/_version.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-01-30 16:30:53.480670 whyis-activitystreams-0.0.4/whyis_activitystreams/activity_agent/
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-01-29 07:53:41.000000 whyis-activitystreams-0.0.4/whyis_activitystreams/activity_agent/__init__.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1665 2024-01-30 15:52:58.000000 whyis-activitystreams-0.0.4/whyis_activitystreams/activity_agent/activity_agent.py
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      137 2024-01-29 05:48:11.000000 whyis-activitystreams-0.0.4/whyis_activitystreams/plugin.py
-drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-01-30 16:30:53.480670 whyis-activitystreams-0.0.4/whyis_activitystreams.egg-info/
--rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-01-30 16:30:53.000000 whyis-activitystreams-0.0.4/whyis_activitystreams.egg-info/PKG-INFO
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      508 2024-01-30 16:30:53.000000 whyis-activitystreams-0.0.4/whyis_activitystreams.egg-info/SOURCES.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        1 2024-01-30 16:30:53.000000 whyis-activitystreams-0.0.4/whyis_activitystreams.egg-info/dependency_links.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      150 2024-01-30 16:30:53.000000 whyis-activitystreams-0.0.4/whyis_activitystreams.egg-info/entry_points.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        6 2024-01-30 16:30:53.000000 whyis-activitystreams-0.0.4/whyis_activitystreams.egg-info/requires.txt
--rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       22 2024-01-30 16:30:53.000000 whyis-activitystreams-0.0.4/whyis_activitystreams.egg-info/top_level.txt
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 06:52:31.156129 whyis_activitystreams-0.0.5/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)    11357 2024-01-28 07:20:34.000000 whyis_activitystreams-0.0.5/LICENSE
+-rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 06:52:31.152130 whyis_activitystreams-0.0.5/PKG-INFO
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     3708 2024-02-06 16:09:12.000000 whyis_activitystreams-0.0.5/README.md
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      517 2024-04-19 03:26:36.000000 whyis_activitystreams-0.0.5/pyproject.toml
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       38 2024-04-19 06:52:31.156129 whyis_activitystreams-0.0.5/setup.cfg
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 06:52:31.152130 whyis_activitystreams-0.0.5/whyis_activitystreams/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       52 2024-02-06 15:00:14.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       71 2024-01-29 08:29:08.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/_version.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 06:52:31.152130 whyis_activitystreams-0.0.5/whyis_activitystreams/activity_agent/
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       30 2024-01-29 07:53:41.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/activity_agent/__init__.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)     1650 2024-04-19 04:22:39.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/activity_agent/activity_agent.py
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      137 2024-01-29 05:48:11.000000 whyis_activitystreams-0.0.5/whyis_activitystreams/plugin.py
+drwxrwxr-x   0 sabbir    (1000) sabbir    (1000)        0 2024-04-19 06:52:31.152130 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/
+-rw-r--r--   0 sabbir    (1000) sabbir    (1000)      183 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/PKG-INFO
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      508 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        1 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)      150 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/entry_points.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)        6 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/requires.txt
+-rw-rw-r--   0 sabbir    (1000) sabbir    (1000)       22 2024-04-19 06:52:31.000000 whyis_activitystreams-0.0.5/whyis_activitystreams.egg-info/top_level.txt
```

### Comparing `whyis-activitystreams-0.0.4/LICENSE` & `whyis_activitystreams-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whyis-activitystreams-0.0.4/pyproject.toml` & `whyis_activitystreams-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name='whyis-activitystreams'
-version='0.0.4'
+version='0.0.5'
 description = "A whyis plugin to support the interpretation of activity streams."
 dependencies=[
   'whyis',
 ]
+
 [tool.setuptools]
 packages=['whyis_activitystreams', 'whyis_activitystreams.activity_agent']
 
 [project.entry-points.whyis]
 whyis_activitystreams = "whyis_activitystreams:ActivityStreamsPlugin"
 whyis_activity_agent = "whyis_activitystreams.activity_agent:ActivityAgent"
```

