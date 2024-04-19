# Comparing `tmp/moodle_dl-2.3.6.tar.gz` & `tmp/moodle_dl-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moodle_dl-2.3.6.tar", last modified: Tue Apr 16 21:17:40 2024, max compression
+gzip compressed data, was "moodle_dl-2.3.7.tar", last modified: Fri Apr 19 12:09:25 2024, max compression
```

## Comparing `moodle_dl-2.3.6.tar` & `moodle_dl-2.3.7.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.608058 moodle_dl-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-16 21:17:40.608058 moodle_dl-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.596058 moodle_dl-2.3.6/moodle_dl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.596058 moodle_dl-2.3.6/moodle_dl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27074 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/cli/config_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/cli/database_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/cli/moodle_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/cli/notifications_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27774 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.600058 moodle_dl-2.3.6/moodle_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/download_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.600058 moodle_dl-2.3.6/moodle_dl/downloader/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/extractors/echo360.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/extractors/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/extractors/helixmedia_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/extractors/kalvidres_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/extractors/opencast_lti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/extractors/owncloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/extractors/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/extractors/sharepointfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/fake_download_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    41242 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/downloader/task.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17840 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.600058 moodle_dl-2.3.6/moodle_dl/moodle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/cookie_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/core_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.604058 moodle_dl-2.3.6/moodle_dl/moodle/mods/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/book.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/forum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/lesson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/quiz.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/mods/workshop.py
--rw-r--r--   0 runner    (1001) docker     (127)    30307 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/moodle_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/moodle_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/request_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/moodle/result_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.604058 moodle_dl-2.3.6/moodle_dl/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.604058 moodle_dl-2.3.6/moodle_dl/notifications/console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/console/console_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.604058 moodle_dl-2.3.6/moodle_dl/notifications/discord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/discord/discord_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/discord/discord_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/discord/discord_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.608058 moodle_dl-2.3.6/moodle_dl/notifications/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/mail/header.png
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/mail/header_extender.png
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/mail/mail_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/mail/mail_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/mail/mail_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/notification_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.608058 moodle_dl-2.3.6/moodle_dl/notifications/telegram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/telegram/telegram_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/telegram/telegram_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/telegram/telegram_shooter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.608058 moodle_dl-2.3.6/moodle_dl/notifications/xmpp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/xmpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/xmpp/xmpp_formater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/xmpp/xmpp_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/notifications/xmpp/xmpp_shooter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    54399 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/moodle_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:17:40.608058 moodle_dl-2.3.6/moodle_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-16 21:17:40.000000 moodle_dl-2.3.6/moodle_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-16 21:17:40.000000 moodle_dl-2.3.6/moodle_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:17:40.000000 moodle_dl-2.3.6/moodle_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 21:17:40.000000 moodle_dl-2.3.6/moodle_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:17:40.000000 moodle_dl-2.3.6/moodle_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 21:17:40.000000 moodle_dl-2.3.6/moodle_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 21:17:40.000000 moodle_dl-2.3.6/moodle_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:17:40.608058 moodle_dl-2.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-16 21:17:31.000000 moodle_dl-2.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.122037 moodle_dl-2.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-19 12:09:25.122037 moodle_dl-2.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.110037 moodle_dl-2.3.7/moodle_dl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.110037 moodle_dl-2.3.7/moodle_dl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27074 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/cli/config_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/cli/database_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/cli/moodle_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/cli/notifications_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27774 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.110037 moodle_dl-2.3.7/moodle_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/download_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.114037 moodle_dl-2.3.7/moodle_dl/downloader/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/extractors/echo360.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/extractors/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/extractors/helixmedia_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/extractors/kalvidres_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/extractors/opencast_lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/extractors/owncloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/extractors/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/extractors/sharepointfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/fake_download_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41242 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/downloader/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17840 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.114037 moodle_dl-2.3.7/moodle_dl/moodle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/cookie_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/core_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.118037 moodle_dl-2.3.7/moodle_dl/moodle/mods/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/book.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/forum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/lesson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/quiz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/mods/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30746 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/moodle_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/moodle_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/request_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/moodle/result_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.118037 moodle_dl-2.3.7/moodle_dl/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.118037 moodle_dl-2.3.7/moodle_dl/notifications/console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/console/console_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.118037 moodle_dl-2.3.7/moodle_dl/notifications/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/discord/discord_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/discord/discord_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/discord/discord_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.118037 moodle_dl-2.3.7/moodle_dl/notifications/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36960 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/mail/header.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/mail/header_extender.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/mail/mail_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/mail/mail_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/mail/mail_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/notification_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.118037 moodle_dl-2.3.7/moodle_dl/notifications/telegram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/telegram/telegram_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/telegram/telegram_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/telegram/telegram_shooter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.122037 moodle_dl-2.3.7/moodle_dl/notifications/xmpp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/xmpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/xmpp/xmpp_formater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/xmpp/xmpp_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/notifications/xmpp/xmpp_shooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54399 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/moodle_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:09:25.122037 moodle_dl-2.3.7/moodle_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-04-19 12:09:25.000000 moodle_dl-2.3.7/moodle_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-19 12:09:25.000000 moodle_dl-2.3.7/moodle_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:09:25.000000 moodle_dl-2.3.7/moodle_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 12:09:25.000000 moodle_dl-2.3.7/moodle_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:09:25.000000 moodle_dl-2.3.7/moodle_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 12:09:25.000000 moodle_dl-2.3.7/moodle_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 12:09:25.000000 moodle_dl-2.3.7/moodle_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 12:09:25.122037 moodle_dl-2.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-19 12:09:17.000000 moodle_dl-2.3.7/setup.py
```

### Comparing `moodle_dl-2.3.6/LICENSE` & `moodle_dl-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/PKG-INFO` & `moodle_dl-2.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.6
+Version: 2.3.7
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle_dl-2.3.6/README.md` & `moodle_dl-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/cli/__init__.py` & `moodle_dl-2.3.7/moodle_dl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/cli/config_wizard.py` & `moodle_dl-2.3.7/moodle_dl/cli/config_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/cli/database_manager.py` & `moodle_dl-2.3.7/moodle_dl/cli/database_manager.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/cli/moodle_wizard.py` & `moodle_dl-2.3.7/moodle_dl/cli/moodle_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/cli/notifications_wizard.py` & `moodle_dl-2.3.7/moodle_dl/cli/notifications_wizard.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/config.py` & `moodle_dl-2.3.7/moodle_dl/config.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/database.py` & `moodle_dl-2.3.7/moodle_dl/database.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/download_service.py` & `moodle_dl-2.3.7/moodle_dl/downloader/download_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/extractors/__init__.py` & `moodle_dl-2.3.7/moodle_dl/downloader/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/extractors/echo360.py` & `moodle_dl-2.3.7/moodle_dl/downloader/extractors/echo360.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/extractors/googledrive.py` & `moodle_dl-2.3.7/moodle_dl/downloader/extractors/googledrive.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/extractors/helixmedia_lti.py` & `moodle_dl-2.3.7/moodle_dl/downloader/extractors/helixmedia_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/extractors/kalvidres_lti.py` & `moodle_dl-2.3.7/moodle_dl/downloader/extractors/kalvidres_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/extractors/opencast_lti.py` & `moodle_dl-2.3.7/moodle_dl/downloader/extractors/opencast_lti.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/extractors/owncloud.py` & `moodle_dl-2.3.7/moodle_dl/downloader/extractors/owncloud.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/extractors/sharepoint.py` & `moodle_dl-2.3.7/moodle_dl/downloader/extractors/sharepoint.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/extractors/sharepointfiles.py` & `moodle_dl-2.3.7/moodle_dl/downloader/extractors/sharepointfiles.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/fake_download_service.py` & `moodle_dl-2.3.7/moodle_dl/downloader/fake_download_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/downloader/task.py` & `moodle_dl-2.3.7/moodle_dl/downloader/task.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/main.py` & `moodle_dl-2.3.7/moodle_dl/main.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/cookie_handler.py` & `moodle_dl-2.3.7/moodle_dl/moodle/cookie_handler.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/core_handler.py` & `moodle_dl-2.3.7/moodle_dl/moodle/core_handler.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/__init__.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/assign.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/assign.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/book.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/book.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/calendar.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/calendar.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,20 @@
     course_events_section_id,
     moodle_event_footer,
     moodle_event_header,
 )
 from moodle_dl.types import Course, File
 from moodle_dl.utils import PathTools as PT
 
+# TODO: should we use locale.setlocale(locale.LC_TIME, "") to set localized version of Date format
+# or should we use https://babel.pocoo.org/en/latest/dates.html
+# babel.dates.format_datetime(datetime_obj) is enough to use local setting, but we could also use user language settings of moodle,
+# by defining locale='user_lang' as extra argument
+# We can also use babel.dates.format_timedelta(time_delta) to print the time delta into the date file
+
 
 class CalendarMod(MoodleMod):
     MOD_NAME = 'calendar'
     MOD_PLURAL_NAME = 'events'
     MOD_MIN_VERSION = 2013051400  # 2.5
 
     @classmethod
```

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/common.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/common.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/data.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/data.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/folder.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/folder.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/forum.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/forum.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/lesson.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/lesson.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/page.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/page.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/quiz.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/quiz.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/mods/workshop.py` & `moodle_dl-2.3.7/moodle_dl/moodle/mods/workshop.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/moodle_constants.py` & `moodle_dl-2.3.7/moodle_dl/moodle/moodle_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,23 @@
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     <link rel="stylesheet" href="http://maxcdn.bootstrapcdn.com/font-awesome/latest/css/font-awesome.min.css">
     <script id="firstthemesheet"
         type="text/css">/** Required in order to fix style inclusion problems in IE with YUI **/</script>
     <link rel="stylesheet" type="text/css"
         href="https://moodle.ruhr-uni-bochum.de/theme/styles.php/boost/1633802793_1/all" />
+        <style>
+        @font-face {
+            font-family: "Font Awesome 6 Free";
+            font-style: normal;
+            font-weight: 900;
+            font-display: block;
+            src: url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.14.0/webfonts/fa-solid-900.woff2) format("woff2"), url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.14.0/webfonts/fa-solid-900.ttf) format("truetype");
+        }
+    </style>
     <script>
         //<![CDATA[
         var M = {}; M.yui = {};
         M.pageloadstarttime = new Date();
         M.cfg = { "wwwroot": "https:\\/\\/moodle.ruhr-uni-bochum.de", "sesskey": "roflAffe", "sessiontimeout": "28800", "themerev": "1633802793", "slasharguments": 1, "theme": "boost", "iconsystemmodule": "core\\/icon_system_fontawesome", "jsrev": "1633802793", "admin": "admin", "svgicons": true, "usertimezone": "Europa\\/London", "contextid": 104, "langrev": 1633946764, "templaterev": "1633802793" }; var yui1ConfigFn = function (me) { if (/-skin|reset|fonts|grids|base/.test(me.name)) { me.type = 'css'; me.path = me.path.replace(/\\.js/, '.css'); me.path = me.path.replace(/\\/yui2-skin/, '/assets/skins/sam/yui2-skin') } };
         var yui2ConfigFn = function (me) {
             var parts = me.name.replace(/^moodle-/, '').split('-'), component = parts.shift(), module = parts[0], min = '-min'; if (/-(skin|core)$/.test(me.name)) { parts.pop(); me.type = 'css'; min = '' }
```

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/moodle_service.py` & `moodle_dl-2.3.7/moodle_dl/moodle/moodle_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/request_helper.py` & `moodle_dl-2.3.7/moodle_dl/moodle/request_helper.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/moodle/result_builder.py` & `moodle_dl-2.3.7/moodle_dl/moodle/result_builder.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/__init__.py` & `moodle_dl-2.3.7/moodle_dl/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/console/console_service.py` & `moodle_dl-2.3.7/moodle_dl/notifications/console/console_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/discord/discord_formatter.py` & `moodle_dl-2.3.7/moodle_dl/notifications/discord/discord_formatter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/discord/discord_service.py` & `moodle_dl-2.3.7/moodle_dl/notifications/discord/discord_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/discord/discord_shooter.py` & `moodle_dl-2.3.7/moodle_dl/notifications/discord/discord_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/mail/header.png` & `moodle_dl-2.3.7/moodle_dl/notifications/mail/header.png`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/mail/header_extender.png` & `moodle_dl-2.3.7/moodle_dl/notifications/mail/header_extender.png`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/mail/mail_formater.py` & `moodle_dl-2.3.7/moodle_dl/notifications/mail/mail_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/mail/mail_service.py` & `moodle_dl-2.3.7/moodle_dl/notifications/mail/mail_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/mail/mail_shooter.py` & `moodle_dl-2.3.7/moodle_dl/notifications/mail/mail_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/notification_service.py` & `moodle_dl-2.3.7/moodle_dl/notifications/notification_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/telegram/telegram_formater.py` & `moodle_dl-2.3.7/moodle_dl/notifications/telegram/telegram_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/telegram/telegram_service.py` & `moodle_dl-2.3.7/moodle_dl/notifications/telegram/telegram_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/telegram/telegram_shooter.py` & `moodle_dl-2.3.7/moodle_dl/notifications/telegram/telegram_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/xmpp/xmpp_formater.py` & `moodle_dl-2.3.7/moodle_dl/notifications/xmpp/xmpp_formater.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/xmpp/xmpp_service.py` & `moodle_dl-2.3.7/moodle_dl/notifications/xmpp/xmpp_service.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/notifications/xmpp/xmpp_shooter.py` & `moodle_dl-2.3.7/moodle_dl/notifications/xmpp/xmpp_shooter.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/types.py` & `moodle_dl-2.3.7/moodle_dl/types.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl/utils.py` & `moodle_dl-2.3.7/moodle_dl/utils.py`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/moodle_dl.egg-info/PKG-INFO` & `moodle_dl-2.3.7/moodle_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moodle-dl
-Version: 2.3.6
+Version: 2.3.7
 Summary: Moodle-DL downloads course content fast from Moodle (eg. lecture pdfs)
 Home-page: https://github.com/C0D3D3V/Moodle-DL
 Author: C0D3D3V
 Author-email: moodle-dl@ist-ein-knaller.de
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/C0D3D3V/Moodle-DL#readme
 Project-URL: Wiki, https://github.com/C0D3D3V/Moodle-DL/wiki
```

### Comparing `moodle_dl-2.3.6/moodle_dl.egg-info/SOURCES.txt` & `moodle_dl-2.3.7/moodle_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moodle_dl-2.3.6/setup.py` & `moodle_dl-2.3.7/setup.py`

 * *Files identical despite different names*

