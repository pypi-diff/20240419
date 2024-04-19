# Comparing `tmp/ultima_scraper_api-2.2.23.tar.gz` & `tmp/ultima_scraper_api-2.2.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-2.2.23.tar", max compression
+gzip compressed data, was "ultima_scraper_api-2.2.24.tar", max compression
```

## Comparing `ultima_scraper_api-2.2.23.tar` & `ultima_scraper_api-2.2.24.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1257 2024-02-19 00:53:44.726439 ultima_scraper_api-2.2.23/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-2.2.23/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2670 2023-12-18 07:32:59.535607 ultima_scraper_api-2.2.23/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-2.2.23/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     3731 2023-11-30 04:05:19.333425 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     2469 2023-12-23 23:02:11.519743 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0     2127 2024-01-07 05:27:39.332979 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/auth_streamliner.py
--rw-r--r--   0        0        0      645 2023-11-30 04:11:43.238177 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     3078 2024-01-07 02:45:02.897270 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0     4702 2023-12-18 07:25:38.835846 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/authenticator.py
--rw-r--r--   0        0        0      249 2023-12-02 19:12:21.898179 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    13161 2024-01-05 16:32:00.286752 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6563 2023-12-08 09:33:53.172671 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0      655 2023-07-08 10:22:46.596423 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/comment_model.py
--rw-r--r--   0        0        0    10154 2024-01-19 07:32:56.430688 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     5901 2023-12-24 00:37:27.225759 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     7306 2023-12-08 09:34:03.579498 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3268 2023-12-08 09:34:06.692880 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0     1089 2023-11-30 08:28:59.843675 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/subscription_model.py
--rw-r--r--   0        0        0    27567 2024-01-06 09:15:49.418317 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     6522 2023-12-23 23:02:41.820454 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     3042 2024-01-06 23:05:25.425987 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0     6350 2024-02-02 02:17:26.567568 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/authenticator.py
--rw-r--r--   0        0        0      205 2023-11-29 18:32:12.431939 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    16913 2024-01-27 18:26:04.212500 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0     1162 2023-12-24 00:29:33.748277 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/chat_model.py
--rw-r--r--   0        0        0      767 2023-12-02 20:22:41.700921 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/comment_model.py
--rw-r--r--   0        0        0    13638 2024-01-27 18:49:15.248861 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      749 2023-12-16 09:18:58.087530 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2866 2024-01-05 20:19:10.377889 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/mass_message_model.py
--rw-r--r--   0        0        0     3398 2024-01-07 04:37:41.374763 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     6124 2023-12-29 18:58:00.754610 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
--rw-r--r--   0        0        0     3973 2023-12-16 08:52:44.831588 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0      287 2023-12-18 12:07:14.644579 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/stat.py
--rw-r--r--   0        0        0     1459 2023-12-16 08:53:28.469427 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0     1824 2023-11-30 06:17:33.423820 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
--rw-r--r--   0        0        0    34647 2024-01-06 21:26:49.133670 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0     2034 2023-12-24 00:53:00.148066 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/vault.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     7505 2023-12-23 23:32:21.266380 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2916 2023-12-23 22:51:25.434556 ultima_scraper_api-2.2.23/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-2.2.23/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-07-11 08:47:19.301278 ultima_scraper_api-2.2.23/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.23/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0     1952 2023-12-02 23:30:30.482767 ultima_scraper_api-2.2.23/ultima_scraper_api/config.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-2.2.23/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-2.2.23/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-2.2.23/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1362 2023-12-02 21:48:17.148944 ultima_scraper_api-2.2.23/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-2.2.23/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-2.2.23/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    10552 2024-01-27 17:24:53.956943 ultima_scraper_api-2.2.23/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-2.2.23/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-2.2.23/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     2318 2023-12-24 11:31:40.994446 ultima_scraper_api-2.2.23/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-2.2.23/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      631 2023-10-08 19:23:00.177284 ultima_scraper_api-2.2.23/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2417 2023-12-23 22:49:39.932066 ultima_scraper_api-2.2.23/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    15648 2024-01-27 17:26:37.159460 ultima_scraper_api-2.2.23/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-2.2.23/ultima_scraper_api/models/__init__.py
--rw-r--r--   0        0        0      641 2023-12-02 23:28:01.235613 ultima_scraper_api-2.2.23/ultima_scraper_api/models/subscription_model.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-2.2.23/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 ultima_scraper_api-2.2.23/PKG-INFO
+-rw-r--r--   0        0        0     1257 2024-04-19 14:33:12.259261 ultima_scraper_api-2.2.24/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-2.2.24/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2670 2023-12-18 07:32:59.535607 ultima_scraper_api-2.2.24/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-2.2.24/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     3731 2023-11-30 04:05:19.333425 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     2469 2023-12-23 23:02:11.519743 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0     2121 2024-04-19 13:03:24.099066 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/auth_streamliner.py
+-rw-r--r--   0        0        0      645 2023-11-30 04:11:43.238177 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     3078 2024-01-07 02:45:02.897270 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0     4702 2023-12-18 07:25:38.835846 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/authenticator.py
+-rw-r--r--   0        0        0      249 2023-12-02 19:12:21.898179 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    13161 2024-01-05 16:32:00.286752 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6563 2023-12-08 09:33:53.172671 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0      655 2023-07-08 10:22:46.596423 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/comment_model.py
+-rw-r--r--   0        0        0    10154 2024-01-19 07:32:56.430688 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     5901 2023-12-24 00:37:27.225759 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     7306 2023-12-08 09:34:03.579498 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3268 2023-12-08 09:34:06.692880 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0     1089 2023-11-30 08:28:59.843675 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/subscription_model.py
+-rw-r--r--   0        0        0    27567 2024-01-06 09:15:49.418317 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     6779 2024-04-07 09:53:53.542364 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     3153 2024-04-19 11:24:28.858672 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0     6350 2024-04-19 11:24:56.548781 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/authenticator.py
+-rw-r--r--   0        0        0      205 2023-11-29 18:32:12.431939 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    16913 2024-01-27 18:26:04.212500 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0     1162 2023-12-24 00:29:33.748277 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/chat_model.py
+-rw-r--r--   0        0        0      767 2023-12-02 20:22:41.700921 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/comment_model.py
+-rw-r--r--   0        0        0    13638 2024-01-27 18:49:15.248861 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      749 2023-12-16 09:18:58.087530 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2866 2024-01-05 20:19:10.377889 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/mass_message_model.py
+-rw-r--r--   0        0        0     3398 2024-01-07 04:37:41.374763 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     6124 2023-12-29 18:58:00.754610 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
+-rw-r--r--   0        0        0     3973 2023-12-16 08:52:44.831588 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0      287 2023-12-18 12:07:14.644579 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/stat.py
+-rw-r--r--   0        0        0     1459 2023-12-16 08:53:28.469427 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0     1824 2023-11-30 06:17:33.423820 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
+-rw-r--r--   0        0        0    34773 2024-04-19 11:22:51.908339 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0     2034 2023-12-24 00:53:00.148066 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/vault.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     7762 2024-04-07 09:52:49.239394 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     4081 2024-04-19 12:18:36.528432 ultima_scraper_api-2.2.24/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-2.2.24/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-07-11 08:47:19.301278 ultima_scraper_api-2.2.24/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-2.2.24/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0     1952 2023-12-02 23:30:30.482767 ultima_scraper_api-2.2.24/ultima_scraper_api/config.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-2.2.24/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-2.2.24/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-2.2.24/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1362 2023-12-02 21:48:17.148944 ultima_scraper_api-2.2.24/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-2.2.24/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-2.2.24/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    10552 2024-01-27 17:24:53.956943 ultima_scraper_api-2.2.24/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-2.2.24/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-2.2.24/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     2318 2024-04-19 11:26:51.545962 ultima_scraper_api-2.2.24/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-2.2.24/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      631 2023-10-08 19:23:00.177284 ultima_scraper_api-2.2.24/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2417 2023-12-23 22:49:39.932066 ultima_scraper_api-2.2.24/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    15648 2024-01-27 17:26:37.159460 ultima_scraper_api-2.2.24/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-2.2.24/ultima_scraper_api/models/__init__.py
+-rw-r--r--   0        0        0      641 2023-12-02 23:28:01.235613 ultima_scraper_api-2.2.24/ultima_scraper_api/models/subscription_model.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-2.2.24/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 ultima_scraper_api-2.2.24/PKG-INFO
```

### Comparing `ultima_scraper_api-2.2.23/pyproject.toml` & `ultima_scraper_api-2.2.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "2.2.23"
+version = "2.2.24"
 description = ""
 authors = ["UltimaHoarder <1285176+UltimaHoarder@users.noreply.github.com>"]
 packages = [{ include = "ultima_scraper_api" }]
 include = ["ultima_scraper_api/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/__init__.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/api_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/api_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/auth_streamliner.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/auth_streamliner.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 class CacheStats:
     def __init__(self) -> None:
         self.processed_at: datetime | None = None
         self.delay_in_seconds = 3600 * 1  # hour in seconds * hour
         self.released_at: datetime | None = None
 
     def activate(self):
-        self.processed_at = datetime.utcnow()
+        self.processed_at = datetime.now()
         self.released_at = self.processed_at + timedelta(seconds=self.delay_in_seconds)
 
     def deactivate(self):
         self.processed_at = self.released_at = None
 
     def is_released(self):
         status = True
         if self.released_at:
-            if datetime.utcnow() < self.released_at:
+            if datetime.now() < self.released_at:
                 status = False
             else:
                 self.processed_at = self.released_at = None
         return status
 
 
 class Cache:
```

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/background_tasks.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/authenticator.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/authenticator.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/comment_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/comment_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/subscription_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from ultima_scraper_api.apis.api_streamliner import StreamlinedAPI
 from ultima_scraper_api.apis.fansly.classes.extras import AuthDetails, endpoint_links
 from ultima_scraper_api.apis.fansly.classes.message_model import create_message
 from ultima_scraper_api.apis.fansly.classes.post_model import create_post
 from ultima_scraper_api.apis.fansly.classes.story_model import create_story
 from ultima_scraper_api.config import UltimaScraperAPIConfig
+from pathlib import Path
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.auth_model import FanslyAuthModel
 
 
 class FanslyAPI(StreamlinedAPI):
     def __init__(
@@ -151,14 +152,20 @@
         def __iter__(self):
             for attr, value in self.__dict__.items():
                 yield attr, value
 
         def get_keys(self):
             return [item[0] for item in self]
 
+        def path_to_key(self, value: Path):
+            for content_type, _ in self:
+                for part in value.parts:
+                    if content_type.lower() == part.lower():
+                        return content_type
+
     class MediaTypes:
         def __init__(self) -> None:
             self.Images = ["photo", "image"]
             self.Videos = ["video", "stream", "gif"]
             self.Audios = ["audio"]
             self.Texts = ["text"]
```

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,20 @@
             url = has_drm
     return urlparse(url) if url else None
 
 
 def preview_url_picker(media_item: dict[str, Any]):
     preview_url: str | None = None
     if "files" in media_item:
-        if "preview" in media_item["files"] and "url" in media_item["files"]["preview"]:
-            preview_url = media_item["files"]["preview"]["url"]
+        if "preview" in media_item["files"]:
+            if (
+                media_item["files"]["preview"] is not None
+                and "url" in media_item["files"]["preview"]
+            ):
+                preview_url = media_item["files"]["preview"]["url"]
     else:
         preview_url = media_item["preview"]
         return urlparse(preview_url) if preview_url else None
 
 
 class SiteContent:
     def __init__(self, option: dict[str, Any], user: create_user) -> None:
```

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/authenticator.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/authenticator.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/chat_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/chat_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/comment_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/comment_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/mass_message_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/mass_message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/only_drm.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/only_drm.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,16 +332,19 @@
         super().__init__(authed)
 
     def get_username(self):
         if not self.username:
             self.username = f"u{self.id}"
         return self.username
 
-    def get_link(self):
-        link = f"https://onlyfans.com/{self.username}"
+    def get_link(self, use_username: bool = False):
+        if use_username:
+            link = f"https://onlyfans.com/{self.username}"
+        else:
+            link = f"https://onlyfans.com/{self.id}"
         return link
 
     def is_authed_user(self):
         if self.id == self.get_authed().id:
             return True
         else:
             return False
@@ -710,17 +713,17 @@
         # If error message, this means the user has socials, but we have to subscribe to see them
         result = bool(
             await self.get_requester().json_request(endpoint_links(self.id).socials)
         )
         return result
 
     async def get_socials(self):
-        results: list[dict[str, Any]] | dict[
-            str, Any
-        ] = await self.get_requester().json_request(endpoint_links(self.id).socials)
+        results: list[dict[str, Any]] | dict[str, Any] = (
+            await self.get_requester().json_request(endpoint_links(self.id).socials)
+        )
         if "error" in results:
             results = []
         assert isinstance(results, list)
         return results
 
     async def get_spotify(self):
         if self.is_spotify_connected:
```

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/classes/vault.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/classes/vault.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/onlyfans/onlyfans.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from contextlib import asynccontextmanager
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal
 
 import requests
 
 from ultima_scraper_api.apis.api_streamliner import StreamlinedAPI
 from ultima_scraper_api.apis.onlyfans.classes.extras import AuthDetails, endpoint_links
 from ultima_scraper_api.apis.onlyfans.classes.hightlight_model import create_highlight
@@ -164,14 +165,20 @@
         def __iter__(self):
             for attr, value in self.__dict__.items():
                 yield attr, value
 
         def get_keys(self):
             return [item[0] for item in self]
 
+        def path_to_key(self, value: Path):
+            for content_type, _ in self:
+                for part in value.parts:
+                    if content_type.lower() == part.lower():
+                        return content_type
+
     class MediaTypes:
         def __init__(self) -> None:
             self.Images = ["photo", "image"]
             self.Videos = ["video", "stream", "gif", "application"]
             self.Audios = ["audio"]
             self.Texts = ["text"]
```

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/apis/user_streamliner.py`

 * *Files 24% similar despite different names*

```diff
@@ -97,7 +97,34 @@
         return self.__authed.auth_session.get_session_manager()  # type: ignore
 
     def get_api(self) -> TAPI:
         return self.__authed.get_api()  # type: ignore
 
     def is_active(self):
         return self.active
+
+    def get_usernames(self, ignore_id: bool = True) -> list[str]:
+        final_usernames: list[str] = [self.username]  # type: ignore
+        for alias in self.get_aliases(ignore_id=ignore_id):
+            if alias not in final_usernames:
+                final_usernames.append(alias)
+        if ignore_id and len(final_usernames) > 1:
+            invalid_usernames = [f"u{self.id}"]  # type: ignore
+            for invalid_username in invalid_usernames:
+                if invalid_username in final_usernames:
+                    final_usernames.remove(invalid_username)
+        assert final_usernames
+        return final_usernames
+
+    def get_aliases(self, ignore_id: bool = True):
+        final_aliases = self.aliases.copy()
+        if ignore_id:
+            invalid_aliases = [f"u{self.id}"]  # type: ignore
+            for invalid_alias in invalid_aliases:
+                if invalid_alias in final_aliases:
+                    final_aliases.remove(invalid_alias)
+        return final_aliases
+
+    def add_aliases(self, aliases: list[str]):
+        for alias in aliases:
+            if alias not in self.aliases:
+                self.aliases.append(alias)
```

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/config.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/config.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-2.2.24/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-2.2.24/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/helpers/main_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/managers/scrape_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/managers/session_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/ultima_scraper_api/models/subscription_model.py` & `ultima_scraper_api-2.2.24/ultima_scraper_api/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-2.2.23/PKG-INFO` & `ultima_scraper_api-2.2.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 2.2.23
+Version: 2.2.24
 Summary: 
 Author: UltimaHoarder
 Author-email: 1285176+UltimaHoarder@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

