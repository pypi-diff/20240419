# Comparing `tmp/rwmapeditor_exgcdwu-1.2.6.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.2.6.tar", last modified: Fri Apr 19 15:21:45 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.2.7.tar", last modified: Fri Apr 19 15:40:41 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.2.6.tar` & `rwmapeditor_exgcdwu-1.2.7.tar`

### file list

```diff
@@ -1,56 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.247768 rwmapeditor_exgcdwu-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44370 2024-04-19 15:21:45.247768 rwmapeditor_exgcdwu-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.243768 rwmapeditor_exgcdwu-1.2.6/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.243768 rwmapeditor_exgcdwu-1.2.6/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_case/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.243768 rwmapeditor_exgcdwu-1.2.6/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.243768 rwmapeditor_exgcdwu-1.2.6/rwmap/_object/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_object/_object_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_object/_object_one.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_object/_object_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_object/_object_pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.243768 rwmapeditor_exgcdwu-1.2.6/rwmap/_tile/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_tile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_tile/_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.247768 rwmapeditor_exgcdwu-1.2.6/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_util/_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_util/_list_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.247768 rwmapeditor_exgcdwu-1.2.6/rwmap/data/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/data/default_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.247768 rwmapeditor_exgcdwu-1.2.6/rwmap/data/tile_group_grid/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/data/tile_group_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/data/tile_group_grid/_tile_group_addlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/data/tile_group_grid/_tile_group_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/data/tile_group_grid/tile_group_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.247768 rwmapeditor_exgcdwu-1.2.6/rwmap/data/tobject_group_COP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/data/tobject_group_COP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.247768 rwmapeditor_exgcdwu-1.2.6/rwmap/other_data/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/rwmap/other_data/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:21:45.247768 rwmapeditor_exgcdwu-1.2.6/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44370 2024-04-19 15:21:45.000000 rwmapeditor_exgcdwu-1.2.6/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-19 15:21:45.000000 rwmapeditor_exgcdwu-1.2.6/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:21:45.000000 rwmapeditor_exgcdwu-1.2.6/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 15:21:45.000000 rwmapeditor_exgcdwu-1.2.6/rwmapeditor_exgcdwu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 15:21:45.000000 rwmapeditor_exgcdwu-1.2.6/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 15:21:45.247768 rwmapeditor_exgcdwu-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 15:21:41.000000 rwmapeditor_exgcdwu-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.629255 rwmapeditor_exgcdwu-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44370 2024-04-19 15:40:41.629255 rwmapeditor_exgcdwu-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.581255 rwmapeditor_exgcdwu-1.2.7/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.581255 rwmapeditor_exgcdwu-1.2.7/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.585255 rwmapeditor_exgcdwu-1.2.7/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.585255 rwmapeditor_exgcdwu-1.2.7/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_object/_object_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_object/_object_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_object/_object_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_object/_object_pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.585255 rwmapeditor_exgcdwu-1.2.7/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.585255 rwmapeditor_exgcdwu-1.2.7/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.585255 rwmapeditor_exgcdwu-1.2.7/rwmap/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/data/default_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.585255 rwmapeditor_exgcdwu-1.2.7/rwmap/data/tile_group_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/data/tile_group_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/data/tile_group_grid/_tile_group_addlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/data/tile_group_grid/_tile_group_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/data/tile_group_grid/tile_group_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.585255 rwmapeditor_exgcdwu-1.2.7/rwmap/data/tobject_group_COP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/data/tobject_group_COP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.589255 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.589255 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.617255 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/bridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/decoration.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/deepwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dirt_details.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/dust.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/fauna.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/fauna_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/fauna_highland.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/misc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sand_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/shallowwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/shortgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/units.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/water.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/decoration.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/misc.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.625255 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.629255 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Deep Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Dirt.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Dirt_Details.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Dust.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Ice.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Lava.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Long Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Mountain.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Sand.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Shallow Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Short Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Snow.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Stone.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/terrain/Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/maps/units.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/rwmap/other_data/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:40:41.629255 rwmapeditor_exgcdwu-1.2.7/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44370 2024-04-19 15:40:41.000000 rwmapeditor_exgcdwu-1.2.7/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13076 2024-04-19 15:40:41.000000 rwmapeditor_exgcdwu-1.2.7/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:40:41.000000 rwmapeditor_exgcdwu-1.2.7/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 15:40:41.000000 rwmapeditor_exgcdwu-1.2.7/rwmapeditor_exgcdwu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 15:40:41.000000 rwmapeditor_exgcdwu-1.2.7/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 15:40:41.629255 rwmapeditor_exgcdwu-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 15:40:35.000000 rwmapeditor_exgcdwu-1.2.7/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.2.6/LICENSE` & `rwmapeditor_exgcdwu-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/PKG-INFO` & `rwmapeditor_exgcdwu-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.2.6
+Version: 1.2.7
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rwmapeditor_exgcdwu-1.2.6/README.md` & `rwmapeditor_exgcdwu-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_case/_layer.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_case/_object.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_case/_object.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_case/_objectgroup.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_case/_tileset.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_core.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_frame/_coordinate.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_frame/_element_property.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_object/_object_one.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_object/_object_one.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_object/_object_pos.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_object/_object_pos.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_object/_object_pro.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_object/_object_pro.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_tile/_tile_group.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_tile/_tile_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.2.7/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.6/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.2.7/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.2.6
+Version: 1.2.7
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rwmapeditor_exgcdwu-1.2.6/setup.py` & `rwmapeditor_exgcdwu-1.2.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # setup.py
 
 import os
 from setuptools import setup, find_packages
 
-__version__ = '1.2.6'
+__version__ = '1.2.7'
 
 def read_file(file:str):
     with open(file) as file:
         return file.read()
 
 def readline_file(file:str):
     with open(file) as file:
         return file.readline()
 
+DATA_PREFIX_MAPS = 'other_data/maps/'
+
 setup(
     name = 'rwmapeditor_exgcdwu',
     version = __version__,
     author = 'exgcdwu',
     author_email = '1006605318@qq.com',
     license = read_file('LICENSE'),
     url = "https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-",
     long_description = read_file('README.md'),
     long_description_content_type = "text/markdown",
     packages = find_packages(exclude=["tests"]),
-    package_data={'rwmap': ['other_data/*.tsx', 'other_data/*.txt', 'other_data/bitmaps/*.png', 'other_data/ridges/*.tsx',
-                             'other_data/ridges/bitmaps/*.png', 'other_data/terrain/*.tsx', 
-                             'other_data/terrain/bitmaps/*.png']},
+    package_data={'rwmap': ['other_data/*.txt', DATA_PREFIX_MAPS + '*.tsx', DATA_PREFIX_MAPS + 'bitmaps/*.png',
+                             DATA_PREFIX_MAPS + 'ridges/*.tsx', DATA_PREFIX_MAPS + 'terrain/*.tsx']},
     python_requires = '>=3.0.0',
     install_requires = readline_file("./rwmap/other_data/requirements.txt")
 )
```

