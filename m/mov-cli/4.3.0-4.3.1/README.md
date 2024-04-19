# Comparing `tmp/mov-cli-4.3.0.tar.gz` & `tmp/mov_cli-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-4.3.0.tar", last modified: Tue Apr  9 23:40:37 2024, max compression
+gzip compressed data, was "mov_cli-4.3.1.tar", last modified: Fri Apr 19 01:33:24 2024, max compression
```

## Comparing `mov-cli-4.3.0.tar` & `mov_cli-4.3.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.279852 mov-cli-4.3.0/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.269852 mov-cli-4.3.0/.github/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.269852 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/addprovider.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/dependabot.yml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.269852 mov-cli-4.3.0/.github/workflows/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.github/workflows/pypi.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov-cli-4.3.0/.github/workflows/ruff.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov-cli-4.3.0/.gitignore
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov-cli-4.3.0/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)      291 2024-04-04 00:43:21.000000 mov-cli-4.3.0/Makefile
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7713 2024-04-09 23:40:37.279852 mov-cli-4.3.0/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5059 2024-04-08 23:54:10.000000 mov-cli-4.3.0/README.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-08 22:18:54.000000 mov-cli-4.3.0/disclaimer.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.273186 mov-cli-4.3.0/mov_cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-08 22:17:33.000000 mov-cli-4.3.0/mov_cli/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/cli/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5589 2024-04-09 23:28:23.000000 mov-cli-4.3.0/mov_cli/cli/__main__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/auto_select.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/configuration.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/episode.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2938 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/play.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1926 2024-04-09 23:06:10.000000 mov-cli-4.3.0/mov_cli/cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4079 2024-04-09 22:27:43.000000 mov-cli-4.3.0/mov_cli/cli/scraper.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1248 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/search.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6423 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/ui.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-09 22:18:23.000000 mov-cli-4.3.0/mov_cli/cli/watch_options.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6913 2024-04-08 23:54:12.000000 mov-cli-4.3.0/mov_cli/config.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      583 2024-04-08 23:54:12.000000 mov-cli-4.3.0/mov_cli/config.template.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1032 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/download.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      942 2024-04-04 00:48:22.000000 mov-cli-4.3.0/mov_cli/errors.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/http_client.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/iterfzf/
--rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov-cli-4.3.0/mov_cli/iterfzf/LICENSE.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/logger.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/media/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/media/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2158 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/media/media.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-09 23:14:07.000000 mov-cli-4.3.0/mov_cli/media/metadata.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/players/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       89 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/players/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/players/custom_player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2556 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/players/mpv.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/players/player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2319 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/players/vlc.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1369 2024-04-08 23:54:12.000000 mov-cli-4.3.0/mov_cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2093 2024-04-09 22:52:58.000000 mov-cli-4.3.0/mov_cli/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.276519 mov-cli-4.3.0/mov_cli/utils/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov-cli-4.3.0/mov_cli/utils/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov-cli-4.3.0/mov_cli/utils/episode_selector.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov-cli-4.3.0/mov_cli/utils/platform.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.279852 mov-cli-4.3.0/mov_cli/utils/scraper/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-08 22:18:54.000000 mov-cli-4.3.0/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3383 2024-04-09 22:26:17.000000 mov-cli-4.3.0/mov_cli/utils/version.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.279852 mov-cli-4.3.0/mov_cli.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7713 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1406 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      215 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-09 23:40:37.000000 mov-cli-4.3.0/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1733 2024-04-08 23:54:10.000000 mov-cli-4.3.0/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov-cli-4.3.0/ruff.toml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-09 23:40:37.279852 mov-cli-4.3.0/scripts/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov-cli-4.3.0/scripts/test_cli.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-09 23:40:37.279852 mov-cli-4.3.0/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.820418 mov_cli-4.3.1/.github/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.820418 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/addprovider.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/dependabot.yml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.823751 mov_cli-4.3.1/.github/workflows/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.github/workflows/pypi.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.3.1/.github/workflows/ruff.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.3.1/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.3.1/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      291 2024-04-04 00:43:21.000000 mov_cli-4.3.1/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-19 01:33:24.830417 mov_cli-4.3.1/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-04-19 00:17:22.000000 mov_cli-4.3.1/README.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-08 22:18:54.000000 mov_cli-4.3.1/disclaimer.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.823751 mov_cli-4.3.1/mov_cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-19 01:33:09.000000 mov_cli-4.3.1/mov_cli/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.827084 mov_cli-4.3.1/mov_cli/cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5589 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/__main__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/auto_select.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2089 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/configuration.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/episode.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2938 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/play.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1926 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4079 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1248 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/search.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6423 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/ui.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/cli/watch_options.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6913 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/config.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      583 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/config.template.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1032 2024-04-08 22:18:54.000000 mov_cli-4.3.1/mov_cli/download.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      942 2024-04-04 00:48:22.000000 mov_cli-4.3.1/mov_cli/errors.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/http_client.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.827084 mov_cli-4.3.1/mov_cli/iterfzf/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.3.1/mov_cli/iterfzf/LICENSE.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/logger.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.827084 mov_cli-4.3.1/mov_cli/media/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/media/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2793 2024-04-19 00:26:10.000000 mov_cli-4.3.1/mov_cli/media/media.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1859 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/media/metadata.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/mov_cli/players/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       89 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/players/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/players/custom_player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2813 2024-04-19 00:37:22.000000 mov_cli-4.3.1/mov_cli/players/mpv.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/players/player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2519 2024-04-19 01:17:33.000000 mov_cli-4.3.1/mov_cli/players/vlc.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1369 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2093 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/mov_cli/utils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.3.1/mov_cli/utils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.3.1/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.3.1/mov_cli/utils/platform.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/mov_cli/utils/scraper/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-08 22:18:54.000000 mov_cli-4.3.1/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-08 22:18:54.000000 mov_cli-4.3.1/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3383 2024-04-19 00:17:22.000000 mov_cli-4.3.1/mov_cli/utils/version.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/mov_cli.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7990 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1406 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      215 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-19 01:33:24.000000 mov_cli-4.3.1/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1733 2024-04-08 23:54:10.000000 mov_cli-4.3.1/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.3.1/ruff.toml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-19 01:33:24.830417 mov_cli-4.3.1/scripts/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.3.1/scripts/test_cli.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-19 01:33:24.830417 mov_cli-4.3.1/setup.cfg
```

### Comparing `mov-cli-4.3.0/.github/ISSUE_TEMPLATE/bug-report.md` & `mov_cli-4.3.1/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/.github/workflows/pypi.yml` & `mov_cli-4.3.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/.github/workflows/ruff.yml` & `mov_cli-4.3.1/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/LICENSE` & `mov_cli-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/PKG-INFO` & `mov_cli-4.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.0
+Version: 4.3.1
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,15 +56,15 @@
 Requires-Dist: build; extra == "dev"
 Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
 
 <a name="readme-top"></a>
 
 [![Stargazers][stars-shield]][stars-url]
 [![Pypi Version][pypi-shield]][pypi-url]
-[![Pypi Downloads][pypi-dl-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-stats-url]
 [![Python Versions][python-shield]][pypi-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 
 
 <div align="center">
 
@@ -97,15 +97,15 @@
 > For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
 
 ### Prerequisites
 - **A supported platform:**
   - Linux
   - Windows
   - Android (via [Termux](https://termux.dev/en/))
-  - iOS (via [iSH Shell](https://ish.app/))
+  - *iOS (via [iSH Shell](https://ish.app/))* (unstable, https://github.com/mov-cli/mov-cli/issues/256)
   - MacOS
 - **[python](https://www.python.org/downloads/)** (**required**, with pip)
 - **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
 - **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
 - **[mpv](https://mpv.io/installation/)** (recommended & default media player)
 
 To get running these are all the prerequisites you'll need.
@@ -138,34 +138,37 @@
 ```sh
 mov-cli -s youtube flight 370
 ```
 <img src="https://github.com/mov-cli/mov-cli/assets/132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118">
 
 > The command above searches for `flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube) plugin, **however once again mov-cli is plugin based and there are many of them [in the wild](https://github.com/topics/mov-cli-plugin). 😉**
 
+## Star Graph ⭐
+[![Star Graph Chart](https://api.star-history.com/svg?repos=mov-cli/mov-cli&type=Date)](https://star-history.com/#mov-cli/mov-cli&Date)
+
 ## Contributing ✨
 Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
 
 <a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
   <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
 </a>
 
 ## Inspiration 🌟
 Inspired by [ani-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/animdl)
 
-
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-cli.svg?style=for-the-badge
 [contributors-url]: https://github.com/mov-cli/mov-cli/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/mov-cli/mov-cli.svg?style=for-the-badge
 [forks-url]: https://github.com/mov-cli/mov-cli/network/members
 [stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli?style=flat
 [stars-url]: https://github.com/mov-cli/mov-cli/stargazers
 [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/
+[pypi-stats-url]: https://pypistats.org/packages/mov-cli
 [python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
 [issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
 [issues-url]: https://github.com/mov-cli/mov-cli/issues
 [license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
 [license-url]: ./LICENSE
 [pypi-dl-shield]: https://img.shields.io/pypi/dm/mov-cli?color=informational&label=pypi%20downloads
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.0 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.1 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -29,30 +29,31 @@
 httpx Requires-Dist: importlib-metadata; python_version < "3.8" Requires-Dist:
 toml Requires-Dist: devgoldyutils>=2.5.7 Requires-Dist: typer>=0.12.2 Requires-
 Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode Requires-
 Dist: deprecation Requires-Dist: packaging Requires-Dist: mov-cli-test>=1.1.0
 Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: build;
 extra == "dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev" [!
 [Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-url]
-[![Pypi Downloads][pypi-dl-shield]][pypi-url] [![Python Versions][python-
+[![Pypi Downloads][pypi-dl-shield]][pypi-stats-url] [![Python Versions][python-
 shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
 [license-shield]][license-url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
 plugins up to date**. Also I would advise not using it as a library yet as the
 API still has many breaking changes. ## Installation ð ï¸ > [!TIP] > For in-
 depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-
 cli/wiki/Installation). ### Prerequisites - **A supported platform:** - Linux -
-Windows - Android (via [Termux](https://termux.dev/en/)) - iOS (via [iSH Shell]
-(https://ish.app/)) - MacOS - **[python](https://www.python.org/downloads/)**
+Windows - Android (via [Termux](https://termux.dev/en/)) - *iOS (via [iSH
+Shell](https://ish.app/))* (unstable, https://github.com/mov-cli/mov-cli/
+issues/256) - MacOS - **[python](https://www.python.org/downloads/)**
 (**required**, with pip) - **[lxml](https://pypi.org/project/lxml/)**
 (optional, â¡ faster scraping) - **[fzf](https://github.com/junegunn/
 fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**) -
 **[mpv](https://mpv.io/installation/)** (recommended & default media player) To
 get running these are all the prerequisites you'll need. With the prerequisites
 installed, mov-cli can be installed via the pip command on all platforms with
 Python version 3.8 or above. ```sh pip install mov-cli -U ``` > Check out the
@@ -70,27 +71,29 @@
 you may also edit by manually opening the config file. See this [Wiki page]
 (https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.
 ```toml [mov-cli.plugins] youtube = "mov-cli-youtube" ``` 2. Scrape away! ```sh
 mov-cli -s youtube flight 370 ``` [https://github.com/mov-cli/mov-cli/assets/
 132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118]> The command above searches for
 `flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube)
 plugin, **however once again mov-cli is plugin based and there are many of them
-[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Contributing
+[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Star Graph
+â­ [![Star Graph Chart](https://api.star-history.com/svg?repos=mov-cli/mov-
+cli&type=Date)](https://star-history.com/#mov-cli/mov-cli&Date) ## Contributing
 â¨ Pull requests are welcome and *appreciated*. For major changes, please open
 an issue first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-
 cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/
 justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/
 animdl) [contributors-shield]: https://img.shields.io/github/contributors/mov-
 cli/mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-
 cli/mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
 forks/mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/
 mov-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
 stars/mov-cli/mov-cli?style=flat [stars-url]: https://github.com/mov-cli/mov-
 cli/stargazers [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
-[pypi-url]: https://pypi.org/project/mov-cli/ [python-shield]: https://
-img.shields.io/pypi/pyversions/mov-cli?style=flat [issues-shield]: https://
-img.shields.io/github/issues/mov-cli/mov-cli?style=flat [issues-url]: https://
-github.com/mov-cli/mov-cli/issues [license-shield]: https://img.shields.io/
-github/license/mov-cli/mov-cli?style=flat [license-url]: ./LICENSE [pypi-dl-
-shield]: https://img.shields.io/pypi/dm/mov-
-cli?color=informational&label=pypi%20downloads
+[pypi-url]: https://pypi.org/project/mov-cli/ [pypi-stats-url]: https://
+pypistats.org/packages/mov-cli [python-shield]: https://img.shields.io/pypi/
+pyversions/mov-cli?style=flat [issues-shield]: https://img.shields.io/github/
+issues/mov-cli/mov-cli?style=flat [issues-url]: https://github.com/mov-cli/mov-
+cli/issues [license-shield]: https://img.shields.io/github/license/mov-cli/mov-
+cli?style=flat [license-url]: ./LICENSE [pypi-dl-shield]: https://
+img.shields.io/pypi/dm/mov-cli?color=informational&label=pypi%20downloads
```

### Comparing `mov-cli-4.3.0/README.md` & `mov_cli-4.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <a name="readme-top"></a>
 
 [![Stargazers][stars-shield]][stars-url]
 [![Pypi Version][pypi-shield]][pypi-url]
-[![Pypi Downloads][pypi-dl-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-stats-url]
 [![Python Versions][python-shield]][pypi-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 
 
 <div align="center">
 
@@ -39,15 +39,15 @@
 > For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
 
 ### Prerequisites
 - **A supported platform:**
   - Linux
   - Windows
   - Android (via [Termux](https://termux.dev/en/))
-  - iOS (via [iSH Shell](https://ish.app/))
+  - *iOS (via [iSH Shell](https://ish.app/))* (unstable, https://github.com/mov-cli/mov-cli/issues/256)
   - MacOS
 - **[python](https://www.python.org/downloads/)** (**required**, with pip)
 - **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
 - **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
 - **[mpv](https://mpv.io/installation/)** (recommended & default media player)
 
 To get running these are all the prerequisites you'll need.
@@ -80,34 +80,37 @@
 ```sh
 mov-cli -s youtube flight 370
 ```
 <img src="https://github.com/mov-cli/mov-cli/assets/132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118">
 
 > The command above searches for `flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube) plugin, **however once again mov-cli is plugin based and there are many of them [in the wild](https://github.com/topics/mov-cli-plugin). 😉**
 
+## Star Graph ⭐
+[![Star Graph Chart](https://api.star-history.com/svg?repos=mov-cli/mov-cli&type=Date)](https://star-history.com/#mov-cli/mov-cli&Date)
+
 ## Contributing ✨
 Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
 
 <a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
   <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
 </a>
 
 ## Inspiration 🌟
 Inspired by [ani-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/animdl)
 
-
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-cli.svg?style=for-the-badge
 [contributors-url]: https://github.com/mov-cli/mov-cli/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/mov-cli/mov-cli.svg?style=for-the-badge
 [forks-url]: https://github.com/mov-cli/mov-cli/network/members
 [stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli?style=flat
 [stars-url]: https://github.com/mov-cli/mov-cli/stargazers
 [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/
+[pypi-stats-url]: https://pypistats.org/packages/mov-cli
 [python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
 [issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
 [issues-url]: https://github.com/mov-cli/mov-cli/issues
 [license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
 [license-url]: ./LICENSE
 [pypi-dl-shield]: https://img.shields.io/pypi/dm/mov-cli?color=informational&label=pypi%20downloads
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
 [![Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-
-url] [![Pypi Downloads][pypi-dl-shield]][pypi-url] [![Python Versions][python-
-shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
-[license-shield]][license-url]
+url] [![Pypi Downloads][pypi-dl-shield]][pypi-stats-url] [![Python Versions]
+[python-shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT
+License][license-shield]][license-url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
 plugins up to date**. Also I would advise not using it as a library yet as the
 API still has many breaking changes. ## Installation ð ï¸ > [!TIP] > For in-
 depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-
 cli/wiki/Installation). ### Prerequisites - **A supported platform:** - Linux -
-Windows - Android (via [Termux](https://termux.dev/en/)) - iOS (via [iSH Shell]
-(https://ish.app/)) - MacOS - **[python](https://www.python.org/downloads/)**
+Windows - Android (via [Termux](https://termux.dev/en/)) - *iOS (via [iSH
+Shell](https://ish.app/))* (unstable, https://github.com/mov-cli/mov-cli/
+issues/256) - MacOS - **[python](https://www.python.org/downloads/)**
 (**required**, with pip) - **[lxml](https://pypi.org/project/lxml/)**
 (optional, â¡ faster scraping) - **[fzf](https://github.com/junegunn/
 fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**) -
 **[mpv](https://mpv.io/installation/)** (recommended & default media player) To
 get running these are all the prerequisites you'll need. With the prerequisites
 installed, mov-cli can be installed via the pip command on all platforms with
 Python version 3.8 or above. ```sh pip install mov-cli -U ``` > Check out the
@@ -36,27 +37,29 @@
 you may also edit by manually opening the config file. See this [Wiki page]
 (https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.
 ```toml [mov-cli.plugins] youtube = "mov-cli-youtube" ``` 2. Scrape away! ```sh
 mov-cli -s youtube flight 370 ``` [https://github.com/mov-cli/mov-cli/assets/
 132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118]> The command above searches for
 `flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube)
 plugin, **however once again mov-cli is plugin based and there are many of them
-[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Contributing
+[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Star Graph
+â­ [![Star Graph Chart](https://api.star-history.com/svg?repos=mov-cli/mov-
+cli&type=Date)](https://star-history.com/#mov-cli/mov-cli&Date) ## Contributing
 â¨ Pull requests are welcome and *appreciated*. For major changes, please open
 an issue first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-
 cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/
 justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/
 animdl) [contributors-shield]: https://img.shields.io/github/contributors/mov-
 cli/mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-
 cli/mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
 forks/mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/
 mov-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
 stars/mov-cli/mov-cli?style=flat [stars-url]: https://github.com/mov-cli/mov-
 cli/stargazers [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
-[pypi-url]: https://pypi.org/project/mov-cli/ [python-shield]: https://
-img.shields.io/pypi/pyversions/mov-cli?style=flat [issues-shield]: https://
-img.shields.io/github/issues/mov-cli/mov-cli?style=flat [issues-url]: https://
-github.com/mov-cli/mov-cli/issues [license-shield]: https://img.shields.io/
-github/license/mov-cli/mov-cli?style=flat [license-url]: ./LICENSE [pypi-dl-
-shield]: https://img.shields.io/pypi/dm/mov-
-cli?color=informational&label=pypi%20downloads
+[pypi-url]: https://pypi.org/project/mov-cli/ [pypi-stats-url]: https://
+pypistats.org/packages/mov-cli [python-shield]: https://img.shields.io/pypi/
+pyversions/mov-cli?style=flat [issues-shield]: https://img.shields.io/github/
+issues/mov-cli/mov-cli?style=flat [issues-url]: https://github.com/mov-cli/mov-
+cli/issues [license-shield]: https://img.shields.io/github/license/mov-cli/mov-
+cli?style=flat [license-url]: ./LICENSE [pypi-dl-shield]: https://
+img.shields.io/pypi/dm/mov-cli?color=informational&label=pypi%20downloads
```

### Comparing `mov-cli-4.3.0/disclaimer.md` & `mov_cli-4.3.1/disclaimer.md`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/cli/__main__.py` & `mov_cli-4.3.1/mov_cli/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/cli/configuration.py` & `mov_cli-4.3.1/mov_cli/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/cli/episode.py` & `mov_cli-4.3.1/mov_cli/cli/episode.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/cli/play.py` & `mov_cli-4.3.1/mov_cli/cli/play.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/cli/plugins.py` & `mov_cli-4.3.1/mov_cli/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/cli/scraper.py` & `mov_cli-4.3.1/mov_cli/cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/cli/search.py` & `mov_cli-4.3.1/mov_cli/cli/search.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/cli/ui.py` & `mov_cli-4.3.1/mov_cli/cli/ui.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/cli/watch_options.py` & `mov_cli-4.3.1/mov_cli/cli/watch_options.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/config.py` & `mov_cli-4.3.1/mov_cli/config.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/config.template.toml` & `mov_cli-4.3.1/mov_cli/config.template.toml`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/download.py` & `mov_cli-4.3.1/mov_cli/download.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/errors.py` & `mov_cli-4.3.1/mov_cli/errors.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/http_client.py` & `mov_cli-4.3.1/mov_cli/http_client.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/iterfzf/LICENSE.txt` & `mov_cli-4.3.1/mov_cli/iterfzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/iterfzf/__init__.py` & `mov_cli-4.3.1/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/media/media.py` & `mov_cli-4.3.1/mov_cli/media/media.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,19 +13,27 @@
     "Single", 
     "Movie", 
     "Series"
 )
 
 class Media():
     """Represents any piece of media in mov-cli that can be streamed or downloaded."""
-    def __init__(self, url: str, title: str, referrer: Optional[str]) -> None:
+    def __init__(
+        self, 
+        url: str, 
+        title: str, 
+        audio_url: Optional[str], 
+        referrer: Optional[str]
+    ) -> None:
         self.url = url
-        """The stream-able url."""
+        """The stream-able url of the media."""
         self.title = title
         """A title to represent this stream-able media."""
+        self.audio_url = audio_url
+        """The stream-able url that provides audio for the media if the main url doesn't stream with audio."""
         self.referrer = referrer
         """The required referrer for streaming the media content."""
 
     @property
     @abstractmethod
     def display_name(self) -> str:
         """The title that should be displayed by the player."""
@@ -34,47 +42,57 @@
 class Multi(Media):
     """Represents a media that has multiple episodes like a TV Series, Anime or Cartoon."""
     def __init__(
         self, 
         url: str, 
         title: str, 
         episode: EpisodeSelector, 
+        audio_url: Optional[str] = None, 
         referrer: Optional[str] = None, 
         subtitles: Optional[dict] = None
     ) -> None:
         self.episode = episode
         """The episode and season of this series."""
         self.subtitles = subtitles
 
         super().__init__(
-            url, title, referrer
+            url, 
+            title = title, 
+            audio_url = audio_url, 
+            referrer = referrer
         )
 
     @property
     def display_name(self) -> str:
         return f"{self.title} - S{self.episode.season} EP{self.episode.episode}"
 
 class Single(Media):
     """Represents a media with a single episode, like a Film/Movie or a YouTube video."""
     def __init__(
         self, 
-        url: str,
-        title: str,
-        referrer: Optional[str] = None,
-        year: Optional[str] = None,
-        subtitles: Optional[dict] = None
+        url: str, 
+        title: str, 
+        audio_url: Optional[str] = None, 
+        referrer: Optional[str] = None, 
+        year: Optional[str] = None, 
+        subtitles: Optional[dict] = None 
     ) -> None:
         self.year = year
         """The year this film was released."""
         self.subtitles = subtitles
 
         super().__init__(
-            url, title, referrer
+            url, 
+            title = title, 
+            audio_url = audio_url, 
+            referrer = referrer
         )
 
     @property
     def display_name(self) -> str:
         return f"{self.title} ({self.year})"
 
 # Backwards compatibility for post v4.3.0 extensions.
 Series = Multi
-Movie = Single
+"""DEPRECATED!!! USE 'Multi' INSTEAD! This will be removed after v4.4."""
+Movie = Single
+"""DEPRECATED!!! USE 'Single' INSTEAD! This will be removed after v4.4."""
```

### Comparing `mov-cli-4.3.0/mov_cli/media/metadata.py` & `mov_cli-4.3.1/mov_cli/media/metadata.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/players/custom_player.py` & `mov_cli-4.3.1/mov_cli/players/custom_player.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/players/mpv.py` & `mov_cli-4.3.1/mov_cli/players/mpv.py`

 * *Files 24% similar despite different names*

```diff
@@ -52,14 +52,17 @@
                     f"--force-media-title={media.display_name}",
                     "--no-terminal",
                 ]
 
                 if media.referrer is not None:
                     args.append(f"--referrer={media.referrer}")
 
+                if media.audio_url is not None:
+                    args.append(f"--audio-file={media.audio_url}")
+
                 if self.config.resolution:
                     args.append(f"--hls-bitrate={self.config.resolution}") # NOTE: This only works when the file is a m3u8
 
                 return subprocess.Popen(args)
 
             elif self.platform == "Darwin":
                 args = [
@@ -69,16 +72,19 @@
                     media.url,
                     f"--mpv-force-media-title={media.display_name}",
                 ]
 
                 if media.referrer is not None:
                     args.append(f"--mpv-referrer={media.referrer}")
 
+                if media.audio_url is not None:
+                    args.append(f"--mpv-audio-file={media.audio_url}")
+
                 if self.config.resolution:
                     args.append(f"--mpv-hls-bitrate={self.config.resolution}") # NOTE: This only works when the file is a m3u8
 
                 return subprocess.Popen(args)
 
-        except ModuleNotFoundError:
+        except (ModuleNotFoundError, FileNotFoundError):
             raise errors.PlayerNotFound(self)
 
         return None
```

### Comparing `mov-cli-4.3.0/mov_cli/players/player.py` & `mov_cli-4.3.1/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/players/vlc.py` & `mov_cli-4.3.1/mov_cli/players/vlc.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,22 +56,26 @@
             return None
 
         elif self.platform == "Linux" or self.platform == "Windows":
             try:
                 args = [
                     "vlc", 
                     f'--meta-title="{media.display_name}"', 
-                    media.url
+                    media.url, 
+                    "--quiet"
                 ]
 
                 if media.referrer is not None:
                     args.append(f'--http-referrer="{media.referrer}"')
 
+                if media.audio_url is not None:
+                    args.append(f"--input-slave={media.audio_url}") # WHY IS THIS UNDOCUMENTED!!!
+
                 if self.config.resolution:
                     args.append(f"--adaptive-maxwidth={self.config.resolution}") # NOTE: I don't really know if that works ~ Ananas
 
                 return subprocess.Popen(args)
 
-            except ModuleNotFoundError:
+            except (ModuleNotFoundError, FileNotFoundError):
                 raise errors.PlayerNotFound(self)
 
         return None
```

### Comparing `mov-cli-4.3.0/mov_cli/plugins.py` & `mov_cli-4.3.1/mov_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/scraper.py` & `mov_cli-4.3.1/mov_cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/utils/episode_selector.py` & `mov_cli-4.3.1/mov_cli/utils/episode_selector.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/utils/platform.py` & `mov_cli-4.3.1/mov_cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/utils/scraper/the_movie_db.py` & `mov_cli-4.3.1/mov_cli/utils/scraper/the_movie_db.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli/utils/version.py` & `mov_cli-4.3.1/mov_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/mov_cli.egg-info/PKG-INFO` & `mov_cli-4.3.1/mov_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.3.0
+Version: 4.3.1
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,15 +56,15 @@
 Requires-Dist: build; extra == "dev"
 Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
 
 <a name="readme-top"></a>
 
 [![Stargazers][stars-shield]][stars-url]
 [![Pypi Version][pypi-shield]][pypi-url]
-[![Pypi Downloads][pypi-dl-shield]][pypi-url]
+[![Pypi Downloads][pypi-dl-shield]][pypi-stats-url]
 [![Python Versions][python-shield]][pypi-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 
 
 <div align="center">
 
@@ -97,15 +97,15 @@
 > For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
 
 ### Prerequisites
 - **A supported platform:**
   - Linux
   - Windows
   - Android (via [Termux](https://termux.dev/en/))
-  - iOS (via [iSH Shell](https://ish.app/))
+  - *iOS (via [iSH Shell](https://ish.app/))* (unstable, https://github.com/mov-cli/mov-cli/issues/256)
   - MacOS
 - **[python](https://www.python.org/downloads/)** (**required**, with pip)
 - **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
 - **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
 - **[mpv](https://mpv.io/installation/)** (recommended & default media player)
 
 To get running these are all the prerequisites you'll need.
@@ -138,34 +138,37 @@
 ```sh
 mov-cli -s youtube flight 370
 ```
 <img src="https://github.com/mov-cli/mov-cli/assets/132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118">
 
 > The command above searches for `flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube) plugin, **however once again mov-cli is plugin based and there are many of them [in the wild](https://github.com/topics/mov-cli-plugin). 😉**
 
+## Star Graph ⭐
+[![Star Graph Chart](https://api.star-history.com/svg?repos=mov-cli/mov-cli&type=Date)](https://star-history.com/#mov-cli/mov-cli&Date)
+
 ## Contributing ✨
 Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
 
 <a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
   <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
 </a>
 
 ## Inspiration 🌟
 Inspired by [ani-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/animdl)
 
-
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-cli.svg?style=for-the-badge
 [contributors-url]: https://github.com/mov-cli/mov-cli/graphs/contributors
 [forks-shield]: https://img.shields.io/github/forks/mov-cli/mov-cli.svg?style=for-the-badge
 [forks-url]: https://github.com/mov-cli/mov-cli/network/members
 [stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli?style=flat
 [stars-url]: https://github.com/mov-cli/mov-cli/stargazers
 [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/
+[pypi-stats-url]: https://pypistats.org/packages/mov-cli
 [python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
 [issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
 [issues-url]: https://github.com/mov-cli/mov-cli/issues
 [license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
 [license-url]: ./LICENSE
 [pypi-dl-shield]: https://img.shields.io/pypi/dm/mov-cli?color=informational&label=pypi%20downloads
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.3.0 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.3.1 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -29,30 +29,31 @@
 httpx Requires-Dist: importlib-metadata; python_version < "3.8" Requires-Dist:
 toml Requires-Dist: devgoldyutils>=2.5.7 Requires-Dist: typer>=0.12.2 Requires-
 Dist: inquirer Requires-Dist: beautifulsoup4 Requires-Dist: Unidecode Requires-
 Dist: deprecation Requires-Dist: packaging Requires-Dist: mov-cli-test>=1.1.0
 Provides-Extra: dev Requires-Dist: ruff; extra == "dev" Requires-Dist: build;
 extra == "dev" Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev" [!
 [Stargazers][stars-shield]][stars-url] [![Pypi Version][pypi-shield]][pypi-url]
-[![Pypi Downloads][pypi-dl-shield]][pypi-url] [![Python Versions][python-
+[![Pypi Downloads][pypi-dl-shield]][pypi-stats-url] [![Python Versions][python-
 shield]][pypi-url] [![Issues][issues-shield]][issues-url] [![MIT License]
 [license-shield]][license-url]
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
 plugins up to date**. Also I would advise not using it as a library yet as the
 API still has many breaking changes. ## Installation ð ï¸ > [!TIP] > For in-
 depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-
 cli/wiki/Installation). ### Prerequisites - **A supported platform:** - Linux -
-Windows - Android (via [Termux](https://termux.dev/en/)) - iOS (via [iSH Shell]
-(https://ish.app/)) - MacOS - **[python](https://www.python.org/downloads/)**
+Windows - Android (via [Termux](https://termux.dev/en/)) - *iOS (via [iSH
+Shell](https://ish.app/))* (unstable, https://github.com/mov-cli/mov-cli/
+issues/256) - MacOS - **[python](https://www.python.org/downloads/)**
 (**required**, with pip) - **[lxml](https://pypi.org/project/lxml/)**
 (optional, â¡ faster scraping) - **[fzf](https://github.com/junegunn/
 fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**) -
 **[mpv](https://mpv.io/installation/)** (recommended & default media player) To
 get running these are all the prerequisites you'll need. With the prerequisites
 installed, mov-cli can be installed via the pip command on all platforms with
 Python version 3.8 or above. ```sh pip install mov-cli -U ``` > Check out the
@@ -70,27 +71,29 @@
 you may also edit by manually opening the config file. See this [Wiki page]
 (https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.
 ```toml [mov-cli.plugins] youtube = "mov-cli-youtube" ``` 2. Scrape away! ```sh
 mov-cli -s youtube flight 370 ``` [https://github.com/mov-cli/mov-cli/assets/
 132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118]> The command above searches for
 `flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube)
 plugin, **however once again mov-cli is plugin based and there are many of them
-[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Contributing
+[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Star Graph
+â­ [![Star Graph Chart](https://api.star-history.com/svg?repos=mov-cli/mov-
+cli&type=Date)](https://star-history.com/#mov-cli/mov-cli&Date) ## Contributing
 â¨ Pull requests are welcome and *appreciated*. For major changes, please open
 an issue first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/
 _c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-
 cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/
 justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/
 animdl) [contributors-shield]: https://img.shields.io/github/contributors/mov-
 cli/mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-
 cli/mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
 forks/mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/
 mov-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
 stars/mov-cli/mov-cli?style=flat [stars-url]: https://github.com/mov-cli/mov-
 cli/stargazers [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
-[pypi-url]: https://pypi.org/project/mov-cli/ [python-shield]: https://
-img.shields.io/pypi/pyversions/mov-cli?style=flat [issues-shield]: https://
-img.shields.io/github/issues/mov-cli/mov-cli?style=flat [issues-url]: https://
-github.com/mov-cli/mov-cli/issues [license-shield]: https://img.shields.io/
-github/license/mov-cli/mov-cli?style=flat [license-url]: ./LICENSE [pypi-dl-
-shield]: https://img.shields.io/pypi/dm/mov-
-cli?color=informational&label=pypi%20downloads
+[pypi-url]: https://pypi.org/project/mov-cli/ [pypi-stats-url]: https://
+pypistats.org/packages/mov-cli [python-shield]: https://img.shields.io/pypi/
+pyversions/mov-cli?style=flat [issues-shield]: https://img.shields.io/github/
+issues/mov-cli/mov-cli?style=flat [issues-url]: https://github.com/mov-cli/mov-
+cli/issues [license-shield]: https://img.shields.io/github/license/mov-cli/mov-
+cli?style=flat [license-url]: ./LICENSE [pypi-dl-shield]: https://
+img.shields.io/pypi/dm/mov-cli?color=informational&label=pypi%20downloads
```

### Comparing `mov-cli-4.3.0/mov_cli.egg-info/SOURCES.txt` & `mov_cli-4.3.1/mov_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mov-cli-4.3.0/pyproject.toml` & `mov_cli-4.3.1/pyproject.toml`

 * *Files identical despite different names*

