# Comparing `tmp/Comel-0.2.3.tar.gz` & `tmp/comel-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Comel-0.2.3.tar", last modified: Sat Apr  6 09:11:26 2024, max compression
+gzip compressed data, was "comel-0.2.4.tar", last modified: Fri Apr 19 09:27:56 2024, max compression
```

## Comparing `Comel-0.2.3.tar` & `comel-0.2.4.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.188325 Comel-0.2.3/
-drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.187325 Comel-0.2.3/Comel.egg-info/
--rw-rw-rw-   0        0        0     5637 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-06 09:11:26.000000 Comel-0.2.3/Comel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2022-11-18 08:59:38.000000 Comel-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       55 2023-10-28 23:55:47.000000 Comel-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5637 2024-04-06 09:11:26.188325 Comel-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3260 2023-10-28 23:55:47.000000 Comel-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.161978 Comel-0.2.3/comel/
--rw-rw-rw-   0        0        0      197 2024-04-06 09:08:54.000000 Comel-0.2.3/comel/__init__.py
--rw-rw-rw-   0        0        0       35 2023-10-26 13:51:01.000000 Comel-0.2.3/comel/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.185328 Comel-0.2.3/comel/icons/
--rw-rw-rw-   0        0        0      334 2024-03-31 07:32:15.000000 Comel-0.2.3/comel/icons/branch-closed.png
--rw-rw-rw-   0        0        0      182 2024-03-31 07:32:13.000000 Comel-0.2.3/comel/icons/branch-end.png
--rw-rw-rw-   0        0        0      136 2024-03-31 07:32:11.000000 Comel-0.2.3/comel/icons/branch-more.png
--rw-rw-rw-   0        0        0      346 2024-03-31 07:32:17.000000 Comel-0.2.3/comel/icons/branch-open.png
--rw-rw-rw-   0        0        0      698 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/checked-disabled.png
--rw-rw-rw-   0        0        0      578 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/checked.png
--rw-rw-rw-   0        0        0     2916 2024-03-31 07:51:14.000000 Comel-0.2.3/comel/icons/dark-branch-closed.png
--rw-rw-rw-   0        0        0     2932 2024-03-31 07:50:38.000000 Comel-0.2.3/comel/icons/dark-branch-end.png
--rw-rw-rw-   0        0        0     2840 2024-03-31 07:50:31.000000 Comel-0.2.3/comel/icons/dark-branch-more.png
--rw-rw-rw-   0        0        0     2912 2024-03-31 07:51:12.000000 Comel-0.2.3/comel/icons/dark-branch-open.png
--rw-rw-rw-   0        0        0      698 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/dark-checked-disabled.png
--rw-rw-rw-   0        0        0      698 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/dark-checked.png
--rw-rw-rw-   0        0        0      881 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/dark-radio-off.png
--rw-rw-rw-   0        0        0     1107 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/dark-radio-on.png
--rw-rw-rw-   0        0        0     2904 2024-03-31 07:50:34.000000 Comel-0.2.3/comel/icons/dark-vline.png
--rw-rw-rw-   0        0        0     1007 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/radio-off.png
--rw-rw-rw-   0        0        0     1275 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/icons/radio-on.png
--rw-rw-rw-   0        0        0      124 2024-03-31 07:32:08.000000 Comel-0.2.3/comel/icons/vline.png
-drwxrwxrwx   0        0        0        0 2024-04-06 09:11:26.187325 Comel-0.2.3/comel/themes/
--rw-rw-rw-   0        0        0     7932 2024-04-06 09:07:05.000000 Comel-0.2.3/comel/themes/dark.qss
--rw-rw-rw-   0        0        0     7914 2024-04-06 09:07:05.000000 Comel-0.2.3/comel/themes/light.qss
--rw-rw-rw-   0        0        0     1150 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/widgets.py
--rw-rw-rw-   0        0        0     1213 2023-10-28 23:55:47.000000 Comel-0.2.3/comel/wrapper.py
--rw-rw-rw-   0        0        0     1422 2023-10-03 15:35:02.000000 Comel-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       21 2023-10-03 14:05:16.000000 Comel-0.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 09:11:26.188325 Comel-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-10-03 15:35:02.000000 Comel-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:27:56.175689 comel-0.2.4/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:27:56.174688 comel-0.2.4/Comel.egg-info/
+-rw-rw-rw-   0        0        0     5637 2024-04-19 09:27:56.000000 comel-0.2.4/Comel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      987 2024-04-19 09:27:56.000000 comel-0.2.4/Comel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:27:56.000000 comel-0.2.4/Comel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-04-19 09:27:56.000000 comel-0.2.4/Comel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-19 09:27:56.000000 comel-0.2.4/Comel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-10-02 06:08:03.000000 comel-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-10-30 01:14:19.000000 comel-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5637 2024-04-19 09:27:56.174688 comel-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3260 2023-10-30 01:14:19.000000 comel-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 09:27:56.158589 comel-0.2.4/comel/
+-rw-rw-rw-   0        0        0      197 2024-04-19 09:25:14.000000 comel-0.2.4/comel/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-10-27 01:18:51.000000 comel-0.2.4/comel/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:27:56.171689 comel-0.2.4/comel/icons/
+-rw-rw-rw-   0        0        0      389 2024-04-19 06:56:39.000000 comel-0.2.4/comel/icons/branch-closed.png
+-rw-rw-rw-   0        0        0      182 2024-04-01 01:28:02.000000 comel-0.2.4/comel/icons/branch-end.png
+-rw-rw-rw-   0        0        0      136 2024-04-01 01:28:02.000000 comel-0.2.4/comel/icons/branch-more.png
+-rw-rw-rw-   0        0        0      377 2024-04-19 06:56:24.000000 comel-0.2.4/comel/icons/branch-open.png
+-rw-rw-rw-   0        0        0      698 2023-10-30 01:14:19.000000 comel-0.2.4/comel/icons/checked-disabled.png
+-rw-rw-rw-   0        0        0      578 2023-10-30 01:14:19.000000 comel-0.2.4/comel/icons/checked.png
+-rw-rw-rw-   0        0        0     2916 2024-04-01 01:28:02.000000 comel-0.2.4/comel/icons/dark-branch-closed.png
+-rw-rw-rw-   0        0        0     2932 2024-04-01 01:28:02.000000 comel-0.2.4/comel/icons/dark-branch-end.png
+-rw-rw-rw-   0        0        0     2840 2024-04-01 01:28:02.000000 comel-0.2.4/comel/icons/dark-branch-more.png
+-rw-rw-rw-   0        0        0     2912 2024-04-01 01:28:02.000000 comel-0.2.4/comel/icons/dark-branch-open.png
+-rw-rw-rw-   0        0        0      698 2023-10-30 01:14:19.000000 comel-0.2.4/comel/icons/dark-checked-disabled.png
+-rw-rw-rw-   0        0        0      698 2023-10-30 01:14:19.000000 comel-0.2.4/comel/icons/dark-checked.png
+-rw-rw-rw-   0        0        0      881 2023-10-30 01:14:19.000000 comel-0.2.4/comel/icons/dark-radio-off.png
+-rw-rw-rw-   0        0        0     1107 2023-10-30 01:14:19.000000 comel-0.2.4/comel/icons/dark-radio-on.png
+-rw-rw-rw-   0        0        0     2904 2024-04-01 01:28:02.000000 comel-0.2.4/comel/icons/dark-vline.png
+-rw-rw-rw-   0        0        0     1007 2023-10-30 01:14:19.000000 comel-0.2.4/comel/icons/radio-off.png
+-rw-rw-rw-   0        0        0     1275 2023-10-30 01:14:19.000000 comel-0.2.4/comel/icons/radio-on.png
+-rw-rw-rw-   0        0        0      152 2024-04-19 07:52:04.000000 comel-0.2.4/comel/icons/splitter-horz-bg.png
+-rw-rw-rw-   0        0        0      279 2024-04-19 07:11:24.000000 comel-0.2.4/comel/icons/splitter-horz.png
+-rw-rw-rw-   0        0        0      147 2024-04-19 07:51:54.000000 comel-0.2.4/comel/icons/splitter-vert-bg.png
+-rw-rw-rw-   0        0        0      273 2024-04-19 07:13:24.000000 comel-0.2.4/comel/icons/splitter-vert.png
+-rw-rw-rw-   0        0        0      124 2024-04-01 01:28:02.000000 comel-0.2.4/comel/icons/vline.png
+drwxrwxrwx   0        0        0        0 2024-04-19 09:27:56.173690 comel-0.2.4/comel/themes/
+-rw-rw-rw-   0        0        0     8094 2024-04-19 09:22:24.000000 comel-0.2.4/comel/themes/dark.qss
+-rw-rw-rw-   0        0        0     8073 2024-04-19 09:22:24.000000 comel-0.2.4/comel/themes/light.qss
+-rw-rw-rw-   0        0        0     1150 2023-10-30 01:14:19.000000 comel-0.2.4/comel/widgets.py
+-rw-rw-rw-   0        0        0     1213 2023-10-30 01:14:19.000000 comel-0.2.4/comel/wrapper.py
+-rw-rw-rw-   0        0        0     1422 2023-10-26 06:10:44.000000 comel-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       21 2023-10-04 01:13:35.000000 comel-0.2.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:27:56.175689 comel-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-10-04 01:13:35.000000 comel-0.2.4/setup.py
```

### Comparing `Comel-0.2.3/Comel.egg-info/PKG-INFO` & `comel-0.2.4/Comel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Comel
-Version: 0.2.3
+Version: 0.2.4
 Summary: Opinionated PySide6 Light/Dark Theme Toggler.
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Huey Yeng
```

### Comparing `Comel-0.2.3/Comel.egg-info/SOURCES.txt` & `comel-0.2.4/Comel.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -26,10 +26,14 @@
 comel/icons/dark-checked-disabled.png
 comel/icons/dark-checked.png
 comel/icons/dark-radio-off.png
 comel/icons/dark-radio-on.png
 comel/icons/dark-vline.png
 comel/icons/radio-off.png
 comel/icons/radio-on.png
+comel/icons/splitter-horz-bg.png
+comel/icons/splitter-horz.png
+comel/icons/splitter-vert-bg.png
+comel/icons/splitter-vert.png
 comel/icons/vline.png
 comel/themes/dark.qss
 comel/themes/light.qss
```

### Comparing `Comel-0.2.3/LICENSE` & `comel-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/PKG-INFO` & `comel-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Comel
-Version: 0.2.3
+Version: 0.2.4
 Summary: Opinionated PySide6 Light/Dark Theme Toggler.
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Huey Yeng
```

### Comparing `Comel-0.2.3/README.md` & `comel-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/checked-disabled.png` & `comel-0.2.4/comel/icons/checked-disabled.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/checked.png` & `comel-0.2.4/comel/icons/checked.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/dark-branch-closed.png` & `comel-0.2.4/comel/icons/dark-branch-closed.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/dark-branch-end.png` & `comel-0.2.4/comel/icons/dark-branch-end.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/dark-branch-more.png` & `comel-0.2.4/comel/icons/dark-branch-more.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/dark-branch-open.png` & `comel-0.2.4/comel/icons/dark-branch-open.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/dark-checked-disabled.png` & `comel-0.2.4/comel/icons/dark-checked-disabled.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/dark-checked.png` & `comel-0.2.4/comel/icons/dark-checked.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/dark-radio-off.png` & `comel-0.2.4/comel/icons/dark-radio-off.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/dark-radio-on.png` & `comel-0.2.4/comel/icons/dark-radio-on.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/dark-vline.png` & `comel-0.2.4/comel/icons/dark-vline.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/radio-off.png` & `comel-0.2.4/comel/icons/radio-off.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/icons/radio-on.png` & `comel-0.2.4/comel/icons/radio-on.png`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/themes/dark.qss` & `comel-0.2.4/comel/themes/dark.qss`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
 ::section {
   background-color: #474f56;
 }
 
 QListView, QTableView, QTreeView {
   background-color: rgb(85, 90, 95);
+  alternate-background-color: rgb(65, 70, 75);
   selection-color: #ffffff;
   selection-background-color: rgb(120, 135, 155);
 }
 
 QListView:disabled, QTableView:disabled, QTreeView:disabled {
   background-color: rgb(49, 54, 59);
   selection-color: rgb(89, 94, 99);
@@ -246,19 +247,21 @@
 QGroupBox::title {
   subcontrol-origin: margin;
   left: 10px;
   padding: 0 3px 0 3px;
 }
 
 QSplitter::handle:horizontal {
-  border: 1px outset rgb(80, 80, 80);
+  image: url(cicons:splitter-horz.png);
+  background-image: url(cicons:splitter-horz-bg.png);
 }
 
 QSplitter::handle:vertical {
-  border: 1px outset rgb(80, 80, 80);
+  image: url(cicons:splitter-vert.png);
+  background-image: url(cicons:splitter-vert-bg.png);
 }
 
 QSpinBox {
   background-color: rgb(85, 90, 95);
   border: 1px solid rgb(128, 128, 128);
 }
```

### Comparing `Comel-0.2.3/comel/themes/light.qss` & `comel-0.2.4/comel/themes/light.qss`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
 ::section {
   background-color: rgb(250, 250, 250);
 }
 
 QListView, QTableView, QTreeView {
   background-color: white;
+  alternate-background-color: rgb(245, 245, 245);
   selection-color: #555555;
   selection-background-color: rgb(230, 239, 253);
 }
 
 QListView:disabled, QTableView:disabled, QTreeView:disabled {
   background-color: rgb(240, 240, 240);
   selection-color: rgb(211, 211, 211);
@@ -246,19 +247,21 @@
 QGroupBox::title {
   subcontrol-origin: margin;
   left: 10px;
   padding: 0 3px 0 3px;
 }
 
 QSplitter::handle:horizontal {
-  border: 1px outset rgb(211, 211, 211);
+  image: url(cicons:splitter-horz.png);
+  background-image: url(cicons:splitter-horz-bg.png);
 }
 
 QSplitter::handle:vertical {
-  border: 1px outset rgb(211, 211, 211);
+  image: url(cicons:splitter-vert.png);
+  background-image: url(cicons:splitter-vert-bg.png);
 }
 
 QSpinBox {
   background-color: white;
   border: 1px solid rgb(184, 184, 184);
 }
```

### Comparing `Comel-0.2.3/comel/widgets.py` & `comel-0.2.4/comel/widgets.py`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/comel/wrapper.py` & `comel-0.2.4/comel/wrapper.py`

 * *Files identical despite different names*

### Comparing `Comel-0.2.3/pyproject.toml` & `comel-0.2.4/pyproject.toml`

 * *Files identical despite different names*

