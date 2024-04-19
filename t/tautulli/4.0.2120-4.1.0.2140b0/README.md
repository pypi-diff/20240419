# Comparing `tmp/tautulli-4.0.2120.tar.gz` & `tmp/tautulli-4.1.0.2140b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tautulli-4.0.2120.tar", last modified: Thu Mar 28 16:07:56 2024, max compression
+gzip compressed data, was "tautulli-4.1.0.2140b0.tar", last modified: Fri Apr 19 07:48:36 2024, max compression
```

## Comparing `tautulli-4.0.2120.tar` & `tautulli-4.1.0.2140b0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:56.147271 tautulli-4.0.2120/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-28 16:07:28.000000 tautulli-4.0.2120/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-28 16:07:28.000000 tautulli-4.0.2120/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-03-28 16:07:56.147271 tautulli-4.0.2120/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-28 16:07:28.000000 tautulli-4.0.2120/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-28 16:07:56.147271 tautulli-4.0.2120/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-28 16:07:28.000000 tautulli-4.0.2120/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:56.131271 tautulli-4.0.2120/tautulli/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/API_VERSIONS.json
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/PYTHON_VERSIONS.json
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:56.135271 tautulli-4.0.2120/tautulli/api/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    97466 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/api/json_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    67678 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/api/object_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:56.135271 tautulli-4.0.2120/tautulli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/exceptions/api_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/exceptions/base_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/exceptions/http_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/exceptions/json_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:56.135271 tautulli-4.0.2120/tautulli/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/internal/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:56.147271 tautulli-4.0.2120/tautulli/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/children_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/collections_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/date_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/export_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/exports_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/geo_ip_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/get_plays_or_stream_types_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/home_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/item_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/item_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/libraries_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/library_media_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/library_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/library_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/library_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/new_rating_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/newsletter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/newsletter_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/newsletter_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/newsletter_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/notification_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/notifier_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/notifier_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/notifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/old_rating_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/playlists_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/plex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/pms_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/recently_added.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/registered_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/search_results.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/server_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/server_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/server_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/server_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/server_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/servers_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    30292 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/stream_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/synced_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/tautulli_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/update_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/user_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/user_logins.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/user_player_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/user_watch_time_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/usernames.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/users_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/models/whois_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:56.147271 tautulli-4.0.2120/tautulli/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/tools/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tautulli/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:56.147271 tautulli-4.0.2120/tautulli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-03-28 16:07:56.000000 tautulli-4.0.2120/tautulli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-03-28 16:07:56.000000 tautulli-4.0.2120/tautulli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 16:07:56.000000 tautulli-4.0.2120/tautulli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-28 16:07:56.000000 tautulli-4.0.2120/tautulli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 16:07:56.000000 tautulli-4.0.2120/tautulli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:07:56.147271 tautulli-4.0.2120/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tests/test_json_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tests/test_object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-28 16:07:28.000000 tautulli-4.0.2120/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:36.123055 tautulli-4.1.0.2140b0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-19 07:48:36.123055 tautulli-4.1.0.2140b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-19 07:48:36.123055 tautulli-4.1.0.2140b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:36.107055 tautulli-4.1.0.2140b0/tautulli/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/API_VERSIONS.json
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/PYTHON_VERSIONS.json
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:36.107055 tautulli-4.1.0.2140b0/tautulli/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97885 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/api/json_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67947 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/api/object_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:36.111055 tautulli-4.1.0.2140b0/tautulli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/exceptions/api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/exceptions/base_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/exceptions/http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/exceptions/json_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:36.111055 tautulli-4.1.0.2140b0/tautulli/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/internal/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:36.119055 tautulli-4.1.0.2140b0/tautulli/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/children_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/collections_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/date_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/export_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/exports_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/geo_ip_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/get_plays_or_stream_types_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/home_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/item_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/item_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/libraries_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/library_media_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/library_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/library_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/library_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/new_rating_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/newsletter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/newsletter_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/newsletter_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/newsletter_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/notification_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/notifier_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/notifier_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/notifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/old_rating_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/playlists_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/plex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/pms_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/recently_added.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/registered_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/search_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/server_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/server_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/server_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/server_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/servers_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30292 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/synced_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/tautulli_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/update_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/user_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/user_logins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/user_player_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/user_watch_time_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/usernames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/users_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/models/whois_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:36.119055 tautulli-4.1.0.2140b0/tautulli/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/tools/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tautulli/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:36.123055 tautulli-4.1.0.2140b0/tautulli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-19 07:48:36.000000 tautulli-4.1.0.2140b0/tautulli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-19 07:48:36.000000 tautulli-4.1.0.2140b0/tautulli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:48:36.000000 tautulli-4.1.0.2140b0/tautulli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-19 07:48:36.000000 tautulli-4.1.0.2140b0/tautulli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 07:48:36.000000 tautulli-4.1.0.2140b0/tautulli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:48:36.123055 tautulli-4.1.0.2140b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tests/test_json_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tests/test_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-19 07:48:11.000000 tautulli-4.1.0.2140b0/tests/test_utils.py
```

### Comparing `tautulli-4.0.2120/LICENSE` & `tautulli-4.1.0.2140b0/LICENSE`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/PKG-INFO` & `tautulli-4.1.0.2140b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tautulli
-Version: 4.0.2120
+Version: 4.1.0.2140b0
 Summary: A complete Python client for Tautulli's API
 Home-page: https://github.com/nwithan8/pytulli
-Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/4.0.02120.tar.gz
+Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/4.1.0.2140b0.tar.gz
 Author: Nate Harris
 Author-email: n8gr8gbln@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: Tautulli,API,client,Plex,PMS,Plex Media Server,media,server,JSON
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tautulli-4.0.2120/README.md` & `tautulli-4.1.0.2140b0/README.md`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/setup.py` & `tautulli-4.1.0.2140b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 from typing import List
 
 import setuptools
 
-__version__ = '4.0.02120'
+__version__ = '4.1.0.2140b0'
 
 __title__ = "tautulli"
 __author__ = 'Nate Harris'
 __author_email__ = 'n8gr8gbln@gmail.com'
 __github_username__ = "nwithan8"
 __github_repo__ = "pytulli"
 __copyright__ = "Copyright © 2024 - Nate Harris"
```

### Comparing `tautulli-4.0.2120/tautulli/api/json_api.py` & `tautulli-4.1.0.2140b0/tautulli/api/json_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -912,15 +912,16 @@
                                        before=before, after=after, section_id=section_id, media_type=media_type,
                                        transcode_decision=transcode_decision, guid=guid, order_column=order_column,
                                        order_dir=order_direction, start=start, length=length, search=search)
         return 'get_history', params
 
     @raw_json
     def get_home_stats(self, grouping: bool = False, time_range: int = 30, stats_type: str = 'plays', start: int = 0,
-                       count: int = 5, stat_id: str = None, user_id: int = None, section_id: int = None) -> List[dict]:
+                       count: int = 5, stat_id: str = None, user_id: int = None, section_id: int = None,
+                       before: datetime = None, after: datetime = None) -> List[dict]:
         """
         Get the homepage watch statistics
 
         :param grouping: Whether to group results (default: False)
         :type grouping: bool, optional
         :param time_range: Time range to calculate statistics (i.e. 30)
         :type time_range: int, optional
@@ -932,27 +933,33 @@
         :type count: int, optional
         :param stat_id: Name of a single statistic to return (i.e. 'top_movies', 'popular_tv', 'most_concurrent')
         :type stat_id: str, optional
         :param user_id: The ID of the Plex user
         :type user_id: int, optional
         :param section_id: The ID of the Plex library section
         :type section_id: int, optional
+        :param before: Results before and including the date
+        :type before: datetime, optional
+        :param after: Results after and including the date
+        :type after: datetime, optional
         :returns: List of data
         :rtype: List[dict]
         """
         grouping = bool_to_int(boolean=grouping)
         if _is_invalid_choice(value=stats_type, variable_name="stats_type",
                               choices=static.stats_type):
             return False, None
         if _is_invalid_choice(value=stat_id, variable_name='stat_id',
                               choices=static.stats_category):
             return False, None
+        before = datetime_to_string(datetime_object=before)
+        after = datetime_to_string(datetime_object=after)
         params = build_optional_params(grouping=grouping, time_range=time_range, stats_type=stats_type,
                                        stats_start=start, stats_count=count, stat_id=stat_id, section_id=section_id,
-                                       user_id=user_id)
+                                       user_id=user_id, before=before, after=after)
         return 'get_home_stats', params
 
     @raw_json
     def get_item_user_stats(self, rating_key: str, grouping: bool = False, media_type: str = None) -> List[dict]:
         """
         Get the user statistics for the media item
```

### Comparing `tautulli-4.0.2120/tautulli/api/object_api.py` & `tautulli-4.1.0.2140b0/tautulli/api/object_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,16 +640,16 @@
         :type search: str, optional
         :returns: History object
         """
         return 'History'
 
     @make_object
     def get_home_stats(self, grouping: bool = False, time_range: int = 30, stats_type: str = 'plays', start: int = 0,
-                       count: int = 5, stat_id: str = None, user_id: int = None, section_id: int = None) -> List[
-        HomeStat]:
+                       count: int = 5, stat_id: str = None, user_id: int = None, section_id: int = None,
+                       before: datetime = None, after: datetime = None) -> List[HomeStat]:
         """
         Get the homepage watch statistics
 
         :param grouping: Whether to group results (default: False)
         :type grouping: bool, optional
         :param time_range: Time range to calculate statistics (i.e. 30)
         :type time_range: int, optional
@@ -661,21 +661,25 @@
         :type count: int, optional
         :param stat_id: Name of a single statistic to return (i.e. 'top_movies', 'popular_tv', 'most_concurrent')
         :type stat_id: str, optional
         :param user_id: The ID of the Plex user
         :type user_id: int, optional
         :param section_id: The ID of the Plex library section
         :type section_id: int, optional
+        :param before: Results before and including the date
+        :type before: datetime, optional
+        :param after: Results after and including the date
+        :type after: datetime, optional
         :returns: List of HomeStat object
         """
         return 'HomeStat'
 
     @make_object
-    def get_item_user_stats(self, rating_key: str, grouping: bool = False, media_type: str = None) -> List[
-        ItemUserStat]:
+    def get_item_user_stats(self, rating_key: str, grouping: bool = False, media_type: str = None) \
+            -> List[ItemUserStat]:
         """
         Get the user statistics for the media item
 
         :param rating_key: Rating key of the media item
         :type rating_key: str
         :param grouping: Whether to group results (default: False)
         :type grouping: bool, optional
```

### Comparing `tautulli-4.0.2120/tautulli/exceptions/http_exception.py` & `tautulli-4.1.0.2140b0/tautulli/exceptions/http_exception.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/exceptions/json_exception.py` & `tautulli-4.1.0.2140b0/tautulli/exceptions/json_exception.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/internal/decorators.py` & `tautulli-4.1.0.2140b0/tautulli/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/internal/static.py` & `tautulli-4.1.0.2140b0/tautulli/internal/static.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/internal/utils.py` & `tautulli-4.1.0.2140b0/tautulli/internal/utils.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/__init__.py` & `tautulli-4.1.0.2140b0/tautulli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/activity.py` & `tautulli-4.1.0.2140b0/tautulli/models/activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,19 @@
     video_profile: Optional[str] = None
     audio_codec: Optional[str] = None
     audio_channels: Optional[str] = None
     audio_channel_layout: Optional[str] = None
     audio_profile: Optional[str] = None
     optimized_version: Optional[int] = None
     channel_call_sign: Optional[str] = None
+    channel_id: Optional[str] = None
     channel_identifier: Optional[str] = None
+    channel_title: Optional[str] = None
     channel_thumb: Optional[str] = None
+    channel_vcn: Optional[str] = None
     file: Optional[str] = None
     file_size: Optional[str] = None
     indexes: Optional[int] = None
     selected: Optional[int] = None
     type: Optional[str] = None
     video_codec_level: Optional[str] = None
     video_bitrate: Optional[str] = None
```

### Comparing `tautulli-4.0.2120/tautulli/models/children_metadata.py` & `tautulli-4.1.0.2140b0/tautulli/models/children_metadata.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/collections_table.py` & `tautulli-4.1.0.2140b0/tautulli/models/collections_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/docs.py` & `tautulli-4.1.0.2140b0/tautulli/models/docs.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/export_fields.py` & `tautulli-4.1.0.2140b0/tautulli/models/export_fields.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/exports_table.py` & `tautulli-4.1.0.2140b0/tautulli/models/exports_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/geo_ip_lookup.py` & `tautulli-4.1.0.2140b0/tautulli/models/geo_ip_lookup.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/history.py` & `tautulli-4.1.0.2140b0/tautulli/models/history.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/home_stats.py` & `tautulli-4.1.0.2140b0/tautulli/models/home_stats.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/libraries.py` & `tautulli-4.1.0.2140b0/tautulli/models/libraries.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/libraries_table.py` & `tautulli-4.1.0.2140b0/tautulli/models/libraries_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/library.py` & `tautulli-4.1.0.2140b0/tautulli/models/library.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/library_media_info.py` & `tautulli-4.1.0.2140b0/tautulli/models/library_media_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/metadata.py` & `tautulli-4.1.0.2140b0/tautulli/models/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,21 @@
     video_bit_depth: Optional[str] = None
     video_chroma_subsampling: Optional[str] = None
     video_color_primaries: Optional[str] = None
     video_color_range: Optional[str] = None
     video_color_space: Optional[str] = None
     video_color_trc: Optional[str] = None
     video_dynamic_range: Optional[str] = None
+    video_dovi_bl_present: Optional[int] = None
+    video_dovi_el_present: Optional[int] = None
+    video_dovi_level: Optional[int] = None
+    video_dovi_present: Optional[int] = None
+    video_dovi_profile: Optional[int] = None
+    video_dovi_rpu_present: Optional[int] = None
+    video_dovi_version: Optional[float] = None
     video_frame_rate: Optional[str] = None
     video_ref_frames: Optional[str] = None
     video_height: Optional[str] = None
     video_width: Optional[str] = None
     video_language: Optional[str] = None
     video_language_code: Optional[str] = None
     video_profile: Optional[str] = None
@@ -65,16 +72,19 @@
     video_profile: Optional[str] = None
     audio_codec: Optional[str] = None
     audio_channels: Optional[str] = None
     audio_channel_layout: Optional[str] = None
     audio_profile: Optional[str] = None
     optimized_version: Optional[int] = None
     channel_call_sign: Optional[str] = None
+    channel_id: Optional[str] = None
     channel_identifier: Optional[str] = None
+    channel_title: Optional[str] = None
     channel_thumb: Optional[str] = None
+    channel_vcn: Optional[str] = None
     parts: Optional[List[PartModel]] = None
 
 class MarkerModel(BaseModel):
     id: Optional[int] = None
     type: Optional[str] = None
     start_time_offset: Optional[int] = None
     end_time_offset: Optional[int] = None
```

### Comparing `tautulli-4.0.2120/tautulli/models/newsletter_config.py` & `tautulli-4.1.0.2140b0/tautulli/models/newsletter_config.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/newsletter_log.py` & `tautulli-4.1.0.2140b0/tautulli/models/newsletter_log.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/notification_log.py` & `tautulli-4.1.0.2140b0/tautulli/models/notification_log.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/notifier_config.py` & `tautulli-4.1.0.2140b0/tautulli/models/notifier_config.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/parser.py` & `tautulli-4.1.0.2140b0/tautulli/models/parser.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/playlists_table.py` & `tautulli-4.1.0.2140b0/tautulli/models/playlists_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/pms_update.py` & `tautulli-4.1.0.2140b0/tautulli/models/pms_update.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/recently_added.py` & `tautulli-4.1.0.2140b0/tautulli/models/recently_added.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/registered_device.py` & `tautulli-4.1.0.2140b0/tautulli/models/registered_device.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/search_results.py` & `tautulli-4.1.0.2140b0/tautulli/models/search_results.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/server_info.py` & `tautulli-4.1.0.2140b0/tautulli/models/server_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/server_list.py` & `tautulli-4.1.0.2140b0/tautulli/models/server_list.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/settings.py` & `tautulli-4.1.0.2140b0/tautulli/models/settings.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/stream_data.py` & `tautulli-4.1.0.2140b0/tautulli/models/stream_data.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/synced_items.py` & `tautulli-4.1.0.2140b0/tautulli/models/synced_items.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/tautulli_info.py` & `tautulli-4.1.0.2140b0/tautulli/models/tautulli_info.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/user.py` & `tautulli-4.1.0.2140b0/tautulli/models/user.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/user_ips.py` & `tautulli-4.1.0.2140b0/tautulli/models/user_ips.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/user_logins.py` & `tautulli-4.1.0.2140b0/tautulli/models/user_logins.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/users.py` & `tautulli-4.1.0.2140b0/tautulli/models/users.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/users_table.py` & `tautulli-4.1.0.2140b0/tautulli/models/users_table.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/models/whois_lookup.py` & `tautulli-4.1.0.2140b0/tautulli/models/whois_lookup.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/tools/api_helper.py` & `tautulli-4.1.0.2140b0/tautulli/tools/api_helper.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli/tools/utils.py` & `tautulli-4.1.0.2140b0/tautulli/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tautulli.egg-info/PKG-INFO` & `tautulli-4.1.0.2140b0/tautulli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tautulli
-Version: 4.0.2120
+Version: 4.1.0.2140b0
 Summary: A complete Python client for Tautulli's API
 Home-page: https://github.com/nwithan8/pytulli
-Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/4.0.02120.tar.gz
+Download-URL: https://github.com/nwithan8/pytulli/archive/refs/tags/4.1.0.2140b0.tar.gz
 Author: Nate Harris
 Author-email: n8gr8gbln@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Keywords: Tautulli,API,client,Plex,PMS,Plex Media Server,media,server,JSON
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tautulli-4.0.2120/tautulli.egg-info/SOURCES.txt` & `tautulli-4.1.0.2140b0/tautulli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tests/test_json_api.py` & `tautulli-4.1.0.2140b0/tests/test_json_api.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tests/test_object_api.py` & `tautulli-4.1.0.2140b0/tests/test_object_api.py`

 * *Files identical despite different names*

### Comparing `tautulli-4.0.2120/tests/test_shortcuts.py` & `tautulli-4.1.0.2140b0/tests/test_shortcuts.py`

 * *Files identical despite different names*

