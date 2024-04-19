# Comparing `tmp/skilleter_thingy-0.0.24.tar.gz` & `tmp/skilleter_thingy-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skilleter_thingy-0.0.24.tar", last modified: Mon Apr  8 08:46:04 2024, max compression
+gzip compressed data, was "skilleter_thingy-0.0.25.tar", last modified: Fri Apr 19 16:16:37 2024, max compression
```

## Comparing `skilleter_thingy-0.0.24.tar` & `skilleter_thingy-0.0.25.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-08 08:46:04.591760 skilleter_thingy-0.0.24/
--rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/LICENSE
--rw-r--r--   0 jms       (1000) jms       (1000)     5231 2024-04-08 08:46:04.587760 skilleter_thingy-0.0.24/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/README.md
--rw-rw-r--   0 jms       (1000) jms       (1000)     2868 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/pyproject.toml
--rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-04-08 08:46:04.591760 skilleter_thingy-0.0.24/setup.cfg
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-08 08:46:04.587760 skilleter_thingy-0.0.24/skilleter_thingy/
--rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/__init__.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/addpath.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    18614 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/aws.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/borger.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/colour.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1786 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/console_colours.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/dc_curses.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/dc_defaults.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/dc_util.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12268 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/dircolors.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/diskspacecheck.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2453 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/docker.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3359 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/docker_purge.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    19373 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/ffind.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4261 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/files.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2493 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/ggit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5876 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/ggrep.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    37887 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    35764 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git2.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5812 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_br.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4981 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_ca.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    10214 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_cleanup.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8225 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_co.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1892 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_common.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4630 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_hold.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3100 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_mr.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2696 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_parent.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    51276 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_review.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    13985 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_update.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3143 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_wt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11279 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gitcmp_helper.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6062 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gitlab.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8925 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gitprompt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5964 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gl.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    22040 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gphotosync.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4316 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/linecount.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/logger.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/moviemover.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4737 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/path.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3178 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/photodupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7823 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/phototidier.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/popup.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3565 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/process.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/py_audit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     9465 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/readable.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4620 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/remdir.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/rmdupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2639 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/rpylint.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12619 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/run.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    13849 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/s3_sync.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/splitpics.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/strreplace.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11348 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/sysmon.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    33712 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/tfm.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    19829 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/tfm_pane.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2993 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/tfparse.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/tidy.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2397 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/trimpath.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/window_rename.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/xchmod.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/yamlcheck.py
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-08 08:46:04.587760 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/
--rw-r--r--   0 jms       (1000) jms       (1000)     5231 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     2012 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/SOURCES.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/dependency_links.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/entry_points.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       76 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/requires.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       17 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/top_level.txt
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-19 16:16:37.918563 skilleter_thingy-0.0.25/
+-rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/LICENSE
+-rw-r--r--   0 jms       (1000) jms       (1000)     5231 2024-04-19 16:16:37.918563 skilleter_thingy-0.0.25/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/README.md
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2868 2024-04-19 16:16:08.000000 skilleter_thingy-0.0.25/pyproject.toml
+-rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-04-19 16:16:37.918563 skilleter_thingy-0.0.25/setup.cfg
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-19 16:16:37.918563 skilleter_thingy-0.0.25/skilleter_thingy/
+-rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/__init__.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/addpath.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/borger.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/colour.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1786 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/console_colours.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/dc_curses.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/dc_defaults.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/dc_util.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12268 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/dircolors.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/diskspacecheck.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2453 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/docker.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3359 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/docker_purge.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    19373 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/ffind.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4261 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/files.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2493 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/ggit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5876 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/ggrep.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    37887 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/git.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    35764 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/git2.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5812 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_br.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4981 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_ca.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    10214 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_cleanup.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8225 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_co.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1892 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_common.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4630 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_hold.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3100 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_mr.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2696 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_parent.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    51276 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_review.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    13985 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_update.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3143 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/git_wt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11279 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/gitcmp_helper.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6062 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/gitlab.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8925 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/gitprompt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5964 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/gl.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    22040 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/gphotosync.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     9120 2024-04-19 16:07:35.000000 skilleter_thingy-0.0.25/skilleter_thingy/imagedupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4316 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/linecount.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/logger.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/moviemover.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4737 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/path.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4195 2024-04-16 15:14:14.000000 skilleter_thingy-0.0.25/skilleter_thingy/photodupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7823 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/phototidier.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/popup.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3565 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/process.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/py_audit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     9465 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/readable.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4620 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/remdir.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/rmdupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2639 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/rpylint.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12619 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/run.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/splitpics.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/strreplace.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11348 2024-03-29 19:35:49.000000 skilleter_thingy-0.0.25/skilleter_thingy/sysmon.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    33712 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/tfm.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    19829 2024-03-06 19:42:35.000000 skilleter_thingy-0.0.25/skilleter_thingy/tfm_pane.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2993 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/tfparse.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/tidy.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2397 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/trimpath.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/window_rename.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-03-29 19:18:20.000000 skilleter_thingy-0.0.25/skilleter_thingy/xchmod.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-02-29 21:18:18.000000 skilleter_thingy-0.0.25/skilleter_thingy/yamlcheck.py
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-19 16:16:37.918563 skilleter_thingy-0.0.25/skilleter_thingy.egg-info/
+-rw-r--r--   0 jms       (1000) jms       (1000)     5231 2024-04-19 16:16:37.000000 skilleter_thingy-0.0.25/skilleter_thingy.egg-info/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1990 2024-04-19 16:16:37.000000 skilleter_thingy-0.0.25/skilleter_thingy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-04-19 16:16:37.000000 skilleter_thingy-0.0.25/skilleter_thingy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-04-19 16:16:37.000000 skilleter_thingy-0.0.25/skilleter_thingy.egg-info/entry_points.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       76 2024-04-19 16:16:37.000000 skilleter_thingy-0.0.25/skilleter_thingy.egg-info/requires.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       17 2024-04-19 16:16:37.000000 skilleter_thingy-0.0.25/skilleter_thingy.egg-info/top_level.txt
```

### Comparing `skilleter_thingy-0.0.24/LICENSE` & `skilleter_thingy-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/PKG-INFO` & `skilleter_thingy-0.0.25/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.24
+Version: 0.0.25
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: boto3
 Requires-Dist: imagehash
 Requires-Dist: inotify
 Requires-Dist: pillow
 Requires-Dist: psutil
 Requires-Dist: pyaml
 Requires-Dist: pygit2
 Requires-Dist: python-dateutil
 Requires-Dist: requests
+Requires-Dist: numpy
 
 # Thingy
 
 Licence: GPL v3
 
 Author: John Skilleter v0.99
```

### Comparing `skilleter_thingy-0.0.24/README.md` & `skilleter_thingy-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/pyproject.toml` & `skilleter_thingy-0.0.25/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skilleter_thingy"
 
 # Version must be incremented to install updated Thingy
 
-version = "0.0.24"
+version = "0.0.25"
 
 authors = [
     {name="John Skilleter", email="john@skilleter.org.uk"},
 ]
 
 description = "A collection of useful utilities, mainly aimed at making Git more friendly"
 
@@ -22,23 +22,23 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "boto3",
     "imagehash",
     "inotify",
     "pillow",
     "psutil",
     "pyaml",
     "pygit2",
     "python-dateutil",
     "requests",
+    "numpy",
 ]
 
 [project.urls]
 Home = "https://skilleter.org.uk"
 
 [project.scripts]
 addpath = "skilleter_thingy:addpath.addpath"
```

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/addpath.py` & `skilleter_thingy-0.0.25/skilleter_thingy/addpath.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/borger.py` & `skilleter_thingy-0.0.25/skilleter_thingy/borger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/colour.py` & `skilleter_thingy-0.0.25/skilleter_thingy/colour.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/console_colours.py` & `skilleter_thingy-0.0.25/skilleter_thingy/console_colours.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/dc_curses.py` & `skilleter_thingy-0.0.25/skilleter_thingy/dc_curses.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/dc_defaults.py` & `skilleter_thingy-0.0.25/skilleter_thingy/dc_defaults.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/dc_util.py` & `skilleter_thingy-0.0.25/skilleter_thingy/dc_util.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/dircolors.py` & `skilleter_thingy-0.0.25/skilleter_thingy/dircolors.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/diskspacecheck.py` & `skilleter_thingy-0.0.25/skilleter_thingy/diskspacecheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/docker.py` & `skilleter_thingy-0.0.25/skilleter_thingy/docker.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/docker_purge.py` & `skilleter_thingy-0.0.25/skilleter_thingy/docker_purge.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/ffind.py` & `skilleter_thingy-0.0.25/skilleter_thingy/ffind.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/files.py` & `skilleter_thingy-0.0.25/skilleter_thingy/files.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/ggit.py` & `skilleter_thingy-0.0.25/skilleter_thingy/ggit.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/ggrep.py` & `skilleter_thingy-0.0.25/skilleter_thingy/ggrep.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git2.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git2.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_br.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_br.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_ca.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_ca.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_cleanup.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_cleanup.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_co.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_co.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_common.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_common.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_hold.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_hold.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_mr.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_mr.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_parent.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_parent.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_review.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_review.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_update.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_update.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/git_wt.py` & `skilleter_thingy-0.0.25/skilleter_thingy/git_wt.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/gitcmp_helper.py` & `skilleter_thingy-0.0.25/skilleter_thingy/gitcmp_helper.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/gitlab.py` & `skilleter_thingy-0.0.25/skilleter_thingy/gitlab.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/gitprompt.py` & `skilleter_thingy-0.0.25/skilleter_thingy/gitprompt.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/gl.py` & `skilleter_thingy-0.0.25/skilleter_thingy/gl.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/gphotosync.py` & `skilleter_thingy-0.0.25/skilleter_thingy/gphotosync.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/linecount.py` & `skilleter_thingy-0.0.25/skilleter_thingy/linecount.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/logger.py` & `skilleter_thingy-0.0.25/skilleter_thingy/logger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/moviemover.py` & `skilleter_thingy-0.0.25/skilleter_thingy/moviemover.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/path.py` & `skilleter_thingy-0.0.25/skilleter_thingy/path.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/phototidier.py` & `skilleter_thingy-0.0.25/skilleter_thingy/phototidier.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/popup.py` & `skilleter_thingy-0.0.25/skilleter_thingy/popup.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/process.py` & `skilleter_thingy-0.0.25/skilleter_thingy/process.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/py_audit.py` & `skilleter_thingy-0.0.25/skilleter_thingy/py_audit.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/readable.py` & `skilleter_thingy-0.0.25/skilleter_thingy/readable.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/remdir.py` & `skilleter_thingy-0.0.25/skilleter_thingy/remdir.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/rmdupe.py` & `skilleter_thingy-0.0.25/skilleter_thingy/rmdupe.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/rpylint.py` & `skilleter_thingy-0.0.25/skilleter_thingy/rpylint.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/run.py` & `skilleter_thingy-0.0.25/skilleter_thingy/run.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/splitpics.py` & `skilleter_thingy-0.0.25/skilleter_thingy/splitpics.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/strreplace.py` & `skilleter_thingy-0.0.25/skilleter_thingy/strreplace.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/sysmon.py` & `skilleter_thingy-0.0.25/skilleter_thingy/sysmon.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/tfm.py` & `skilleter_thingy-0.0.25/skilleter_thingy/tfm.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/tfm_pane.py` & `skilleter_thingy-0.0.25/skilleter_thingy/tfm_pane.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/tfparse.py` & `skilleter_thingy-0.0.25/skilleter_thingy/tfparse.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/tidy.py` & `skilleter_thingy-0.0.25/skilleter_thingy/tidy.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/trimpath.py` & `skilleter_thingy-0.0.25/skilleter_thingy/trimpath.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/window_rename.py` & `skilleter_thingy-0.0.25/skilleter_thingy/window_rename.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/xchmod.py` & `skilleter_thingy-0.0.25/skilleter_thingy/xchmod.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy/yamlcheck.py` & `skilleter_thingy-0.0.25/skilleter_thingy/yamlcheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy.egg-info/PKG-INFO` & `skilleter_thingy-0.0.25/skilleter_thingy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.24
+Version: 0.0.25
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: boto3
 Requires-Dist: imagehash
 Requires-Dist: inotify
 Requires-Dist: pillow
 Requires-Dist: psutil
 Requires-Dist: pyaml
 Requires-Dist: pygit2
 Requires-Dist: python-dateutil
 Requires-Dist: requests
+Requires-Dist: numpy
 
 # Thingy
 
 Licence: GPL v3
 
 Author: John Skilleter v0.99
```

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy.egg-info/SOURCES.txt` & `skilleter_thingy-0.0.25/skilleter_thingy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 skilleter_thingy/__init__.py
 skilleter_thingy/addpath.py
-skilleter_thingy/aws.py
 skilleter_thingy/borger.py
 skilleter_thingy/colour.py
 skilleter_thingy/console_colours.py
 skilleter_thingy/dc_curses.py
 skilleter_thingy/dc_defaults.py
 skilleter_thingy/dc_util.py
 skilleter_thingy/dircolors.py
@@ -32,29 +31,29 @@
 skilleter_thingy/git_update.py
 skilleter_thingy/git_wt.py
 skilleter_thingy/gitcmp_helper.py
 skilleter_thingy/gitlab.py
 skilleter_thingy/gitprompt.py
 skilleter_thingy/gl.py
 skilleter_thingy/gphotosync.py
+skilleter_thingy/imagedupe.py
 skilleter_thingy/linecount.py
 skilleter_thingy/logger.py
 skilleter_thingy/moviemover.py
 skilleter_thingy/path.py
 skilleter_thingy/photodupe.py
 skilleter_thingy/phototidier.py
 skilleter_thingy/popup.py
 skilleter_thingy/process.py
 skilleter_thingy/py_audit.py
 skilleter_thingy/readable.py
 skilleter_thingy/remdir.py
 skilleter_thingy/rmdupe.py
 skilleter_thingy/rpylint.py
 skilleter_thingy/run.py
-skilleter_thingy/s3_sync.py
 skilleter_thingy/splitpics.py
 skilleter_thingy/strreplace.py
 skilleter_thingy/sysmon.py
 skilleter_thingy/tfm.py
 skilleter_thingy/tfm_pane.py
 skilleter_thingy/tfparse.py
 skilleter_thingy/tidy.py
```

### Comparing `skilleter_thingy-0.0.24/skilleter_thingy.egg-info/entry_points.txt` & `skilleter_thingy-0.0.25/skilleter_thingy.egg-info/entry_points.txt`

 * *Files identical despite different names*

