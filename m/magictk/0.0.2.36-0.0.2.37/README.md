# Comparing `tmp/magictk-0.0.2.36.tar.gz` & `tmp/magictk-0.0.2.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.36.tar", last modified: Fri Apr 19 08:34:03 2024, max compression
+gzip compressed data, was "magictk-0.0.2.37.tar", last modified: Fri Apr 19 08:36:59 2024, max compression
```

## Comparing `magictk-0.0.2.36.tar` & `magictk-0.0.2.37.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:34:03.025200 magictk-0.0.2.36/
--rw-r--r--   0 root         (0) root         (0)       24 2024-04-19 08:34:02.000000 magictk-0.0.2.36/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-19 08:34:03.025200 magictk-0.0.2.36/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-19 08:34:02.000000 magictk-0.0.2.36/README.md
--rw-r--r--   0 root         (0) root         (0)     3585 2024-04-19 08:34:02.000000 magictk-0.0.2.36/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:34:03.021200 magictk-0.0.2.36/magictk/
--rw-r--r--   0 root         (0) root         (0)      323 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9778 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11146 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    11910 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     6036 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0)     6077 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10457 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:34:03.025200 magictk-0.0.2.36/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      275 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 08:34:02.000000 magictk-0.0.2.36/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 08:34:03.025200 magictk-0.0.2.36/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-19 08:34:02.000000 magictk-0.0.2.36/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:36:59.801680 magictk-0.0.2.37/
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-19 08:36:59.000000 magictk-0.0.2.37/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-19 08:36:59.801680 magictk-0.0.2.37/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-19 08:36:59.000000 magictk-0.0.2.37/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:36:59.801680 magictk-0.0.2.37/magictk/
+-rw-r--r--   0 root         (0) root         (0)      323 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    11910 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     6036 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)    21933 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     6077 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10457 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 08:36:59.801680 magictk-0.0.2.37/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      523 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-19 08:36:59.000000 magictk-0.0.2.37/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 08:36:59.801680 magictk-0.0.2.37/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-19 08:36:59.000000 magictk-0.0.2.37/setup.py
```

### Comparing `magictk-0.0.2.36/README.md` & `magictk-0.0.2.37/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/_window_ctl.py` & `magictk-0.0.2.37/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/_window_size.py` & `magictk-0.0.2.37/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/button.py` & `magictk-0.0.2.37/magictk/button.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/checkbox.py` & `magictk-0.0.2.37/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/color_tmpl.py` & `magictk-0.0.2.37/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/entry.py` & `magictk-0.0.2.37/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/fontconfig.py` & `magictk-0.0.2.37/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/photoload.py` & `magictk-0.0.2.37/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/progressbar.py` & `magictk-0.0.2.37/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/select.py` & `magictk-0.0.2.37/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/submenu.py` & `magictk-0.0.2.37/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/window.py` & `magictk-0.0.2.37/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/magictk/workspace.py` & `magictk-0.0.2.37/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.36/setup.py` & `magictk-0.0.2.37/setup.py`

 * *Files identical despite different names*
