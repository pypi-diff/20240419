# Comparing `tmp/bumpify-0.0.0.tar.gz` & `tmp/bumpify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpify-0.0.0.tar", max compression
+gzip compressed data, was "bumpify-0.0.2.tar", max compression
```

## Comparing `bumpify-0.0.0.tar` & `bumpify-0.0.2.tar`

### file list

```diff
@@ -1,62 +1,61 @@
--rw-r--r--   0        0        0     1072 2024-03-12 16:35:44.434151 bumpify-0.0.0/LICENSE
--rw-r--r--   0        0        0     4152 2024-04-19 16:30:54.413708 bumpify-0.0.0/README.md
--rw-r--r--   0        0        0       22 2024-04-19 16:14:15.338478 bumpify-0.0.0/bumpify/__init__.py
--rw-r--r--   0        0        0      624 2024-04-18 16:41:01.326312 bumpify-0.0.0/bumpify/context.py
--rw-r--r--   0        0        0        0 2024-03-07 19:29:11.075522 bumpify-0.0.0/bumpify/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 15:35:26.965369 bumpify-0.0.0/bumpify/core/api/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-18 17:07:34.068733 bumpify-0.0.0/bumpify/core/api/commands.py
--rw-r--r--   0        0        0     2597 2024-04-15 16:10:38.830468 bumpify-0.0.0/bumpify/core/api/interface.py
--rw-r--r--   0        0        0     1744 2024-04-16 19:23:13.577027 bumpify-0.0.0/bumpify/core/api/presenters.py
--rw-r--r--   0        0        0     4078 2024-04-18 17:07:34.176743 bumpify-0.0.0/bumpify/core/api/providers.py
--rw-r--r--   0        0        0        0 2024-03-10 07:53:20.475774 bumpify-0.0.0/bumpify/core/config/__init__.py
--rw-r--r--   0        0        0     2538 2024-04-04 17:37:20.529014 bumpify-0.0.0/bumpify/core/config/exc.py
--rw-r--r--   0        0        0      513 2024-04-04 16:53:29.562462 bumpify-0.0.0/bumpify/core/config/helpers.py
--rw-r--r--   0        0        0     2450 2024-04-06 12:30:22.576021 bumpify-0.0.0/bumpify/core/config/implementation.py
--rw-r--r--   0        0        0     1506 2024-04-04 16:42:36.994003 bumpify-0.0.0/bumpify/core/config/interface.py
--rw-r--r--   0        0        0     4797 2024-04-18 17:07:34.024729 bumpify-0.0.0/bumpify/core/config/objects.py
--rw-r--r--   0        0        0        0 2024-04-15 16:10:38.830468 bumpify-0.0.0/bumpify/core/console/__init__.py
--rw-r--r--   0        0        0      746 2024-04-18 16:54:52.753336 bumpify-0.0.0/bumpify/core/console/_message_formatter.py
--rw-r--r--   0        0        0     2956 2024-04-17 17:54:34.015362 bumpify-0.0.0/bumpify/core/console/helpers.py
--rw-r--r--   0        0        0      660 2024-04-16 18:58:25.634553 bumpify-0.0.0/bumpify/core/console/input.py
--rw-r--r--   0        0        0     1793 2024-04-17 17:47:33.454580 bumpify-0.0.0/bumpify/core/console/interface.py
--rw-r--r--   0        0        0      702 2024-04-16 15:25:37.521149 bumpify-0.0.0/bumpify/core/console/objects.py
--rw-r--r--   0        0        0     1003 2024-04-17 17:52:10.960873 bumpify-0.0.0/bumpify/core/console/output.py
--rw-r--r--   0        0        0        0 2023-08-30 15:49:08.797200 bumpify-0.0.0/bumpify/core/filesystem/__init__.py
--rw-r--r--   0        0        0      668 2024-04-07 18:08:58.080512 bumpify-0.0.0/bumpify/core/filesystem/exc.py
--rw-r--r--   0        0        0     2388 2024-03-25 17:52:31.631528 bumpify-0.0.0/bumpify/core/filesystem/helpers.py
--rw-r--r--   0        0        0     4671 2024-04-18 16:50:41.897612 bumpify-0.0.0/bumpify/core/filesystem/implementation.py
--rw-r--r--   0        0        0     2805 2024-04-07 18:53:30.425676 bumpify-0.0.0/bumpify/core/filesystem/interface.py
--rw-r--r--   0        0        0        0 2024-03-23 19:27:28.167843 bumpify-0.0.0/bumpify/core/semver/__init__.py
--rw-r--r--   0        0        0     1473 2024-03-26 19:30:36.317811 bumpify-0.0.0/bumpify/core/semver/_changelog_formatters.py
--rw-r--r--   0        0        0      680 2024-03-23 19:32:54.226807 bumpify-0.0.0/bumpify/core/semver/_constants.py
--rw-r--r--   0        0        0     3821 2024-03-23 19:36:47.079301 bumpify-0.0.0/bumpify/core/semver/_parsing.py
--rw-r--r--   0        0        0     2735 2024-04-04 15:23:46.154973 bumpify-0.0.0/bumpify/core/semver/_version_file_updater.py
--rw-r--r--   0        0        0      964 2024-04-03 19:51:35.840854 bumpify-0.0.0/bumpify/core/semver/exc.py
--rw-r--r--   0        0        0     1600 2024-04-18 17:07:33.916720 bumpify-0.0.0/bumpify/core/semver/helpers.py
--rw-r--r--   0        0        0     4444 2024-04-18 17:07:34.108737 bumpify-0.0.0/bumpify/core/semver/implementation.py
--rw-r--r--   0        0        0     3107 2024-04-18 17:07:34.092735 bumpify-0.0.0/bumpify/core/semver/interface.py
--rw-r--r--   0        0        0    18959 2024-04-15 16:10:38.830468 bumpify-0.0.0/bumpify/core/semver/objects.py
--rw-r--r--   0        0        0        0 2024-03-12 19:03:24.995488 bumpify-0.0.0/bumpify/core/vcs/__init__.py
--rw-r--r--   0        0        0     1483 2024-03-21 19:38:29.688251 bumpify-0.0.0/bumpify/core/vcs/exc.py
--rw-r--r--   0        0        0     1610 2024-03-24 20:46:26.798825 bumpify-0.0.0/bumpify/core/vcs/helpers.py
--rw-r--r--   0        0        0        0 2024-03-12 19:18:55.540853 bumpify-0.0.0/bumpify/core/vcs/implementation/__init__.py
--rw-r--r--   0        0        0     7973 2024-03-21 19:38:30.112265 bumpify-0.0.0/bumpify/core/vcs/implementation/git.py
--rw-r--r--   0        0        0     2044 2024-04-16 19:23:14.025036 bumpify-0.0.0/bumpify/core/vcs/implementation/proxy.py
--rw-r--r--   0        0        0     4049 2024-03-18 17:30:16.765852 bumpify-0.0.0/bumpify/core/vcs/interface.py
--rw-r--r--   0        0        0     1226 2024-03-12 19:10:09.856784 bumpify-0.0.0/bumpify/core/vcs/objects.py
--rw-r--r--   0        0        0        0 2024-04-07 07:11:14.841930 bumpify-0.0.0/bumpify/delivery/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 07:11:27.278214 bumpify-0.0.0/bumpify/delivery/cli/__init__.py
--rw-r--r--   0        0        0     3015 2024-04-18 17:30:25.387453 bumpify-0.0.0/bumpify/delivery/cli/__main__.py
--rw-r--r--   0        0        0      723 2024-04-18 14:14:09.999993 bumpify-0.0.0/bumpify/delivery/cli/decorators.py
--rw-r--r--   0        0        0      575 2024-04-18 13:53:18.885824 bumpify-0.0.0/bumpify/di/__init__.py
--rw-r--r--   0        0        0     1931 2024-04-18 13:51:03.604807 bumpify-0.0.0/bumpify/di/api.py
--rw-r--r--   0        0        0     1060 2024-04-18 13:51:03.604807 bumpify-0.0.0/bumpify/di/config.py
--rw-r--r--   0        0        0      485 2024-04-18 14:07:57.195797 bumpify-0.0.0/bumpify/di/console.py
--rw-r--r--   0        0        0     1079 2024-04-18 17:07:34.120738 bumpify-0.0.0/bumpify/di/filesystem.py
--rw-r--r--   0        0        0     1091 2024-04-18 13:51:03.604807 bumpify-0.0.0/bumpify/di/semver.py
--rw-r--r--   0        0        0     1226 2024-04-18 17:14:35.654238 bumpify-0.0.0/bumpify/di/vcs.py
--rw-r--r--   0        0        0     2921 2024-03-11 17:52:51.041959 bumpify-0.0.0/bumpify/exc.py
--rw-r--r--   0        0        0     5579 2024-04-08 15:20:57.639432 bumpify-0.0.0/bumpify/utils.py
--rw-r--r--   0        0        0      947 2024-04-19 16:39:44.368317 bumpify-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     5512 1970-01-01 00:00:00.000000 bumpify-0.0.0/setup.py
--rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 bumpify-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-19 18:05:09.732730 bumpify-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4152 2024-04-19 18:05:09.732730 bumpify-0.0.2/README.md
+-rw-r--r--   0        0        0       22 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/__init__.py
+-rw-r--r--   0        0        0      624 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/context.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/core/api/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/core/api/commands.py
+-rw-r--r--   0        0        0     2597 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/core/api/interface.py
+-rw-r--r--   0        0        0     1744 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/core/api/presenters.py
+-rw-r--r--   0        0        0     4078 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/core/api/providers.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/core/config/__init__.py
+-rw-r--r--   0        0        0     2538 2024-04-19 18:05:09.732730 bumpify-0.0.2/bumpify/core/config/exc.py
+-rw-r--r--   0        0        0      513 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/config/helpers.py
+-rw-r--r--   0        0        0     2450 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/config/implementation.py
+-rw-r--r--   0        0        0     1506 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/config/interface.py
+-rw-r--r--   0        0        0     4797 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/config/objects.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/console/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/console/_message_formatter.py
+-rw-r--r--   0        0        0     2956 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/console/helpers.py
+-rw-r--r--   0        0        0      660 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/console/input.py
+-rw-r--r--   0        0        0     1793 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/console/interface.py
+-rw-r--r--   0        0        0      702 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/console/objects.py
+-rw-r--r--   0        0        0     1003 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/console/output.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/filesystem/__init__.py
+-rw-r--r--   0        0        0      668 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/filesystem/exc.py
+-rw-r--r--   0        0        0     2388 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/filesystem/helpers.py
+-rw-r--r--   0        0        0     4671 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/filesystem/implementation.py
+-rw-r--r--   0        0        0     2805 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/filesystem/interface.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/_changelog_formatters.py
+-rw-r--r--   0        0        0      680 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/_constants.py
+-rw-r--r--   0        0        0     3821 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/_parsing.py
+-rw-r--r--   0        0        0     2735 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/_version_file_updater.py
+-rw-r--r--   0        0        0      964 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/exc.py
+-rw-r--r--   0        0        0     1600 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/helpers.py
+-rw-r--r--   0        0        0     4444 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/implementation.py
+-rw-r--r--   0        0        0     3107 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/interface.py
+-rw-r--r--   0        0        0    18959 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/semver/objects.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/vcs/__init__.py
+-rw-r--r--   0        0        0     1483 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/vcs/exc.py
+-rw-r--r--   0        0        0     1610 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/vcs/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/vcs/implementation/__init__.py
+-rw-r--r--   0        0        0     7973 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/vcs/implementation/git.py
+-rw-r--r--   0        0        0     2044 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/vcs/implementation/proxy.py
+-rw-r--r--   0        0        0     4049 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/vcs/interface.py
+-rw-r--r--   0        0        0     1226 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/core/vcs/objects.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/delivery/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/delivery/cli/__init__.py
+-rw-r--r--   0        0        0     3029 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/delivery/cli/__main__.py
+-rw-r--r--   0        0        0      723 2024-04-19 18:05:09.736730 bumpify-0.0.2/bumpify/delivery/cli/decorators.py
+-rw-r--r--   0        0        0      575 2024-04-19 18:05:09.740730 bumpify-0.0.2/bumpify/di/__init__.py
+-rw-r--r--   0        0        0     1931 2024-04-19 18:05:09.740730 bumpify-0.0.2/bumpify/di/api.py
+-rw-r--r--   0        0        0     1060 2024-04-19 18:05:09.740730 bumpify-0.0.2/bumpify/di/config.py
+-rw-r--r--   0        0        0      485 2024-04-19 18:05:09.740730 bumpify-0.0.2/bumpify/di/console.py
+-rw-r--r--   0        0        0     1079 2024-04-19 18:05:09.740730 bumpify-0.0.2/bumpify/di/filesystem.py
+-rw-r--r--   0        0        0     1091 2024-04-19 18:05:09.740730 bumpify-0.0.2/bumpify/di/semver.py
+-rw-r--r--   0        0        0     1212 2024-04-19 18:05:09.740730 bumpify-0.0.2/bumpify/di/vcs.py
+-rw-r--r--   0        0        0     2921 2024-04-19 18:05:09.740730 bumpify-0.0.2/bumpify/exc.py
+-rw-r--r--   0        0        0     5579 2024-04-19 18:05:09.740730 bumpify-0.0.2/bumpify/utils.py
+-rw-r--r--   0        0        0      947 2024-04-19 18:05:09.740730 bumpify-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 bumpify-0.0.2/PKG-INFO
```

### Comparing `bumpify-0.0.0/LICENSE` & `bumpify-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/README.md` & `bumpify-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/context.py` & `bumpify-0.0.2/bumpify/context.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/api/commands.py` & `bumpify-0.0.2/bumpify/core/api/commands.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/api/interface.py` & `bumpify-0.0.2/bumpify/core/api/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/api/presenters.py` & `bumpify-0.0.2/bumpify/core/api/presenters.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/api/providers.py` & `bumpify-0.0.2/bumpify/core/api/providers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/config/exc.py` & `bumpify-0.0.2/bumpify/core/config/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/config/helpers.py` & `bumpify-0.0.2/bumpify/core/config/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/config/implementation.py` & `bumpify-0.0.2/bumpify/core/config/implementation.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/config/interface.py` & `bumpify-0.0.2/bumpify/core/config/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/config/objects.py` & `bumpify-0.0.2/bumpify/core/config/objects.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/console/_message_formatter.py` & `bumpify-0.0.2/bumpify/core/console/_message_formatter.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/console/helpers.py` & `bumpify-0.0.2/bumpify/core/console/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/console/input.py` & `bumpify-0.0.2/bumpify/core/console/input.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/console/interface.py` & `bumpify-0.0.2/bumpify/core/console/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/console/objects.py` & `bumpify-0.0.2/bumpify/core/console/objects.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/console/output.py` & `bumpify-0.0.2/bumpify/core/console/output.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/filesystem/exc.py` & `bumpify-0.0.2/bumpify/core/filesystem/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/filesystem/helpers.py` & `bumpify-0.0.2/bumpify/core/filesystem/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/filesystem/implementation.py` & `bumpify-0.0.2/bumpify/core/filesystem/implementation.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/filesystem/interface.py` & `bumpify-0.0.2/bumpify/core/filesystem/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/semver/_changelog_formatters.py` & `bumpify-0.0.2/bumpify/core/semver/_changelog_formatters.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/semver/_constants.py` & `bumpify-0.0.2/bumpify/core/semver/_constants.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/semver/_parsing.py` & `bumpify-0.0.2/bumpify/core/semver/_parsing.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/semver/_version_file_updater.py` & `bumpify-0.0.2/bumpify/core/semver/_version_file_updater.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/semver/exc.py` & `bumpify-0.0.2/bumpify/core/semver/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/semver/helpers.py` & `bumpify-0.0.2/bumpify/core/semver/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/semver/implementation.py` & `bumpify-0.0.2/bumpify/core/semver/implementation.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/semver/interface.py` & `bumpify-0.0.2/bumpify/core/semver/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/semver/objects.py` & `bumpify-0.0.2/bumpify/core/semver/objects.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/vcs/exc.py` & `bumpify-0.0.2/bumpify/core/vcs/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/vcs/helpers.py` & `bumpify-0.0.2/bumpify/core/vcs/helpers.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/vcs/implementation/git.py` & `bumpify-0.0.2/bumpify/core/vcs/implementation/git.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/vcs/implementation/proxy.py` & `bumpify-0.0.2/bumpify/core/vcs/implementation/proxy.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/vcs/interface.py` & `bumpify-0.0.2/bumpify/core/vcs/interface.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/core/vcs/objects.py` & `bumpify-0.0.2/bumpify/core/vcs/objects.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/delivery/cli/__main__.py` & `bumpify-0.0.2/bumpify/delivery/cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import click
 from click_help_colors import HelpColorsGroup
 from pydio.api import Injector
 from pydio.base import IInjector
 
-from bumpify import utils, __version__
+from bumpify import __version__, utils
 from bumpify.core.api.interface import IBumpCommand, IInitCommand
 from bumpify.di import provider
 
 from .decorators import catch_errors
 
 
 @click.group(
@@ -62,26 +62,26 @@
     ctx.obj = ctx.with_resource(injector)
 
 
 @bumpify.command()
 @click.pass_obj
 @catch_errors
 def init(injector: IInjector):
-    """Create initial configuration file interactively."""
+    """Initialize Bumpify for the current project."""
     command = utils.inject_type(injector, IInitCommand)
     provider = utils.inject_type(injector, IInitCommand.IInitProvider)
     presenter = utils.inject_type(injector, IInitCommand.IInitPresenter)
     command.init(provider, presenter)
 
 
 @bumpify.command()
 @click.pass_obj
 @catch_errors
 def bump(injector: IInjector):
-    """Bump project's version.
+    """Create new release of the current project.
 
     This command analyzes severity of recent changes and based on that
     determines which version component should be bumped. Once new version is
     calculated, the command then updates version and changelog files, and makes
     a bump commit, which finally is tagged with a newly calculated version tag.
     """
     command = utils.inject_type(injector, IBumpCommand)
```

### Comparing `bumpify-0.0.0/bumpify/delivery/cli/decorators.py` & `bumpify-0.0.2/bumpify/delivery/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/di/__init__.py` & `bumpify-0.0.2/bumpify/di/__init__.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/di/api.py` & `bumpify-0.0.2/bumpify/di/api.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/di/config.py` & `bumpify-0.0.2/bumpify/di/config.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/di/filesystem.py` & `bumpify-0.0.2/bumpify/di/filesystem.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/di/semver.py` & `bumpify-0.0.2/bumpify/di/semver.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/di/vcs.py` & `bumpify-0.0.2/bumpify/di/vcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,13 @@
     return GitVcsConnector(filesystem_reader)
 
 
 @provider.provides(IVcsReaderWriter)
 def make_vcs_reader_writer(injector):
     context = utils.inject_context(injector)
     config = utils.inject_type(injector, Config)
-    connector = utils.inject_variant(
-        injector, IVcsConnector, what=config.vcs.type
-    )
+    connector = utils.inject_variant(injector, IVcsConnector, what=config.vcs.type)
     obj = connector.connect()
     if not context.dry_run:
         return obj
     cout = utils.inject_type(injector, IConsoleOutput)
     return DryRunVcsReaderWriterProxy(obj, cout)
```

### Comparing `bumpify-0.0.0/bumpify/exc.py` & `bumpify-0.0.2/bumpify/exc.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/bumpify/utils.py` & `bumpify-0.0.2/bumpify/utils.py`

 * *Files identical despite different names*

### Comparing `bumpify-0.0.0/pyproject.toml` & `bumpify-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bumpify"
-version = "0.0.0"
+version = "0.0.2"
 description = "Semantic versioning automation tool for software projects"
 authors = ["Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mwiatrzyk/bumpify"
 keywords = ["semantic", "versioning", "cli", "tool"]
 classifiers = [
```

### Comparing `bumpify-0.0.0/PKG-INFO` & `bumpify-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpify
-Version: 0.0.0
+Version: 0.0.2
 Summary: Semantic versioning automation tool for software projects
 Home-page: https://github.com/mwiatrzyk/bumpify
 License: MIT
 Keywords: semantic,versioning,cli,tool
 Author: Maciej Wiatrzyk
 Author-email: maciej.wiatrzyk@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -12,14 +12,15 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: click-help-colors (>=0.9.4,<0.10.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pydio (>=0.4.1,<0.5.0)
 Requires-Dist: tomlkit (>=0.12.4,<0.13.0)
```

