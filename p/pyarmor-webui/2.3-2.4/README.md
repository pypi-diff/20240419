# Comparing `tmp/pyarmor-webui-2.3.zip` & `tmp/pyarmor-webui-2.4.zip`

## zipinfo {}

```diff
@@ -1,58 +1,58 @@
-Zip file size: 362477 bytes, number of entries: 56
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 15:08 pyarmor-webui-2.3/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 15:08 pyarmor-webui-2.3/pyarmor_webui.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 15:08 pyarmor-webui-2.3/test/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 15:08 pyarmor-webui-2.3/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 15:08 pyarmor-webui-2.3/data/
--rw-r--r--  2.0 unx     4848 b- defN 24-Mar-27 15:08 pyarmor-webui-2.3/PKG-INFO
--rw-r--r--  2.0 unx     9109 b- defN 24-Mar-27 13:25 pyarmor-webui-2.3/server.py
--rw-r--r--  2.0 unx    18983 b- defN 23-May-12 14:58 pyarmor-webui-2.3/handler.py
--rw-r--r--  2.0 unx     1068 b- defN 19-Dec-31 08:11 pyarmor-webui-2.3/LICENSE
--rwxr-xr-x  2.0 unx        0 b- defN 20-Mar-27 08:49 pyarmor-webui-2.3/__init__.py
--rw-r--r--  2.0 unx    18450 b- defN 24-Mar-27 15:04 pyarmor-webui-2.3/handler8.py
--rw-r--r--  2.0 unx     2241 b- defN 24-Mar-27 13:25 pyarmor-webui-2.3/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Mar-27 15:08 pyarmor-webui-2.3/setup.cfg
--rw-r--r--  2.0 unx     4009 b- defN 24-Mar-27 15:07 pyarmor-webui-2.3/README.rst
--rw-r--r--  2.0 unx     4848 b- defN 24-Mar-27 15:08 pyarmor-webui-2.3/pyarmor_webui.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     1331 b- defN 24-Mar-27 15:08 pyarmor-webui-2.3/pyarmor_webui.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       61 b- defN 24-Mar-27 15:08 pyarmor-webui-2.3/pyarmor_webui.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 24-Mar-27 15:08 pyarmor-webui-2.3/pyarmor_webui.egg-info/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Mar-27 15:08 pyarmor-webui-2.3/pyarmor_webui.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-27 15:08 pyarmor-webui-2.3/pyarmor_webui.egg-info/dependency_links.txt
--rwxr-xr-x  2.0 unx     1027 b- defN 20-Apr-27 09:39 pyarmor-webui-2.3/test/pack_one_folder_bundle.robot
--rwxr-xr-x  2.0 unx      693 b- defN 20-Oct-30 08:30 pyarmor-webui-2.3/test/generate_expired_license.robot
--rwxr-xr-x  2.0 unx     1475 b- defN 20-Apr-27 09:39 pyarmor-webui-2.3/test/pack_one_file_bundle_with_outer_license.robot
--rwxr-xr-x  2.0 unx     1245 b- defN 20-Jan-19 10:10 pyarmor-webui-2.3/test/obfuscate_multiple_entries.robot
--rwxr-xr-x  2.0 unx      890 b- defN 20-Apr-27 09:40 pyarmor-webui-2.3/test/generate_machine_license.robot
--rwxr-xr-x  2.0 unx     1164 b- defN 20-Jan-19 10:08 pyarmor-webui-2.3/test/obfuscate_one_script.robot
--rw-r--r--  2.0 unx     1899 b- defN 20-Apr-27 09:25 pyarmor-webui-2.3/test/README.md
--rwxr-xr-x  2.0 unx      777 b- defN 20-Apr-27 09:41 pyarmor-webui-2.3/test/generate_extra_data_license.robot
--rwxr-xr-x  2.0 unx     1230 b- defN 20-Jan-19 10:30 pyarmor-webui-2.3/test/obfuscate_one_package.robot
--rwxr-xr-x  2.0 unx     6422 b- defN 23-May-12 10:17 pyarmor-webui-2.3/test/resource.robot
--rwxr-xr-x  2.0 unx     1358 b- defN 20-Apr-27 09:39 pyarmor-webui-2.3/test/pack_with_data_file.robot
--rwxr-xr-x  2.0 unx     1139 b- defN 20-Apr-27 09:38 pyarmor-webui-2.3/test/pack_one_file_bundle.robot
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 15:08 pyarmor-webui-2.3/static/css/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 15:08 pyarmor-webui-2.3/static/js/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 15:08 pyarmor-webui-2.3/static/img/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-27 15:08 pyarmor-webui-2.3/static/fonts/
--rw-r--r--  2.0 unx     4286 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/favicon.ico
--rw-r--r--  2.0 unx      898 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/index.html
--rw-r--r--  2.0 unx    19211 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/reqwest.js
--rw-r--r--  2.0 unx   191299 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/css/chunk-vendors.b79ff3a2.css
--rw-r--r--  2.0 unx     1166 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/css/app.31abab10.css
--rw-r--r--  2.0 unx   127753 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/js/app.d0b3d54c.js
--rw-r--r--  2.0 unx   718168 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/js/chunk-vendors.4afc1da0.js
--rw-r--r--  2.0 unx      890 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/cog.svg
--rw-r--r--  2.0 unx      207 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/folder-solid.svg
--rw-r--r--  2.0 unx      356 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/tablet-alt.svg
--rw-r--r--  2.0 unx      339 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/shield-alt.svg
--rw-r--r--  2.0 unx      935 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/calendar-alt.svg
--rw-r--r--  2.0 unx    14781 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/logo.a8954ff0.png
--rw-r--r--  2.0 unx      734 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/registered.svg
--rw-r--r--  2.0 unx      446 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/calendar-minus.svg
--rw-r--r--  2.0 unx      349 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/calendar.svg
--rw-r--r--  2.0 unx      307 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/img/folder.svg
--rw-r--r--  2.0 unx    28200 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/fonts/element-icons.535877f5.woff
--rw-r--r--  2.0 unx    55956 b- defN 24-Mar-27 14:28 pyarmor-webui-2.3/static/fonts/element-icons.732389de.ttf
--rw-r--r--  2.0 unx      205 b- defN 23-May-20 06:08 pyarmor-webui-2.3/data/copy_license.py
-56 files, 1250815 bytes uncompressed, 353595 bytes compressed:  71.7%
+Zip file size: 362567 bytes, number of entries: 56
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 19:12 pyarmor-webui-2.4/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 19:12 pyarmor-webui-2.4/pyarmor_webui.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 19:12 pyarmor-webui-2.4/test/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 19:12 pyarmor-webui-2.4/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 19:12 pyarmor-webui-2.4/data/
+-rw-r--r--  2.0 unx     4990 b- defN 24-Apr-19 19:12 pyarmor-webui-2.4/PKG-INFO
+-rw-r--r--  2.0 unx     9109 b- defN 24-Apr-19 18:20 pyarmor-webui-2.4/server.py
+-rw-r--r--  2.0 unx    19099 b- defN 24-Apr-19 15:49 pyarmor-webui-2.4/handler.py
+-rw-r--r--  2.0 unx     1068 b- defN 19-Dec-31 08:11 pyarmor-webui-2.4/LICENSE
+-rwxr-xr-x  2.0 unx        0 b- defN 20-Mar-27 08:49 pyarmor-webui-2.4/__init__.py
+-rw-r--r--  2.0 unx    18450 b- defN 24-Mar-27 15:04 pyarmor-webui-2.4/handler8.py
+-rw-r--r--  2.0 unx     2241 b- defN 24-Apr-19 17:17 pyarmor-webui-2.4/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-19 19:12 pyarmor-webui-2.4/setup.cfg
+-rw-r--r--  2.0 unx     4151 b- defN 24-Apr-19 17:16 pyarmor-webui-2.4/README.rst
+-rw-r--r--  2.0 unx     4990 b- defN 24-Apr-19 19:12 pyarmor-webui-2.4/pyarmor_webui.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     1331 b- defN 24-Apr-19 19:12 pyarmor-webui-2.4/pyarmor_webui.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       61 b- defN 24-Apr-19 19:12 pyarmor-webui-2.4/pyarmor_webui.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 24-Apr-19 19:12 pyarmor-webui-2.4/pyarmor_webui.egg-info/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 19:12 pyarmor-webui-2.4/pyarmor_webui.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-19 19:12 pyarmor-webui-2.4/pyarmor_webui.egg-info/dependency_links.txt
+-rwxr-xr-x  2.0 unx     1027 b- defN 20-Apr-27 09:39 pyarmor-webui-2.4/test/pack_one_folder_bundle.robot
+-rwxr-xr-x  2.0 unx      693 b- defN 20-Oct-30 08:30 pyarmor-webui-2.4/test/generate_expired_license.robot
+-rwxr-xr-x  2.0 unx     1475 b- defN 20-Apr-27 09:39 pyarmor-webui-2.4/test/pack_one_file_bundle_with_outer_license.robot
+-rwxr-xr-x  2.0 unx     1245 b- defN 20-Jan-19 10:10 pyarmor-webui-2.4/test/obfuscate_multiple_entries.robot
+-rwxr-xr-x  2.0 unx      890 b- defN 20-Apr-27 09:40 pyarmor-webui-2.4/test/generate_machine_license.robot
+-rwxr-xr-x  2.0 unx     1164 b- defN 20-Jan-19 10:08 pyarmor-webui-2.4/test/obfuscate_one_script.robot
+-rw-r--r--  2.0 unx     1899 b- defN 20-Apr-27 09:25 pyarmor-webui-2.4/test/README.md
+-rwxr-xr-x  2.0 unx      777 b- defN 20-Apr-27 09:41 pyarmor-webui-2.4/test/generate_extra_data_license.robot
+-rwxr-xr-x  2.0 unx     1230 b- defN 20-Jan-19 10:30 pyarmor-webui-2.4/test/obfuscate_one_package.robot
+-rwxr-xr-x  2.0 unx     6422 b- defN 23-May-12 10:17 pyarmor-webui-2.4/test/resource.robot
+-rwxr-xr-x  2.0 unx     1358 b- defN 20-Apr-27 09:39 pyarmor-webui-2.4/test/pack_with_data_file.robot
+-rwxr-xr-x  2.0 unx     1139 b- defN 20-Apr-27 09:38 pyarmor-webui-2.4/test/pack_one_file_bundle.robot
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 19:12 pyarmor-webui-2.4/static/css/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 19:12 pyarmor-webui-2.4/static/js/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 19:12 pyarmor-webui-2.4/static/img/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-19 19:12 pyarmor-webui-2.4/static/fonts/
+-rw-r--r--  2.0 unx     4286 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/favicon.ico
+-rw-r--r--  2.0 unx      898 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/index.html
+-rw-r--r--  2.0 unx    19211 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/reqwest.js
+-rw-r--r--  2.0 unx   191299 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/css/chunk-vendors.b79ff3a2.css
+-rw-r--r--  2.0 unx     1166 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/css/app.85ddf991.css
+-rw-r--r--  2.0 unx   127774 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/js/app.19b525d6.js
+-rw-r--r--  2.0 unx   718117 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/js/chunk-vendors.4afc1da0.js
+-rw-r--r--  2.0 unx      890 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/cog.svg
+-rw-r--r--  2.0 unx      207 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/folder-solid.svg
+-rw-r--r--  2.0 unx      356 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/tablet-alt.svg
+-rw-r--r--  2.0 unx      339 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/shield-alt.svg
+-rw-r--r--  2.0 unx      935 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/calendar-alt.svg
+-rw-r--r--  2.0 unx    14781 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/logo.a8954ff0.png
+-rw-r--r--  2.0 unx      734 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/registered.svg
+-rw-r--r--  2.0 unx      446 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/calendar-minus.svg
+-rw-r--r--  2.0 unx      349 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/calendar.svg
+-rw-r--r--  2.0 unx      307 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/img/folder.svg
+-rw-r--r--  2.0 unx    28200 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/fonts/element-icons.535877f5.woff
+-rw-r--r--  2.0 unx    55956 b- defN 24-Apr-19 19:05 pyarmor-webui-2.4/static/fonts/element-icons.732389de.ttf
+-rw-r--r--  2.0 unx      205 b- defN 23-May-20 06:08 pyarmor-webui-2.4/data/copy_license.py
+56 files, 1251327 bytes uncompressed, 353685 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -1,169 +1,169 @@
-Filename: pyarmor-webui-2.3/
+Filename: pyarmor-webui-2.4/
 Comment: 
 
-Filename: pyarmor-webui-2.3/pyarmor_webui.egg-info/
+Filename: pyarmor-webui-2.4/pyarmor_webui.egg-info/
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/
+Filename: pyarmor-webui-2.4/test/
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/
+Filename: pyarmor-webui-2.4/static/
 Comment: 
 
-Filename: pyarmor-webui-2.3/data/
+Filename: pyarmor-webui-2.4/data/
 Comment: 
 
-Filename: pyarmor-webui-2.3/PKG-INFO
+Filename: pyarmor-webui-2.4/PKG-INFO
 Comment: 
 
-Filename: pyarmor-webui-2.3/server.py
+Filename: pyarmor-webui-2.4/server.py
 Comment: 
 
-Filename: pyarmor-webui-2.3/handler.py
+Filename: pyarmor-webui-2.4/handler.py
 Comment: 
 
-Filename: pyarmor-webui-2.3/LICENSE
+Filename: pyarmor-webui-2.4/LICENSE
 Comment: 
 
-Filename: pyarmor-webui-2.3/__init__.py
+Filename: pyarmor-webui-2.4/__init__.py
 Comment: 
 
-Filename: pyarmor-webui-2.3/handler8.py
+Filename: pyarmor-webui-2.4/handler8.py
 Comment: 
 
-Filename: pyarmor-webui-2.3/setup.py
+Filename: pyarmor-webui-2.4/setup.py
 Comment: 
 
-Filename: pyarmor-webui-2.3/setup.cfg
+Filename: pyarmor-webui-2.4/setup.cfg
 Comment: 
 
-Filename: pyarmor-webui-2.3/README.rst
+Filename: pyarmor-webui-2.4/README.rst
 Comment: 
 
-Filename: pyarmor-webui-2.3/pyarmor_webui.egg-info/PKG-INFO
+Filename: pyarmor-webui-2.4/pyarmor_webui.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyarmor-webui-2.3/pyarmor_webui.egg-info/SOURCES.txt
+Filename: pyarmor-webui-2.4/pyarmor_webui.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyarmor-webui-2.3/pyarmor_webui.egg-info/entry_points.txt
+Filename: pyarmor-webui-2.4/pyarmor_webui.egg-info/entry_points.txt
 Comment: 
 
-Filename: pyarmor-webui-2.3/pyarmor_webui.egg-info/requires.txt
+Filename: pyarmor-webui-2.4/pyarmor_webui.egg-info/requires.txt
 Comment: 
 
-Filename: pyarmor-webui-2.3/pyarmor_webui.egg-info/top_level.txt
+Filename: pyarmor-webui-2.4/pyarmor_webui.egg-info/top_level.txt
 Comment: 
 
-Filename: pyarmor-webui-2.3/pyarmor_webui.egg-info/dependency_links.txt
+Filename: pyarmor-webui-2.4/pyarmor_webui.egg-info/dependency_links.txt
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/pack_one_folder_bundle.robot
+Filename: pyarmor-webui-2.4/test/pack_one_folder_bundle.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/generate_expired_license.robot
+Filename: pyarmor-webui-2.4/test/generate_expired_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/pack_one_file_bundle_with_outer_license.robot
+Filename: pyarmor-webui-2.4/test/pack_one_file_bundle_with_outer_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/obfuscate_multiple_entries.robot
+Filename: pyarmor-webui-2.4/test/obfuscate_multiple_entries.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/generate_machine_license.robot
+Filename: pyarmor-webui-2.4/test/generate_machine_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/obfuscate_one_script.robot
+Filename: pyarmor-webui-2.4/test/obfuscate_one_script.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/README.md
+Filename: pyarmor-webui-2.4/test/README.md
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/generate_extra_data_license.robot
+Filename: pyarmor-webui-2.4/test/generate_extra_data_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/obfuscate_one_package.robot
+Filename: pyarmor-webui-2.4/test/obfuscate_one_package.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/resource.robot
+Filename: pyarmor-webui-2.4/test/resource.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/pack_with_data_file.robot
+Filename: pyarmor-webui-2.4/test/pack_with_data_file.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/test/pack_one_file_bundle.robot
+Filename: pyarmor-webui-2.4/test/pack_one_file_bundle.robot
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/css/
+Filename: pyarmor-webui-2.4/static/css/
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/js/
+Filename: pyarmor-webui-2.4/static/js/
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/
+Filename: pyarmor-webui-2.4/static/img/
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/fonts/
+Filename: pyarmor-webui-2.4/static/fonts/
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/favicon.ico
+Filename: pyarmor-webui-2.4/static/favicon.ico
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/index.html
+Filename: pyarmor-webui-2.4/static/index.html
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/reqwest.js
+Filename: pyarmor-webui-2.4/static/reqwest.js
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/css/chunk-vendors.b79ff3a2.css
+Filename: pyarmor-webui-2.4/static/css/chunk-vendors.b79ff3a2.css
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/css/app.31abab10.css
+Filename: pyarmor-webui-2.4/static/css/app.85ddf991.css
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/js/app.d0b3d54c.js
+Filename: pyarmor-webui-2.4/static/js/app.19b525d6.js
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/js/chunk-vendors.4afc1da0.js
+Filename: pyarmor-webui-2.4/static/js/chunk-vendors.4afc1da0.js
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/cog.svg
+Filename: pyarmor-webui-2.4/static/img/cog.svg
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/folder-solid.svg
+Filename: pyarmor-webui-2.4/static/img/folder-solid.svg
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/tablet-alt.svg
+Filename: pyarmor-webui-2.4/static/img/tablet-alt.svg
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/shield-alt.svg
+Filename: pyarmor-webui-2.4/static/img/shield-alt.svg
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/calendar-alt.svg
+Filename: pyarmor-webui-2.4/static/img/calendar-alt.svg
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/logo.a8954ff0.png
+Filename: pyarmor-webui-2.4/static/img/logo.a8954ff0.png
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/registered.svg
+Filename: pyarmor-webui-2.4/static/img/registered.svg
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/calendar-minus.svg
+Filename: pyarmor-webui-2.4/static/img/calendar-minus.svg
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/calendar.svg
+Filename: pyarmor-webui-2.4/static/img/calendar.svg
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/img/folder.svg
+Filename: pyarmor-webui-2.4/static/img/folder.svg
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/fonts/element-icons.535877f5.woff
+Filename: pyarmor-webui-2.4/static/fonts/element-icons.535877f5.woff
 Comment: 
 
-Filename: pyarmor-webui-2.3/static/fonts/element-icons.732389de.ttf
+Filename: pyarmor-webui-2.4/static/fonts/element-icons.732389de.ttf
 Comment: 
 
-Filename: pyarmor-webui-2.3/data/copy_license.py
+Filename: pyarmor-webui-2.4/data/copy_license.py
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor-webui-2.3/PKG-INFO` & `pyarmor-webui-2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor-webui
-Version: 2.3
+Version: 2.4
 Summary: A webui tool used to obfuscate and pack python scripts based on pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor-webui
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -64,14 +64,19 @@
 - `snapshots <https://github.com/dashingsoft/pyarmor-webui/tree/master/snapshots>`_
 - `pyarmor <https://github.com/dashingsoft/pyarmor>`_
 - `pyarmor-vue <https://github.com/dashingsoft/pyarmor-vue>`_
 
 Change Logs
 -----------
 
+2.4
+~~~~~
+* Fix Windows issue: create new path failed
+* Fix issue: if option `--port` is set, `pyarmor-webui` could not connect to `pyarmor`
+
 2.3
 ~~~~~
 * Add one extra checkbox `Clean output path` when starting to build
 
   - If it is checked, remove the output path automatically before building
   - If it isn't checked, report error when output path exists
```

## Comparing `pyarmor-webui-2.3/server.py` & `pyarmor-webui-2.4/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     from .handler import RootHandler
     from .handler8 import RootHandler as RootHandler8
 except Exception:
     from .handler import RootHandler
     from .handler8 import RootHandler as RootHandler8
 
 
-__version__ = '2.3'
+__version__ = '2.4'
 
 __config__ = {
     'version': __version__,
     'wwwroot': os.path.join(os.path.dirname(__file__), 'static'),
     'basepath': os.path.dirname(__file__),
     'homepath': os.path.expanduser(os.path.join('~', '.pyarmor')),
 }
```

## Comparing `pyarmor-webui-2.3/handler.py` & `pyarmor-webui-2.4/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,25 +130,28 @@
 
     def __init__(self, config):
         super(DirectoryHandler, self).__init__(config)
         self.name = 'directory'
 
     def do_new(self, args):
         self._check_arg('path', args)
+        path = self._format_path(args)
+        self._check_arg('path', path)
 
-        if not os.path.exists(args):
-            os.makedirs(args)
-        return os.path.abspath(args)
+        if not os.path.exists(path):
+            os.makedirs(path)
+        return os.path.abspath(path)
 
     def do_remove(self, args):
         self._check_arg('path', args, invalids=['.', '/'])
-        self._check_path(args)
+        path = self._format_path(args)
+        self._check_path(path)
 
-        os.rmdir(args)
-        return os.path.abspath(args)
+        os.rmdir(path)
+        return os.path.abspath(path)
 
     def do_list(self, args):
         path = os.path.expandvars(args.get('path', '/'))
         if sys.platform == 'win32':
             if path == '/':
                 from ctypes import cdll
                 drives = cdll.kernel32.GetLogicalDrives()
```

## Comparing `pyarmor-webui-2.3/LICENSE` & `pyarmor-webui-2.4/LICENSE`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/handler8.py` & `pyarmor-webui-2.4/handler8.py`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/setup.py` & `pyarmor-webui-2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sys import platform
 from setuptools import setup
 
-__version__ = '2.3'
+__version__ = '2.4'
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='pyarmor-webui',
     version=__version__,
```

## Comparing `pyarmor-webui-2.3/README.rst` & `pyarmor-webui-2.4/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 - `snapshots <https://github.com/dashingsoft/pyarmor-webui/tree/master/snapshots>`_
 - `pyarmor <https://github.com/dashingsoft/pyarmor>`_
 - `pyarmor-vue <https://github.com/dashingsoft/pyarmor-vue>`_
 
 Change Logs
 -----------
 
+2.4
+~~~~~
+* Fix Windows issue: create new path failed
+* Fix issue: if option `--port` is set, `pyarmor-webui` could not connect to `pyarmor`
+
 2.3
 ~~~~~
 * Add one extra checkbox `Clean output path` when starting to build
 
   - If it is checked, remove the output path automatically before building
   - If it isn't checked, report error when output path exists
```

## Comparing `pyarmor-webui-2.3/pyarmor_webui.egg-info/PKG-INFO` & `pyarmor-webui-2.4/pyarmor_webui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor-webui
-Version: 2.3
+Version: 2.4
 Summary: A webui tool used to obfuscate and pack python scripts based on pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor-webui
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -64,14 +64,19 @@
 - `snapshots <https://github.com/dashingsoft/pyarmor-webui/tree/master/snapshots>`_
 - `pyarmor <https://github.com/dashingsoft/pyarmor>`_
 - `pyarmor-vue <https://github.com/dashingsoft/pyarmor-vue>`_
 
 Change Logs
 -----------
 
+2.4
+~~~~~
+* Fix Windows issue: create new path failed
+* Fix issue: if option `--port` is set, `pyarmor-webui` could not connect to `pyarmor`
+
 2.3
 ~~~~~
 * Add one extra checkbox `Clean output path` when starting to build
 
   - If it is checked, remove the output path automatically before building
   - If it isn't checked, report error when output path exists
```

## Comparing `pyarmor-webui-2.3/pyarmor_webui.egg-info/SOURCES.txt` & `pyarmor-webui-2.4/pyarmor_webui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 ./handler.py
 ./handler8.py
 ./server.py
 ./data/copy_license.py
 ./static/favicon.ico
 ./static/index.html
 ./static/reqwest.js
-./static/css/app.31abab10.css
+./static/css/app.85ddf991.css
 ./static/css/chunk-vendors.b79ff3a2.css
 ./static/fonts/element-icons.535877f5.woff
 ./static/fonts/element-icons.732389de.ttf
 ./static/img/calendar-alt.svg
 ./static/img/calendar-minus.svg
 ./static/img/calendar.svg
 ./static/img/cog.svg
 ./static/img/folder-solid.svg
 ./static/img/folder.svg
 ./static/img/logo.a8954ff0.png
 ./static/img/registered.svg
 ./static/img/shield-alt.svg
 ./static/img/tablet-alt.svg
-./static/js/app.d0b3d54c.js
+./static/js/app.19b525d6.js
 ./static/js/chunk-vendors.4afc1da0.js
 ./test/README.md
 ./test/generate_expired_license.robot
 ./test/generate_extra_data_license.robot
 ./test/generate_machine_license.robot
 ./test/obfuscate_multiple_entries.robot
 ./test/obfuscate_one_package.robot
```

## Comparing `pyarmor-webui-2.3/test/pack_one_folder_bundle.robot` & `pyarmor-webui-2.4/test/pack_one_folder_bundle.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/generate_expired_license.robot` & `pyarmor-webui-2.4/test/generate_expired_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/pack_one_file_bundle_with_outer_license.robot` & `pyarmor-webui-2.4/test/pack_one_file_bundle_with_outer_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/obfuscate_multiple_entries.robot` & `pyarmor-webui-2.4/test/obfuscate_multiple_entries.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/generate_machine_license.robot` & `pyarmor-webui-2.4/test/generate_machine_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/obfuscate_one_script.robot` & `pyarmor-webui-2.4/test/obfuscate_one_script.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/README.md` & `pyarmor-webui-2.4/test/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/generate_extra_data_license.robot` & `pyarmor-webui-2.4/test/generate_extra_data_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/obfuscate_one_package.robot` & `pyarmor-webui-2.4/test/obfuscate_one_package.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/resource.robot` & `pyarmor-webui-2.4/test/resource.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/pack_with_data_file.robot` & `pyarmor-webui-2.4/test/pack_with_data_file.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/test/pack_one_file_bundle.robot` & `pyarmor-webui-2.4/test/pack_one_file_bundle.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/static/favicon.ico` & `pyarmor-webui-2.4/static/favicon.ico`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/static/index.html` & `pyarmor-webui-2.4/static/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1"><link rel="icon" href="/favicon.ico"><title>Pyarmor</title><link href="/css/app.31abab10.css" rel="preload" as="style"><link href="/css/chunk-vendors.b79ff3a2.css" rel="preload" as="style"><link href="/js/app.d0b3d54c.js" rel="preload" as="script"><link href="/js/chunk-vendors.4afc1da0.js" rel="preload" as="script"><link href="/css/chunk-vendors.b79ff3a2.css" rel="stylesheet"><link href="/css/app.31abab10.css" rel="stylesheet"></head><body><noscript><strong>We're sorry but pyarmor-vue doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script src="/js/chunk-vendors.4afc1da0.js"></script><script src="/js/app.d0b3d54c.js"></script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charset="utf-8"><meta http-equiv="X-UA-Compatible" content="IE=edge"><meta name="viewport" content="width=device-width,initial-scale=1"><link rel="icon" href="/favicon.ico"><title>Pyarmor</title><link href="/css/app.85ddf991.css" rel="preload" as="style"><link href="/css/chunk-vendors.b79ff3a2.css" rel="preload" as="style"><link href="/js/app.19b525d6.js" rel="preload" as="script"><link href="/js/chunk-vendors.4afc1da0.js" rel="preload" as="script"><link href="/css/chunk-vendors.b79ff3a2.css" rel="stylesheet"><link href="/css/app.85ddf991.css" rel="stylesheet"></head><body><noscript><strong>We're sorry but pyarmor-vue doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript><div id="app"></div><script src="/js/chunk-vendors.4afc1da0.js"></script><script src="/js/app.19b525d6.js"></script></body></html>
```

## Comparing `pyarmor-webui-2.3/static/reqwest.js` & `pyarmor-webui-2.4/static/reqwest.js`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/static/css/chunk-vendors.b79ff3a2.css` & `pyarmor-webui-2.4/static/css/chunk-vendors.b79ff3a2.css`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/static/js/app.d0b3d54c.js` & `pyarmor-webui-2.4/static/js/app.19b525d6.js`

 * *Files 0% similar despite different names*

### js-beautify {}

```diff
@@ -71,16 +71,16 @@
     for (var c = 0; c < i.length; c++) t(i[c]);
     var u = l;
     n.push([0, "chunk-vendors"]), o()
 })({
     0: function(e, t, o) {
         e.exports = o("56d7")
     },
+    "0591": function(e, t, o) {},
     "0c06": function(e, t, o) {},
-    "103e": function(e, t, o) {},
     "1ef4": function(e, t, o) {
         "use strict";
         o("9b4a")
     },
     2733: function(e, t, o) {
         "use strict";
         o("a7a7")
@@ -381,14 +381,18 @@
             }))
     },
     "35d2": function(e, t, o) {},
     "3c61": function(e, t, o) {
         "use strict";
         o("7458")
     },
+    "50c9": function(e, t, o) {
+        "use strict";
+        o("0591")
+    },
     "56d7": function(e, t, o) {
         "use strict";
         o.r(t);
         o("e260"), o("e6cf"), o("cca6"), o("a79d");
         var a = o("2b0e"),
             r = function() {
                 var e = this,
@@ -2018,15 +2022,15 @@
                     t = e._self._c;
                 return t("div", {
                     staticClass: "about"
                 }, [t("h1", {
                     staticStyle: {
                         "text-align": "center"
                     }
-                }, [e._v(e._s(e.$t("About")))]), t("p", [e._v("pyarmor-vue: 0.4.1")]), e.versionInfo.version ? t("div", [t("p", [e._v("pyarmor-server: " + e._s(e.versionInfo.server))]), t("p", [e._v("Python: " + e._s(e.versionInfo.python))]), e.versionInfo.regcode.length ? t("p", [e._v(" pyarmor (" + e._s(e.versionInfo.regcode.slice(-6)) + "): " + e._s(e.versionInfo.version) + " ")]) : t("p", [e._v("pyarmor (" + e._s(e.versionInfo.tag) + "): " + e._s(e.versionInfo.version))]), e.versionInfo.reginfo.length ? t("p", [e._v(e._s(e.versionInfo.reginfo))]) : e._e()]) : t("div", [t("p", [e._v(e._s(e.$t("Pyarmor server is not running on")) + " "), t("span", [e._v("http://localhost:9096/")]), e._v(". " + e._s(e.$t("Make sure the server is running, or click here to")) + " "), t("el-button", {
+                }, [e._v(e._s(e.$t("About")))]), t("p", [e._v("pyarmor-vue: 0.4.2")]), e.versionInfo.version ? t("div", [t("p", [e._v("pyarmor-server: " + e._s(e.versionInfo.server))]), t("p", [e._v("Python: " + e._s(e.versionInfo.python))]), e.versionInfo.regcode.length ? t("p", [e._v(" pyarmor (" + e._s(e.versionInfo.regcode.slice(-6)) + "): " + e._s(e.versionInfo.version) + " ")]) : t("p", [e._v("pyarmor (" + e._s(e.versionInfo.tag) + "): " + e._s(e.versionInfo.version))]), e.versionInfo.reginfo.length ? t("p", [e._v(e._s(e.versionInfo.reginfo))]) : e._e()]) : t("div", [t("p", [e._v(e._s(e.$t("Pyarmor server is not running on")) + " "), t("span", [e._v("http://localhost:9096/")]), e._v(". " + e._s(e.$t("Make sure the server is running, or click here to")) + " "), t("el-button", {
                     attrs: {
                         type: "text"
                     },
                     on: {
                         click: function(t) {
                             return e.$emit("connect-server")
                         }
@@ -2072,15 +2076,15 @@
             },
             G = [],
             X = {
                 name: "HomeTabAbout",
                 props: ["versionInfo"]
             },
             J = X,
-            Q = (o("8f70"), Object(D["a"])(J, U, G, !1, null, "0a2f8081", null)),
+            Q = (o("af86"), Object(D["a"])(J, U, G, !1, null, "6ce844e0", null)),
             K = Q.exports,
             Z = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "project-main"
                 }, [t("el-page-header", {
@@ -4226,15 +4230,15 @@
                             reginfo: "",
                             server: "",
                             python: ""
                         }
                     }
                 },
                 mounted: function() {
-                    C.$on("connect-changed", this.onServerChanged), this.connectServer(), "zh-cn" === localStorage.getItem("language") ? this.changeLanguage("zh-cn") : "jp" === localStorage.getItem("language") && this.changeLanguage("jp")
+                    this.serverUrl = "http://".concat(document.location.host, "/"), C.$on("connect-changed", this.onServerChanged), this.connectServer(), "zh-cn" === localStorage.getItem("language") ? this.changeLanguage("zh-cn") : "jp" === localStorage.getItem("language") && this.changeLanguage("jp")
                 },
                 computed: {
                     currentMode: function() {
                         return parseInt(this.versionInfo.version) > 7 ? this.v8mode ? "8" : "7+" : "7"
                     },
                     currentTabComponent: function() {
                         return this.currentTabName
@@ -4279,15 +4283,15 @@
                             }))
                         };
                         t(this), localStorage.setItem("language", e)
                     }
                 }
             },
             Ye = Ze,
-            et = (o("baa0"), o("5bb9"), Object(D["a"])(Ye, r, n, !1, null, "c232ea8c", null)),
+            et = (o("50c9"), o("a076"), Object(D["a"])(Ye, r, n, !1, null, "0bd6e5ec", null)),
             tt = et.exports,
             ot = function() {
                 var e = this,
                     t = e._self._c;
                 return t("div", {
                     staticClass: "about"
                 }, [e._v(" Generate Lecense ")])
@@ -5262,40 +5266,35 @@
         "use strict";
         o("0c06")
     },
     "59d9": function(e, t, o) {
         "use strict";
         o("d630")
     },
-    "5bb9": function(e, t, o) {
-        "use strict";
-        o("103e")
-    },
     7458: function(e, t, o) {},
-    8748: function(e, t, o) {},
-    "8f70": function(e, t, o) {
+    "7da1": function(e, t, o) {},
+    "93a8": function(e, t, o) {},
+    "9b4a": function(e, t, o) {},
+    a076: function(e, t, o) {
         "use strict";
-        o("e18a")
+        o("7da1")
     },
-    "9b4a": function(e, t, o) {},
     a7a7: function(e, t, o) {},
-    baa0: function(e, t, o) {
+    af86: function(e, t, o) {
         "use strict";
-        o("8748")
+        o("93a8")
     },
     c0fb: function(e, t, o) {
         "use strict";
         o("35d2")
     },
     c504: function(e, t, o) {},
     cf05: function(e, t, o) {
         e.exports = o.p + "img/logo.a8954ff0.png"
     },
     d630: function(e, t, o) {},
-    e18a: function(e, t, o) {},
     ea38: function(e, t, o) {},
     f571: function(e, t, o) {
         "use strict";
         o("ea38")
     }
-});
-//# sourceMappingURL=app.d0b3d54c.js.map
+});
```

## Comparing `pyarmor-webui-2.3/static/js/chunk-vendors.4afc1da0.js` & `pyarmor-webui-2.4/static/js/chunk-vendors.4afc1da0.js`

 * *Files 0% similar despite different names*

### js-beautify {}

```diff
@@ -34367,9 +34367,8 @@
             e.exports = i && !Symbol.sham && "symbol" == typeof Symbol.iterator
         },
         fe07: function(e, t, n) {},
         fed5: function(e, t) {
             t.f = Object.getOwnPropertySymbols
         }
     }
-]);
-//# sourceMappingURL=chunk-vendors.4afc1da0.js.map
+]);
```

## Comparing `pyarmor-webui-2.3/static/img/cog.svg` & `pyarmor-webui-2.4/static/img/cog.svg`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/static/img/calendar-alt.svg` & `pyarmor-webui-2.4/static/img/calendar-alt.svg`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/static/img/logo.a8954ff0.png` & `pyarmor-webui-2.4/static/img/logo.a8954ff0.png`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/static/img/registered.svg` & `pyarmor-webui-2.4/static/img/registered.svg`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/static/fonts/element-icons.535877f5.woff` & `pyarmor-webui-2.4/static/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.3/static/fonts/element-icons.732389de.ttf` & `pyarmor-webui-2.4/static/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

