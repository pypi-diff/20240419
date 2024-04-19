# Comparing `tmp/pyvispr-2024.3.tar.gz` & `tmp/pyvispr-2024.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvispr-2024.3.tar", last modified: Mon Apr 15 11:19:49 2024, max compression
+gzip compressed data, was "pyvispr-2024.4.tar", last modified: Fri Apr 19 14:42:39 2024, max compression
```

## Comparing `pyvispr-2024.3.tar` & `pyvispr-2024.4.tar`

### file list

```diff
@@ -1,96 +1,94 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/
--rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.3/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5681 2024-04-15 11:19:49.366336 pyvispr-2024.3/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.3/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.3/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     4652 2024-02-07 09:03:58.000000 pyvispr-2024.3/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.359669 pyvispr-2024.3/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     2421 2024-02-07 09:22:47.000000 pyvispr-2024.3/documentation/wiki/description.asciidoc
--rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.3/pyproject.toml
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/
--rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.3/pyvispr/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/catalog/factory/
--rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.3/pyvispr/catalog/factory/image_loader.py
--rwx------   0 eric      (1000) users      (984)    15487 2024-04-15 11:08:52.000000 pyvispr-2024.3/pyvispr/catalog/factory/image_viewer.py
--rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.3/pyvispr/catalog/factory/numexpr_calculator.py
--rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.3/pyvispr/catalog/factory/value.py
--rwx------   0 eric      (1000) users      (984)     5762 2024-04-13 15:12:28.000000 pyvispr-2024.3/pyvispr/catalog/factory/value_viewer.py
--rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.3/pyvispr/catalog/installer.py
--rwx------   0 eric      (1000) users      (984)     4114 2024-04-11 12:31:33.000000 pyvispr-2024.3/pyvispr/catalog/parser.py
--rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.3/pyvispr/catalog/type.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/config/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/config/appearance/
--rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.3/pyvispr/config/appearance/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.3/pyvispr/config/appearance/behavior.py
--rwx------   0 eric      (1000) users      (984)     2586 2024-01-19 18:43:09.000000 pyvispr-2024.3/pyvispr/config/appearance/color.py
--rwx------   0 eric      (1000) users      (984)     1711 2023-12-13 13:08:28.000000 pyvispr-2024.3/pyvispr/config/appearance/geometry.py
--rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/config/path.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.3/pyvispr/constant/app.py
--rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.3/pyvispr/constant/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.3/pyvispr/constant/function.py
--rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.3/pyvispr/constant/path.py
--rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.3/pyvispr/constant/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.363003 pyvispr-2024.3/pyvispr/constant/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/constant/widget/function_header.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.3/pyvispr/constant/widget/list.py
--rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.3/pyvispr/constant/widget/node.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/extension/
--rwx------   0 eric      (1000) users      (984)    11820 2024-04-11 13:59:35.000000 pyvispr-2024.3/pyvispr/extension/function.py
--rwx------   0 eric      (1000) users      (984)     2907 2024-04-11 10:11:11.000000 pyvispr-2024.3/pyvispr/extension/module.py
--rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.3/pyvispr/extension/qt6.py
--rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.3/pyvispr/extension/string_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/flow/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/flow/descriptive/
--rwx------   0 eric      (1000) users      (984)     7851 2024-04-11 14:03:03.000000 pyvispr-2024.3/pyvispr/flow/descriptive/node.py
--rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.3/pyvispr/flow/descriptive/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/flow/functional/
--rwx------   0 eric      (1000) users      (984)     6827 2024-04-11 08:16:26.000000 pyvispr-2024.3/pyvispr/flow/functional/graph.py
--rwx------   0 eric      (1000) users      (984)     4509 2023-12-12 21:43:02.000000 pyvispr-2024.3/pyvispr/flow/functional/link.py
--rwx------   0 eric      (1000) users      (984)    10964 2024-04-12 14:30:49.000000 pyvispr-2024.3/pyvispr/flow/functional/node_isolated.py
--rwx------   0 eric      (1000) users      (984)     3621 2024-04-13 16:08:47.000000 pyvispr-2024.3/pyvispr/flow/functional/node_linked.py
--rwx------   0 eric      (1000) users      (984)     2549 2024-04-10 14:37:49.000000 pyvispr-2024.3/pyvispr/flow/functional/socket.py
--rwx------   0 eric      (1000) users      (984)     2169 2024-04-10 16:31:30.000000 pyvispr-2024.3/pyvispr/flow/messenger.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/flow/visual/
--rwx------   0 eric      (1000) users      (984)    18732 2024-04-11 08:03:57.000000 pyvispr-2024.3/pyvispr/flow/visual/graph.py
--rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.3/pyvispr/flow/visual/ii_value.py
--rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.3/pyvispr/flow/visual/link.py
--rwx------   0 eric      (1000) users      (984)    13413 2024-04-15 11:07:24.000000 pyvispr-2024.3/pyvispr/flow/visual/node.py
--rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/flow/visual/socket.py
--rwx------   0 eric      (1000) users      (984)     7968 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/flow/visual/whiteboard.py
--rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/install.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.359669 pyvispr-2024.3/pyvispr/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/interface/storage/
--rwx------   0 eric      (1000) users      (984)     2993 2024-04-10 14:07:15.000000 pyvispr-2024.3/pyvispr/interface/storage/loading.py
--rwx------   0 eric      (1000) users      (984)     3550 2024-04-10 14:07:15.000000 pyvispr-2024.3/pyvispr/interface/storage/stowing.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/interface/window/
--rwx------   0 eric      (1000) users      (984)    15868 2024-04-11 14:00:34.000000 pyvispr-2024.3/pyvispr/interface/window/installer.py
--rwx------   0 eric      (1000) users      (984)     1841 2023-12-13 13:55:15.000000 pyvispr-2024.3/pyvispr/interface/window/messenger.py
--rwx------   0 eric      (1000) users      (984)     7880 2024-04-11 10:10:11.000000 pyvispr-2024.3/pyvispr/interface/window/runner.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/interface/window/widget/
--rwx------   0 eric      (1000) users      (984)    16048 2024-04-11 13:33:15.000000 pyvispr-2024.3/pyvispr/interface/window/widget/function_header.py
--rwx------   0 eric      (1000) users      (984)     4147 2024-04-11 13:01:01.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list.py
--rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list_file.py
--rwx------   0 eric      (1000) users      (984)     2458 2024-01-19 20:05:03.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list_function.py
--rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list_module.py
--rwx------   0 eric      (1000) users      (984)     3818 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/interface/window/widget/list_node.py
--rwx------   0 eric      (1000) users      (984)     2412 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/interface/window/widget/menu.py
--rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.3/pyvispr/run.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr/runtime/
--rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.3/pyvispr/runtime/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.3/pyvispr/runtime/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1628 2024-04-10 14:44:17.000000 pyvispr-2024.3/pyvispr/runtime/messenger.py
--rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.3/pyvispr/runtime/socket.py
--rwx------   0 eric      (1000) users      (984)     1577 2024-04-15 11:18:11.000000 pyvispr-2024.3/pyvispr/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-15 11:19:49.366336 pyvispr-2024.3/pyvispr.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5681 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     2280 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)       99 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-15 11:19:49.000000 pyvispr-2024.3/pyvispr.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)       99 2024-04-10 14:52:27.000000 pyvispr-2024.3/requirements.txt
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-15 11:19:49.366336 pyvispr-2024.3/setup.cfg
--rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.3/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/
+-rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.4/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5710 2024-04-19 14:42:39.524234 pyvispr-2024.4/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.4/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.4/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4652 2024-02-07 09:03:58.000000 pyvispr-2024.4/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.514234 pyvispr-2024.4/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.517568 pyvispr-2024.4/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     2421 2024-02-07 09:22:47.000000 pyvispr-2024.4/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.4/pyproject.toml
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.517568 pyvispr-2024.4/pyvispr/
+-rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.4/pyvispr/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/catalog/factory/
+-rwx------   0 eric      (1000) users      (984)     1715 2024-04-19 07:34:07.000000 pyvispr-2024.4/pyvispr/catalog/factory/image_256.py
+-rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.4/pyvispr/catalog/factory/image_loader.py
+-rwx------   0 eric      (1000) users      (984)    15855 2024-04-19 14:39:58.000000 pyvispr-2024.4/pyvispr/catalog/factory/image_viewer.py
+-rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.4/pyvispr/catalog/factory/numexpr_calculator.py
+-rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.4/pyvispr/catalog/factory/value.py
+-rwx------   0 eric      (1000) users      (984)     5762 2024-04-18 07:03:13.000000 pyvispr-2024.4/pyvispr/catalog/factory/value_viewer.py
+-rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.4/pyvispr/catalog/installer.py
+-rwx------   0 eric      (1000) users      (984)     4160 2024-04-19 07:40:32.000000 pyvispr-2024.4/pyvispr/catalog/parser.py
+-rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.4/pyvispr/catalog/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/config/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/config/appearance/
+-rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.4/pyvispr/config/appearance/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.4/pyvispr/config/appearance/behavior.py
+-rwx------   0 eric      (1000) users      (984)     2662 2024-04-19 14:06:18.000000 pyvispr-2024.4/pyvispr/config/appearance/color.py
+-rwx------   0 eric      (1000) users      (984)     1727 2024-04-19 14:06:38.000000 pyvispr-2024.4/pyvispr/config/appearance/geometry.py
+-rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/config/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.4/pyvispr/constant/app.py
+-rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.4/pyvispr/constant/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.4/pyvispr/constant/function.py
+-rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.4/pyvispr/constant/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.4/pyvispr/constant/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/constant/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/constant/widget/function_header.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.4/pyvispr/constant/widget/list.py
+-rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.4/pyvispr/constant/widget/node.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.520901 pyvispr-2024.4/pyvispr/extension/
+-rwx------   0 eric      (1000) users      (984)    11886 2024-04-19 06:09:59.000000 pyvispr-2024.4/pyvispr/extension/function.py
+-rwx------   0 eric      (1000) users      (984)     2907 2024-04-19 07:15:15.000000 pyvispr-2024.4/pyvispr/extension/module.py
+-rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.4/pyvispr/extension/qt6.py
+-rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.4/pyvispr/extension/string_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.517568 pyvispr-2024.4/pyvispr/flow/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/flow/descriptive/
+-rwx------   0 eric      (1000) users      (984)     7948 2024-04-19 07:15:25.000000 pyvispr-2024.4/pyvispr/flow/descriptive/node.py
+-rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.4/pyvispr/flow/descriptive/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/flow/functional/
+-rwx------   0 eric      (1000) users      (984)     4471 2024-04-19 13:44:55.000000 pyvispr-2024.4/pyvispr/flow/functional/graph.py
+-rwx------   0 eric      (1000) users      (984)     4508 2024-04-19 14:19:48.000000 pyvispr-2024.4/pyvispr/flow/functional/link.py
+-rwx------   0 eric      (1000) users      (984)    10587 2024-04-19 14:36:55.000000 pyvispr-2024.4/pyvispr/flow/functional/node_isolated.py
+-rwx------   0 eric      (1000) users      (984)     5179 2024-04-19 14:41:22.000000 pyvispr-2024.4/pyvispr/flow/functional/node_linked.py
+-rwx------   0 eric      (1000) users      (984)     2548 2024-04-19 14:19:48.000000 pyvispr-2024.4/pyvispr/flow/functional/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/flow/visual/
+-rwx------   0 eric      (1000) users      (984)    18596 2024-04-19 13:37:01.000000 pyvispr-2024.4/pyvispr/flow/visual/graph.py
+-rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.4/pyvispr/flow/visual/ii_value.py
+-rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.4/pyvispr/flow/visual/link.py
+-rwx------   0 eric      (1000) users      (984)    13289 2024-04-19 13:42:58.000000 pyvispr-2024.4/pyvispr/flow/visual/node.py
+-rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/flow/visual/socket.py
+-rwx------   0 eric      (1000) users      (984)     7879 2024-04-19 13:11:30.000000 pyvispr-2024.4/pyvispr/flow/visual/whiteboard.py
+-rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/install.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.517568 pyvispr-2024.4/pyvispr/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/interface/storage/
+-rwx------   0 eric      (1000) users      (984)     3187 2024-04-19 06:39:34.000000 pyvispr-2024.4/pyvispr/interface/storage/loading.py
+-rwx------   0 eric      (1000) users      (984)     3592 2024-04-19 14:39:57.000000 pyvispr-2024.4/pyvispr/interface/storage/stowing.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/interface/window/
+-rwx------   0 eric      (1000) users      (984)    16232 2024-04-19 06:27:12.000000 pyvispr-2024.4/pyvispr/interface/window/installer.py
+-rwx------   0 eric      (1000) users      (984)     7880 2024-04-18 07:10:06.000000 pyvispr-2024.4/pyvispr/interface/window/runner.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/interface/window/widget/
+-rwx------   0 eric      (1000) users      (984)    16183 2024-04-18 07:10:09.000000 pyvispr-2024.4/pyvispr/interface/window/widget/function_header.py
+-rwx------   0 eric      (1000) users      (984)     4147 2024-04-18 07:06:06.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list.py
+-rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list_file.py
+-rwx------   0 eric      (1000) users      (984)     2710 2024-04-18 11:56:51.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list_function.py
+-rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list_module.py
+-rwx------   0 eric      (1000) users      (984)     3942 2024-04-19 14:11:04.000000 pyvispr-2024.4/pyvispr/interface/window/widget/list_node.py
+-rwx------   0 eric      (1000) users      (984)     2412 2024-04-18 07:06:19.000000 pyvispr-2024.4/pyvispr/interface/window/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.4/pyvispr/run.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr/runtime/
+-rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.4/pyvispr/runtime/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.4/pyvispr/runtime/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.4/pyvispr/runtime/socket.py
+-rwx------   0 eric      (1000) users      (984)     1577 2024-04-19 14:42:19.000000 pyvispr-2024.4/pyvispr/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-19 14:42:39.524234 pyvispr-2024.4/pyvispr.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5710 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     2224 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-19 14:42:39.000000 pyvispr-2024.4/pyvispr.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-17 16:13:58.000000 pyvispr-2024.4/requirements.txt
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-19 14:42:39.527568 pyvispr-2024.4/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.4/setup.py
```

### Comparing `pyvispr-2024.3/PKG-INFO` & `pyvispr-2024.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.3
+Version: 2024.4
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyVispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
@@ -21,14 +21,15 @@
 Requires-Dist: json_any
 Requires-Dist: logger_36
 Requires-Dist: numexpr
 Requires-Dist: numpy
 Requires-Dist: platformdirs
 Requires-Dist: PyQt6
 Requires-Dist: scikit-image
+Requires-Dist: sio-messenger
 Requires-Dist: str_to_obj
 
 ..
    Copyright CNRS/Inria/UniCA
    Contributor(s): Eric Debreuve (since 2017)
 
    eric.debreuve@cnrs.fr
```

### Comparing `pyvispr-2024.3/README-COPYRIGHT-utf8.txt` & `pyvispr-2024.4/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/README-LICENCE-utf8.txt` & `pyvispr-2024.4/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/README.rst` & `pyvispr-2024.4/README.rst`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/documentation/wiki/description.asciidoc` & `pyvispr-2024.4/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/__init__.py` & `pyvispr-2024.4/pyvispr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/catalog/factory/image_loader.py` & `pyvispr-2024.4/pyvispr/catalog/factory/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/catalog/factory/image_viewer.py` & `pyvispr-2024.4/pyvispr/catalog/factory/image_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from os.path import dirname as DetermineFolder
 from os.path import expanduser as ExpandTildeBasePath
 
 import numpy
 import PyQt6.QtGui as qtui
 import PyQt6.QtWidgets as wdgt
 from pyvispr.extension.qt6 import ExecuteApp, QtApp
-from pyvispr.interface.window.messenger import CreateMessageCanal
+from pyvispr.runtime.backend import SCREEN_BACKEND
 
 
 def pyVisprImageViewer(image: numpy.ndarray, /) -> None:
     """"""
     img_shape = image.shape
     if 1 < len(img_shape) < 4:
         height = img_shape[0]
@@ -82,73 +82,83 @@
         )
         median_value = numpy.around(
             [numpy.median(image[:, :, _elm]) for _elm in range(depth)],
             decimals=2,
         )
 
     app, should_exec = QtApp()
-    q_img = _NewQImage(image, min_value, max_value, width, height, depth)
+    q_img, np_img = _NewQImage(image, min_value, max_value, width, height, depth)
     viewer = viewer_t(
         width,
         height,
         depth,
         img_format_as_str,
         min_value,
         max_value,
         mean_value,
         median_value,
         q_img,
+        np_img,
         wdgt.QApplication.activeWindow(),
     )
     viewer.show()
     ExecuteApp(app, should_exec)
 
 
 def _NewQImage(
     image: numpy.ndarray,
     min_value: int | float | numpy.ndarray,
     max_value: int | float | numpy.ndarray,
     width: int,
     height: int,
     depth: int,
     /,
-) -> qtui.QImage:
+) -> tuple[qtui.QImage, numpy.ndarray]:
     """"""
     # Min and max ignoring alpha channel.
     if isinstance(min_value, numpy.ndarray):
         global_min = numpy.amin(min_value[: min(depth, 3)])
         global_max = numpy.amax(max_value[: min(depth, 3)])
     else:
         global_min, global_max = min_value, max_value
 
     if depth < 4:
         only_colors = image
     else:
         only_colors = image[..., :3]
     if global_max > global_min:
         factor = 255.0 / (global_max - global_min)
-        only_colors = factor * (only_colors - global_min)
+        only_colors = numpy.round(
+            factor * (only_colors.astype(numpy.float64, copy=False) - global_min)
+        )
     if depth < 4:
-        image_for_display = only_colors
+        np_img = only_colors
     else:
-        image_for_display = numpy.empty_like(image)
-        image_for_display[..., :3] = only_colors.astype(image.dtype)[...]
-        image_for_display[..., 3] = image[..., 3]
-    image_for_display = numpy.uint8(numpy.around(image_for_display))
+        np_img = numpy.dstack((only_colors, image[..., 3]))
+    np_img = np_img.astype(numpy.uint8, copy=False)
 
     if depth == 1:
         img_format = qtui.QImage.Format.Format_Indexed8
     elif depth == 3:
         img_format = qtui.QImage.Format.Format_RGB888
     elif depth == 4:
         img_format = qtui.QImage.Format.Format_RGBA8888
     else:  # Only to avoid checker waring; Cannot happen in practice.
         img_format = None
 
-    return qtui.QImage(image_for_display.data, width, height, depth * width, img_format)
+    try:
+        q_img = qtui.QImage(np_img.data, width, height, depth * width, img_format)
+    except TypeError:
+        # /!\ Without .copy(), qtui.QImage sometimes complains with:
+        #     QImage(): too many arguments
+        #     ...
+        np_img = np_img.copy()
+        q_img = qtui.QImage(np_img.data, width, height, depth * width, img_format)
+
+    return q_img, np_img
 
 
 class viewer_t(wdgt.QMainWindow):
     DEFAULT_SAVE_EXTENSION = "png"  # lowercase
 
     def __init__(
         self,
@@ -157,28 +167,30 @@
         depth: int,
         img_format_as_str: str,
         min_value: int | float | numpy.ndarray,
         max_value: int | float | numpy.ndarray,
         mean_value: int | float | numpy.ndarray,
         median_value: int | float | numpy.ndarray,
         q_img: qtui.QImage,
+        np_img: numpy.ndarray,
         wdw: wdgt.QWidget,
     ):
         """"""
         super().__init__(wdw)
 
         self.quit_action = None
         self.save_action = None
         self.copy_action = None
         self.zoom_in_action = None
         self.zoom_out_action = None
         self.original_size_action = None
         self.fit_to_window_action = None
 
         self.q_img = q_img
+        self.np_img = np_img
         self.last_save_location = ExpandTildeBasePath("~")
 
         screen_size = qtui.QGuiApplication.primaryScreen().availableGeometry()
         wdw_width = min(width, int(0.75 * screen_size.width()))
         wdw_height = min(height, int(0.75 * screen_size.height()))
 
         self.setWindowTitle("pyVispr Image Viewer")
@@ -316,15 +328,15 @@
             attributes,
             entries,
             shortcuts,
             Functions,
         ):
             action = qtui.QAction(entry, self)
             action.setShortcut(shortcut)
-            CreateMessageCanal(action, "triggered", Function)
+            SCREEN_BACKEND.CreateMessageCanal(action, "triggered", Function)
             setattr(self, f"{attribute}_action", action)
 
         self.fit_to_window_action.setCheckable(True)
 
     def _UpdateActions(self) -> None:
         """"""
         self.zoom_in_action.setEnabled(not self.fit_to_window_action.isChecked())
@@ -445,15 +457,17 @@
             current_min = min_value[p_idx]
             current_max = max_value[p_idx]
         else:
             current_min = min_value
             current_max = max_value
 
         non_empty_plane = numpy.repeat(
-            numpy.arange(current_max, current_min - 1, -1)[:, None], 20, axis=1
+            numpy.flipud(numpy.linspace(current_min, current_max, num=256))[:, None],
+            20,
+            axis=1,
         )
         if (p_idx < 3) and (depth > 1):
             n_planes = 3
             img_format = qtui.QImage.Format.Format_RGB888
             all_planes = numpy.zeros(
                 non_empty_plane.shape + (n_planes,), dtype=numpy.uint8
             )
```

### Comparing `pyvispr-2024.3/pyvispr/catalog/factory/numexpr_calculator.py` & `pyvispr-2024.4/pyvispr/catalog/factory/numexpr_calculator.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/catalog/factory/value.py` & `pyvispr-2024.4/pyvispr/catalog/factory/value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/catalog/factory/value_viewer.py` & `pyvispr-2024.4/pyvispr/catalog/factory/value_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import pprint as pprt
 import typing as h
 
 import PyQt6.QtGui as qtui
 import PyQt6.QtWidgets as wdgt
 from PyQt6.QtCore import QThreadPool as thread_manager_t
 from pyvispr.extension.qt6 import ExecuteApp, QtApp
-from pyvispr.interface.window.messenger import CreateMessageCanal
+from pyvispr.runtime.backend import SCREEN_BACKEND
 
 
 def pyVisprValueViewer(value: h.Any, /) -> None:
     """"""
     app, should_exec = QtApp()
     value_viewer = value_viewer_t(value, wdgt.QApplication.activeWindow())
     value_viewer.show()
@@ -86,15 +86,15 @@
 
         central = wdgt.QWidget()
         central.setLayout(layout)
         self.setCentralWidget(central)
 
         self.setWindowTitle("pyVispr Value Viewer")
 
-        CreateMessageCanal(done, "clicked", self.close)
+        SCREEN_BACKEND.CreateMessageCanal(done, "clicked", self.close)
 
     def PopulateTable(self) -> None:
         """"""
         self.value: cllt.Iterable[cllt.Iterable]
         self.viewer: wdgt.QTableView
         self.model: qtui.QStandardItemModel
```

### Comparing `pyvispr-2024.3/pyvispr/catalog/installer.py` & `pyvispr-2024.4/pyvispr/catalog/installer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/catalog/parser.py` & `pyvispr-2024.4/pyvispr/catalog/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import importlib as mprt
 import inspect as spct
-import types as t
+from pathlib import Path as path_t
 
 from pyvispr.constant.catalog import (
     ACTUAL_SOURCE,
     FUNCTION_NAME,
     INPUT_II_NAMES,
     NODE_NAME,
     OUTPUT_NAMES,
@@ -59,61 +59,59 @@
     )
 
 
 def AllFunctions(
     module_name: str, /, *, recursively: bool = False
 ) -> tuple[function_t | None, ...]:
     """"""
-    module = mprt.import_module(module_name)
-    if recursively:
-        output = []
-        modules = []
-        _AllFunctionsRecursively(f"{module_name}.", module, modules, output)
-    else:
-        output = _AllFunctions(module)
-        if output.__len__() == 0:
-            modules = []
-            _AllFunctionsRecursively(f"{module_name}.", module, modules, output)
+    functions = []
+    modules = {module_name}
+    parent_path = IsInnerModule_ = None
+    while modules.__len__() > 0:
+        module_or_name = modules.pop()
+        if isinstance(module_or_name, str):
+            module = mprt.import_module(module_or_name)
+            parent_path = path_t(module.__path__[0])
+            IsInnerModule_ = lambda _elm: IsInnerModule(_elm, parent_path)
+        else:
+            module = module_or_name
+
+        functions.extend(
+            (f"{module.__name__}.{elm[0]}", elm[1], module)
+            for elm in spct.getmembers(module, IsFunction)
+            if elm[0][0] != "_"
+        )
+        if recursively:
+            modules.update(
+                elm[1]
+                for elm in spct.getmembers(module, IsInnerModule_)
+                if elm[0][0] != "_"
+            )
+
+    filtered = {}
+    for full_name, function, module in functions:
+        if function in filtered:
+            if filtered[function][0].__len__() > full_name.__len__():
+                filtered[function] = (full_name, module)
+        else:
+            filtered[function] = (full_name, module)
+
+    output = []
+    for function, (full_name, module) in filtered.items():
+        _, name = full_name.rsplit(".", maxsplit=1)
+        output.append(function_t.NewFromInstance(function, name, module))
 
     return tuple(output)
 
 
-def _AllFunctions(module: t.ModuleType, /) -> list[function_t | None]:
+def IsFunction(element: object, /) -> bool:
     """"""
-    output = []
+    return spct.isfunction(element) or hasattr(element, "__call__")
 
-    for name in dir(module):
-        if name[0] == "_":
-            continue
-
-        element = getattr(module, name)
-        if (is_function := spct.isfunction(element)) or hasattr(element, "__call__"):
-            if is_function:
-                function = element
-            else:
-                function = element.__call__
-            output.append(function_t.NewFromInstance(function, name, module))
-
-    return output
-
-
-def _AllFunctionsRecursively(
-    prefix: str,
-    module: t.ModuleType,
-    modules: list[t.ModuleType],
-    output: list[function_t | None],
-    /,
-) -> None:
-    """"""
-    modules.append(module)
 
-    OnlyModulesOrFunctions = lambda _arg: spct.ismodule(_arg) or spct.isfunction(_arg)
-    for name, element in spct.getmembers(module, OnlyModulesOrFunctions):
-        # Explicitly defined: spct.getmodule(function) == module
-        if name[0] == "_":
-            continue
-
-        if spct.ismodule(element):
-            if element not in modules:
-                _AllFunctionsRecursively(prefix, element, modules, output)
-        elif module.__name__.startswith(prefix):
-            output.append(function_t.NewFromInstance(element, name, module))
+def IsInnerModule(element: object, parent_path: path_t, /) -> bool:
+    """"""
+    return (
+        spct.ismodule(element)
+        and hasattr(element, "__path__")
+        and path_t(element.__path__[0]).is_relative_to(parent_path)
+    )
```

### Comparing `pyvispr-2024.3/pyvispr/catalog/type.py` & `pyvispr-2024.4/pyvispr/catalog/type.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/config/appearance/backend.py` & `pyvispr-2024.4/pyvispr/config/appearance/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/config/appearance/behavior.py` & `pyvispr-2024.4/pyvispr/config/appearance/behavior.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/config/appearance/color.py` & `pyvispr-2024.4/pyvispr/config/appearance/color.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from PyQt6.QtCore import Qt as constant_e
 from PyQt6.QtGui import QBrush
 from PyQt6.QtGui import QColorConstants as _colors
 from PyQt6.QtGui import QPen
+from pyvispr.config.appearance.geometry import LINK_WIDTH
 
 color_e = _colors.Svg
 
 
 NODE_BRUSH_RESTING = QBrush(color_e.lightgray)
 NODE_BRUSH_RUNNING = QBrush(color_e.limegreen)
 NODE_BRUSH_SELECTED = QBrush(color_e.chartreuse)
@@ -47,15 +48,15 @@
 BUTTON_BRUSH_STATE_DOING = QBrush(color_e.dodgerblue)
 BUTTON_BRUSH_STATE_DONE = QBrush(color_e.mediumblue)
 BUTTON_BRUSH_STATE_TODO = QBrush(color_e.gold)
 
 INOUT_BRUSH_ACTIVE = QBrush(color_e.chartreuse)
 INOUT_BRUSH_INACTIVE = QBrush(color_e.dodgerblue)
 
-LINK_PEN_EMPTY = QPen(color_e.dodgerblue, 3, constant_e.PenStyle.DashLine)
-LINK_PEN_FULL = QPen(color_e.dodgerblue, 3, constant_e.PenStyle.SolidLine)
+LINK_PEN_EMPTY = QPen(color_e.dodgerblue, LINK_WIDTH, constant_e.PenStyle.DashLine)
+LINK_PEN_FULL = QPen(color_e.dodgerblue, LINK_WIDTH, constant_e.PenStyle.SolidLine)
 LINK_BRUSH_ARROW = QBrush(color_e.dodgerblue)
 
 GRID_PEN = QPen(color_e.gainsboro)
 
 ORANGE_BRUSH = QBrush(color_e.orange)
 BLACK_BRUSH = QBrush(color_e.black)
```

### Comparing `pyvispr-2024.3/pyvispr/config/appearance/geometry.py` & `pyvispr-2024.4/pyvispr/config/appearance/geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 
 WHITEBOARD_WIDTH = 640
 WHITEBOARD_HEIGHT = 480
 
 NODE_WIDTH_TOTAL = 120
 NODE_HEIGHT_TOTAL = 75
 BUTTON_WIDTH = 15
+
+LINK_WIDTH = 5
 LINK_MIN_HORIZONTAL_SHIFT = 3 * BUTTON_WIDTH
```

### Comparing `pyvispr-2024.3/pyvispr/config/path.py` & `pyvispr-2024.4/pyvispr/config/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/constant/app.py` & `pyvispr-2024.4/pyvispr/constant/app.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/constant/catalog.py` & `pyvispr-2024.4/pyvispr/constant/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/constant/function.py` & `pyvispr-2024.4/pyvispr/constant/function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/constant/path.py` & `pyvispr-2024.4/pyvispr/constant/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/constant/socket.py` & `pyvispr-2024.4/pyvispr/constant/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/constant/widget/function_header.py` & `pyvispr-2024.4/pyvispr/constant/widget/function_header.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/constant/widget/list.py` & `pyvispr-2024.4/pyvispr/constant/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/constant/widget/node.py` & `pyvispr-2024.4/pyvispr/constant/widget/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/extension/function.py` & `pyvispr-2024.4/pyvispr/extension/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,18 @@
     ) -> function_t:
         """"""
         path = getattr(module, "__file__", None)
         pypath = module.__name__
 
         try:
             source = spct.getsource(instance)
-        except TypeError:  # See documentation.
+        except (OSError, TypeError):  # See documentation.
+            as_str = getattr(instance, "__name__", str(instance))
             LOGGER.error(
-                f"Cannot read source of {pypath}.{instance.__name__}; Returning dummy function"
+                f"Cannot read source of {pypath}.{as_str}; Returning dummy function"
             )
             return cls.Dummy(instance, expected_name, module, path, pypath)
 
         imports = []
         header_inputs: dict[str, str | tuple[str, str]] = {}
 
         function_node = FirstFunctionAsAstNode(source)
```

### Comparing `pyvispr-2024.3/pyvispr/extension/module.py` & `pyvispr-2024.4/pyvispr/extension/module.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/extension/qt6.py` & `pyvispr-2024.4/pyvispr/extension/qt6.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/extension/string_.py` & `pyvispr-2024.4/pyvispr/extension/string_.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/flow/descriptive/node.py` & `pyvispr-2024.4/pyvispr/flow/descriptive/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,19 @@
         else:  # source_e.local or source_e.referenced
             ModuleAndFunction = M_F_FromPathAndName
         self.module, self.Function = ModuleAndFunction(
             self.actual.path, self.actual.name
         )
         self.documentation = spct.getdoc(self.Function)
 
-        # Always use the signature of the proxy function since it might have been corrected.
-        _, Function = M_F_FromPathAndName(self.proxy.path, self.proxy.name)
+        if self.proxy is self.actual:
+            Function = self.Function
+        else:
+            # Always use the signature of the proxy function since it might have been corrected.
+            _, Function = M_F_FromPathAndName(self.proxy.path, self.proxy.name)
         signature = spct.signature(Function)
 
         spct_inputs = signature.parameters
         for name, input_ in self.inputs.items():
             if input_.UpdateFromSignature(spct_inputs[name]):
                 self.requires_completion = True
```

### Comparing `pyvispr-2024.3/pyvispr/flow/descriptive/socket.py` & `pyvispr-2024.4/pyvispr/flow/descriptive/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/flow/functional/link.py` & `pyvispr-2024.4/pyvispr/flow/functional/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 f"Link {output_name} ⮞ {target.unique_name}.{input_name} already present."
             )
         else:
             links.append((target, input_name))
 
         source_output_name = source.UniqueOutputName(output_name)
         value = source.outputs[output_name].value
-        target.inputs[input_name].Activate(source_output_name, value)
+        target.inputs[input_name].Connect(source_output_name, value)
 
     def Remove(
         self, output_name: str | None, target: node_t | None, input_name: str | None, /
     ) -> None:
         """"""
         for current_out, links in self.items():
             for current_target, current_in in links:
@@ -74,15 +74,15 @@
                     output_name,
                     target,
                     input_name,
                     current_out,
                     current_target,
                     current_in,
                 ):
-                    current_target.inputs[current_in].DeActivate()
+                    current_target.inputs[current_in].Disconnect()
 
         if output_name is None:
             self.clear()
             return
 
         if target is None:
             # Could be del self[output_name] directly. Implemented indirectly for "coherence" with the other cases.
```

### Comparing `pyvispr-2024.3/pyvispr/flow/functional/node_isolated.py` & `pyvispr-2024.4/pyvispr/flow/functional/node_isolated.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,22 @@
 from enum import Enum as enum_t
 
 from json_any import JsonStringOf
 from logger_36 import LOGGER
 from pyvispr.constant.socket import OUTPUT_SET, OUTPUT_UNSET
 from pyvispr.flow.descriptive.node import node_t as description_t
 from pyvispr.flow.functional.socket import input_t, output_t
-from pyvispr.runtime.messenger import MESSENGER
+from sio_messenger.instance import MESSENGER
 
 
 class state_e(enum_t):
-    disabled = 1
-    todo = 2
-    running = 3
-    done = 4
+    disabled = 0
+    todo = 1
+    doing = 2
+    done = 3
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class node_t:
     """
     The description is shared among all the functional nodes.
 
@@ -112,44 +112,36 @@
                 f"{name}{node_t.UNIQUE_NAME_SEPARATOR}"
                 f"{uid}{node_t.UNIQUE_OUTPUT_NAME_SEPARATOR}"
                 f"{output_name}"
             )
 
     def InvalidateInputValue(self, /, *, name: str | None = None) -> None:
         """"""
-        if self.state is state_e.disabled:
+        if self.state in (state_e.todo, state_e.disabled):
             return
 
         if name is None:
             for input_ in self.inputs.values():
                 input_.Invalidate()
         else:
             self.inputs[name].Invalidate()
-        self.state = state_e.todo
-        MESSENGER.TransmitMessage(state_e.todo, self)
+
+        self.InvalidateOutputValues()
 
     def InvalidateOutputValues(self) -> None:
         """"""
-        if self.state is state_e.disabled:
+        if self.state in (state_e.todo, state_e.disabled):
             return
 
         for output in self.outputs.values():
             output.Invalidate()
-        self.state = state_e.todo
-        MESSENGER.TransmitMessage(state_e.todo, self)
-        MESSENGER.TransmitMessage(OUTPUT_UNSET, self)
 
-    def ToggleAbility(self) -> None:
-        """"""
-        if self.state is state_e.disabled:
-            self.state = state_e.todo
-            MESSENGER.TransmitMessage(state_e.todo, self)
-        else:
-            self.state = state_e.disabled
-            MESSENGER.TransmitMessage(state_e.disabled, self)
+        self.state = state_e.todo
+        MESSENGER.Transmit(self.state, self)
+        MESSENGER.Transmit(OUTPUT_UNSET, self)
 
     @property
     def can_run(self) -> bool:
         """
         It must have been checked that the state is not disabled.
 
         This method is meant to be called from functional.graph.Run,
@@ -163,16 +155,16 @@
             for _elm in self.inputs
         )
 
     def Run(self, /, *, script_accessor: h.TextIO = None) -> None:
         """
         It must have been checked that the state is not disabled.
         """
-        self.state = state_e.running
-        MESSENGER.TransmitMessage(state_e.running, self)
+        self.state = state_e.doing
+        MESSENGER.Transmit(self.state, self)
 
         should_save_as_script = script_accessor is not None
 
         if should_save_as_script:
             if self.description.n_outputs > 1:
                 output_assignments = (
                     self.UniqueOutputName(_elm) for _elm in self.outputs
@@ -239,15 +231,15 @@
         if n_outputs > 1:
             for name, value in zip(output_names, output_values):
                 self._SetOutputValue(name, value)
         elif n_outputs > 0:
             self._SetOutputValue(output_names[0], output_values)
 
         self.state = state_e.done
-        MESSENGER.TransmitMessage(state_e.done, self)
+        MESSENGER.Transmit(self.state, self)
 
     def _SafeOutputValues(
         self,
         anonymous_args: h.Sequence[h.Any] | None,
         named_args: dict[str, h.Any] | None,
         /,
     ) -> h.Any | None:
@@ -268,15 +260,15 @@
     def SetInputValue(self, name: str, value: h.Any, /) -> None:
         """"""
         self.inputs[name].value = value
 
     def _SetOutputValue(self, name: str, value: h.Any, /) -> None:
         """"""
         self.outputs[name].value = value
-        MESSENGER.TransmitMessage(OUTPUT_SET, self)
+        MESSENGER.Transmit(OUTPUT_SET, self)
 
 
 def _EncodedValue(value: h.Any, /) -> str:
     """"""
     as_str, issues = JsonStringOf(value)
     if issues is None:
         as_str = as_str.replace('"', '\\"')
```

### Comparing `pyvispr-2024.3/pyvispr/flow/functional/node_linked.py` & `pyvispr-2024.4/pyvispr/interface/window/widget/list_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,71 +25,72 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from __future__ import annotations
-
 import dataclasses as dtcl
+from re import search as SearchRegEx
 
-from pyvispr.flow.functional.link import outbound_links_t
-from pyvispr.flow.functional.node_isolated import node_t as base_t
-from pyvispr.flow.functional.node_isolated import state_e
-
-
-@dtcl.dataclass(repr=False, eq=False)
-class node_t(base_t):
-    """
-    links[idx]: Outbound links of node of index idx in list "nodes":
-        - None if node has no outbound links.
-        - If not None, dictionary with:
-            - key=name of output and...
-            - value=list of alternating target nodes and name of target inputs.
-
-    Cannot be sloted because of QThread issue with weak reference (see visual.graph).
-    """
+from PyQt6.QtCore import Qt as constant_e
+from pyvispr.config.appearance.color import ORANGE_BRUSH
+from pyvispr.flow.descriptive.node import node_t
+from pyvispr.interface.window.widget.list import list_wgt_t
+from pyvispr.runtime.catalog import NODE_CATALOG
 
-    links: outbound_links_t = dtcl.field(init=False, default_factory=outbound_links_t)
 
-    def AddLink(self, output_name: str, target: node_t, input_name: str, /) -> None:
-        """"""
-        self.links.Add(
-            self,
-            output_name,
-            target,
-            input_name,
-        )
-
-    def RemoveLink(
-        self, output_name: str | None, target: node_t | None, input_name: str | None, /
-    ) -> None:
-        """"""
-        self.links.Remove(output_name, target, input_name)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class node_list_wgt_t(list_wgt_t):
+    nodes: dict[str, node_t] = dtcl.field(init=False, default_factory=dict)
 
-    def OutputIsLinked(self, name: str, /) -> bool:
+    def ActualReload(self) -> None:
         """"""
-        return name in self.links
+        for node in NODE_CATALOG:
+            self.nodes[node.name] = node
 
-    @property
-    def needs_running(self) -> bool:
-        """
-        Note: the decision is based on whether the outputs are valid for use downward in the workflow,
-        not on whether the inputs have changed since the last run.
-        """
-        if self.state is state_e.disabled:
-            return False
-
-        if self.description.n_outputs == 0:
-            return True
-
-        return any(
-            self.OutputIsLinked(_nme) and (not _rcd.has_value)
-            for _nme, _rcd in self.outputs.items()
-        )
+            self.addItem(node.name)
+            item = self.item(self.count() - 1)
+            if node.documentation is not None:
+                item.setToolTip(node.documentation)
+            if node.requires_completion:
+                item.setForeground(ORANGE_BRUSH)
 
-    def SendOutputsToSuccessors(self) -> None:
+    def Filter(self, new_filter: str, /) -> None:
         """"""
-        for name, output in self.outputs.items():
-            for next_node, next_in_name in self.links[name]:
-                next_node.SetInputValue(next_in_name, output.value)
+        if new_filter.__len__() > 0:
+            matched_items = self.findItems(
+                new_filter, constant_e.MatchFlag.MatchContains
+            )
+
+            for item_idx in range(self.count()):
+                node_item = self.item(item_idx)
+                node_description = NODE_CATALOG.NodeDescription(node_item.text())
+
+                if node_description.keywords is None:
+                    mismatches_key_xpressions = True
+                else:
+                    mismatches_key_xpressions = (
+                        new_filter not in node_description.keywords
+                    )
+
+                if node_description.short_description is None:
+                    mismatches_short_description = True
+                else:
+                    mismatches_short_description = (
+                        SearchRegEx(
+                            "\b" + new_filter + "\b", node_description.short_description
+                        )
+                        is None
+                    )
+
+                if (
+                    (node_item not in matched_items)
+                    and mismatches_key_xpressions
+                    and mismatches_short_description
+                ):
+                    node_item.setHidden(True)
+                else:
+                    node_item.setHidden(False)
+        else:
+            for item_idx in range(self.count()):
+                self.item(item_idx).setHidden(False)
```

### Comparing `pyvispr-2024.3/pyvispr/flow/functional/socket.py` & `pyvispr-2024.4/pyvispr/flow/functional/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,21 +54,21 @@
     """
     Used only for script output (no need to save).
     """
 
     is_linked: bool = False
     source_output_name: str | None = None
 
-    def Activate(self, output_unique_name: str, output_value: h.Any, /) -> None:
+    def Connect(self, output_unique_name: str, output_value: h.Any, /) -> None:
         """"""
         self.is_linked = True
         self.source_output_name = output_unique_name
         self.value = output_value
 
-    def DeActivate(self) -> None:
+    def Disconnect(self) -> None:
         """"""
         self.is_linked = False
         self.source_output_name = None
         self.value = VALUE_NOT_SET
 
 
 output_t = _base_t
```

### Comparing `pyvispr-2024.3/pyvispr/flow/messenger.py` & `pyvispr-2024.4/pyvispr/runtime/socket.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,26 +25,20 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import typing as h
-from enum import Enum as enum_t
 
+class assign_when_importing_t:
+    pass
 
-class messenger_t(dict[str | enum_t, list[h.Callable]]):
-    def AddCanal(
-        self, name: str | enum_t, AcknowledgeMessage: h.Callable[[...], None]
-    ) -> None:
-        """
-        Canal: From message name to message acknowledgement function.
-        """
-        if name not in self:
-            self[name] = []
-        self[name].append(AcknowledgeMessage)
-
-    def TransmitMessage(self, name: str | enum_t, /, *args, **kwargs) -> None:
-        """"""
-        for AcknowledgeMessage in self.get(name, ()):
-            AcknowledgeMessage(*args, **kwargs)
+
+ASSIGN_WHEN_ACTIVATING = assign_when_importing_t()
+
+
+class value_not_set_t:
+    pass
+
+
+VALUE_NOT_SET = value_not_set_t()
```

### Comparing `pyvispr-2024.3/pyvispr/flow/visual/graph.py` & `pyvispr-2024.4/pyvispr/flow/visual/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,18 @@
 from pyvispr.flow.functional.graph import graph_t as graph_functional_t
 from pyvispr.flow.functional.node_isolated import state_e
 from pyvispr.flow.functional.node_linked import node_t as functional_t
 from pyvispr.flow.visual.ii_value import invalid_ii_value_t
 from pyvispr.flow.visual.link import link_t
 from pyvispr.flow.visual.node import node_t
 from pyvispr.flow.visual.socket import active_socket_t
-from pyvispr.interface.window.messenger import CreateMessageCanal
+from pyvispr.runtime.backend import SCREEN_BACKEND
 from pyvispr.runtime.catalog import NODE_CATALOG
-from pyvispr.runtime.messenger import MESSENGER
 from pyvispr.runtime.socket import VALUE_NOT_SET
+from sio_messenger.instance import MESSENGER
 from str_to_obj.task.comparison import TypesAreCompatible
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class graph_t(wdgt.QGraphicsScene):
     functional: graph_functional_t = dtcl.field(
         init=False, default_factory=graph_functional_t
@@ -83,19 +83,19 @@
 
     def __post_init__(self) -> None:
         """"""
         wdgt.QGraphicsScene.__init__(self)
         # Does not seem to have an effet.
         # self.setSceneRect(QRectF(-500, -500, 1000, 1000))
 
-        CreateMessageCanal(self, "changed", self.UpdateLinks)
+        SCREEN_BACKEND.CreateMessageCanal(self, "changed", self.UpdateLinks)
 
         MESSENGER.AddCanal(state_e.disabled, self.AcknowledgeDisabled)
-        MESSENGER.AddCanal(state_e.todo, self.AcknowledgeToDo)
-        MESSENGER.AddCanal(state_e.running, self.AcknowledgeRunningStarted)
+        MESSENGER.AddCanal(state_e.todo, self.AcknowledgeNeedsRunning)
+        MESSENGER.AddCanal(state_e.doing, self.AcknowledgeRunningStarted)
         MESSENGER.AddCanal(state_e.done, self.AcknowledgeRunningEnded)
         MESSENGER.AddCanal(OUTPUT_SET, self.AcknowledgeLinkFull)
         MESSENGER.AddCanal(OUTPUT_UNSET, self.AcknowledgeLinkEmpty)
 
     @classmethod
     def __NewFromJsonDescription__(cls, description, /) -> graph_t:
         """"""
@@ -267,17 +267,15 @@
         source: node_t,
         output_name: str,
         target: node_t,
         input_name: str,
         /,
     ) -> None:
         """"""
-        self.functional.AddLink(
-            source.functional, output_name, target.functional, input_name
-        )
+        source.functional.AddLink(output_name, target.functional, input_name)
         found = None
         for link in self.links:
             if (link.source_node is source) and (link.target_node is target):
                 found = link
                 break
         if found:
             found.SetTooltip()
@@ -313,24 +311,22 @@
         /,
         output_name: str | None = None,
         input_name: str | None = None,
     ) -> None:
         """"""
         if output_name is None:  # input_name must also be None.
             for output_name, input_name in link.UnderlyingFunctionals():
-                self.functional.RemoveLink(
-                    link.source_node.functional,
+                link.source_node.functional.RemoveLink(
                     output_name,
                     link.target_node.functional,
                     input_name,
                 )
             should_be_actually_removed = True
         else:  # Both names are not None.
-            self.functional.RemoveLink(
-                link.source_node.functional,
+            link.source_node.functional.RemoveLink(
                 output_name,
                 link.target_node.functional,
                 input_name,
             )
             should_be_actually_removed = link.UnderlyingFunctionals().__len__() == 0
 
         if should_be_actually_removed:
@@ -338,15 +334,15 @@
             self.removeItem(link)
             self.removeItem(link.arrow)
         else:
             link.SetTooltip()
 
     def UpdateLinks(self, _: h.Sequence[QRectF], /) -> None:
         """"""
-        for node in self.selectedItems():
+        for node in self.items():
             if isinstance(node, node_t) and node.position_has_changed:
                 for link in self.links:
                     link.SetPath(
                         link.source_node.output_anchor_coordinates,
                         link.target_node.input_anchor_coordinates,
                     )
                 node.position_has_changed = False
@@ -430,15 +426,15 @@
 
     def AcknowledgeDisabled(self, functional: functional_t, /) -> None:
         """"""
         self._AcknowledgeNodeState(
             functional, "Disabled", (NODE_BRUSH_RESTING, BUTTON_BRUSH_STATE_DISABLED)
         )
 
-    def AcknowledgeToDo(self, functional: functional_t, /) -> None:
+    def AcknowledgeNeedsRunning(self, functional: functional_t, /) -> None:
         """"""
         self._AcknowledgeNodeState(
             functional, "Needs Running", (NODE_BRUSH_RESTING, BUTTON_BRUSH_STATE_TODO)
         )
 
     def AcknowledgeRunningStarted(self, functional: functional_t, /) -> None:
         """"""
@@ -477,16 +473,15 @@
         self._AcknowledgeLinkState(functional, LINK_PEN_FULL)
 
     def _AcknowledgeLinkState(self, functional: functional_t, pen: QPen, /) -> None:
         """"""
         for link in self.links:
             if link.source_node.functional is functional:
                 link.setPen(pen)
-                QCoreApplication.processEvents()
-                break
+        QCoreApplication.processEvents()
 
 
 def _SocketSelection(
     possible_names: tuple[str, ...], position: QPoint, /
 ) -> str | None:
     """"""
     menu = wdgt.QMenu()
```

### Comparing `pyvispr-2024.3/pyvispr/flow/visual/ii_value.py` & `pyvispr-2024.4/pyvispr/flow/visual/ii_value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/flow/visual/link.py` & `pyvispr-2024.4/pyvispr/flow/visual/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/flow/visual/node.py` & `pyvispr-2024.4/pyvispr/flow/visual/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     NEEDS_RUNNING,
     TOP_OF_BOTTOM_BUTTONS,
     WIDTH_OF_LATERAL_BUTTONS,
 )
 from pyvispr.flow.descriptive.socket import assignment_e
 from pyvispr.flow.functional.node_linked import node_t as functional_t
 from pyvispr.flow.visual.ii_value import invalid_ii_value_t
-from pyvispr.interface.window.messenger import CreateMessageCanal
 from pyvispr.runtime.backend import SCREEN_BACKEND
 from pyvispr.runtime.socket import VALUE_NOT_SET, value_not_set_t
 from str_to_obj import annotation_t
 
 
 class ii_widget_p(wdgt.QWidget):
     def Assign(
@@ -94,16 +93,16 @@
     interactive_inputs: dict[str, ii_widget_p] | None = dtcl.field(
         init=False, default=None
     )
     position_has_changed: bool = dtcl.field(init=False, default=False)
 
     def __post_init__(self) -> None:
         """"""
-        # If using: self.setRect(QRectF(0, 0, NODE_WIDTH_TOTAL, NODE_HEIGHT_TOTAL)), Python complains about super-init
-        # not having been called.
+        # If using: self.setRect(QRectF(0, 0, NODE_WIDTH_TOTAL, NODE_HEIGHT_TOTAL)),
+        # Python complains about super-init not having been called.
         wdgt.QGraphicsRectItem.__init__(
             self, QRectF(0, 0, NODE_WIDTH_TOTAL, NODE_HEIGHT_TOTAL)
         )
 
         for item in (
             self.label,
             self.in_btn,
@@ -289,17 +288,15 @@
                 layout.addWidget(value_wgt.library_wgt, i_idx, 2, 1, 1)
 
                 if isinstance(value_wgt.library_wgt, wdgt.QStackedWidget):
                     widgets = (_elm for _elm in value_wgt.values)
                 else:
                     widgets = (value_wgt,)
                 for widget in widgets:
-                    widget.SetAcknowledgeValueChangeFunction(
-                        self.functional.InvalidateOutputValues
-                    )
+                    widget.SetAcknowledgeValueChangeFunction(self.functional.Invalidate)
 
         if n_widgets > 0:
             self.interactive_inputs = interactive_inputs
 
             widget = wdgt.QWidget()
             widget.setLayout(layout)
             widget.setStyleSheet(f"background-color: {color_e.deepskyblue.name()};")
```

### Comparing `pyvispr-2024.3/pyvispr/flow/visual/socket.py` & `pyvispr-2024.4/pyvispr/flow/visual/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/flow/visual/whiteboard.py` & `pyvispr-2024.4/pyvispr/flow/visual/whiteboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,15 @@
 
                 item_global_pos = self.mapToGlobal(view_position)
                 selected_action = menu.exec(item_global_pos)
 
                 if (selected_action is None) or (selected_action is cancel_action):
                     return
                 if selected_action is invalidate_action:
-                    self.graph.functional.InvalidateNodesInCascadeFromNode(
-                        item.functional
-                    )
+                    item.functional.Invalidate()
                 elif selected_action is disable_action:
                     item.functional.ToggleAbility()
                 if selected_action is remove_action:
                     self.graph.RemoveNode(item)
             else:
                 wdgt.QGraphicsView.mousePressEvent(self, event)
         else:
```

### Comparing `pyvispr-2024.3/pyvispr/install.py` & `pyvispr-2024.4/pyvispr/install.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/interface/storage/loading.py` & `pyvispr-2024.4/pyvispr/interface/storage/loading.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,9 +71,18 @@
         )
         loading_mode.exec()
 
         is_update = loading_mode.clickedButton() == merging
     else:
         is_update = False
 
-    loaded = LoadFromJSON(filename)
+    try:
+        loaded = LoadFromJSON(filename)
+    except Exception as exception:
+        wdgt.QMessageBox.critical(
+            None,
+            f"Workflow Loading Error",
+            str(exception),
+        )
+        return
+
     manager.whiteboard.SetGraph(graph=loaded, is_update=is_update)
```

### Comparing `pyvispr-2024.3/pyvispr/interface/storage/stowing.py` & `pyvispr-2024.4/pyvispr/interface/storage/stowing.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,15 +78,17 @@
     last_save_as_script_location = ExtractPathPart(filename)
 
     _SaveAsScript(manager.whiteboard.graph, filename)
 
 
 def _Save(graph: graph_t, filename: str, /) -> None:
     """"""
-    path = StoreAsJSON(graph, filename, should_continue_on_error=True)
+    path = StoreAsJSON(
+        graph, filename, should_continue_on_error=True, should_overwrite_path=True
+    )
     if isinstance(path, path_t):
         wdgt.QMessageBox.about(
             None,
             "Workflow Successfully Saved",
             f"Workflow Successfully Saved in: {path}.",
         )
     else:
```

### Comparing `pyvispr-2024.3/pyvispr/interface/window/installer.py` & `pyvispr-2024.4/pyvispr/interface/window/installer.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     UpdateFunction,
 )
 from pyvispr.config.appearance.behavior import TOO_MANY_SELECTED
 from pyvispr.config.appearance.color import BLACK_BRUSH
 from pyvispr.constant.app import APP_NAME
 from pyvispr.extension.function import function_t
 from pyvispr.flow.descriptive.node import source_e
-from pyvispr.interface.window.messenger import CreateMessageCanal
 from pyvispr.interface.window.widget.function_header import HeaderDialog, header_wgt_t
 from pyvispr.interface.window.widget.list_file import file_list_wgt_t
 from pyvispr.interface.window.widget.list_function import function_list_wgt_t
 from pyvispr.interface.window.widget.list_module import module_list_wgt_t
 from pyvispr.interface.window.widget.list_node import node_list_wgt_t
 from pyvispr.runtime.backend import SCREEN_BACKEND
 
@@ -104,17 +103,21 @@
         layout.addWidget(tabs)
         layout.addWidget(done)
 
         central = wdgt.QWidget()
         central.setLayout(layout)
         self.setCentralWidget(central)
 
-        CreateMessageCanal(self.node_list, "itemClicked", self.CorrectHeaderOrUninstall)
-        CreateMessageCanal(self.module_list, "itemClicked", self.LoadFunctions)
-        CreateMessageCanal(done, "clicked", self.close)
+        SCREEN_BACKEND.CreateMessageCanal(
+            self.node_list, "itemClicked", self.CorrectHeaderOrUninstall
+        )
+        SCREEN_BACKEND.CreateMessageCanal(
+            self.module_list, "itemClicked", self.LoadFunctions
+        )
+        SCREEN_BACKEND.CreateMessageCanal(done, "clicked", self.close)
 
     @classmethod
     def New(cls) -> installer_wdw_t:
         """"""
         node_list = node_list_wgt_t(element_name="Nodes")
         file_list = file_list_wgt_t(element_name="Python Files")
         module_list = module_list_wgt_t(element_name="Modules")
@@ -226,25 +229,29 @@
 
     def InstallSystemFunction(self) -> None:
         """"""
         if self.function_list.module is None:
             return
 
         selected_s = self.function_list.SelectedItemsOrAll()
-        module_pypath = self.function_list.module
         should_correct_header = selected_s.__len__() < TOO_MANY_SELECTED
         for selected in selected_s:
-            function_name = selected.text()
+            function_display_name = selected.text()
+            if "." in function_display_name:
+                _, function_name = function_display_name.rsplit(".", maxsplit=1)
+            else:
+                function_name = function_display_name
+            module_pypath = self.function_list.functions[function_display_name].pypath
             where = PathForSystem(module_pypath, function_name)
             if where.is_file() and _ShouldNotProceedWithInstallation(
                 f"{module_pypath}.{function_name}"
             ):
                 continue
 
-            function = self.function_list.functions[function_name]
+            function = self.function_list.functions[function_display_name]
             if should_correct_header:
                 header_dialog = HeaderDialog(
                     None,
                     function,
                     self._HeaderRetrievalInitialization,
                     self._RetrieveFinalHeader,
                     self,
@@ -364,18 +371,18 @@
 
     layout = wdgt.QVBoxLayout()
 
     layout.addWidget(local)
     layout.addWidget(referenced)
     output.setLayout(layout)
 
-    CreateMessageCanal(
+    SCREEN_BACKEND.CreateMessageCanal(
         local, "clicked", lambda *args, **kwargs: InstallUserFunction(source_e.local)
     )
-    CreateMessageCanal(
+    SCREEN_BACKEND.CreateMessageCanal(
         referenced,
         "clicked",
         lambda *args, **kwargs: InstallUserFunction(source_e.referenced),
     )
 
     return output
 
@@ -411,21 +418,21 @@
     right.addWidget(install_referenced)
 
     main_layout.addLayout(left)
     main_layout.addLayout(right)
 
     output.setLayout(main_layout)
 
-    CreateMessageCanal(select, "clicked", ChooseUserFolder)
-    CreateMessageCanal(
+    SCREEN_BACKEND.CreateMessageCanal(select, "clicked", ChooseUserFolder)
+    SCREEN_BACKEND.CreateMessageCanal(
         install_local,
         "clicked",
         lambda *args, **kwargs: InstallUserFolder(source_e.local),
     )
-    CreateMessageCanal(
+    SCREEN_BACKEND.CreateMessageCanal(
         install_referenced,
         "clicked",
         lambda *args, **kwargs: InstallUserFolder(source_e.referenced),
     )
 
     return output
 
@@ -445,15 +452,15 @@
     for col, widget in enumerate((module_list, function_list)):
         layout.addWidget(widget, 0, col)
         layout.addWidget(widget.filter_wgt, 1, col)
     layout.addWidget(install, 2, 0, 1, 2)
 
     output.setLayout(layout)
 
-    CreateMessageCanal(install, "clicked", InstallSystemFunction_)
+    SCREEN_BACKEND.CreateMessageCanal(install, "clicked", InstallSystemFunction_)
 
     return output
 
 
 def _ShouldNotProceedWithInstallation(what: str, /, *, how_installed: str = "") -> bool:
     """"""
     answer_cancel = wdgt.QMessageBox.StandardButton.Cancel
```

### Comparing `pyvispr-2024.3/pyvispr/interface/window/messenger.py` & `pyvispr-2024.4/pyvispr/interface/window/widget/list_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,18 +25,19 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import typing as h
+import dataclasses as dtcl
 
-from PyQt6.QtCore import QObject, pyqtBoundSignal
+from logger_36.task.inspection import Modules
+from pyvispr.interface.window.widget.list import list_wgt_t
 
 
-def CreateMessageCanal(
-    messenger: QObject, message: str, AcknowledgeMessage: h.Callable, /
-) -> None:
-    """"""
-    signal: pyqtBoundSignal = getattr(messenger, message)
-    signal.connect(AcknowledgeMessage)
+@dtcl.dataclass(slots=True, repr=False, eq=False)
+class module_list_wgt_t(list_wgt_t):
+    def ActualReload(self) -> None:
+        """"""
+        for module in Modules(False, False, only_loaded=False):
+            self.addItem(module)
```

### Comparing `pyvispr-2024.3/pyvispr/interface/window/runner.py` & `pyvispr-2024.4/pyvispr/interface/window/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 import PyQt6.QtWidgets as wdgt
 from logger_36 import AddGenericHandler
 from pyvispr import __version__
 from pyvispr.constant.app import APP_NAME
 from pyvispr.flow.visual.whiteboard import whiteboard_t
 from pyvispr.interface.storage.loading import LoadWorkflow
 from pyvispr.interface.storage.stowing import SaveWorkflow, SaveWorkflowAsScript
-from pyvispr.interface.window.messenger import CreateMessageCanal
 from pyvispr.interface.window.widget.list_node import node_list_wgt_t
 from pyvispr.interface.window.widget.menu import AddEntryToMenu
+from pyvispr.runtime.backend import SCREEN_BACKEND
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class runner_wdw_t(wdgt.QMainWindow):
     node_list: node_list_wgt_t
     whiteboard: whiteboard_t
     status_bar: wdgt.QStatusBar = dtcl.field(init=False)
@@ -76,15 +76,15 @@
         central = wdgt.QWidget()
         central.setLayout(layout)
         self.setCentralWidget(central)
 
         self._AddMenuBar()
         self.status_bar = self.statusBar()
 
-        CreateMessageCanal(self.node_list, "itemClicked", self.AddNode)
+        SCREEN_BACKEND.CreateMessageCanal(self.node_list, "itemClicked", self.AddNode)
 
     @classmethod
     def New(cls) -> runner_wdw_t:
         """"""
         node_list = node_list_wgt_t(element_name="Nodes")
         whiteboard = whiteboard_t()
```

### Comparing `pyvispr-2024.3/pyvispr/interface/window/widget/function_header.py` & `pyvispr-2024.4/pyvispr/interface/window/widget/function_header.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     HINT_CHARACTER_SET,
     HINT_COL_IDX,
     INPUT_OUTPUT_ROW_INCREMENT,
     MISSING_DETAIL,
     N_LAYOUT_COLS,
 )
 from pyvispr.extension.function import function_t
-from pyvispr.interface.window.messenger import CreateMessageCanal
+from pyvispr.runtime.backend import SCREEN_BACKEND
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class header_wgt_t(wdgt.QWidget):
     proxy_function: function_t | None
     actual_function: function_t | None
     #
@@ -240,26 +240,30 @@
         is_input: bool,
         /,
     ) -> None:
         """"""
         for col, element in enumerate(elements):
             detail = wdgt.QLineEdit(element)
             layout.addWidget(detail, row, col)
-            CreateMessageCanal(detail, "textEdited", self.BuildHeaderOutput)
+            SCREEN_BACKEND.CreateMessageCanal(
+                detail, "textEdited", self.BuildHeaderOutput
+            )
         if is_input:
             ii_input = wdgt.QCheckBox("")
             layout.addWidget(ii_input, row, N_LAYOUT_COLS - 2)
-            CreateMessageCanal(ii_input, "stateChanged", self.BuildHeaderOutput)
+            SCREEN_BACKEND.CreateMessageCanal(
+                ii_input, "stateChanged", self.BuildHeaderOutput
+            )
 
         remove_btn = wdgt.QPushButton("x")
         remove_btn.setStyleSheet("color:coral")
         width = remove_btn.fontMetrics().boundingRect("x").width() + 12
         remove_btn.setMaximumWidth(width)
         layout.addWidget(remove_btn, row, N_LAYOUT_COLS - 1)
-        CreateMessageCanal(
+        SCREEN_BACKEND.CreateMessageCanal(
             remove_btn,
             "clicked",
             lambda *args, **kwargs: self._RemoveParameter(remove_btn, is_input),
         )
 
     def _AddNewParameterButton(
         self, layout: wdgt.QGridLayout, row: int, is_input: bool, /
@@ -270,15 +274,15 @@
 
         layout.addWidget(new_btn, row, 0, 1, N_LAYOUT_COLS)
 
         if is_input:
             action = self._AddInputParameter
         else:
             action = self._AddOutputParameter
-        CreateMessageCanal(new_btn, "clicked", action)
+        SCREEN_BACKEND.CreateMessageCanal(new_btn, "clicked", action)
 
     def _AddInputParameter(self) -> None:
         """"""
         self._AddParameter(True)
 
     def _AddOutputParameter(self) -> None:
         """"""
@@ -383,16 +387,16 @@
     layout.addLayout(layout_btn)
     output.setLayout(layout)
 
     HeaderRetrievalInitialization()
     FinalHeaderTransmission_ = lambda *args, **kwargs: FinalHeaderTransmission(
         header_wgt, output
     )
-    CreateMessageCanal(cancel_btn, "clicked", output.close)
-    CreateMessageCanal(done_btn, "clicked", FinalHeaderTransmission_)
+    SCREEN_BACKEND.CreateMessageCanal(cancel_btn, "clicked", output.close)
+    SCREEN_BACKEND.CreateMessageCanal(done_btn, "clicked", FinalHeaderTransmission_)
 
     return output
 
 
 def _AddParameterHeader(
     layout: wdgt.QGridLayout, what: str, titles: h.Sequence[str], from_row: int, /
 ) -> None:
```

### Comparing `pyvispr-2024.3/pyvispr/interface/window/widget/list.py` & `pyvispr-2024.4/pyvispr/interface/window/widget/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 
 import PyQt6.QtWidgets as wdgt
 from PyQt6.QtCore import Qt as constant_e
 from pyvispr.constant.widget.list import COL_SIZE_PADDING
-from pyvispr.interface.window.messenger import CreateMessageCanal
+from pyvispr.runtime.backend import SCREEN_BACKEND
 
 
 @dtcl.dataclass(slots=True, repr=False, eq=False)
 class list_wgt_t(wdgt.QListWidget):
     filter_wgt: wdgt.QLineEdit = dtcl.field(init=False)
     element_name: dtcl.InitVar[str] = ""
 
@@ -46,15 +46,15 @@
         """"""
         wdgt.QListWidget.__init__(self)
         self.setSelectionMode(wdgt.QAbstractItemView.SelectionMode.NoSelection)
 
         self.filter_wgt = wdgt.QLineEdit()
         self.filter_wgt.setPlaceholderText(f"Filter {element_name}")
         self.filter_wgt.setClearButtonEnabled(True)
-        CreateMessageCanal(self.filter_wgt, "textEdited", self.Filter)
+        SCREEN_BACKEND.CreateMessageCanal(self.filter_wgt, "textEdited", self.Filter)
 
         self.Reload()
 
     def AddDisabledItem(self, text: str, /) -> None:
         """"""
         self.addItem(text)
         _DisableItem(self.item(self.count() - 1))
```

### Comparing `pyvispr-2024.3/pyvispr/interface/window/widget/list_file.py` & `pyvispr-2024.4/pyvispr/interface/window/widget/list_file.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/interface/window/widget/list_function.py` & `pyvispr-2024.4/pyvispr/interface/window/widget/list_function.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,18 +44,23 @@
     def ActualReload(self) -> None:
         """"""
         if self.module is None:
             self.AddDisabledItem("No Functions")
             return
 
         try:
-            functions = AllFunctions(self.module)
+            functions = AllFunctions(self.module, recursively=True)
         except RuntimeError:
             functions = ()
 
         if functions.__len__() == 0:
             self.AddDisabledItem("No Functions Found")
             return
 
         for function in functions:
-            self.addItem(function.name)
-            self.functions[function.name] = function
+            if "." in function.pypath:
+                _, rel_pypath = function.pypath.split(".", maxsplit=1)
+                display_name = f"{rel_pypath}.{function.name}"
+            else:
+                display_name = function.name
+            self.addItem(display_name)
+            self.functions[display_name] = function
```

### Comparing `pyvispr-2024.3/pyvispr/interface/window/widget/list_module.py` & `pyvispr-2024.4/pyvispr/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,19 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-import dataclasses as dtcl
-
-from logger_36.task.inspection import Modules
-from pyvispr.interface.window.widget.list import list_wgt_t
-
-
-@dtcl.dataclass(slots=True, repr=False, eq=False)
-class module_list_wgt_t(list_wgt_t):
-    def ActualReload(self) -> None:
-        """"""
-        for module in Modules(False, False, only_loaded=False):
-            self.addItem(module)
+__version__ = "2024.4"
```

### Comparing `pyvispr-2024.3/pyvispr/interface/window/widget/menu.py` & `pyvispr-2024.4/pyvispr/interface/window/widget/menu.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from typing import Callable
 
 import PyQt6.QtWidgets as wdgt
 from PyQt6.QtGui import QAction
-from pyvispr.interface.window.messenger import CreateMessageCanal
+from pyvispr.runtime.backend import SCREEN_BACKEND
 
 
 def AddEntryToMenu(
     menu: wdgt.QMenu,
     parent: wdgt.QWidget,
     text: str,
     action: Callable,
@@ -46,15 +46,15 @@
     disabled: bool = False,
     checkable: bool = False,
     checked: bool = False,
 ) -> None:
     """"""
     entry = QAction(text, parent=parent)
     if action is not None:
-        CreateMessageCanal(entry, "triggered", action)
+        SCREEN_BACKEND.CreateMessageCanal(entry, "triggered", action)
     if status_tip is not None:
         entry.setStatusTip(status_tip)
     if shortcut is not None:
         entry.setShortcut(shortcut)
     if disabled:
         entry.setEnabled(False)
     if checkable:
```

### Comparing `pyvispr-2024.3/pyvispr/run.py` & `pyvispr-2024.4/pyvispr/run.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/runtime/backend.py` & `pyvispr-2024.4/pyvispr/runtime/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/runtime/catalog.py` & `pyvispr-2024.4/pyvispr/runtime/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.3/pyvispr/runtime/messenger.py` & `pyvispr-2024.4/pyvispr/catalog/factory/image_256.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,15 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from pyvispr.flow.messenger import messenger_t
+import numpy
 
-MESSENGER = messenger_t()
+
+def pyVisprImage256() -> numpy.ndarray:
+    """
+    _outputs: image
+    """
+    return numpy.random.random_integers(0, high=255, size=(256, 256))
```

### Comparing `pyvispr-2024.3/pyvispr.egg-info/PKG-INFO` & `pyvispr-2024.4/pyvispr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.3
+Version: 2024.4
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyVispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyVispr/
@@ -21,14 +21,15 @@
 Requires-Dist: json_any
 Requires-Dist: logger_36
 Requires-Dist: numexpr
 Requires-Dist: numpy
 Requires-Dist: platformdirs
 Requires-Dist: PyQt6
 Requires-Dist: scikit-image
+Requires-Dist: sio-messenger
 Requires-Dist: str_to_obj
 
 ..
    Copyright CNRS/Inria/UniCA
    Contributor(s): Eric Debreuve (since 2017)
 
    eric.debreuve@cnrs.fr
```

### Comparing `pyvispr-2024.3/pyvispr.egg-info/SOURCES.txt` & `pyvispr-2024.4/pyvispr.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pyvispr.egg-info/dependency_links.txt
 pyvispr.egg-info/entry_points.txt
 pyvispr.egg-info/requires.txt
 pyvispr.egg-info/top_level.txt
 pyvispr/catalog/installer.py
 pyvispr/catalog/parser.py
 pyvispr/catalog/type.py
+pyvispr/catalog/factory/image_256.py
 pyvispr/catalog/factory/image_loader.py
 pyvispr/catalog/factory/image_viewer.py
 pyvispr/catalog/factory/numexpr_calculator.py
 pyvispr/catalog/factory/value.py
 pyvispr/catalog/factory/value_viewer.py
 pyvispr/config/path.py
 pyvispr/config/appearance/backend.py
@@ -37,15 +38,14 @@
 pyvispr/constant/widget/function_header.py
 pyvispr/constant/widget/list.py
 pyvispr/constant/widget/node.py
 pyvispr/extension/function.py
 pyvispr/extension/module.py
 pyvispr/extension/qt6.py
 pyvispr/extension/string_.py
-pyvispr/flow/messenger.py
 pyvispr/flow/descriptive/node.py
 pyvispr/flow/descriptive/socket.py
 pyvispr/flow/functional/graph.py
 pyvispr/flow/functional/link.py
 pyvispr/flow/functional/node_isolated.py
 pyvispr/flow/functional/node_linked.py
 pyvispr/flow/functional/socket.py
@@ -54,20 +54,18 @@
 pyvispr/flow/visual/link.py
 pyvispr/flow/visual/node.py
 pyvispr/flow/visual/socket.py
 pyvispr/flow/visual/whiteboard.py
 pyvispr/interface/storage/loading.py
 pyvispr/interface/storage/stowing.py
 pyvispr/interface/window/installer.py
-pyvispr/interface/window/messenger.py
 pyvispr/interface/window/runner.py
 pyvispr/interface/window/widget/function_header.py
 pyvispr/interface/window/widget/list.py
 pyvispr/interface/window/widget/list_file.py
 pyvispr/interface/window/widget/list_function.py
 pyvispr/interface/window/widget/list_module.py
 pyvispr/interface/window/widget/list_node.py
 pyvispr/interface/window/widget/menu.py
 pyvispr/runtime/backend.py
 pyvispr/runtime/catalog.py
-pyvispr/runtime/messenger.py
 pyvispr/runtime/socket.py
```

### Comparing `pyvispr-2024.3/setup.py` & `pyvispr-2024.4/setup.py`

 * *Files identical despite different names*

