# Comparing `tmp/ossapi-3.4.4.tar.gz` & `tmp/ossapi-4.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossapi-3.4.4.tar", last modified: Fri Feb  9 23:17:00 2024, max compression
+gzip compressed data, was "ossapi-4.0.0b1.tar", last modified: Fri Apr 19 01:49:42 2024, max compression
```

## Comparing `ossapi-3.4.4.tar` & `ossapi-4.0.0b1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-09 23:17:00.208051 ossapi-3.4.4/
--rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.4.4/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)    10530 2024-02-09 23:17:00.207697 ossapi-3.4.4/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)     9874 2023-10-24 05:01:52.000000 ossapi-3.4.4/README.md
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-09 23:17:00.204620 ossapi-3.4.4/ossapi/
--rw-r--r--   0 tybug      (501) staff       (20)     5352 2023-10-21 20:55:09.000000 ossapi-3.4.4/ossapi/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      925 2023-04-18 20:48:24.000000 ossapi-3.4.4/ossapi/encoder.py
--rw-r--r--   0 tybug      (501) staff       (20)    17733 2024-02-04 18:52:35.000000 ossapi-3.4.4/ossapi/enums.py
--rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-10-21 20:55:09.000000 ossapi-3.4.4/ossapi/mod.py
--rw-r--r--   0 tybug      (501) staff       (20)    39426 2024-02-04 18:57:57.000000 ossapi-3.4.4/ossapi/models.py
--rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-10-23 19:56:04.000000 ossapi-3.4.4/ossapi/ossapi.py
--rw-r--r--   0 tybug      (501) staff       (20)    96781 2024-02-04 18:44:40.000000 ossapi-3.4.4/ossapi/ossapiv2.py
--rw-r--r--   0 tybug      (501) staff       (20)    99863 2023-10-23 20:46:05.000000 ossapi-3.4.4/ossapi/ossapiv2_async.py
--rw-r--r--   0 tybug      (501) staff       (20)     3681 2023-11-27 05:14:11.000000 ossapi-3.4.4/ossapi/replay.py
--rw-r--r--   0 tybug      (501) staff       (20)    11119 2023-10-21 20:55:09.000000 ossapi-3.4.4/ossapi/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-09 23:17:00.207095 ossapi-3.4.4/ossapi.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)    10530 2024-02-09 23:17:00.000000 ossapi-3.4.4/ossapi.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      460 2024-02-09 23:17:00.000000 ossapi-3.4.4/ossapi.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2024-02-09 23:17:00.000000 ossapi-3.4.4/ossapi.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       71 2024-02-09 23:17:00.000000 ossapi-3.4.4/ossapi.egg-info/requires.txt
--rw-r--r--   0 tybug      (501) staff       (20)        7 2024-02-09 23:17:00.000000 ossapi-3.4.4/ossapi.egg-info/top_level.txt
--rw-r--r--   0 tybug      (501) staff       (20)      638 2024-02-09 23:16:48.000000 ossapi-3.4.4/pyproject.toml
--rw-r--r--   0 tybug      (501) staff       (20)       38 2024-02-09 23:17:00.208117 ossapi-3.4.4/setup.cfg
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-09 23:17:00.206700 ossapi-3.4.4/tests/
--rw-r--r--   0 tybug      (501) staff       (20)     3074 2023-10-23 20:01:01.000000 ossapi-3.4.4/tests/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.4.4/tests/test_cursor.py
--rw-r--r--   0 tybug      (501) staff       (20)    11884 2024-02-04 18:57:47.000000 ossapi-3.4.4/tests/test_endpoints.py
--rw-r--r--   0 tybug      (501) staff       (20)     4039 2023-07-16 04:59:00.000000 ossapi-3.4.4/tests/test_models.py
--rw-r--r--   0 tybug      (501) staff       (20)     1133 2023-07-16 04:59:00.000000 ossapi-3.4.4/tests/test_v1.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-19 01:49:42.008122 ossapi-4.0.0b1/
+-rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-4.0.0b1/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)    10697 2024-04-19 01:49:42.007824 ossapi-4.0.0b1/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)    10039 2024-04-17 01:30:55.000000 ossapi-4.0.0b1/README.md
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-19 01:49:42.005907 ossapi-4.0.0b1/ossapi/
+-rw-r--r--   0 tybug      (501) staff       (20)     6151 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      917 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/encoder.py
+-rw-r--r--   0 tybug      (501) staff       (20)    18069 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/enums.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11982 2024-04-19 01:42:59.000000 ossapi-4.0.0b1/ossapi/mod.py
+-rw-r--r--   0 tybug      (501) staff       (20)    39778 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/models.py
+-rw-r--r--   0 tybug      (501) staff       (20)    15363 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/ossapi.py
+-rw-r--r--   0 tybug      (501) staff       (20)    99648 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/ossapiv2.py
+-rw-r--r--   0 tybug      (501) staff       (20)   102924 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/ossapiv2_async.py
+-rw-r--r--   0 tybug      (501) staff       (20)     3681 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/replay.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11087 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-19 01:49:42.007466 ossapi-4.0.0b1/ossapi.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)    10697 2024-04-19 01:49:41.000000 ossapi-4.0.0b1/ossapi.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      442 2024-04-19 01:49:42.000000 ossapi-4.0.0b1/ossapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2024-04-19 01:49:41.000000 ossapi-4.0.0b1/ossapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)       71 2024-04-19 01:49:41.000000 ossapi-4.0.0b1/ossapi.egg-info/requires.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        7 2024-04-19 01:49:41.000000 ossapi-4.0.0b1/ossapi.egg-info/top_level.txt
+-rw-r--r--   0 tybug      (501) staff       (20)      643 2024-04-19 01:47:53.000000 ossapi-4.0.0b1/pyproject.toml
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2024-04-19 01:49:42.008162 ossapi-4.0.0b1/setup.cfg
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-19 01:49:42.007258 ossapi-4.0.0b1/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)      524 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/tests/test_cursor.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11434 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/tests/test_endpoints.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4028 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/tests/test_models.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1140 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/tests/test_v1.py
```

### Comparing `ossapi-3.4.4/LICENSE` & `ossapi-4.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ossapi-3.4.4/PKG-INFO` & `ossapi-4.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.4.4
+Version: 4.0.0b1
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/tybug/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,14 @@
 ossapi is the definitive python wrapper for the osu! api. ossapi has complete coverage of [api v2](https://osu.ppy.sh/docs/index.html) and [api v1](https://github.com/ppy/osu-api/wiki), and provides both sync (`Ossapi`) and async (`OssapiAsync`) versions for api v2.
 
 If you need support or would like to contribute, feel free to ask in the `#ossapi` channel of the [circleguard discord](https://discord.gg/e84qxkQ).
 
 * [Installation](#installation)
 * [Quickstart](#quickstart)
 * [Async](#async)
-* [Lazer](#lazer)
 * [Endpoints](#endpoints)
   * [Beatmap Packs](#endpoints-beatmap-packs)
   * [Beatmaps](#endpoints-beatmaps)
   * [Beatmapsets](#endpoints-beatmapsets)
   * [Changelog](#endpoints-changelog)
   * [Chat](#endpoints-chat)
   * [Comments](#endpoints-comments)
@@ -45,14 +44,15 @@
   * [Rankings](#endpoints-rankings)
   * [Rooms](#endpoints-rooms)
   * [Scores](#endpoints-scores)
   * [Seasonal Backgrounds](#endpoints-seasonal-backgrounds)
   * [Spotlights](#endpoints-spotlights)
   * [Users](#endpoints-users)
   * [Wiki](#endpoints-wiki)
+* [Other domains](#other-domains)
 * [API v1 Usage](#api-v1-usage)
 
 
 ## Installation
 
 To install:
 
@@ -100,26 +100,26 @@
     await api.user("tybug")
 
 asyncio.run(main())
 ```
 
 [Read more about OssapiAsync on the docs.](https://tybug.github.io/ossapi/async.html)
 
-## Lazer
+## Other domains
 
-You can retrieve lazer-specific data (scores, leaderboards, etc) with ossapi:
+You can use ossapi to interact with the api of other deployments of the osu website, such as https://dev.ppy.sh.
 
 ```python
 from ossapi import Ossapi
 
-api_lazer = Ossapi(client_id, client_secret, domain="lazer")
-
-# best score on the lazer server (lazer + osu scores combined)
-scores = api_lazer.user_scores(12092800, "best")
-print(scores[0].pp)
+api = Ossapi(client_id, client_secret, domain="dev")
+# get the dev server pp leaderboards
+ranking = api.ranking("osu", "performance").ranking
+# pearline06, as of 2023
+print(ranking[0].user.username)
 ```
 
 [Read more about domains on the docs.](https://tybug.github.io/ossapi/domains.html)
 
 ## Endpoints
 
 All endpoints for api v2.
@@ -179,14 +179,15 @@
   * [`api.multiplayer_scores`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.multiplayer_scores)
   * [`api.room`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.room)
   * [`api.room_leaderboard`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.room_leaderboard)
   * [`api.rooms`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.rooms)
 * Scores<a name="endpoints-scores"></a>
   * [`api.download_score`](https://tybug.github.io/ossapi/scores.html#ossapi.ossapiv2.Ossapi.download_score)
   * [`api.score`](https://tybug.github.io/ossapi/scores.html#ossapi.ossapiv2.Ossapi.score)
+  * [`api.score_mode`](https://tybug.github.io/ossapi/scores.html#ossapi.ossapiv2.Ossapi.score_mode)
 * Seasonal Backgrounds<a name="endpoints-seasonal-backgrounds"></a>
   * [`api.seasonal_backgrounds`](https://tybug.github.io/ossapi/seasonal%20backgrounds.html#ossapi.ossapiv2.Ossapi.seasonal_backgrounds)
 * Spotlights<a name="endpoints-spotlights"></a>
   * [`api.spotlights`](https://tybug.github.io/ossapi/spotlights.html#ossapi.ossapiv2.Ossapi.spotlights)
 * Users<a name="endpoints-users"></a>
   * [`api.user`](https://tybug.github.io/ossapi/users.html#ossapi.ossapiv2.Ossapi.user)
   * [`api.user_beatmaps`](https://tybug.github.io/ossapi/users.html#ossapi.ossapiv2.Ossapi.user_beatmaps)
```

### Comparing `ossapi-3.4.4/README.md` & `ossapi-4.0.0b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 ossapi is the definitive python wrapper for the osu! api. ossapi has complete coverage of [api v2](https://osu.ppy.sh/docs/index.html) and [api v1](https://github.com/ppy/osu-api/wiki), and provides both sync (`Ossapi`) and async (`OssapiAsync`) versions for api v2.
 
 If you need support or would like to contribute, feel free to ask in the `#ossapi` channel of the [circleguard discord](https://discord.gg/e84qxkQ).
 
 * [Installation](#installation)
 * [Quickstart](#quickstart)
 * [Async](#async)
-* [Lazer](#lazer)
 * [Endpoints](#endpoints)
   * [Beatmap Packs](#endpoints-beatmap-packs)
   * [Beatmaps](#endpoints-beatmaps)
   * [Beatmapsets](#endpoints-beatmapsets)
   * [Changelog](#endpoints-changelog)
   * [Chat](#endpoints-chat)
   * [Comments](#endpoints-comments)
@@ -26,14 +25,15 @@
   * [Rankings](#endpoints-rankings)
   * [Rooms](#endpoints-rooms)
   * [Scores](#endpoints-scores)
   * [Seasonal Backgrounds](#endpoints-seasonal-backgrounds)
   * [Spotlights](#endpoints-spotlights)
   * [Users](#endpoints-users)
   * [Wiki](#endpoints-wiki)
+* [Other domains](#other-domains)
 * [API v1 Usage](#api-v1-usage)
 
 
 ## Installation
 
 To install:
 
@@ -81,26 +81,26 @@
     await api.user("tybug")
 
 asyncio.run(main())
 ```
 
 [Read more about OssapiAsync on the docs.](https://tybug.github.io/ossapi/async.html)
 
-## Lazer
+## Other domains
 
-You can retrieve lazer-specific data (scores, leaderboards, etc) with ossapi:
+You can use ossapi to interact with the api of other deployments of the osu website, such as https://dev.ppy.sh.
 
 ```python
 from ossapi import Ossapi
 
-api_lazer = Ossapi(client_id, client_secret, domain="lazer")
-
-# best score on the lazer server (lazer + osu scores combined)
-scores = api_lazer.user_scores(12092800, "best")
-print(scores[0].pp)
+api = Ossapi(client_id, client_secret, domain="dev")
+# get the dev server pp leaderboards
+ranking = api.ranking("osu", "performance").ranking
+# pearline06, as of 2023
+print(ranking[0].user.username)
 ```
 
 [Read more about domains on the docs.](https://tybug.github.io/ossapi/domains.html)
 
 ## Endpoints
 
 All endpoints for api v2.
@@ -160,14 +160,15 @@
   * [`api.multiplayer_scores`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.multiplayer_scores)
   * [`api.room`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.room)
   * [`api.room_leaderboard`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.room_leaderboard)
   * [`api.rooms`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.rooms)
 * Scores<a name="endpoints-scores"></a>
   * [`api.download_score`](https://tybug.github.io/ossapi/scores.html#ossapi.ossapiv2.Ossapi.download_score)
   * [`api.score`](https://tybug.github.io/ossapi/scores.html#ossapi.ossapiv2.Ossapi.score)
+  * [`api.score_mode`](https://tybug.github.io/ossapi/scores.html#ossapi.ossapiv2.Ossapi.score_mode)
 * Seasonal Backgrounds<a name="endpoints-seasonal-backgrounds"></a>
   * [`api.seasonal_backgrounds`](https://tybug.github.io/ossapi/seasonal%20backgrounds.html#ossapi.ossapiv2.Ossapi.seasonal_backgrounds)
 * Spotlights<a name="endpoints-spotlights"></a>
   * [`api.spotlights`](https://tybug.github.io/ossapi/spotlights.html#ossapi.ossapiv2.Ossapi.spotlights)
 * Users<a name="endpoints-users"></a>
   * [`api.user`](https://tybug.github.io/ossapi/users.html#ossapi.ossapiv2.Ossapi.user)
   * [`api.user_beatmaps`](https://tybug.github.io/ossapi/users.html#ossapi.ossapiv2.Ossapi.user_beatmaps)
```

### Comparing `ossapi-3.4.4/ossapi/encoder.py` & `ossapi-4.0.0b1/ossapi/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from json import JSONEncoder
 from datetime import datetime
 from enum import Enum
 
 from ossapi.models import Model
 from ossapi.mod import Mod
 
+
 class ModelEncoder(JSONEncoder):
     def default(self, o):
         if isinstance(o, datetime):
             return 1000 * int(o.timestamp())
         if isinstance(o, Enum):
             return o.value
         if isinstance(o, Mod):
@@ -24,9 +25,8 @@
                 to_serialize[name] = value
             return to_serialize
 
         return super().default(o)
 
 
 def serialize_model(model, ensure_ascii=False, **kwargs):
-    return json.dumps(model, cls=ModelEncoder,  ensure_ascii=ensure_ascii,
-        **kwargs)
+    return json.dumps(model, cls=ModelEncoder, ensure_ascii=ensure_ascii, **kwargs)
```

### Comparing `ossapi-3.4.4/ossapi/enums.py` & `ossapi-4.0.0b1/ossapi/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from typing import Optional, List, Any
 
-from ossapi.utils import (EnumModel, Datetime, Model, Field, IntFlagModel)
+from ossapi.utils import EnumModel, Datetime, Model, Field, IntFlagModel
 
 # ================
 # Documented Enums
 # ================
 
+
 class ProfilePage(EnumModel):
     ME = "me"
     RECENT_ACTIVITY = "recent_activity"
     BEATMAPS = "beatmaps"
     HISTORICAL = "historical"
     KUDOSU = "kudosu"
     TOP_RANKS = "top_ranks"
     MEDALS = "medals"
 
+
 class GameMode(EnumModel):
-    OSU   = "osu"
+    OSU = "osu"
     TAIKO = "taiko"
     CATCH = "fruits"
     MANIA = "mania"
 
+
 class PlayStyles(IntFlagModel):
     MOUSE = 1
     KEYBOARD = 2
     TABLET = 4
     TOUCH = 8
 
     @classmethod
@@ -46,14 +49,15 @@
             return PlayStyles.KEYBOARD
         if value == "tablet":
             return PlayStyles.TABLET
         if value == "touch":
             return PlayStyles.TOUCH
         return super()._missing_(value)
 
+
 class RankStatus(EnumModel):
     GRAVEYARD = -2
     WIP = -1
     PENDING = 0
     RANKED = 1
     APPROVED = 2
     QUALIFIED = 3
@@ -78,37 +82,40 @@
             return cls(2)
         if value == "qualified":
             return cls(3)
         if value == "loved":
             return cls(4)
         return super()._missing_(value)
 
+
 class UserAccountHistoryType(EnumModel):
     NOTE = "note"
     RESTRICTION = "restriction"
     SILENCE = "silence"
     # TODO undocumented
     TOURNAMENT_BAN = "tournament_ban"
 
+
 class MessageType(EnumModel):
     HYPE = "hype"
     MAPPER_NOTE = "mapper_note"
     PRAISE = "praise"
     PROBLEM = "problem"
     REVIEW = "review"
     SUGGESTION = "suggestion"
 
+
 class BeatmapsetEventType(EnumModel):
-    APPROVE =  "approve"
+    APPROVE = "approve"
     BEATMAP_OWNER_CHANGE = "beatmap_owner_change"
-    DISCUSSION_DELETE =  "discussion_delete"
-    DISCUSSION_LOCK =  "discussion_lock"
-    DISCUSSION_POST_DELETE =  "discussion_post_delete"
-    DISCUSSION_POST_RESTORE =  "discussion_post_restore"
-    DISCUSSION_RESTORE =  "discussion_restore"
+    DISCUSSION_DELETE = "discussion_delete"
+    DISCUSSION_LOCK = "discussion_lock"
+    DISCUSSION_POST_DELETE = "discussion_post_delete"
+    DISCUSSION_POST_RESTORE = "discussion_post_restore"
+    DISCUSSION_RESTORE = "discussion_restore"
     DISCUSSION_UNLOCK = "discussion_unlock"
     DISQUALIFY = "disqualify"
     DISQUALIFY_LEGACY = "disqualify_legacy"
     GENRE_EDIT = "genre_edit"
     ISSUE_REOPEN = "issue_reopen"
     ISSUE_RESOLVE = "issue_resolve"
     KUDOSU_ALLOW = "kudosu_allow"
@@ -123,39 +130,45 @@
     NOMINATION_RESET = "nomination_reset"
     NOMINATION_RESET_RECEIVED = "nomination_reset_received"
     QUALIFY = "qualify"
     RANK = "rank"
     REMOVE_FROM_LOVED = "remove_from_loved"
     NSFW_TOGGLE = "nsfw_toggle"
 
+
 class BeatmapsetDownload(EnumModel):
     ALL = "all"
     NO_VIDEO = "no_video"
     DIRECT = "direct"
 
+
 class UserListFilters(EnumModel):
     ALL = "all"
     ONLINE = "online"
     OFFLINE = "offline"
 
+
 class UserListSorts(EnumModel):
     LAST_VISIT = "last_visit"
     RANK = "rank"
     USERNAME = "username"
 
+
 class UserListViews(EnumModel):
     CARD = "card"
     LIST = "list"
     BRICK = "brick"
 
+
 class KudosuAction(EnumModel):
     GIVE = "vote.give"
     RESET = "vote.reset"
     REVOKE = "vote.revoke"
 
+
 class EventType(EnumModel):
     ACHIEVEMENT = "achievement"
     BEATMAP_PLAYCOUNT = "beatmapPlaycount"
     BEATMAPSET_APPROVE = "beatmapsetApprove"
     BEATMAPSET_DELETE = "beatmapsetDelete"
     BEATMAPSET_REVIVE = "beatmapsetRevive"
     BEATMAPSET_UPDATE = "beatmapsetUpdate"
@@ -163,66 +176,75 @@
     RANK = "rank"
     RANK_LOST = "rankLost"
     USER_SUPPORT_FIRST = "userSupportFirst"
     USER_SUPPORT_AGAIN = "userSupportAgain"
     USER_SUPPORT_GIFT = "userSupportGift"
     USERNAME_CHANGE = "usernameChange"
 
+
 # used for `EventType.BEATMAPSET_APPROVE`
 class BeatmapsetApproval(EnumModel):
     RANKED = "ranked"
     APPROVED = "approved"
     QUALIFIED = "qualified"
     LOVED = "loved"
 
+
 class ForumTopicType(EnumModel):
     NORMAL = "normal"
     STICKY = "sticky"
     ANNOUNCEMENT = "announcement"
 
+
 class ChangelogMessageFormat(EnumModel):
     HTML = "html"
     MARKDOWN = "markdown"
 
+
 # ==================
 # Undocumented Enums
 # ==================
 
+
 class UserRelationType(EnumModel):
     # undocumented
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/
     # UserRelationTransformer.php#L20
     FRIEND = "friend"
     BLOCK = "block"
 
+
 class Grade(EnumModel):
     SSH = "XH"
     SS = "X"
     SH = "SH"
     S = "S"
     A = "A"
     B = "B"
     C = "C"
     D = "D"
     F = "F"
 
+
 class RoomType(EnumModel):
     # https://github.com/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b2d43
     # 0a2/resources/js/interfaces/room-json.ts#L10
     PLAYLISTS = "playlists"
     HEAD_TO_HEAD = "head_to_head"
     TEAM_VERSUS = "team_versus"
 
+
 class RoomCategory(EnumModel):
     # https://github.com/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b2d
     # 430a2/resources/js/interfaces/room-json.ts#L7
     NORMAL = "normal"
     SPOTLIGHT = "spotlight"
     FEATURED_ARTIST = "featured_artist"
 
+
 class MatchEventType(EnumModel):
     # https://github.dev/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b2
     # d430a2/app/Models/LegacyMatch/Event.php#L30
     PLAYER_LEFT = "player-left"
     PLAYER_JOINED = "player-joined"
     PLAYER_KICKED = "player-kicked"
     MATCH_CREATED = "match-created"
@@ -235,138 +257,159 @@
     # https://github.com/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b2d4
     # 30a2/app/Models/LegacyMatch/Game.php#L40
     SCORE = "score"
     ACCURACY = "accuracy"
     COMBO = "combo"
     SCORE_V2 = "scorev2"
 
+
 class TeamType(EnumModel):
     # https://github.com/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b2d43
     # 0a2/app/Models/LegacyMatch/Game.php#L47
     HEAD_TO_HEAD = "head-to-head"
     TAG_COOP = "tag-coop"
     TEAM_VS = "team-vs"
     TAG_TEAM_VS = "tag-team-vs"
 
+
 class Variant(EnumModel):
     # can't start a python identifier with an integer
     KEY_4 = "4k"
     KEY_7 = "7k"
 
 
 # ===============
 # Parameter Enums
 # ===============
 
+
 class ScoreType(EnumModel):
     BEST = "best"
     FIRSTS = "firsts"
     RECENT = "recent"
 
+
 class RankingFilter(EnumModel):
     ALL = "all"
     FRIENDS = "friends"
 
+
 class RankingType(EnumModel):
     CHARTS = "charts"
     COUNTRY = "country"
     PERFORMANCE = "performance"
     SCORE = "score"
 
+
 class UserLookupKey(EnumModel):
     ID = "id"
     USERNAME = "username"
 
+
 class UserBeatmapType(EnumModel):
     FAVOURITE = "favourite"
     GRAVEYARD = "graveyard"
     LOVED = "loved"
     MOST_PLAYED = "most_played"
     RANKED = "ranked"
     PENDING = "pending"
     GUEST = "guest"
     NOMINATED = "nominated"
 
+
 class BeatmapDiscussionPostSort(EnumModel):
     NEW = "id_desc"
     OLD = "id_asc"
 
+
 class BeatmapsetStatus(EnumModel):
     ALL = "all"
     RANKED = "ranked"
     QUALIFIED = "qualified"
     DISQUALIFIED = "disqualified"
     NEVER_QUALIFIED = "never_qualified"
 
+
 class ChannelType(EnumModel):
     PUBLIC = "PUBLIC"
     PRIVATE = "PRIVATE"
     MULTIPLAYER = "MULTIPLAYER"
     SPECTATOR = "SPECTATOR"
     TEMPORARY = "TEMPORARY"
     PM = "PM"
     GROUP = "GROUP"
     ANNOUNCE = "ANNOUNCE"
 
+
 class CommentableType(EnumModel):
     NEWS_POST = "news_post"
     CHANGELOG = "build"
     BEATMAPSET = "beatmapset"
 
+
 class CommentSort(EnumModel):
     NEW = "new"
     OLD = "old"
     TOP = "top"
 
+
 class ForumTopicSort(EnumModel):
     NEW = "id_desc"
     OLD = "id_asc"
 
+
 class SearchMode(EnumModel):
     ALL = "all"
     USERS = "user"
     WIKI = "wiki_page"
 
+
 class MultiplayerScoresSort(EnumModel):
     NEW = "score_desc"
     OLD = "score_asc"
 
+
 class BeatmapsetDiscussionVote(EnumModel):
     UPVOTE = 1
     DOWNVOTE = -1
 
+
 class BeatmapsetDiscussionVoteSort(EnumModel):
     NEW = "id_desc"
     OLD = "id_asc"
 
+
 class BeatmapsetSearchCategory(EnumModel):
     ANY = "any"
     HAS_LEADERBOARD = "leaderboard"
     RANKED = "ranked"
     QUALIFIED = "qualified"
     LOVED = "loved"
     FAVOURITES = "favourites"
     PENDING = "pending"
     WIP = "wip"
     GRAVEYARD = "graveyard"
     MY_MAPS = "mine"
 
+
 class BeatmapsetSearchMode(EnumModel):
     # made up value. this is the default option and doesn't cause a value to
     # appear in the query string.
     ANY = -1
     OSU = 0
     TAIKO = 1
     CATCH = 2
     MANIA = 3
 
+
 class BeatmapsetSearchExplicitContent(EnumModel):
     HIDE = "hide"
     SHOW = "show"
 
+
 class BeatmapsetSearchGenre(EnumModel):
     # default option, made up value
     ANY = 0
     UNSPECIFIED = 1
     VIDEO_GAME = 2
     ANIME = 3
     ROCK = 4
@@ -376,14 +419,15 @@
     HIP_HOP = 9
     ELECTRONIC = 10
     METAL = 11
     CLASSICAL = 12
     FOLK = 13
     JAZZ = 14
 
+
 class BeatmapsetSearchLanguage(EnumModel):
     # default option, made up value
     ANY = 0
     UNSPECIFIED = 1
     ENGLISH = 2
     JAPANESE = 3
     CHINESE = 4
@@ -394,14 +438,15 @@
     SWEDISH = 9
     SPANISH = 10
     ITALIAN = 11
     RUSSIAN = 12
     POLISH = 13
     OTHER = 14
 
+
 class BeatmapsetSearchSort(EnumModel):
     TITLE_DESCENDING = "title_desc"
     TITLE_ASCENDING = "title_asc"
 
     ARTIST_DESCENDING = "artist_desc"
     ARTIST_ASCENDING = "artist_asc"
 
@@ -421,75 +466,83 @@
     FAVORITES_ASCENDING = "favourites_asc"
 
 
 class NewsPostKey(EnumModel):
     SLUG = "slug"
     ID = "id"
 
+
 # `RoomType` is already taken as a model name (and more appropriate elsewhere)
 class RoomSearchMode(EnumModel):
     ACTIVE = "active"
     ALL = "all"
     ENDED = "ended"
     PARTICIPATED = "participated"
     OWNED = "owned"
 
+
 class EventsSort(EnumModel):
     NEW = "id_desc"
     OLD = "id_asc"
 
+
 class BeatmapPackType(EnumModel):
     STANDARD = "standard"
     FEATURED = "featured"
     TOURNAMENT = "tournament"
     LOVED = "loved"
     CHART = "chart"
     THEME = "theme"
     ARTIST = "artist"
 
 
 # =================
 # Documented Models
 # =================
 
+
 class Failtimes(Model):
     exit: Optional[List[int]]
     fail: Optional[List[int]]
 
+
 class Ranking(Model):
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/CountryTransformer.php#L30
     active_users: int
     play_count: int
     ranked_score: int
     performance: int
 
+
 class Country(Model):
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/CountryTransformer.php#L10
     code: str
     name: str
 
     # optional fields
     # ---------------
     display: Optional[int]
     ranking: Optional[Ranking]
 
+
 class Cover(Model):
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserCompactTransformer.php#L158
     custom_url: Optional[str]
     url: str
     # api should really return an int here instead...open an issue?
     id: Optional[str]
 
 
 class ProfileBanner(Model):
     id: int
     tournament_id: int
     image: str
     image_2x: str = Field(name="image@2x")
 
+
 class UserAccountHistory(Model):
     description: Optional[str]
     id: int
     length: int
     permanent: bool
     timestamp: Datetime
     type: UserAccountHistoryType
@@ -498,209 +551,245 @@
 class UserBadge(Model):
     awarded_at: Datetime
     description: str
     image_url: str
     image_2x_url: str = Field(name="image@2x_url")
     url: str
 
+
 class GroupDescription(Model):
     html: str
     markdown: str
 
+
 class UserGroup(Model):
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserGroupTransformer.php#L10
     id: int
     identifier: str
     name: str
     short_name: str
     colour: Optional[str]
     description: Optional[GroupDescription]
     playmodes: Optional[List[GameMode]]
     is_probationary: bool
     has_listing: bool
     has_playmodes: bool
 
+
 class Covers(Model):
     """
     https://osu.ppy.sh/docs/index.html#beatmapsetcompact-covers
     """
+
     cover: str
     cover_2x: str = Field(name="cover@2x")
     card: str
     card_2x: str = Field(name="card@2x")
     list: str
     list_2x: str = Field(name="list@2x")
     slimcover: str
     slimcover_2x: str = Field(name="slimcover@2x")
 
+
 class Statistics(Model):
-    count_50: int
-    count_100: int
-    count_300: int
-    count_geki: int
-    count_katu: int
-    count_miss: int
+    # I think any of these attributes can be null if the corresponding gamemode
+    # doesn't have the judgment as a possible judgement. eg taiko doesn't have 50s
+    # and catch doesn't have geki.
+    count_50: Optional[int]
+    count_100: Optional[int]
+    count_300: Optional[int]
+    count_geki: Optional[int]
+    count_katu: Optional[int]
+    count_miss: Optional[int]
+
 
 class Availability(Model):
     download_disabled: bool
     more_information: Optional[str]
 
+
 class Hype(Model):
     current: int
     required: int
 
+
 class Nominations(Model):
     current: int
     required: int
 
+
 class Nomination(Model):
     beatmapset_id: int
     rulesets: List[GameMode]
     reset: bool
     user_id: int
 
+
 class Kudosu(Model):
     total: int
     available: int
 
+
 class KudosuGiver(Model):
     url: str
     username: str
 
+
 class KudosuPost(Model):
     url: Optional[str]
     # will be "[deleted beatmap]" for deleted beatmaps. See
     # https://osu.ppy.sh/docs/index.html#kudosuhistory
     title: str
 
+
 class KudosuVote(Model):
     user_id: int
     score: int
 
     def user(self):
         return self._fk_user(self.user_id)
 
+
 class EventUser(Model):
     username: str
     url: str
     previousUsername: Optional[str]
 
+
 class EventBeatmap(Model):
     title: str
     url: str
 
+
 class EventBeatmapset(Model):
     title: str
     url: str
 
+
 class EventAchivement(Model):
     icon_url: str
     id: int
     name: str
     # TODO `grouping` can probably be enumified (example value: "Dedication"),
     # need to find full list first though
     grouping: str
     ordering: int
     slug: str
     description: str
     mode: Optional[GameMode]
     instructions: Optional[Any]
 
+
 class GithubUser(Model):
     display_name: str
     github_username: Optional[str]
     github_url: Optional[str]
     id: Optional[int]
     osu_username: Optional[str]
     user_id: Optional[int]
     user_url: Optional[str]
 
     def user(self):
         return self._fk_user(self.user_id)
 
+
 class ChangelogSearch(Model):
     from_: Optional[str] = Field(name="from")
     limit: int
     max_id: Optional[int]
     stream: Optional[str]
     to: Optional[str]
 
+
 class NewsSearch(Model):
     limit: int
     sort: str
     # undocumented
     year: Optional[int]
 
+
 class ForumPostBody(Model):
     html: str
     raw: str
 
+
 class ForumPollText(Model):
     bbcode: str
     html: str
 
+
 class ForumPollTitle(Model):
     bbcode: str
     html: str
 
+
 class ReviewsConfig(Model):
     max_blocks: int
 
+
 class RankHighest(Model):
     rank: int
     updated_at: Datetime
 
+
 class BeatmapPackUserCompletionData(Model):
     beatmapset_ids: List[int]
     completed: bool
 
 
 # ===================
 # Undocumented Models
 # ===================
 
+
 class UserMonthlyPlaycount(Model):
     # undocumented
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserMonthlyPlaycountTransformer.php
     start_date: Datetime
     count: int
 
+
 class UserPage(Model):
     # undocumented (and not a class on osu-web)
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserCompactTransformer.php#L270
     html: str
     raw: str
 
+
 class UserLevel(Model):
     # undocumented (and not a class on osu-web)
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserStatisticsTransformer.php#L27
     current: int
     progress: int
 
+
 class UserGradeCounts(Model):
     # undocumented (and not a class on osu-web)
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserStatisticsTransformer.php#L43
     ss: int
     ssh: int
     s: int
     sh: int
     a: int
 
+
 class UserReplaysWatchedCount(Model):
     # undocumented
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserReplaysWatchedCountTransformer.php
     start_date: Datetime
     count: int
 
+
 class UserAchievement(Model):
     # undocumented
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserAchievementTransformer.php#L10
     achieved_at: Datetime
     achievement_id: int
 
+
 class UserProfileCustomization(Model):
     # undocumented
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserCompactTransformer.php#L363
     # https://github.com/ppy/osu-web/blob/master/app/Models/UserProfileCustomization.php
     audio_autoplay: Optional[bool]
     audio_muted: Optional[bool]
     audio_volume: Optional[int]
@@ -710,16 +799,18 @@
     comments_show_deleted: Optional[bool]
     forum_posts_show_deleted: bool
     ranking_expanded: bool
     user_list_filter: Optional[UserListFilters]
     user_list_sort: Optional[UserListSorts]
     user_list_view: Optional[UserListViews]
 
+
 class RankHistory(Model):
     # undocumented
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/RankHistoryTransformer.php
     mode: GameMode
     data: List[int]
 
+
 class Weight(Model):
     percentage: float
     pp: float
```

### Comparing `ossapi-3.4.4/ossapi/mod.py` & `ossapi-4.0.0b1/ossapi/mod.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.4.4/ossapi/models.py` & `ossapi-4.0.0b1/ossapi/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,75 @@
 # https://docs.python.org/3.7/whatsnew/3.7.html#pep-563-postponed-evaluation-
 # of-annotations
 from __future__ import annotations
 from typing import Optional, TypeVar, Generic, Any, List, Union, Dict
 from dataclasses import dataclass
 
 from ossapi.mod import Mod
-from ossapi.enums import (UserAccountHistory, ProfileBanner, UserBadge, Country,
-    Cover, UserGroup, UserMonthlyPlaycount, UserPage, UserReplaysWatchedCount,
-    UserAchievement, UserProfileCustomization, RankHistory, Kudosu, PlayStyles,
-    ProfilePage, GameMode, RankStatus, Failtimes, Covers, Hype, Availability,
-    Nominations, Statistics, Grade, Weight, MessageType, KudosuAction,
-    KudosuGiver, KudosuPost, EventType, EventAchivement, EventUser,
-    EventBeatmap, BeatmapsetApproval, EventBeatmapset, KudosuVote,
-    BeatmapsetEventType, UserRelationType, UserLevel, UserGradeCounts,
-    GithubUser, ChangelogSearch, ForumTopicType, ForumPostBody, ForumTopicSort,
-    ChannelType, ReviewsConfig, NewsSearch, Nomination, RankHighest, RoomType,
-    RoomCategory, MatchEventType, ScoringType, TeamType, Variant, ForumPollText,
-    ForumPollTitle, BeatmapPackUserCompletionData)
+from ossapi.enums import (
+    UserAccountHistory,
+    ProfileBanner,
+    UserBadge,
+    Country,
+    Cover,
+    UserGroup,
+    UserMonthlyPlaycount,
+    UserPage,
+    UserReplaysWatchedCount,
+    UserAchievement,
+    UserProfileCustomization,
+    RankHistory,
+    Kudosu,
+    PlayStyles,
+    ProfilePage,
+    GameMode,
+    RankStatus,
+    Failtimes,
+    Covers,
+    Hype,
+    Availability,
+    Nominations,
+    Statistics,
+    Grade,
+    Weight,
+    MessageType,
+    KudosuAction,
+    KudosuGiver,
+    KudosuPost,
+    EventType,
+    EventAchivement,
+    EventUser,
+    EventBeatmap,
+    BeatmapsetApproval,
+    EventBeatmapset,
+    KudosuVote,
+    BeatmapsetEventType,
+    UserRelationType,
+    UserLevel,
+    UserGradeCounts,
+    GithubUser,
+    ChangelogSearch,
+    ForumTopicType,
+    ForumPostBody,
+    ForumTopicSort,
+    ChannelType,
+    ReviewsConfig,
+    NewsSearch,
+    Nomination,
+    RankHighest,
+    RoomType,
+    RoomCategory,
+    MatchEventType,
+    ScoringType,
+    TeamType,
+    Variant,
+    ForumPollText,
+    ForumPollTitle,
+    BeatmapPackUserCompletionData,
+)
 from ossapi.utils import Datetime, Model, BaseModel, Field
 
 T = TypeVar("T")
 S = TypeVar("S")
 
 """
 a type hint of ``Optional[Any]`` or ``Any`` means that I don't know what type it
@@ -52,14 +101,15 @@
 # This is essentially a reimplementation of SimpleNamespace to deal with
 # BaseModels being passed the data as a single dict (`_data`) instead of as
 # **kwargs, plus some other weird stuff we're doing like handling cursor
 # objects being passed as data
 # We want cursors to also be instantiatable manually (eg `Cursor(page=199)`),
 # so make `_data` optional and also allow arbitrary `kwargs`.
 
+
 class Cursor(BaseModel):
     def __init__(self, _data=None, **kwargs):
         super().__init__()
         # allow Cursor to be instantiated with another cursor as a no-op
         if isinstance(_data, Cursor):
             _data = _data.__dict__
         _data = _data or kwargs
@@ -69,24 +119,28 @@
         keys = sorted(self.__dict__)
         items = (f"{k}={self.__dict__[k]!r}" for k in keys)
         return f"{type(self).__name__}({', '.join(items)})"
 
     def __eq__(self, other):
         return self.__dict__ == other.__dict__
 
+
 # if there are no more results, a null cursor is returned instead.
 # So always let the cursor be nullable to catch this. It's the user's
 # responsibility to check for a null cursor to see if there are any more
 # results.
 CursorT = Optional[Cursor]
+CursorStringT = Optional[str]
+
 
 class UserCompact(Model):
     """
     https://osu.ppy.sh/docs/index.html#usercompact
     """
+
     # required fields
     # ---------------
     avatar_url: str
     country_code: str
     id: int
     is_active: bool
     is_bot: bool
@@ -141,18 +195,18 @@
     # deprecated, replaced by pending_beatmapset_count
     unranked_beatmapset_count: Optional[int]
     unread_pm_count: Optional[int]
     user_achievements: Optional[List[UserAchievement]]
     user_preferences: Optional[UserProfileCustomization]
     session_verified: Optional[bool]
 
-
     def expand(self) -> User:
         return self._fk_user(self.id)
 
+
 class User(UserCompact):
     comments_count: int
     cover_url: str
     discord: Optional[str]
     has_supported: bool
     interests: Optional[str]
     join_date: Datetime
@@ -200,16 +254,16 @@
     def expand(self) -> Beatmap:
         return self._fk_beatmap(self.id)
 
     def user(self) -> User:
         return self._fk_user(self.user_id)
 
     def beatmapset(self) -> Union[Beatmapset, BeatmapsetCompact]:
-        return self._fk_beatmapset(self.beatmapset_id,
-            existing=self._beatmapset)
+        return self._fk_beatmapset(self.beatmapset_id, existing=self._beatmapset)
+
 
 class Beatmap(BeatmapCompact):
     total_length: int
     version: str
     accuracy: float
     ar: float
     bpm: Optional[float]
@@ -239,22 +293,22 @@
     # -----------------
     _beatmapset: Optional[Beatmapset] = Field(name="beatmapset")
 
     def expand(self) -> Beatmap:
         return self
 
     def beatmapset(self) -> Beatmapset:
-        return self._fk_beatmapset(self.beatmapset_id,
-            existing=self._beatmapset)
+        return self._fk_beatmapset(self.beatmapset_id, existing=self._beatmapset)
 
 
 class BeatmapsetCompact(Model):
     """
     https://osu.ppy.sh/docs/index.html#beatmapsetcompact
     """
+
     # required fields
     # ---------------
     artist: str
     artist_unicode: str
     covers: Covers
     creator: str
     favourite_count: int
@@ -296,14 +350,15 @@
 
     def expand(self) -> Beatmapset:
         return self._fk_beatmapset(self.id)
 
     def user(self) -> Union[UserCompact, User]:
         return self._fk_user(self.user_id, existing=self._user)
 
+
 class Beatmapset(BeatmapsetCompact):
     availability: Availability
     bpm: float
     can_be_hyped: bool
     deleted_at: Optional[Datetime]
     discussion_enabled: bool
     discussion_locked: bool
@@ -316,24 +371,27 @@
     storyboard: bool
     submitted_date: Optional[Datetime]
     tags: str
 
     def expand(self) -> Beatmapset:
         return self
 
+
 # undocumented, but defined here to avoid a forward reference in Score.
 class ScoreMatchInfo(Model):
     slot: int
     team: str
     pass_: bool = Field(name="pass")
 
+
 class Score(Model):
     """
     https://osu.ppy.sh/docs/index.html#score
     """
+
     # can be null for match scores, eg the scores
     # in https://osu.ppy.sh/community/matches/97947404
     id: Optional[int]
     best_id: Optional[int]
     user_id: int
     accuracy: float
     mods: Mod
@@ -369,21 +427,24 @@
 
     def user(self) -> Union[UserCompact, User]:
         return self._fk_user(self.user_id, existing=self._user)
 
     def download(self):
         return self._api.download_score(self.mode, self.id)
 
+
 class BeatmapUserScore(Model):
     position: int
     score: Score
 
+
 class BeatmapUserScores(Model):
     scores: List[Score]
 
+
 class BeatmapScores(Model):
     scores: List[Score]
     userScore: Optional[BeatmapUserScore]
 
 
 class CommentableMeta(Model):
     # title is the only attribute returned for deleted commentables.
@@ -391,17 +452,19 @@
     title: str
     type: Optional[str]
     url: Optional[str]
     owner_id: Optional[int]
     owner_title: Optional[str]
     current_user_attributes: Optional[CommentableMetaCurrentUserAttributes]
 
+
 class CommentableMetaCurrentUserAttributes(Model):
     can_new_comment_reason: Optional[str]
 
+
 class Comment(Model):
     # null for deleted commentables, eg on /comments/3.
     commentable_id: Optional[int]
     # null for deleted commentables, eg on /comments/3.
     commentable_type: Optional[str]
     created_at: Datetime
     deleted_at: Optional[Datetime]
@@ -421,14 +484,15 @@
 
     def user(self) -> User:
         return self._fk_user(self.user_id)
 
     def edited_by(self) -> Optional[User]:
         return self._fk_user(self.edited_by_id)
 
+
 class CommentBundle(Model):
     commentable_meta: List[CommentableMeta]
     comments: List[Comment]
     cursor: CursorT
     has_more: bool
     has_more_id: Optional[int]
     included_comments: List[Comment]
@@ -437,14 +501,15 @@
     sort: str
     top_level_count: Optional[int]
     total: Optional[int]
     user_follow: bool
     user_votes: List[int]
     users: List[UserCompact]
 
+
 class ForumPost(Model):
     created_at: Datetime
     deleted_at: Optional[Datetime]
     edited_at: Optional[Datetime]
     edited_by_id: Optional[int]
     forum_id: int
     id: int
@@ -454,14 +519,15 @@
 
     def user(self) -> User:
         return self._fk_user(self.user_id)
 
     def edited_by(self) -> Optional[User]:
         return self._fk_user(self.edited_by_id)
 
+
 class ForumTopic(Model):
     created_at: Datetime
     deleted_at: Optional[Datetime]
     first_post_id: int
     forum_id: int
     id: int
     is_locked: bool
@@ -472,97 +538,112 @@
     updated_at: Datetime
     user_id: int
     poll: Optional[ForumPollModel]
 
     def user(self) -> User:
         return self._fk_user(self.user_id)
 
+
 class ForumPollModel(Model):
     allow_vote_change: bool
     ended_at: Optional[Datetime]
     hide_incomplete_results: bool
     last_vote_at: Optional[Datetime]
     max_votes: int
     options: List[ForumPollOption]
     started_at: Datetime
     title: ForumPollTitle
     total_vote_count: int
 
+
 class ForumPollOption(Model):
     id: int
     text: ForumPollText
     vote_count: Optional[int]
 
+
 class ForumTopicAndPosts(Model):
     cursor: CursorT
     search: ForumTopicSearch
     posts: List[ForumPost]
     topic: ForumTopic
-    cursor_string: Optional[str]
+    cursor_string: CursorStringT
+
 
 class CreateForumTopicResponse(Model):
     post: ForumPost
     topic: ForumTopic
 
+
 class ForumTopicSearch(Model):
     sort: Optional[ForumTopicSort]
     limit: Optional[int]
     start: Optional[int]
     end: Optional[int]
 
+
 class SearchResult(Generic[T], Model):
     data: List[T]
     total: int
 
+
 class WikiPage(Model):
     layout: str
     locale: str
     markdown: str
     path: str
     subtitle: Optional[str]
     tags: List[str]
     title: str
     available_locales: List[str]
 
+
 class Search(Model):
     users: Optional[SearchResult[UserCompact]] = Field(name="user")
     wiki_pages: Optional[SearchResult[WikiPage]] = Field(name="wiki_page")
 
+
 class Spotlight(Model):
     end_date: Datetime
     id: int
     mode_specific: bool
     participant_count: Optional[int]
     name: str
     start_date: Datetime
     type: str
 
+
 class Spotlights(Model):
     spotlights: List[Spotlight]
 
+
 # return-value wrapper for https://osu.ppy.sh/docs/index.html#get-users.
 class Users(Model):
     users: List[UserCompact]
 
+
 # return-value wrapper for https://osu.ppy.sh/docs/index.html#get-beatmaps.
 class Beatmaps(Model):
     beatmaps: List[Beatmap]
 
+
 class BeatmapPacks(Model):
     cursor: CursorT
-    cursor_string: str
+    cursor_string: CursorStringT
     beatmap_packs: List[BeatmapPack]
 
+
 class Rankings(Model):
     beatmapsets: Optional[List[Beatmapset]]
     cursor: CursorT
     ranking: Union[List[UserStatistics], List[CountryStatistics]]
     spotlight: Optional[Spotlight]
     total: int
 
+
 class BeatmapsetDiscussionPost(Model):
     id: int
     beatmapset_discussion_id: int
     user_id: int
     last_editor_id: Optional[int]
     deleted_by_id: Optional[int]
     system: bool
@@ -576,14 +657,15 @@
 
     def last_editor(self) -> Optional[User]:
         return self._fk_user(self.last_editor_id)
 
     def deleted_by(self) -> Optional[User]:
         return self._fk_user(self.deleted_by_id)
 
+
 class BeatmapsetDiscussion(Model):
     id: int
     beatmapset_id: int
     beatmap_id: Optional[int]
     user_id: int
     deleted_by_id: Optional[int]
     message_type: MessageType
@@ -607,47 +689,49 @@
     def user(self) -> User:
         return self._fk_user(self.user_id)
 
     def deleted_by(self) -> Optional[User]:
         return self._fk_user(self.deleted_by_id)
 
     def beatmapset(self) -> Union[Beatmapset, BeatmapsetCompact]:
-        return self._fk_beatmapset(self.beatmapset_id,
-            existing=self._beatmapset)
+        return self._fk_beatmapset(self.beatmapset_id, existing=self._beatmapset)
 
     def beatmap(self) -> Union[Optional[Beatmap], BeatmapCompact]:
         return self._fk_beatmap(self.beatmap_id, existing=self._beatmap)
 
+
 class BeatmapsetDiscussionVote(Model):
     id: int
     score: int
     user_id: int
     beatmapset_discussion_id: int
     created_at: Datetime
     updated_at: Datetime
     # TODO is this field ever actually returned? not documented and can't find
     # a repro case.
-    cursor_string: Optional[str]
+    cursor_string: CursorStringT
 
     def user(self):
         return self._fk_user(self.user_id)
 
+
 class KudosuHistory(Model):
     id: int
     action: KudosuAction
     amount: int
     # TODO enumify this. Described as "Object type which the exchange happened
     # on (forum_post, etc)." in https://osu.ppy.sh/docs/index.html#kudosuhistory
     model: str
     created_at: Datetime
     giver: Optional[KudosuGiver]
     post: KudosuPost
     # see https://github.com/ppy/osu-web/issues/7549
     details: Any
 
+
 class BeatmapPlaycount(Model):
     beatmap_id: int
     _beatmap: Optional[BeatmapCompact] = Field(name="beatmap")
     beatmapset: Optional[BeatmapsetCompact]
     count: int
 
     def beatmap(self) -> Union[Beatmap, BeatmapCompact]:
@@ -668,100 +752,118 @@
             EventType.BEATMAPSET_UPDATE: BeatmapsetUpdateEvent,
             EventType.BEATMAPSET_UPLOAD: BeatmapsetUploadEvent,
             EventType.RANK: RankEvent,
             EventType.RANK_LOST: RankLostEvent,
             EventType.USER_SUPPORT_FIRST: UserSupportFirstEvent,
             EventType.USER_SUPPORT_AGAIN: UserSupportAgainEvent,
             EventType.USER_SUPPORT_GIFT: UserSupportGiftEvent,
-            EventType.USERNAME_CHANGE: UsernameChangeEvent
+            EventType.USERNAME_CHANGE: UsernameChangeEvent,
         }
         type_ = EventType(data["type"])
         return mapping[type_]
 
+
 class Event(Model):
     created_at: Datetime
     createdAt: Datetime
     id: int
     type: EventType
 
+
 class AchievementEvent(Event):
     achievement: EventAchivement
     user: EventUser
 
+
 class BeatmapPlaycountEvent(Event):
     beatmap: EventBeatmap
     count: int
 
+
 class BeatmapsetApproveEvent(Event):
     approval: BeatmapsetApproval
     beatmapset: EventBeatmapset
     user: EventUser
 
+
 class BeatmapsetDeleteEvent(Event):
     beatmapset: EventBeatmapset
 
+
 class BeatmapsetReviveEvent(Event):
     beatmapset: EventBeatmapset
     user: EventUser
 
+
 class BeatmapsetUpdateEvent(Event):
     beatmapset: EventBeatmapset
     user: EventUser
 
+
 class BeatmapsetUploadEvent(Event):
     beatmapset: EventBeatmapset
     user: EventUser
 
+
 class RankEvent(Event):
     scoreRank: str
     rank: int
     mode: GameMode
     beatmap: EventBeatmap
     user: EventUser
 
+
 class RankLostEvent(Event):
     mode: GameMode
     beatmap: EventBeatmap
     user: EventUser
 
+
 class UserSupportFirstEvent(Event):
     user: EventUser
 
+
 class UserSupportAgainEvent(Event):
     user: EventUser
 
+
 class UserSupportGiftEvent(Event):
     user: EventUser
 
+
 class UsernameChangeEvent(Event):
     user: EventUser
 
+
 class Build(Model):
     created_at: Datetime
     display_version: str
     id: int
     update_stream: Optional[UpdateStream]
     users: int
     version: Optional[str]
     changelog_entries: Optional[List[ChangelogEntry]]
     versions: Optional[Versions]
     youtube_id: Optional[str]
 
+
 class Versions(Model):
     next: Optional[Build]
     previous: Optional[Build]
 
+
 class UpdateStream(Model):
     display_name: Optional[str]
     id: int
     is_featured: bool
     name: str
     latest_build: Optional[Build]
     user_count: Optional[int]
 
+
 class ChangelogEntry(Model):
     category: str
     created_at: Optional[Datetime]
     github_pull_request_id: Optional[int]
     github_url: Optional[str]
     id: Optional[int]
     major: bool
@@ -769,26 +871,29 @@
     message_html: Optional[str]
     repository: Optional[str]
     title: Optional[str]
     type: str
     url: Optional[str]
     github_user: GithubUser
 
+
 class ChangelogListing(Model):
     builds: List[Build]
     search: ChangelogSearch
     streams: List[UpdateStream]
 
+
 class MultiplayerScores(Model):
-    cursor_string: str
+    cursor_string: CursorStringT
     params: str
     scores: List[MultiplayerScore]
     total: Optional[int]
     user_score: Optional[MultiplayerScore]
 
+
 class MultiplayerScore(Model):
     id: int
     user_id: int
     room_id: int
     playlist_item_id: int
     beatmap_id: int
     rank: int
@@ -800,58 +905,67 @@
     position: Optional[int]
     scores_around: Optional[MultiplayerScoresAround]
     user: User
 
     def beatmap(self):
         return self._fk_beatmap(self.beatmap_id)
 
+
 class MultiplayerScoresAround(Model):
     higher: List[MultiplayerScore]
     lower: List[MultiplayerScore]
 
+
 class NewsListing(Model):
     cursor: CursorT
-    cursor_string: str
+    cursor_string: CursorStringT
     news_posts: List[NewsPost]
     news_sidebar: NewsSidebar
     search: NewsSearch
 
+
 class NewsPost(Model):
     author: str
     edit_url: str
     first_image: Optional[str]
     id: int
     published_at: Datetime
     slug: str
     title: str
     updated_at: Datetime
     content: Optional[str]
     navigation: Optional[NewsNavigation]
     preview: Optional[str]
 
+
 class NewsNavigation(Model):
     newer: Optional[NewsPost]
     older: Optional[NewsPost]
 
+
 class NewsSidebar(Model):
     current_year: int
     news_posts: List[NewsPost]
     years: List[int]
 
+
 class SeasonalBackgrounds(Model):
     ends_at: Datetime
     backgrounds: List[SeasonalBackground]
 
+
 class SeasonalBackground(Model):
     url: str
     user: UserCompact
 
+
 class DifficultyAttributes(Model):
     attributes: BeatmapDifficultyAttributes
 
+
 class BeatmapDifficultyAttributes(Model):
     max_combo: int
     star_rating: float
 
     # osu attributes
     aim_difficulty: Optional[float]
     approach_rate: Optional[float]
@@ -871,141 +985,160 @@
     # ctb attributes
     approach_rate: Optional[float]
 
     # mania attributes
     great_hit_window: Optional[float]
     score_multiplier: Optional[float]
 
+
 class Events(Model):
     cursor: CursorT
-    cursor_string: str
+    cursor_string: CursorStringT
     events: List[Event] = Field(deserialize_type=List[_Event])
 
+
 class BeatmapPack(Model):
     author: str
     date: Datetime
     name: str
     no_diff_reduction: bool
     # marked as nonnull on docs
     ruleset_id: Optional[int]
     tag: str
     url: str
 
     # optional attributes
     beatmapsets: Optional[List[Beatmapset]]
     user_completion_data: Optional[BeatmapPackUserCompletionData]
 
+
 # ================
 # Parameter Models
 # ================
 
 # models which aren't used for serialization, but passed to OssapiV2 methods.
 
+
 @dataclass
 class ForumPoll:
     options: List[str]
     title: str
 
     # default values taken from https://osu.ppy.sh/docs/index.html#create-topic
     hide_results: bool = False
     length_days: int = 0
     max_options: int = 1
     vote_change: bool = False
 
 
-
 # ===================
 # Undocumented Models
 # ===================
 
+
 class BeatmapsetSearchResult(Model):
     beatmapsets: List[Beatmapset]
     cursor: CursorT
     recommended_difficulty: Optional[float]
     error: Optional[str]
     total: int
     search: Any
     cursor_string: Optional[str]
 
+
 class BeatmapsetDiscussions(Model):
     beatmaps: List[Beatmap]
     cursor: CursorT
     discussions: List[BeatmapsetDiscussion]
     included_discussions: List[BeatmapsetDiscussion]
     reviews_config: ReviewsConfig
     users: List[UserCompact]
     cursor_string: Optional[str]
     beatmapsets: List[Beatmapset]
 
+
 class BeatmapsetDiscussionReview(Model):
     # https://github.com/ppy/osu-web/blob/master/app/Libraries/BeatmapsetDis
     # cussionReview.php
     max_blocks: int
 
+
 class BeatmapsetDiscussionPosts(Model):
     beatmapsets: List[BeatmapsetCompact]
     discussions: List[BeatmapsetDiscussion]
     cursor: CursorT
     posts: List[BeatmapsetDiscussionPost]
     users: List[UserCompact]
     cursor_string: Optional[str]
 
+
 class BeatmapsetDiscussionVotes(Model):
     cursor: CursorT
     discussions: List[BeatmapsetDiscussion]
     votes: List[BeatmapsetDiscussionVote]
     users: List[UserCompact]
     cursor_string: Optional[str]
 
+
 class BeatmapsetEventComment(Model):
     beatmap_discussion_id: int
     beatmap_discussion_post_id: int
 
+
 class BeatmapsetEventCommentNoPost(Model):
     beatmap_discussion_id: int
     beatmap_discussion_post_id: None
 
+
 class BeatmapsetEventCommentNone(Model):
     beatmap_discussion_id: None
     beatmap_discussion_post_id: None
 
 
 class BeatmapsetEventCommentChange(Generic[S], BeatmapsetEventCommentNone):
     old: S
     new: S
 
+
 class BeatmapsetEventCommentLovedRemoval(BeatmapsetEventCommentNone):
     reason: str
 
+
 class BeatmapsetEventCommentKudosuChange(BeatmapsetEventCommentNoPost):
     new_vote: KudosuVote
     votes: List[KudosuVote]
 
+
 class BeatmapsetEventCommentKudosuRecalculate(BeatmapsetEventCommentNoPost):
     new_vote: Optional[KudosuVote]
 
+
 class BeatmapsetEventCommentOwnerChange(BeatmapsetEventCommentNone):
     beatmap_id: int
     beatmap_version: str
     new_user_id: int
     new_user_username: str
 
+
 class BeatmapsetEventCommentNominate(Model):
     # for some reason this comment type doesn't have the normal
     # beatmap_discussion_id and beatmap_discussion_post_id attributes (they're
     # not even null, just missing).
     modes: List[GameMode]
 
+
 class BeatmapsetEventCommentWithNominators(BeatmapsetEventCommentNoPost):
     nominator_ids: Optional[List[int]]
 
+
 class BeatmapsetEventCommentWithSourceUser(BeatmapsetEventCommentNoPost):
     source_user_id: int
     source_user_username: str
 
+
 class BeatmapsetEvent(Model):
     # https://github.com/ppy/osu-web/blob/master/app/Models/BeatmapsetEvent.php
     #
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/BeatmapsetEv
     # entTransformer.php
 
     id: int
@@ -1055,14 +1188,15 @@
         }
         type_ = BeatmapsetEventType(self.type)
         return {"comment": mapping[type_]}
 
     def user(self) -> Optional[User]:
         return self._fk_user(self.user_id)
 
+
 class ChatChannel(Model):
     channel_id: int
     description: Optional[str]
     icon: Optional[str]
     moderated: Optional[bool]
     name: str
     type: ChannelType
@@ -1072,50 +1206,55 @@
     # optional fields
     # ---------------
     last_message_id: Optional[int]
     last_read_id: Optional[int]
     recent_messages: Optional[List[ChatMessage]]
     users: Optional[List[int]]
 
+
 class ChatMessage(Model):
     channel_id: int
     content: str
     is_action: bool
     message_id: int
     sender: UserCompact
     sender_id: int
     timestamp: Datetime
     # TODO enumify, example value: "plain"
     type: str
 
+
 class CountryStatistics(Model):
     code: str
     active_users: int
     play_count: int
     ranked_score: int
     performance: int
     country: Country
 
+
 class CreatePMResponse(Model):
     message: ChatMessage
     new_channel_id: int
 
     # undocumented
     channel: ChatChannel
 
     # documented but not present in response
     presence: Optional[List[ChatChannel]]
 
+
 class ModdingHistoryEventsBundle(Model):
     # https://github.com/ppy/osu-web/blob/master/app/Libraries/ModdingHistor
     # yEventsBundle.php#L84
     events: List[BeatmapsetEvent]
     reviewsConfig: BeatmapsetDiscussionReview
     users: List[UserCompact]
 
+
 class UserRelation(Model):
     # undocumented (and not a class on osu-web)
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserRelatio
     # nTransformer.php#L16
     target_id: int
     relation_type: UserRelationType
     mutual: bool
@@ -1123,21 +1262,23 @@
     # optional fields
     # ---------------
     target: Optional[UserCompact]
 
     def target(self) -> Union[User, UserCompact]:
         return self._fk_user(self.target_id, existing=self.target)
 
+
 class StatisticsVariant(Model):
     mode: GameMode
     variant: Variant
     country_rank: Optional[int]
     global_rank: Optional[int]
     pp: float
 
+
 class UserStatistics(Model):
     count_100: int
     count_300: int
     count_50: int
     count_miss: int
     country_rank: Optional[int]
     grade_counts: UserGradeCounts
@@ -1156,27 +1297,30 @@
     ranked_score: int
     replays_watched_by_others: int
     total_hits: int
     total_score: int
     user: Optional[UserCompact]
     variants: Optional[List[StatisticsVariant]]
 
+
 class UserStatisticsRulesets(Model):
     # undocumented
     # https://github.com/ppy/osu-web/blob/master/app/Transformers/UserStatisti
     # csRulesetsTransformer.php
     osu: Optional[UserStatistics]
     taiko: Optional[UserStatistics]
     fruits: Optional[UserStatistics]
     mania: Optional[UserStatistics]
 
+
 class RoomPlaylistItemMod(Model):
     acronym: str
     settings: Dict[str, Any]
 
+
 class RoomPlaylistItem(Model):
     id: int
     room_id: int
     beatmap_id: int
     ruleset_id: int
     allowed_mods: List[RoomPlaylistItemMod]
     required_mods: List[RoomPlaylistItemMod]
@@ -1184,14 +1328,15 @@
     owner_id: int
     # null for playlist items which haven't finished yet, I think
     playlist_order: Optional[int]
     # null for playlist items which haven't finished yet, I think
     played_at: Optional[Datetime]
     beatmap: BeatmapCompact
 
+
 class Room(Model):
     id: int
     name: str
     category: RoomCategory
     type: RoomType
     user_id: int
     starts_at: Datetime
@@ -1203,43 +1348,49 @@
     has_password: bool
     queue_mode: str
     auto_skip: bool
     host: UserCompact
     playlist: List[RoomPlaylistItem]
     recent_participants: List[UserCompact]
 
+
 class RoomLeaderboardScore(Model):
     accuracy: float
     attempts: int
     completed: int
     pp: float
     room_id: int
     total_score: int
     user_id: int
     user: UserCompact
 
+
 class RoomLeaderboardUserScore(RoomLeaderboardScore):
     position: int
 
+
 class RoomLeaderboard(Model):
     leaderboard: List[RoomLeaderboardScore]
     user_score: RoomLeaderboardUserScore
 
+
 class Match(Model):
     id: int
     start_time: Datetime
     # null for matches which haven't finished yet, I think
     end_time: Optional[Datetime]
     name: str
 
+
 class Matches(Model):
     matches: List[Match]
     cursor: CursorT
     params: Any
-    cursor_string: str
+    cursor_string: CursorStringT
+
 
 class MatchGame(Model):
     id: int
     start_time: Datetime
     # null for in-progress matches.
     end_time: Optional[Datetime]
     mode: GameMode
@@ -1250,44 +1401,49 @@
     # null for deleted beatmaps,
     # e.g. https://osu.ppy.sh/community/matches/103721175.
     # TODO doesn't match docs
     beatmap: Optional[BeatmapCompact]
     beatmap_id: int
     scores: List[Score]
 
+
 class MatchEventDetail(Model):
     type: MatchEventType
     # seems to only be used for MatchEventType.OTHER
     text: Optional[str]
 
+
 class MatchEvent(Model):
     id: int
     detail: MatchEventDetail
     timestamp: Datetime
     # can be none for MatchEventType.OTHER
     user_id: Optional[int]
     game: Optional[MatchGame]
 
+
 class MatchResponse(Model):
     match: Match
     events: List[MatchEvent]
     users: List[UserCompact]
     first_event_id: int
     latest_event_id: int
     current_game_id: Optional[int]
 
 
 # ==================
 # Provisional Models
 # ==================
 
+
 class _NonLegacyBeatmapScores(Model):
     scores: List[_NonLegacyScore]
     userScore: Optional[BeatmapUserScore]
 
+
 class _NonLegacyMod(BaseModel):
     # returned in a new format. e.g.:
     # "mods": [
     #      {
     #          "acronym": "HR"
     #      },
     #      {
@@ -1296,14 +1452,15 @@
     #      {
     #          "acronym": "CL"
     #      }
     #  ],
     def __init__(self, value):
         self.value = value
 
+
 class _NonLegacyStatistics(Model):
     # these values simply aren't present if they are 0. oversight?
     miss: Optional[int]
     meh: Optional[int]
     ok: Optional[int]
     good: Optional[int]
     great: Optional[int]
@@ -1319,28 +1476,29 @@
     large_bonus: Optional[int]
     ignore_miss: Optional[int]
     ignore_hit: Optional[int]
     combo_break: Optional[int]
     slider_tail_hit: Optional[int]
     legacy_combo_increase: Optional[int]
 
+
 class _NonLegacyScore(Model):
     id: Optional[int]
     best_id: Optional[int]
     user_id: int
     accuracy: float
     max_combo: int
     statistics: _NonLegacyStatistics
     pp: Optional[float]
     rank: Grade
 
     passed: bool
     current_user_attributes: Any
     replay: bool
-    maximum_statistics: Any # TODO property typing
+    maximum_statistics: Any  # TODO property typing
     mods: _NonLegacyMod
     ruleset_id: int
     started_at: Optional[Datetime]
     ended_at: Datetime
     ranked: bool
     preserve: bool
     beatmap_id: int
```

### Comparing `ossapi-3.4.4/ossapi/ossapi.py` & `ossapi-4.0.0b1/ossapi/ossapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 from requests import RequestException
 
 from ossapi.mod import Mod
 
 # log level below debug
 TRACE = 5
 
+
 class APIException(Exception):
     """An error involving the osu! api."""
 
+
 class InvalidKeyException(APIException):
     def __init__(self):
         super().__init__("Please provide a valid api key")
 
+
 class ReplayUnavailableException(APIException):
     pass
 
+
 class OssapiV1:
     """
     A simple api wrapper. Every public method takes a dict as its argument,
     mapping keys to values.
 
     No attempt is made to ratelimit the connection or catch request errors.
     This is left to the user implementation.
@@ -57,45 +61,47 @@
         params["k"] = self._key
         url = f"{self.BASE_URL}{endpoint}"
         self.log.debug(f"making request to url {url} with params {params}")
 
         try:
             r = requests.get(url, params=params, timeout=self.TIMEOUT)
         except RequestException as e:
-            self.log.warning(f"Request exception: {e}. Likely a network issue; "
-                "sleeping for 5 seconds then retrying")
+            self.log.warning(
+                f"Request exception: {e}. Likely a network issue; "
+                "sleeping for 5 seconds then retrying"
+            )
             time.sleep(5)
             return self._get(endpoint, params, type_, list_, _beatmap_id)
 
         self.log.log(TRACE, f"made request to url {r.request.url}")
 
         try:
             data = r.json()
         except JSONDecodeError:
-            self.log.warning("the api returned invalid json. Likely a "
-                "temporary issue, waiting and retrying")
+            self.log.warning(
+                "the api returned invalid json. Likely a "
+                "temporary issue, waiting and retrying"
+            )
             time.sleep(3)
             return self._get(endpoint, params, type_, list_, _beatmap_id)
 
         self.log.log(TRACE, f"got data from api: {data}")
 
         if "error" in data:
             error = data["error"]
             if error == "Replay not available.":
-                raise ReplayUnavailableException("Could not find any replay "
-                    "data")
+                raise ReplayUnavailableException("Could not find any replay data")
             if error == "Requesting too fast! Slow your operation, cap'n!":
                 self._enforce_ratelimit()
                 return self._get(endpoint, params, type_, list_, _beatmap_id)
             if error == "Replay retrieval failed.":
                 raise ReplayUnavailableException("Replay retrieval failed")
             if error == "Please provide a valid API key.":
                 raise InvalidKeyException()
-            raise APIException("Unknown error when requesting a "
-                f"replay: {error}.")
+            raise APIException(f"Unknown error when requesting a replay: {error}.")
 
         if list_:
             ret = []
             for entry in data:
                 if _beatmap_id:
                     entry["beatmap_id"] = _beatmap_id
                 ret.append(type_(entry))
@@ -114,71 +120,110 @@
         # sleep the remainder of the reset cycle so we guarantee it's been that
         # long since the first request
         sleep_seconds = self.RATELIMIT_REFRESH - seconds_passed
         sleep_seconds = max(sleep_seconds, 0)
         self.log.info("Ratelimited, sleeping for %s seconds.", sleep_seconds)
         time.sleep(sleep_seconds)
 
-    def get_beatmaps(self, since=None, beatmapset_id=None, beatmap_id=None,
-        user=None, user_type=None, mode=None, include_converts=None,
-        beatmap_hash=None, limit=None, mods=None
+    def get_beatmaps(
+        self,
+        since=None,
+        beatmapset_id=None,
+        beatmap_id=None,
+        user=None,
+        user_type=None,
+        mode=None,
+        include_converts=None,
+        beatmap_hash=None,
+        limit=None,
+        mods=None,
     ) -> List["Beatmap"]:
-        params = {"since": since, "s": beatmapset_id, "b": beatmap_id,
-            "u": user, "type": user_type, "m": mode, "a": include_converts,
-            "h": beatmap_hash, "limit": limit, "mods": mods}
+        params = {
+            "since": since,
+            "s": beatmapset_id,
+            "b": beatmap_id,
+            "u": user,
+            "type": user_type,
+            "m": mode,
+            "a": include_converts,
+            "h": beatmap_hash,
+            "limit": limit,
+            "mods": mods,
+        }
         return self._get("get_beatmaps", params, Beatmap, list_=True)
 
     def get_match(self, match_id) -> "MatchInfo":
         params = {"mp": match_id}
         return self._get("get_match", params, MatchInfo)
 
-    def get_scores(self, beatmap_id, user=None, mode=None, mods=None,
-        user_type=None, limit=None
+    def get_scores(
+        self, beatmap_id, user=None, mode=None, mods=None, user_type=None, limit=None
     ) -> List["Score"]:
-        params = {"b": beatmap_id, "u": user, "m": mode, "mods": mods,
-            "type": user_type, "limit": limit}
-        return self._get("get_scores", params, Score, list_=True,
-            _beatmap_id=beatmap_id)
-
-    def get_replay(self, beatmap_id=None, user=None, mode=None, score_id=None,
-        user_type=None, mods=None
+        params = {
+            "b": beatmap_id,
+            "u": user,
+            "m": mode,
+            "mods": mods,
+            "type": user_type,
+            "limit": limit,
+        }
+        return self._get(
+            "get_scores", params, Score, list_=True, _beatmap_id=beatmap_id
+        )
+
+    def get_replay(
+        self,
+        beatmap_id=None,
+        user=None,
+        mode=None,
+        score_id=None,
+        user_type=None,
+        mods=None,
     ) -> str:
-        params = {"b": beatmap_id, "u": user, "m": mode, "s": score_id,
-            "type": user_type, "mods": mods}
+        params = {
+            "b": beatmap_id,
+            "u": user,
+            "m": mode,
+            "s": score_id,
+            "type": user_type,
+            "mods": mods,
+        }
         r = self._get("get_replay", params, Replay)
         return r.content
 
-    def get_user(self, user, mode=None, user_type=None, event_days=None) \
-        -> "User":
-        params = {"u": user, "m": mode, "type": user_type,
-            "event_days": event_days}
+    def get_user(self, user, mode=None, user_type=None, event_days=None) -> "User":
+        params = {"u": user, "m": mode, "type": user_type, "event_days": event_days}
         users = self._get("get_user", params, User, list_=True)
         # api returns a list of users even though we never get more than one
         # user, just extract it manually
         return users[0] if users else users
 
-    def get_user_best(self, user, mode=None, limit=None, user_type=None) \
-        -> List["Score"]:
+    def get_user_best(
+        self, user, mode=None, limit=None, user_type=None
+    ) -> List["Score"]:
         params = {"u": user, "m": mode, "limit": limit, "type": user_type}
         return self._get("get_user_best", params, Score, list_=True)
 
-    def get_user_recent(self, user, mode=None, limit=None, user_type=None) \
-        -> List["Score"]:
+    def get_user_recent(
+        self, user, mode=None, limit=None, user_type=None
+    ) -> List["Score"]:
         params = {"u": user, "m": mode, "limit": limit, "type": user_type}
         return self._get("get_user_recent", params, Score, list_=True)
 
+
 # ideally we'd use the ossapiv2 machinery (dataclasses + annotations) for these
 # models instead of this manual drudgery. Unfortunately said machinery requires
 # python 3.8+ and I'm not willing to drop support for python 3.7 quite yet
 # (I'd be okay with dropping 3.6 though). This is a temporary meassure until
 # such a time when I can justify dropping 3.7.
 # Should be a 'write once and forget about it' kind of thing anyway since v1 is
 # extremely stable, but would be nice to migrate over to v2's way of doing
 # things at some point.
 
+
 class Model:
     def __init__(self, data):
         self._data = data
 
     def _get(self, attr, optional=False):
         if attr not in self._data and optional:
             return None
@@ -212,15 +257,14 @@
         if attr is None:
             return None
 
         if attr == "1":
             return True
         return False
 
-
     def _mod(self, attr):
         attr = self._data[attr]
         if attr is None:
             return None
 
         return Mod(int(attr))
 
@@ -265,14 +309,15 @@
         self.count_spinners = self._int("count_spinner")
         self.max_combo = self._int("max_combo")
         self.storyboard = self._bool("storyboard")
         self.video = self._bool("video")
         self.download_unavailable = self._bool("download_unavailable")
         self.audio_unavailable = self._bool("audio_unavailable")
 
+
 class User(Model):
     def __init__(self, data):
         super().__init__(data)
 
         self.user_id = self._int("user_id")
         self.username = self._get("username")
         self.join_date = self._date("join_date")
@@ -296,24 +341,26 @@
         self.country_rank = self._int("pp_country_rank")
 
         self.events = []
         for event in data["events"]:
             event = Event(event)
             self.events.append(event)
 
+
 class Event(Model):
     def __init__(self, data):
         super().__init__(data)
 
         self.display_html = self._get("display_html")
         self.beatmap_id = self._int("beatmap_id")
         self.beatmapset_id = self._int("beatmapset_id")
         self.date = self._date("date")
         self.epic_factor = self._int("epicfactor")
 
+
 class Score(Model):
     def __init__(self, data):
         super().__init__(data)
 
         self.beatmap_id = self._int("beatmap_id")
         self.replay_id = self._int("score_id")
         self.score = self._int("score")
@@ -328,16 +375,18 @@
         self.perfect = self._bool("perfect")
         self.mods = self._mod("enabled_mods")
         self.user_id = self._int("user_id")
         self.date = self._date("date")
         self.rank = self._get("rank")
         # get_user_recent doesn't provide pp or replay_available at all
         self.pp = self._float("pp") if "pp" in data else None
-        self.replay_available = (self._bool("replay_available") if
-            "replay_available" in data else None)
+        self.replay_available = (
+            self._bool("replay_available") if "replay_available" in data else None
+        )
+
 
 class Replay(Model):
     def __init__(self, data):
         super().__init__(data)
         self.content = self._get("content")
 
 
@@ -358,14 +407,15 @@
         super().__init__(data)
 
         self.match_id = self._int("match_id")
         self.name = self._get("name")
         self.start_time = self._date("start_time")
         self.end_time = self._date("end_time")
 
+
 class MatchGame(Model):
     def __init__(self, data):
         super().__init__(data)
 
         self.game_id = self._int("game_id")
         self.start_time = self._date("start_time")
         self.end_time = self._date("end_time")
```

### Comparing `ossapi-3.4.4/ossapi/ossapiv2.py` & `ossapi-4.0.0b1/ossapi/ossapiv2_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# This file has been copied wholesale from ossapiv2.py, with minor adjustments
+# to make functions async and work around aiohttp vs requests differences.
+# No changes should be made here without changing ossapiv2 as well (the
+# converse may not necessarily be true, as I consider the sync part of the
+# library more important than the async).
+# I may eventually write a code generator to copy ossapiv2.py and automatically
+# adjust for async. I'm not sure it's worthwhile just yet given how finnicky it
+# will be to hardcode the insertion points of all the particular changes I've
+# made.
+
 from typing import Union, TypeVar, Optional, List, _GenericAlias
 import logging
 import webbrowser
 import socket
 import pickle
 from pathlib import Path
 from datetime import datetime
@@ -10,60 +20,194 @@
 import inspect
 import json
 import hashlib
 import functools
 import sys
 
 from requests_oauthlib import OAuth2Session
-from oauthlib.oauth2 import (BackendApplicationClient, TokenExpiredError,
-    AccessDeniedError, OAuth2Error)
+from requests_oauthlib.oauth2_session import TokenUpdated
+from oauthlib.oauth2 import (
+    BackendApplicationClient,
+    TokenExpiredError,
+    AccessDeniedError,
+    InsecureTransportError,
+    is_secure_transport,
+    OAuth2Error,
+)
 from oauthlib.oauth2.rfc6749.errors import InsufficientScopeError
 from oauthlib.oauth2.rfc6749.tokens import OAuth2Token
 import osrparse
 from typing_utils import issubtype, get_type_hints, get_origin, get_args
 
 import ossapi
-from ossapi.models import (Beatmap, BeatmapCompact, BeatmapUserScore,
-    ForumTopicAndPosts, Search, CommentBundle, Cursor, Score,
-    BeatmapsetSearchResult, ModdingHistoryEventsBundle, User, Rankings,
-    BeatmapScores, KudosuHistory, Beatmapset, BeatmapPlaycount, Spotlight,
-    Spotlights, WikiPage, _Event, Event, BeatmapsetDiscussionPosts, Build,
-    ChangelogListing, MultiplayerScores,
-    BeatmapsetDiscussionVotes, CreatePMResponse, BeatmapsetDiscussions,
-    UserCompact, NewsListing, NewsPost, SeasonalBackgrounds, BeatmapsetCompact,
-    BeatmapUserScores, DifficultyAttributes, Users, Beatmaps,
-    CreateForumTopicResponse, ForumPoll, ForumPost, ForumTopic, Room,
-    RoomLeaderboard, Matches, Match, MatchResponse, ChatChannel, Events,
-    BeatmapPack, BeatmapPacks, _NonLegacyBeatmapScores)
-from ossapi.enums import (GameMode, ScoreType, RankingFilter, RankingType,
-    UserBeatmapType, BeatmapDiscussionPostSort, UserLookupKey,
-    BeatmapsetEventType, CommentableType, CommentSort, ForumTopicSort,
-    SearchMode, MultiplayerScoresSort, BeatmapsetDiscussionVote,
-    BeatmapsetDiscussionVoteSort, BeatmapsetStatus, MessageType,
-    BeatmapsetSearchCategory, BeatmapsetSearchMode,
-    BeatmapsetSearchExplicitContent, BeatmapsetSearchGenre,
-    BeatmapsetSearchLanguage, NewsPostKey, BeatmapsetSearchSort, RoomSearchMode,
-    ChangelogMessageFormat, EventsSort, BeatmapPackType)
-from ossapi.utils import (is_primitive_type, is_optional, is_base_model_type,
-    is_model_type, is_high_model_type, Field, convert_primitive_type)
+from ossapi.models import (
+    Beatmap,
+    BeatmapCompact,
+    BeatmapUserScore,
+    ForumTopicAndPosts,
+    Search,
+    CommentBundle,
+    Cursor,
+    Score,
+    BeatmapsetSearchResult,
+    ModdingHistoryEventsBundle,
+    User,
+    Rankings,
+    BeatmapScores,
+    KudosuHistory,
+    Beatmapset,
+    BeatmapPlaycount,
+    Spotlight,
+    Spotlights,
+    WikiPage,
+    _Event,
+    Event,
+    BeatmapsetDiscussionPosts,
+    Build,
+    ChangelogListing,
+    MultiplayerScores,
+    BeatmapsetDiscussionVotes,
+    CreatePMResponse,
+    BeatmapsetDiscussions,
+    UserCompact,
+    NewsListing,
+    NewsPost,
+    SeasonalBackgrounds,
+    BeatmapsetCompact,
+    BeatmapUserScores,
+    DifficultyAttributes,
+    Users,
+    Beatmaps,
+    CreateForumTopicResponse,
+    ForumPoll,
+    ForumPost,
+    ForumTopic,
+    Room,
+    RoomLeaderboard,
+    Matches,
+    Match,
+    MatchResponse,
+    ChatChannel,
+    Events,
+    BeatmapPack,
+    BeatmapPacks,
+)
+from ossapi.enums import (
+    GameMode,
+    ScoreType,
+    RankingFilter,
+    RankingType,
+    UserBeatmapType,
+    BeatmapDiscussionPostSort,
+    UserLookupKey,
+    BeatmapsetEventType,
+    CommentableType,
+    CommentSort,
+    ForumTopicSort,
+    SearchMode,
+    MultiplayerScoresSort,
+    BeatmapsetDiscussionVote,
+    BeatmapsetDiscussionVoteSort,
+    BeatmapsetStatus,
+    MessageType,
+    BeatmapsetSearchCategory,
+    BeatmapsetSearchMode,
+    BeatmapsetSearchExplicitContent,
+    BeatmapsetSearchGenre,
+    BeatmapsetSearchLanguage,
+    NewsPostKey,
+    BeatmapsetSearchSort,
+    RoomSearchMode,
+    ChangelogMessageFormat,
+    EventsSort,
+    BeatmapPackType,
+)
+from ossapi.utils import (
+    is_primitive_type,
+    is_optional,
+    is_base_model_type,
+    is_model_type,
+    is_high_model_type,
+    Field,
+    convert_primitive_type,
+)
 from ossapi.mod import Mod
 from ossapi.replay import Replay
 
+
+class Oauth2SessionAsync(OAuth2Session):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        headers = {"User-Agent": f"ossapi (v{ossapi.__version__})"}
+        self.headers.update(headers)
+
+    # this method is shamelessly copied from `OAuth2Session.request`, modified
+    # to call `self.session.request` instead of `super().request`.
+    # Any OAuth2Session code which calls `request` will remain sync, but we have
+    # control over the vast majority of code which interacts with the session
+    # object and can switch to calling this async function instead.
+    # This means things like refreshing the token will still be sync. A
+    # negligible hit for a huge maintainability increase.
+    async def request_async(
+        self,
+        method,
+        url,
+        *,
+        session,
+        data=None,
+        headers=None,
+        withhold_token=False,
+        client_id=None,
+        client_secret=None,
+        **kwargs,
+    ):
+        import aiohttp
+
+        if not is_secure_transport(url):
+            raise InsecureTransportError()
+        if self.token and not withhold_token:
+            for hook in self.compliance_hook["protected_request"]:
+                url, headers, data = hook(url, headers, data)
+
+            try:
+                url, headers, data = self._client.add_token(
+                    url, http_method=method, body=data, headers=headers
+                )
+            except TokenExpiredError:
+                if self.auto_refresh_url:
+                    auth = kwargs.pop("auth", None)
+                    if client_id and client_secret and (auth is None):
+                        auth = aiohttp.BasicAuth(client_id, client_secret)
+                    token = self.refresh_token(
+                        self.auto_refresh_url, auth=auth, **kwargs
+                    )
+                    if self.token_updater:
+                        self.token_updater(token)
+                        url, headers, data = self._client.add_token(
+                            url, http_method=method, body=data, headers=headers
+                        )
+                    else:
+                        raise TokenUpdated(token)
+                else:
+                    raise
+
+        return await session.request(method, url, headers=headers, data=data, **kwargs)
+
+
 # our `request` function below relies on the ordering of these types. The
 # base type must come first, with any auxiliary types that the base type accepts
 # coming after.
 # These types are intended to provide better type hinting for consumers. We
 # want to support the ability to pass `"osu"` instead of `GameMode.STD`,
 # for instance. We automatically convert any value to its base class if the
 # relevant parameter has a type hint of the form below (see `request` for
 # details).
 GameModeT = Union[GameMode, str]
 ScoreTypeT = Union[ScoreType, str]
-# XXX this cannot be recursively typed without breaking our runtime type hint
-# inspection.
 ModT = Union[Mod, str, int, List[Union[Mod, str, int]]]
 RankingFilterT = Union[RankingFilter, str]
 RankingTypeT = Union[RankingType, str]
 UserBeatmapTypeT = Union[UserBeatmapType, str]
 BeatmapDiscussionPostSortT = Union[BeatmapDiscussionPostSort, str]
 UserLookupKeyT = Union[UserLookupKey, str]
 BeatmapsetEventTypeT = Union[BeatmapsetEventType, str]
@@ -89,14 +233,15 @@
 
 BeatmapIdT = Union[int, BeatmapCompact]
 UserIdT = Union[int, UserCompact]
 BeatmapsetIdT = Union[int, BeatmapCompact, BeatmapsetCompact]
 RoomIdT = Union[int, Room]
 MatchIdT = Union[int, Match]
 
+
 def request(scope, *, requires_user=False, category):
     """
     Handles various validation and preparation tasks for any endpoint request
     method.
 
     This method does the following things:
     * makes sure the client has the requuired scope to access the endpoint in
@@ -121,39 +266,44 @@
     requires_user: bool
         Whether this endpoint requires a user to be associated with the grant.
         Currently, only authtorization code grants can access these endpoints.
     category: str
         What category of endpoints this endpoint belongs to. Used for grouping
         in the docs.
     """
+
     def decorator(function):
         instantiate = {}
         for name, type_ in function.__annotations__.items():
             origin = get_origin(type_)
             args = get_args(type_)
             if origin is Union and is_base_model_type(args[0]):
                 instantiate[name] = type_
 
         arg_names = list(inspect.signature(function).parameters)
 
         @functools.wraps(function)
         def wrapper(*args, **kwargs):
             self = args[0]
             if scope is not None and scope not in self.scopes:
-                raise InsufficientScopeError(f"A scope of {scope} is required "
+                raise InsufficientScopeError(
+                    f"A scope of {scope} is required "
                     "for this endpoint. Your client's current scopes are "
-                    f"{self.scopes}")
+                    f"{self.scopes}"
+                )
 
             if requires_user and self.grant is Grant.CLIENT_CREDENTIALS:
-                raise AccessDeniedError("To access this endpoint you must be "
+                raise AccessDeniedError(
+                    "To access this endpoint you must be "
                     "authorized using the authorization code grant. You are "
                     "currently authorized with the client credentials grant."
                     "\n\n"
                     "For more details, see "
-                    "https://tybug.github.io/ossapi/grants.html.")
+                    "https://tybug.github.io/ossapi/grants.html."
+                )
 
             # we may need to edit this later so convert from tuple
             args = list(args)
 
             def id_from_id_type(arg_name, arg):
                 annotations = function.__annotations__
                 if arg_name not in annotations:
@@ -211,75 +361,75 @@
             return function(*args, **kwargs)
 
         # for docs generation
         wrapper.__ossapi_category__ = category
         wrapper.__ossapi_scope__ = scope
 
         return wrapper
+
     return decorator
 
 
 class ReauthenticationRequired(Exception):
     """
     Indicates that either the user has revoked this application from their
     account, or osu-web itself has invalidated the refresh token associated with
     this application.
-
     This exception is only raised when a manual access_token is passed to
     Ossapi, to bypass Ossapi's default authentication methods. The expectation
     is that in these cases, the consumer has their own way of authenticating
     with the user. That method should be used here to handle the
     reauthentication.
     """
+
     pass
 
+
 class Grant(Enum):
     """
     The grant types used by the api.
     """
+
     CLIENT_CREDENTIALS = "client"
     AUTHORIZATION_CODE = "authorization"
 
+
 class Scope(Enum):
     """
     The OAuth scopes used by the api.
     """
+
     CHAT_WRITE = "chat.write"
     CHAT_WRITE_MANAGE = "chat.write_manage"
     CHAT_READ = "chat.read"
     DELEGATE = "delegate"
     FORUM_WRITE = "forum.write"
     FRIENDS_READ = "friends.read"
     IDENTIFY = "identify"
     PUBLIC = "public"
 
+
 class Domain(Enum):
     """
     Different possible api domains. These correspond to different deployments of
-    the osu server: osu.ppy.sh, lazer.ppy.sh, and dev.ppy.sh respectively.
+    the osu server, such as osu.ppy.sh or dev.ppy.sh.
 
     The default domain, and the one the vast majority of users want, is
     :data:`Domain.OSU <ossapi.ossapiv2.Domain.OSU>`, and corresponds to the
-    main website. To retrieve information from the lazer website or the dev
-    website, use the corresponding domain.
+    main website.
     """
+
     OSU = "osu"
-    LAZER = "lazer"
     DEV = "dev"
 
-class Oauth2SessionOssapi(OAuth2Session):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
 
-        headers = {"User-Agent": f"ossapi (v{ossapi.__version__})"}
-        self.headers.update(headers)
-
-class Ossapi:
+class OssapiAsync:
     """
-    A wrapper around osu! api v2. The main entry point for ossapi.
+    Async equivalent of :class:`~ossapi.ossapiv2.Ossapi`. Main (async) entry
+    point into osu! api v2.
 
     Parameters
     ----------
     client_id: int
         The id of the client to authenticate with.
     client_secret: str
         The secret of the client to authenticate with.
@@ -338,43 +488,43 @@
         osu! api. Optional if using :data:`Grant.CLIENT_CREDENTIALS
         <ossapi.ossapiv2.Grant.CLIENT_CREDENTIALS>`.
     domain: Domain or str
         The domain to retrieve information from. This defaults to
         :data:`Domain.OSU <ossapi.ossapiv2.Domain.OSU>`, which corresponds to
         osu.ppy.sh, the main website.
         |br|
-        To retrieve information from lazer.ppy.sh - for instance, the
-        leaderboards on lazer, or a user's best score on lazer - specify
-        :data:`Domain.LAZER <ossapi.ossapiv2.Domain.LAZER>`. To retrieve
-        information from dev.ppy.sh, specify
+        To retrieve information from dev.ppy.sh, specify
         :data:`Domain.DEV <ossapi.ossapiv2.Domain.DEV>`.
         |br|
         See :doc:`Domains <domains>` for more about domains.
     """
+
     TOKEN_URL = "https://{domain}.ppy.sh/oauth/token"
     AUTH_CODE_URL = "https://{domain}.ppy.sh/oauth/authorize"
     BASE_URL = "https://{domain}.ppy.sh/api/v2"
 
-    def __init__(self,
+    def __init__(
+        self,
         client_id: int,
         client_secret: str,
         redirect_uri: Optional[str] = None,
         scopes: List[Union[str, Scope]] = [Scope.PUBLIC],
         *,
         grant: Optional[Union[Grant, str]] = None,
         strict: bool = False,
         token_directory: Optional[str] = None,
         token_key: Optional[str] = None,
         access_token: Optional[str] = None,
         refresh_token: Optional[str] = None,
-        domain: Union[str, Domain] = Domain.OSU
+        domain: Union[str, Domain] = Domain.OSU,
     ):
         if not grant:
-            grant = (Grant.AUTHORIZATION_CODE if redirect_uri else
-                Grant.CLIENT_CREDENTIALS)
+            grant = (
+                Grant.AUTHORIZATION_CODE if redirect_uri else Grant.CLIENT_CREDENTIALS
+            )
         grant = Grant(grant)
 
         domain = Domain(domain)
 
         self.token_url = self.TOKEN_URL.format(domain=domain.value)
         self.auth_code_url = self.AUTH_CODE_URL.format(domain=domain.value)
         self.base_url = self.BASE_URL.format(domain=domain.value)
@@ -384,57 +534,64 @@
         self.client_secret = client_secret
         self.redirect_uri = redirect_uri
         self.scopes = [Scope(scope) for scope in scopes]
         self.strict = strict
         self.domain = domain
 
         self.log = logging.getLogger(__name__)
-        self.token_key = token_key or self.gen_token_key(self.grant,
-            self.client_id, self.client_secret, self.scopes, self.domain.value)
+        self.token_key = token_key or self.gen_token_key(
+            self.grant,
+            self.client_id,
+            self.client_secret,
+            self.scopes,
+            self.domain.value,
+        )
         self._type_hints_cache = {}
 
         # support saving tokens when being run from pyinstaller
-        if hasattr(sys, '_MEIPASS') and not token_directory:
-            token_directory = sys._MEIPASS # pylint: disable=no-member
+        if hasattr(sys, "_MEIPASS") and not token_directory:
+            token_directory = sys._MEIPASS  # pylint: disable=no-member
 
         self.token_directory = (
             Path(token_directory) if token_directory else Path(__file__).parent
         )
         self.token_file = self.token_directory / f"{self.token_key}.pickle"
 
         if self.grant is Grant.CLIENT_CREDENTIALS:
             if self.scopes != [Scope.PUBLIC]:
-                raise ValueError(f"`scopes` must be ['public'] if the "
-                    f"client credentials grant is used. Got {self.scopes}")
+                raise ValueError(
+                    f"`scopes` must be ['public'] if the "
+                    f"client credentials grant is used. Got {self.scopes}"
+                )
 
         if self.grant is Grant.AUTHORIZATION_CODE and not self.redirect_uri:
-            raise ValueError("`redirect_uri` must be passed if the "
-                "authorization code grant is used.")
+            raise ValueError(
+                "`redirect_uri` must be passed if the "
+                "authorization code grant is used."
+            )
 
         # whether the consumer passed a token to ossapi to bypass authentication
         self.access_token_passed = False
         token = None
         if access_token is not None:
             # allow refresh_token to be null for the case of client credentials
             # grant from access token, which does not have an associated refresh
             # token.
             params = {
                 "token_type": "Bearer",
                 "access_token": access_token,
-                "refresh_token": refresh_token
+                "refresh_token": refresh_token,
             }
             token = OAuth2Token(params)
             self.access_token_passed = True
 
         self.session = self.authenticate(token=token)
 
     @staticmethod
-    def gen_token_key(grant, client_id, client_secret, scopes,
-        domain=Domain.OSU
-    ):
+    def gen_token_key(grant, client_id, client_secret, scopes, domain=Domain.OSU):
         """
         The unique key / hash for the given set of parameters. This is intended
         to provide a way to allow multiple OssapiV2's to live at the same time,
         by eg saving their tokens to different files based on their key.
 
         This function is also deterministic, to eg allow tokens to be reused if
         OssapiV2 is instantiated twice with the same parameters. This avoids the
@@ -451,16 +608,14 @@
 
         for scope in scopes:
             m.update(scope.value.encode("utf-8"))
 
         # for backwards compatability, only hash the domain when it's
         # non-default. This ensures keys from before and after domains were
         # introduced coincide.
-        # This intentionally treats Domain.OSU and Domain.LAZER as the same key,
-        # as those domains share account and oauth credentials.
         if domain is Domain.DEV:
             m.update(domain.value.encode("utf-8"))
 
         return m.hexdigest()
 
     @staticmethod
     def remove_token(key, token_directory=None):
@@ -488,205 +643,239 @@
         # try saved token file first
         if self.token_file.exists() or token is not None:
             if token is None:
                 with open(self.token_file, "rb") as f:
                     token = pickle.load(f)
 
             if self.grant is Grant.CLIENT_CREDENTIALS:
-                return Oauth2SessionOssapi(self.client_id, token=token)
+                return Oauth2SessionAsync(self.client_id, token=token)
 
             if self.grant is Grant.AUTHORIZATION_CODE:
                 auto_refresh_kwargs = {
                     "client_id": self.client_id,
-                    "client_secret": self.client_secret
+                    "client_secret": self.client_secret,
                 }
-                return Oauth2SessionOssapi(self.client_id, token=token,
+                return Oauth2SessionAsync(
+                    self.client_id,
+                    token=token,
                     redirect_uri=self.redirect_uri,
                     auto_refresh_url=self.token_url,
                     auto_refresh_kwargs=auto_refresh_kwargs,
                     token_updater=self._save_token,
-                    scope=[scope.value for scope in self.scopes])
+                    scope=[scope.value for scope in self.scopes],
+                )
 
         # otherwise, authorize from scratch
         return self._new_grant()
 
     def _new_grant(self):
         if self.grant is Grant.CLIENT_CREDENTIALS:
             return self._new_client_grant(self.client_id, self.client_secret)
 
-        return self._new_authorization_grant(self.client_id, self.client_secret,
-            self.redirect_uri, self.scopes)
+        return self._new_authorization_grant(
+            self.client_id, self.client_secret, self.redirect_uri, self.scopes
+        )
 
     def _new_client_grant(self, client_id, client_secret):
         """
         Authenticates with the api from scratch on the client grant.
         """
         self.log.info("initializing client credentials grant")
         client = BackendApplicationClient(client_id=client_id, scope=["public"])
-        session = Oauth2SessionOssapi(client=client)
-        token = session.fetch_token(token_url=self.token_url,
-            client_id=client_id, client_secret=client_secret)
+        session = Oauth2SessionAsync(client=client)
+        token = session.fetch_token(
+            token_url=self.token_url, client_id=client_id, client_secret=client_secret
+        )
 
         self._save_token(token)
         return session
 
-    def _new_authorization_grant(self, client_id, client_secret, redirect_uri,
-        scopes):
+    def _new_authorization_grant(self, client_id, client_secret, redirect_uri, scopes):
         """
         Authenticates with the api from scratch on the authorization code grant.
         """
         self.log.info("initializing authorization code")
 
-        auto_refresh_kwargs = {
-            "client_id": client_id,
-            "client_secret": client_secret
-        }
-        session = OAuth2Session(client_id, redirect_uri=redirect_uri,
+        auto_refresh_kwargs = {"client_id": client_id, "client_secret": client_secret}
+        session = Oauth2SessionAsync(
+            client_id,
+            redirect_uri=redirect_uri,
             auto_refresh_url=self.token_url,
             auto_refresh_kwargs=auto_refresh_kwargs,
             token_updater=self._save_token,
-            scope=[scope.value for scope in scopes])
-
-        authorization_url, _state = (
-            session.authorization_url(self.auth_code_url)
+            scope=[scope.value for scope in scopes],
         )
+
+        authorization_url, _state = session.authorization_url(self.auth_code_url)
         webbrowser.open(authorization_url)
 
         # open up a temporary socket so we can receive the GET request to the
         # callback url
         port = int(redirect_uri.rsplit(":", 1)[1].split("/")[0])
         serversocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         serversocket.bind(("localhost", port))
         serversocket.listen(1)
         connection, _ = serversocket.accept()
         # arbitrary "large enough" byte receive size
         data = str(connection.recv(8192))
         connection.send(b"HTTP/1.0 200 OK\n")
         connection.send(b"Content-Type: text/html\n")
         connection.send(b"\n")
-        connection.send(b"""<html><body>
+        connection.send(
+            b"""<html><body>
             <h2>Ossapi has received your authentication.</h2> You
             may now close this tab safely.
             </body></html>
-        """)
+        """
+        )
         connection.close()
         serversocket.close()
 
         code = data.split("code=")[1].split("&state=")[0]
-        token = session.fetch_token(self.token_url, client_id=client_id,
-            client_secret=client_secret, code=code)
+        token = session.fetch_token(
+            self.token_url, client_id=client_id, client_secret=client_secret, code=code
+        )
         self._save_token(token)
 
         return session
 
     def _save_token(self, token):
         """
         Saves the token to this OssapiV2's associated token file.
         """
         self.log.info(f"saving token to {self.token_file}")
         with open(self.token_file, "wb+") as f:
             pickle.dump(token, f)
 
-    def _request(self, type_, method, url, params={}, data={}):
+    async def _request(self, type_, method, url, params={}, data={}):
+        from aiohttp import ClientSession
+
         # I don't *think* type hints should change over the lifetime of a
         # program, but clear them every request out of an abundance of caution.
         # This costs us almost nothing and may avoid bugs when eg a consumer
         # changes type hints of a custom model dynamically at some point.
         # They should certainly not be doing so in the middle of a request,
         # however.
         self._clear_type_hints_cache()
+
         params = self._format_params(params)
         # also format data for post requests
         data = self._format_params(data)
 
-        def make_request():
-            return self.session.request(method, f"{self.base_url}{url}",
-                params=params, data=data)
+        # No, we should not be using a session for every request. Yes, we are
+        # not achieving 100% performance by doing this. The benefit is that we
+        # don't require `async with OssapiAsync(...) as api:` syntax in order to
+        # use ossapi.
+        aiohttp_session = ClientSession()
+
+        async def make_request():
+            return await self.session.request_async(
+                method,
+                f"{self.base_url}{url}",
+                session=aiohttp_session,
+                params=params,
+                data=data,
+            )
 
-        def reauthenticate_and_retry():
+        async def reauthenticate_and_retry():
             # don't automatically re-authenticate if the user passed an access
             # token. They should handle re-authentication with the user
             # manually (since they may have a bespoke system, like a website).
             if self.access_token_passed:
-                self.log.info("refresh token is invalid. raising for consumer "
-                    "to handle since access token was passed originally.")
+                self.log.info(
+                    "refresh token is invalid. raising for consumer "
+                    "to handle since access token was passed originally."
+                )
                 raise ReauthenticationRequired()
 
-            self.log.info("refresh token invalid, re-authenticating (grant: "
-                f"{self.grant})")
+            self.log.info(
+                f"refresh token invalid, re-authenticating (grant: {self.grant})"
+            )
             # don't use .authenticate, that falls back to cached tokens. go
             # straight to authenticating from scratch.
             self.session = self._new_grant()
             # redo the request now that we have a valid session
-            return make_request()
+            return await make_request()
 
         try:
-            r = make_request()
+            r = await make_request()
         except TokenExpiredError:
             # provide "auto refreshing" for client credentials grant. The client
             # grant doesn't actually provide a refresh token, so we can't hook
             # onto OAuth2Session's auto_refresh functionality like we do for the
             # authorization code grant. But we can do something effectively
             # equivalent: whenever we make a request with an expired client
             # grant token, just request a new one.
             if self.grant is not Grant.CLIENT_CREDENTIALS:
                 raise
-            self.session = self._new_client_grant(self.client_id,
-                self.client_secret)
+            self.session = self._new_client_grant(self.client_id, self.client_secret)
             # redo the request now that we have a valid token
-            r = make_request()
+            r = await make_request()
         except OAuth2Error as e:
             if e.description != "The refresh token is invalid.":
                 raise
 
-            r = reauthenticate_and_retry()
-
-        self.log.info(f"made {method} request to {r.request.url}, data {data}")
-        json_ = r.json()
+            r = await reauthenticate_and_retry()
 
+        # aiohttp annoyingly differentiates between url (no url fragments, for
+        # some reason) and real_url (actual url). They also use a URL object
+        # here instead of a string.
+        # XXX don't overwrite url passed in function, used in
+        # authenticate_and_retry
+        url_ = str(r.real_url)
+        self.log.info(f"made {method} request to {url_}, data {data}")
+
+        # aiohttp throws on unexpected encoding (non-json mimetype). Match
+        # requests behavior by automatically detecting encoding.
+        # See https://github.com/tybug/ossapi/issues/60.
+        json_ = await r.json(encoding=None)
         # occurs if a client gets revoked and the token hasn't officially
         # expired yet (so it doesn't error earlier up in the chain with
         # Oauth2Error).
         if json_ == {"authentication": "basic"}:
-            r = reauthenticate_and_retry()
-            json_ = r.json()
+            r = await reauthenticate_and_retry()
+            json_ = await r.json(encoding=None)
+
+        # aiohttp sessions have to live as long as any responses returned via
+        # the session. Wait to close it until we're done with the response `r`.
+        # Make sure we close this before we call _check_response, or any errors
+        # there will result in the session not being closed. We should probably
+        # move this to a try/finally block at some point for safety.
+        await aiohttp_session.close()
 
         self.log.debug(f"received json: \n{json.dumps(json_, indent=4)}")
-        self._check_response(json_, r.url)
+        self._check_response(json_, url_)
 
         return self._instantiate_type(type_, json_)
 
     def _check_response(self, json_, url):
         # TODO this should just be `if "error" in json`, but for some reason
         # `self.search_beatmaps` always returns an error in the response...
         # open an issue on osu-web?
         if len(json_) == 1 and "error" in json_:
-            raise ValueError(f"api returned an error of `{json_['error']}` for "
-                f"a request to {unquote(url)}")
-
-        # some endpoints only require authorization grant for some endpoints.
-        # e.g. normally api.match only requires client credentials grant, but for
-        # private matches like api.match(111632899), it will return this error.
-        if json_ == {"authentication": "basic"}:
-            raise ValueError("Permission denied for a request to "
-                f"{unquote(url)}. This request may require "
-                "Grant.AUTHORIZATION_CODE.")
+            raise ValueError(
+                f"api returned an error of `{json_['error']}` for "
+                f"a request to {unquote(url)}"
+            )
 
-    def _get(self, type_, url, params={}):
-        return self._request(type_, "GET", url, params=params)
+    async def _get(self, type_, url, params={}):
+        return await self._request(type_, "GET", url, params=params)
 
-    def _post(self, type_, url, data={}):
-        return self._request(type_, "POST", url, data=data)
+    async def _post(self, type_, url, data={}):
+        return await self._request(type_, "POST", url, data=data)
 
-    def _put(self, type_, url, data={}):
-        return self._request(type_, "PUT", url, data=data)
+    async def _put(self, type_, url, data={}):
+        return await self._request(type_, "PUT", url, data=data)
 
     def _format_params(self, params):
         for key, value in params.copy().items():
-            if isinstance(value, list):
+            # requests ignores None values, but aiohttp doesn't. Make compliant.
+            if value is None:
+                del params[key]
+            elif isinstance(value, list):
                 # we need to pass multiple values for this key, so make its
                 # value a list https://stackoverflow.com/a/62042144
                 params[f"{key}[]"] = []
                 for v in value:
                     params[f"{key}[]"].append(self._format_value(v))
                 del params[key]
             elif isinstance(value, Cursor):
@@ -769,15 +958,15 @@
             # skipping fields that are null which aren't supposed to be, and
             # prevent that error from being caught.
             if value is None and is_optional(type_):
                 continue
             self.log.debug(f"resolving attribute {attr}")
 
             value = self._instantiate_type(type_, value, obj, attr_name=attr)
-            if value is None:
+            if not value:
                 continue
             setattr(obj, attr, value)
         self.log.debug(f"resolved annotations for type {type(obj)}")
         return obj
 
     def _instantiate_type(self, type_, value, obj=None, attr_name=None):
         # `attr_name` is purely for debugging, it's the name of the attribute
@@ -802,29 +991,32 @@
         def _check_primitive_type():
             # The osu api occasionally makes attributes optional, so allow null
             # values even for non-optional fields if we're not in
             # strict mode.
             if not self.strict and value is None:
                 return
             if not isinstance(value, type_):
-                raise TypeError(f"expected type {type_} for value {value}, got "
+                raise TypeError(
+                    f"expected type {type_} for value {value}, got "
                     f"type {type(value)}"
-                    f" (for attribute: {attr_name})" if attr_name else "")
+                    f" (for attribute: {attr_name})"
+                    if attr_name
+                    else ""
+                )
 
         if is_primitive_type(type_):
             value = convert_primitive_type(value, type_)
             _check_primitive_type()
             return value
 
         if is_base_model_type(type_):
             self.log.debug(f"instantiating base type {type_}")
             return type_(value)
 
-        if origin is list and (is_model_type(args[0]) or
-            isinstance(args[0], TypeVar)):
+        if origin is list and (is_model_type(args[0]) or isinstance(args[0], TypeVar)):
             assert len(args) == 1
             # check if the list has been instantiated generically; if so,
             # use the concrete type backing the generic type.
             if isinstance(args[0], TypeVar):
                 # `__orig_class__` is how we can get the concrete type of
                 # a generic. See https://stackoverflow.com/a/60984681 and
                 # https://www.python.org/dev/peps/pep-0560/#mro-entries.
@@ -856,27 +1048,29 @@
             new_value = None
             # purely for debugging. errors for each arg are shown when we can't
             # deserialize any of them.
             fail_reasons = []
             for arg in args:
                 try:
                     import copy
+
                     v = copy.deepcopy(value)
                     # _instantiate_type implicitly mutates the passed value.
                     # this is probably something we should change - but for now,
                     # fix it here, as we may reuse `value`.
-                    new_value = self._instantiate_type(arg, v, obj,
-                        attr_name)
+                    new_value = self._instantiate_type(arg, v, obj, attr_name)
                 except Exception as e:
                     fail_reasons.append(str(e))
                     continue
 
             if new_value is None:
-                raise ValueError(f"Failed to satisfy union: no type in {args} "
-                    f"satisfied {attr_name} (fail reasons: {fail_reasons})")
+                raise ValueError(
+                    f"Failed to satisfy union: no type in {args} "
+                    f"satisfied {attr_name} (fail reasons: {fail_reasons})"
+                )
             return new_value
 
         # either we ourself are a model type (eg `Search`), or we are
         # a special indexed type (eg `type_ == SearchResult[UserCompact]`,
         # `origin == UserCompact`). In either case we want to instantiate
         # `type_`.
         if not is_model_type(type_) and not is_model_type(origin):
@@ -908,38 +1102,30 @@
             type_hints = self._get_type_hints(type_)
         except TypeError:
             assert type(type_) is _GenericAlias
 
             signature_type = get_origin(type_)
             type_hints = self._get_type_hints(signature_type)
 
-        # field override name to existing attribute name
         field_names = {}
-        # existing attribute name to field deserialize type
-        field_deserialize_types = {}
-        # process Field attributes.
         for name in type_hints:
             # any inherited attributes will be present in the annotations
             # (type_hints) but not actually an attribute of the type. Just skip
             # them for now. TODO I'm pretty sure this is going to cause issues
             # if we ever have a field on a model and then another model
             # inheriting from it; the inheriting model won't have the field
             # picked up here and the override name won't come into play.
             # probably just traverse the mro?
             if not hasattr(type_, name):
                 continue
             value = getattr(type_, name)
             if not isinstance(value, Field):
                 continue
-
-            if value.name is not None:
+            if value.name:
                 field_names[value.name] = name
-            if value.deserialize_type is not None:
-                field_deserialize_types[name] = value.deserialize_type
-
 
         # make a copy so we can modify while iterating
         for key in list(kwargs):
             value = kwargs.pop(key)
             if key in field_names:
                 key = field_names[key]
             kwargs[key] = value
@@ -971,42 +1157,33 @@
         kwargs_ = {}
 
         for k, v in kwargs.items():
             if k in parameters:
                 kwargs_[k] = v
             else:
                 if self.strict:
-                    raise TypeError(f"unexpected parameter `{k}` for type "
-                        f"{type_}")
+                    raise TypeError(f"unexpected parameter `{k}` for type {type_}")
                 # this is an INFO log in spirit, but can be spammy with Union
                 # type resolution where the first union case hits nonfatal
                 # errors like this before a fatal error causes it to backtrack.
                 # In practice, it makes no difference for developing ossapi,
                 # as tests and local development are all done in strict mode.
-                self.log.debug(f"ignoring unexpected parameter `{k}` from "
-                    f"api response for type {type_}")
+                self.log.debug(
+                    f"ignoring unexpected parameter `{k}` from "
+                    f"api response for type {type_}"
+                )
 
         # every model gets a special `_api` parameter, which is the
         # `OssapiV2` instance which loaded it (aka us).
         kwargs_["_api"] = self
 
         try:
             val = type_(**kwargs_)
         except TypeError as e:
-            raise TypeError(f"type error while instantiating class {type_}: "
-                f"{e}") from e
-
-        for name, deserialize_type in field_deserialize_types.items():
-            val.__annotations__[name] = deserialize_type
-
-        # modifying the type hints of an object dynamically invalidates its
-        # cache. Avoid looking up stale type hints if we had looked up its
-        # previous value before modifying it here.
-        if field_deserialize_types:
-            del self._type_hints_cache[type(val)]
+            raise TypeError(f"type error while instantiating class {type_}: {e}") from e
 
         return val
 
     def _get_type_hints(self, obj):
         # type hints are expensive to compute. Our models should never change
         # their type hints, so cache them.
         if obj in self._type_hints_cache:
@@ -1015,27 +1192,26 @@
         type_hints = get_type_hints(obj)
         self._type_hints_cache[obj] = type_hints
         return type_hints
 
     def _clear_type_hints_cache(self):
         self._type_hints_cache = {}
 
-
     # =========
     # Endpoints
     # =========
 
-
     # /beatmaps/packs
     # ---------------
 
     @request(Scope.PUBLIC, category="beatmap packs")
-    def beatmap_packs(self,
+    async def beatmap_packs(
+        self,
         type: Optional[BeatmapPackTypeT] = None,
-        cursor_string: Optional[str] = None
+        cursor_string: Optional[str] = None,
     ) -> BeatmapPacks:
         """
         Get a list of beatmap packs. If you want to retrieve a specific pack,
         see :meth:`beatmap_pack`.
 
         Parameters
         ----------
@@ -1045,42 +1221,41 @@
         Notes
         -----
         Implements the `Beatmap Packs
         <https://osu.ppy.sh/docs/index.html#get-beatmap-packs>`__
         endpoint.
         """
         params = {"type": type, "cursor_string": cursor_string}
-        return self._get(BeatmapPacks, "/beatmaps/packs", params)
+        return await self._get(BeatmapPacks, "/beatmaps/packs", params)
 
     @request(Scope.PUBLIC, category="beatmap packs")
-    def beatmap_pack(self,
-        pack: str
-    ) -> BeatmapPack:
+    async def beatmap_pack(self, pack: str) -> BeatmapPack:
         """
         Get a beatmap pack. If you want to retrieve a list of beatmap packs, see
         see :meth:`beatmap_packs`.
 
         Notes
         -----
         Implements the `Beatmap Pack
         <https://osu.ppy.sh/docs/index.html#get-beatmap-pack>`__
         endpoint.
         """
-        return self._get(BeatmapPack, f"/beatmaps/packs/{pack}")
+        return await self._get(BeatmapPack, f"/beatmaps/packs/{pack}")
 
     # /beatmaps
     # ---------
 
     @request(Scope.PUBLIC, category="beatmaps")
-    def beatmap_user_score(self,
+    async def beatmap_user_score(
+        self,
         beatmap_id: BeatmapIdT,
         user_id: UserIdT,
         *,
         mode: Optional[GameModeT] = None,
-        mods: Optional[ModT] = None
+        mods: Optional[ModT] = None,
     ) -> BeatmapUserScore:
         """
         Get a user's best score on a beatmap. If you want to retrieve all
         scores, see :meth:`beatmap_user_scores`.
 
         Parameters
         ----------
@@ -1096,23 +1271,25 @@
         Notes
         -----
         Implements the `User Beatmap Score
         <https://osu.ppy.sh/docs/index.html#get-a-user-beatmap-score>`__
         endpoint.
         """
         params = {"mode": mode, "mods": mods}
-        return self._get(BeatmapUserScore,
-            f"/beatmaps/{beatmap_id}/scores/users/{user_id}", params)
+        return await self._get(
+            BeatmapUserScore, f"/beatmaps/{beatmap_id}/scores/users/{user_id}", params
+        )
 
     @request(Scope.PUBLIC, category="beatmaps")
-    def beatmap_user_scores(self,
+    async def beatmap_user_scores(
+        self,
         beatmap_id: BeatmapIdT,
         user_id: UserIdT,
         *,
-        mode: Optional[GameModeT] = None
+        mode: Optional[GameModeT] = None,
     ) -> List[Score]:
         """
         Get all of a user's scores on a beatmap. If you only want the top user
         score, see :meth:`beatmap_user_score`.
 
         Parameters
         ----------
@@ -1126,26 +1303,30 @@
         Notes
         -----
         Implements to `User Beatmap Scores
         <https://osu.ppy.sh/docs/index.html#get-a-user-beatmap-scores>`__
         endpoint.
         """
         params = {"mode": mode}
-        scores = self._get(BeatmapUserScores,
-            f"/beatmaps/{beatmap_id}/scores/users/{user_id}/all", params)
+        scores = await self._get(
+            BeatmapUserScores,
+            f"/beatmaps/{beatmap_id}/scores/users/{user_id}/all",
+            params,
+        )
         return scores.scores
 
     @request(Scope.PUBLIC, category="beatmaps")
-    def beatmap_scores(self,
+    async def beatmap_scores(
+        self,
         beatmap_id: BeatmapIdT,
         *,
         mode: Optional[GameModeT] = None,
         mods: Optional[ModT] = None,
         type: Optional[RankingTypeT] = None,
-        limit: Optional[int] = None
+        limit: Optional[int] = None,
     ) -> BeatmapScores:
         """
         Get the top scores of a beatmap.
 
         Parameters
         ----------
         beatmap_id
@@ -1162,41 +1343,19 @@
 
         Notes
         -----
         Implements the `Get Beatmap Scores
         <https://osu.ppy.sh/docs/index.html#get-beatmap-scores>`__ endpoint.
         """
         params = {"mode": mode, "mods": mods, "type": type, "limit": limit}
-        return self._get(BeatmapScores, f"/beatmaps/{beatmap_id}/scores",
-            params)
-
-    def _beatmap_scores_non_legacy(self,
-        beatmap_id: BeatmapIdT,
-        *,
-        mode: Optional[GameModeT] = None,
-        mods: Optional[ModT] = None,
-        type: Optional[RankingTypeT] = None,
-        limit: Optional[int] = None,
-        legacy_only: Optional[bool] = None
-    ) -> _NonLegacyBeatmapScores:
-        """
-        This is a provisional method. It may change or disappear in the future.
-        Feel free to use it, but don't expect ossapi to maintain backwards
-        compatability here.
-
-        I'll decide what to do about these provisional methods once the lazer
-        migration settles down.
-        """
-        params = {"mode": mode, "mods": mods, "type": type, "limit": limit,
-            "legacy_only": legacy_only}
-        return self._get(_NonLegacyBeatmapScores, f"/beatmaps/{beatmap_id}/solo-scores",
-            params)
+        return await self._get(BeatmapScores, f"/beatmaps/{beatmap_id}/scores", params)
 
     @request(Scope.PUBLIC, category="beatmaps")
-    def beatmap(self,
+    async def beatmap(
+        self,
         beatmap_id: Optional[BeatmapIdT] = None,
         *,
         checksum: Optional[str] = None,
         filename: Optional[str] = None,
     ) -> Beatmap:
         """
         Get a beatmap from an id, checksum, or filename.
@@ -1214,23 +1373,22 @@
         -----
         Combines the
         `Get Beatmap <https://osu.ppy.sh/docs/index.html#get-beatmap>`_ and
         `Lookup Beatmap <https://osu.ppy.sh/docs/index.html#lookup-beatmap>`_
         endpoints.
         """
         if not (beatmap_id or checksum or filename):
-            raise ValueError("at least one of beatmap_id, checksum, or "
-                "filename must be passed")
+            raise ValueError(
+                "at least one of beatmap_id, checksum, or filename must be passed"
+            )
         params = {"checksum": checksum, "filename": filename, "id": beatmap_id}
-        return self._get(Beatmap, "/beatmaps/lookup", params)
+        return await self._get(Beatmap, "/beatmaps/lookup", params)
 
     @request(Scope.PUBLIC, category="beatmaps")
-    def beatmaps(self,
-        beatmap_ids: List[BeatmapIdT]
-    ) -> List[Beatmap]:
+    async def beatmaps(self, beatmap_ids: List[BeatmapIdT]) -> List[Beatmap]:
         """
         Batch get beatmaps by id. If you only want to retrieve a single beatmap,
         or want to retrieve beatmaps by something other than id (eg checksum),
         see :meth:`beatmap`.
 
         Parameters
         ----------
@@ -1239,23 +1397,25 @@
 
         Notes
         -----
         Implements the `Get Beatmaps
         <https://osu.ppy.sh/docs/index.html#get-beatmaps>`__ endpoint.
         """
         params = {"ids": beatmap_ids}
-        return self._get(Beatmaps, "/beatmaps", params).beatmaps
+        beatmaps = await self._get(Beatmaps, "/beatmaps", params)
+        return beatmaps.beatmaps
 
     @request(Scope.PUBLIC, category="beatmaps")
-    def beatmap_attributes(self,
+    async def beatmap_attributes(
+        self,
         beatmap_id: int,
         *,
         mods: Optional[ModT] = None,
         ruleset: Optional[GameModeT] = None,
-        ruleset_id: Optional[int] = None
+        ruleset_id: Optional[int] = None,
     ) -> DifficultyAttributes:
         """
         Get the difficult attributes of a beatmap. Used for pp calculation.
 
         Parameters
         ----------
         beatmap_id
@@ -1270,30 +1430,31 @@
 
         Notes
         -----
         Implements the `Get Beatmap Attributes
         <https://osu.ppy.sh/docs/index.html#get-beatmap-attributes>`__ endpoint.
         """
         data = {"mods": mods, "ruleset": ruleset, "ruleset_id": ruleset_id}
-        return self._post(DifficultyAttributes,
-            f"/beatmaps/{beatmap_id}/attributes", data=data)
-
+        return await self._post(
+            DifficultyAttributes, f"/beatmaps/{beatmap_id}/attributes", data=data
+        )
 
     # /beatmapsets
     # ------------
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    def beatmapset_discussion_posts(self,
+    async def beatmapset_discussion_posts(
+        self,
         beatmapset_discussion_id: Optional[int] = None,
         *,
         limit: Optional[int] = None,
         page: Optional[int] = None,
         sort: Optional[BeatmapDiscussionPostSortT] = None,
         user_id: Optional[UserIdT] = None,
-        with_deleted: Optional[bool] = None
+        with_deleted: Optional[bool] = None,
     ) -> BeatmapsetDiscussionPosts:
         """
         Get the posts of a beatmapset discussion.
 
         Parameters
         ----------
         beatmapset_discussion_id
@@ -1312,31 +1473,38 @@
 
         Notes
         -----
         Implements the `Get Beatmapset Discussion Posts
         <https://osu.ppy.sh/docs/index.html#get-beatmapset-discussion-posts>`__
         endpoint.
         """
-        params = {"beatmapset_discussion_id": beatmapset_discussion_id,
-            "limit": limit, "page": page, "sort": sort, "user": user_id,
-            "with_deleted": with_deleted}
-        return self._get(BeatmapsetDiscussionPosts,
-            "/beatmapsets/discussions/posts", params)
+        params = {
+            "beatmapset_discussion_id": beatmapset_discussion_id,
+            "limit": limit,
+            "page": page,
+            "sort": sort,
+            "user": user_id,
+            "with_deleted": with_deleted,
+        }
+        return await self._get(
+            BeatmapsetDiscussionPosts, "/beatmapsets/discussions/posts", params
+        )
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    def beatmapset_discussion_votes(self,
+    async def beatmapset_discussion_votes(
+        self,
         *,
         beatmapset_discussion_id: Optional[int] = None,
         limit: Optional[int] = None,
         page: Optional[int] = None,
         receiver_id: Optional[int] = None,
         vote: Optional[BeatmapsetDiscussionVoteT] = None,
         sort: Optional[BeatmapsetDiscussionVoteSortT] = None,
         user_id: Optional[UserIdT] = None,
-        with_deleted: Optional[bool] = None
+        with_deleted: Optional[bool] = None,
     ) -> BeatmapsetDiscussionVotes:
         """
         Get beatmapset discussion votes.
 
         Parameters
         ----------
         beatmapset_discussion_id
@@ -1359,23 +1527,31 @@
 
         Notes
         -----
         Implements the `Get Beatmapset Discussion Posts
         <https://osu.ppy.sh/docs/index.html#get-beatmapset-discussion-posts>`__
         endpoint.
         """
-        params = {"beatmapset_discussion_id": beatmapset_discussion_id,
-            "limit": limit, "page": page, "receiver": receiver_id,
-            "score": vote, "sort": sort, "user": user_id,
-            "with_deleted": with_deleted}
-        return self._get(BeatmapsetDiscussionVotes,
-            "/beatmapsets/discussions/votes", params)
+        params = {
+            "beatmapset_discussion_id": beatmapset_discussion_id,
+            "limit": limit,
+            "page": page,
+            "receiver": receiver_id,
+            "score": vote,
+            "sort": sort,
+            "user": user_id,
+            "with_deleted": with_deleted,
+        }
+        return await self._get(
+            BeatmapsetDiscussionVotes, "/beatmapsets/discussions/votes", params
+        )
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    def beatmapset_discussions(self,
+    async def beatmapset_discussions(
+        self,
         *,
         beatmapset_id: Optional[BeatmapsetIdT] = None,
         beatmap_id: Optional[BeatmapIdT] = None,
         beatmapset_status: Optional[BeatmapsetStatusT] = None,
         limit: Optional[int] = None,
         message_types: Optional[List[MessageTypeT]] = None,
         only_unresolved: Optional[bool] = None,
@@ -1413,44 +1589,51 @@
 
         Notes
         -----
         Implements the `Get Beatmapset Discussion Posts
         <https://osu.ppy.sh/docs/index.html#get-beatmapset-discussion-posts>`__
         endpoint.
         """
-        params = {"beatmapset_id": beatmapset_id, "beatmap_id": beatmap_id,
-            "beatmapset_status": beatmapset_status, "limit": limit,
-            "message_types": message_types, "only_unresolved": only_unresolved,
-            "page": page, "sort": sort, "user": user_id,
-            "with_deleted": with_deleted}
-        return self._get(BeatmapsetDiscussions,
-            "/beatmapsets/discussions", params)
+        params = {
+            "beatmapset_id": beatmapset_id,
+            "beatmap_id": beatmap_id,
+            "beatmapset_status": beatmapset_status,
+            "limit": limit,
+            "message_types": message_types,
+            "only_unresolved": only_unresolved,
+            "page": page,
+            "sort": sort,
+            "user": user_id,
+            "with_deleted": with_deleted,
+        }
+        return await self._get(
+            BeatmapsetDiscussions, "/beatmapsets/discussions", params
+        )
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    def search_beatmapsets(self,
+    async def search_beatmapsets(
+        self,
         query: Optional[str] = None,
         *,
         mode: BeatmapsetSearchModeT = BeatmapsetSearchMode.ANY,
-        category: BeatmapsetSearchCategoryT =
-            BeatmapsetSearchCategory.HAS_LEADERBOARD,
-        explicit_content: BeatmapsetSearchExplicitContentT =
-            BeatmapsetSearchExplicitContent.HIDE,
+        category: BeatmapsetSearchCategoryT = BeatmapsetSearchCategory.HAS_LEADERBOARD,
+        explicit_content: BeatmapsetSearchExplicitContentT = BeatmapsetSearchExplicitContent.HIDE,
         genre: BeatmapsetSearchGenreT = BeatmapsetSearchGenre.ANY,
         language: BeatmapsetSearchLanguageT = BeatmapsetSearchLanguage.ANY,
         # "Extra"
         force_video: bool = False,
         force_storyboard: bool = False,
         # "General"
         force_recommended_difficulty: bool = False,
         include_converts: bool = False,
         force_followed_mappers: bool = False,
         force_spotlights: bool = False,
         force_featured_artists: bool = False,
         cursor: Optional[Cursor] = None,
-        sort: Optional[BeatmapsetSearchSortT] = None
+        sort: Optional[BeatmapsetSearchSortT] = None,
     ) -> BeatmapsetSearchResult:
         """
         Search beatmapsets. Equivalent to the beatmapset search page on the
         website (https://osu.ppy.sh/beatmapsets).
 
         Parameters
         ----------
@@ -1516,34 +1699,44 @@
             generals.append("follows")
         if force_spotlights:
             generals.append("spotlights")
         if force_featured_artists:
             generals.append("featured_artists")
         general = ".".join(generals)
 
-        params = {"cursor": cursor, "q": query, "s": category, "m": mode,
-            "g": genre, "l": language, "nsfw": explicit_content, "e": extra,
-            "c": general, "sort": sort}
+        params = {
+            "cursor": cursor,
+            "q": query,
+            "s": category,
+            "m": mode,
+            "g": genre,
+            "l": language,
+            "nsfw": explicit_content,
+            "e": extra,
+            "c": general,
+            "sort": sort,
+        }
 
         # BeatmapsetSearchGenre.ANY is the default and doesn't have a correct
         # corresponding value
         if genre is BeatmapsetSearchGenre.ANY:
             del params["g"]
 
         # same for BeatmapsetSearchLanguage.ANY
         if language is BeatmapsetSearchLanguage.ANY:
             del params["l"]
 
-        return self._get(BeatmapsetSearchResult, "/beatmapsets/search/", params)
+        return await self._get(BeatmapsetSearchResult, "/beatmapsets/search/", params)
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    def beatmapset(self,
+    async def beatmapset(
+        self,
         beatmapset_id: Optional[BeatmapsetIdT] = None,
         *,
-        beatmap_id: Optional[BeatmapIdT] = None
+        beatmap_id: Optional[BeatmapIdT] = None,
     ) -> Beatmapset:
         """
         Get a beatmapset from a beatmapset id or a beatmap id.
 
         Parameters
         ----------
         beatmapset_id
@@ -1555,30 +1748,32 @@
         -----
         Combines the `Get Beatmapset
         <https://osu.ppy.sh/docs/index.html#beatmapsetsbeatmapset>`__ and
         `Beatmapset Lookup
         <https://osu.ppy.sh/docs/index.html#beatmapsetslookup>`__ endpoints.
         """
         if not bool(beatmap_id) ^ bool(beatmapset_id):
-            raise ValueError("exactly one of beatmap_id and beatmapset_id must "
-                "be passed.")
+            raise ValueError(
+                "exactly one of beatmap_id and beatmapset_id must be passed."
+            )
         if beatmap_id:
             params = {"beatmap_id": beatmap_id}
-            return self._get(Beatmapset, "/beatmapsets/lookup", params)
-        return self._get(Beatmapset, f"/beatmapsets/{beatmapset_id}")
+            return await self._get(Beatmapset, "/beatmapsets/lookup", params)
+        return await self._get(Beatmapset, f"/beatmapsets/{beatmapset_id}")
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    def beatmapset_events(self,
+    async def beatmapset_events(
+        self,
         *,
         limit: Optional[int] = None,
         page: Optional[int] = None,
         user_id: Optional[UserIdT] = None,
         types: Optional[List[BeatmapsetEventTypeT]] = None,
         min_date: Optional[datetime] = None,
-        max_date: Optional[datetime] = None
+        max_date: Optional[datetime] = None,
     ) -> ModdingHistoryEventsBundle:
         """
         Get beatmapset events. Equivalent to the events search page on the
         website (https://osu.ppy.sh/beatmapsets/events).
 
         Parameters
         ----------
@@ -1597,28 +1792,31 @@
 
         Notes
         -----
         Implements the `Beatmapset Events
         <https://osu.ppy.sh/docs/index.html#beatmapsetsevents>`__ endpoint.
         """
         # limit is 5-50
-        params = {"limit": limit, "page": page, "user": user_id,
-            "min_date": min_date, "max_date": max_date, "types": types}
-        return self._get(ModdingHistoryEventsBundle, "/beatmapsets/events",
-            params)
-
+        params = {
+            "limit": limit,
+            "page": page,
+            "user": user_id,
+            "min_date": min_date,
+            "max_date": max_date,
+            "types": types,
+        }
+        return await self._get(
+            ModdingHistoryEventsBundle, "/beatmapsets/events", params
+        )
 
     # /changelog
     # ----------
 
     @request(scope=None, category="changelog")
-    def changelog_build(self,
-        stream: str,
-        build: str
-    ) -> Build:
+    async def changelog_build(self, stream: str, build: str) -> Build:
         """
         Get changelog build details.
 
         Parameters
         ----------
         stream
             The changelog stream name (eg ``stable40``).
@@ -1626,25 +1824,28 @@
             The changelog build name (eg ``20230121.1``)
 
         Notes
         -----
         Implements the `Get Changelog Build
         <https://osu.ppy.sh/docs/index.html#get-changelog-build>`__ endpoint.
         """
-        return self._get(Build, f"/changelog/{stream}/{build}")
+        return await self._get(Build, f"/changelog/{stream}/{build}")
 
     @request(scope=None, category="changelog")
-    def changelog_listing(self,
+    async def changelog_listing(
+        self,
         *,
         from_: Optional[str] = None,
         to: Optional[str] = None,
         max_id: Optional[int] = None,
         stream: Optional[str] = None,
-        message_formats: List[ChangelogMessageFormat] =
-            [ChangelogMessageFormat.HTML, ChangelogMessageFormat.MARKDOWN]
+        message_formats: List[ChangelogMessageFormat] = [
+            ChangelogMessageFormat.HTML,
+            ChangelogMessageFormat.MARKDOWN,
+        ],
     ) -> ChangelogListing:
         """
         Get list of changelogs.
 
         Parameters
         ----------
         from_
@@ -1659,27 +1860,35 @@
             Format to return text of changelog entries in.
 
         Notes
         -----
         Implements the `Get Changelog Listing
         <https://osu.ppy.sh/docs/index.html#get-changelog-listing>`__ endpoint.
         """
-        params = {"from": from_, "to": to, "max_id": max_id, "stream": stream,
-            "message_formats": message_formats}
-        return self._get(ChangelogListing, "/changelog", params)
+        params = {
+            "from": from_,
+            "to": to,
+            "max_id": max_id,
+            "stream": stream,
+            "message_formats": message_formats,
+        }
+        return await self._get(ChangelogListing, "/changelog", params)
 
     # TODO can almost certainly be combined with changelog_build endpoint, in
     # line with other get/lookup endpoint combinations (beatmap, beatmapset)
     @request(scope=None, category="changelog")
-    def changelog_build_lookup(self,
+    async def changelog_build_lookup(
+        self,
         changelog: str,
         *,
         key: Optional[str] = None,
-        message_formats: List[ChangelogMessageFormat] =
-            [ChangelogMessageFormat.HTML, ChangelogMessageFormat.MARKDOWN]
+        message_formats: List[ChangelogMessageFormat] = [
+            ChangelogMessageFormat.HTML,
+            ChangelogMessageFormat.MARKDOWN,
+        ],
     ) -> Build:
         """
         Look up a changelog build by version, update stream name, or id.
 
         Parameters
         ----------
         changelog
@@ -1693,26 +1902,22 @@
         Notes
         -----
         Implements the `Lookup Changelog Build
         <https://osu.ppy.sh/docs/index.html#lookup-changelog-build>`__ endpoint.
 
         """
         params = {"key": key, "message_formats": message_formats}
-        return self._get(Build, f"/changelog/{changelog}", params)
-
+        return await self._get(Build, f"/changelog/{changelog}", params)
 
     # /chat
     # -----
 
     @request(Scope.CHAT_WRITE, category="chat")
-    def send_pm(self,
-        user_id: UserIdT,
-        message: str,
-        *,
-        is_action: Optional[bool] = False
+    async def send_pm(
+        self, user_id: UserIdT, message: str, *, is_action: Optional[bool] = False
     ) -> CreatePMResponse:
         """
         Send a pm to a user.
 
         Parameters
         ----------
         user_id
@@ -1722,22 +1927,22 @@
         is_action
 
         Notes
         -----
         Implements the `Create New PM
         <https://osu.ppy.sh/docs/index.html#create-new-pm>`__ endpoint.
         """
-        data = {"target_id": user_id, "message": message,
-            "is_action": is_action}
-        return self._post(CreatePMResponse, "/chat/new", data=data)
+        data = {"target_id": user_id, "message": message, "is_action": is_action}
+        return await self._post(CreatePMResponse, "/chat/new", data=data)
 
     # this method requires a user in the announce group, so I've never tested
     # it.
     @request(Scope.CHAT_WRITE_MANAGE, category="chat")
-    def send_announcement(self,
+    async def send_announcement(
+        self,
         channel_name: str,
         channel_description: str,
         message: str,
         # TODO need to add support to automatic conversion for lists of id types
         # instead of just bare types (: UserIdT)
         target_ids: List[UserIdT],
     ) -> ChatChannel:
@@ -1771,34 +1976,34 @@
         dm me on discord (tybug#8490)!
         """
         data = {
             "channel.name": channel_name,
             "channel.description": channel_description,
             "message": message,
             "target_ids": target_ids,
-            "type": "ANNOUNCE"
+            "type": "ANNOUNCE",
         }
-        return self._post(ChatChannel, "/chat/channels", data=data)
-
+        return await self._post(ChatChannel, "/chat/channels", data=data)
 
     # /comments
     # ---------
 
     @request(Scope.PUBLIC, category="comments")
-    def comments(self,
+    async def comments(
+        self,
         *,
         commentable_type: Optional[CommentableTypeT] = None,
         commentable_id: Optional[int] = None,
         cursor: Optional[Cursor] = None,
         parent_id: Optional[int] = None,
-        sort: Optional[CommentSortT] = None
+        sort: Optional[CommentSortT] = None,
     ) -> CommentBundle:
         """
-        Get recent comments and their replies (up to 2 levels deep). If you only
-        want to retrieve a single comment, see :meth:`comment`.
+        Get comments and their replies (up to 2 levels deep). If you only want
+        to retrieve a single comment, see :meth:`comment`.
 
         Parameters
         ----------
         commentable_type
             The type of resource to get comments for.
         commentable_id
             The id of the resource to get comments for.
@@ -1811,47 +2016,46 @@
             the user-specified default when authenticated.
 
         Notes
         -----
         Implements the `Get Comments
         <https://osu.ppy.sh/docs/index.html#get-comments>`__ endpoint.
         """
-        params = {"commentable_type": commentable_type,
-            "commentable_id": commentable_id, "cursor": cursor,
-            "parent_id": parent_id, "sort": sort}
-        return self._get(CommentBundle, "/comments", params)
+        params = {
+            "commentable_type": commentable_type,
+            "commentable_id": commentable_id,
+            "cursor": cursor,
+            "parent_id": parent_id,
+            "sort": sort,
+        }
+        return await self._get(CommentBundle, "/comments", params)
 
     @request(scope=None, category="comments")
-    def comment(self,
-        comment_id: int
-    ) -> CommentBundle:
+    async def comment(self, comment_id: int) -> CommentBundle:
         """
         Get a comment and its replies (up to 2 levels deep).
 
         Parameters
         ----------
         comment_id
             The comment to get.
 
         Notes
         -----
         Implements the `Get a Comment
         <https://osu.ppy.sh/docs/index.html#get-a-comment>`__ endpoint.
         """
-        return self._get(CommentBundle, f"/comments/{comment_id}")
-
+        return await self._get(CommentBundle, f"/comments/{comment_id}")
 
     # /events
     # -------
 
     @request(Scope.PUBLIC, category="events")
-    def events(self,
-        *,
-        sort: Optional[EventsSortT] = None,
-        cursor_string: Optional[str] = None
+    async def events(
+        self, *, sort: Optional[EventsSortT] = None, cursor_string: Optional[str] = None
     ) -> Events:
         """
         Get most recent events, in order of creation time.
 
         Parameters
         ----------
         sort
@@ -1861,28 +2065,28 @@
 
         Notes
         -----
         Implements the `Get Events
         <https://osu.ppy.sh/docs/index.html#get-events>`__ endpoint.
         """
         params = {"cursor_string": cursor_string, "sort": sort}
-        return self._get(Events, "/events", params)
-
+        return await self._get(Events, "/events", params)
 
     # /forums
     # -------
 
     @request(Scope.FORUM_WRITE, category="forums")
-    def forum_create_topic(self,
-       forum_id: int,
-       title: str,
-       body: str,
-       *,
-       poll: Optional[ForumPoll] = None,
-   ) -> CreateForumTopicResponse:
+    async def forum_create_topic(
+        self,
+        forum_id: int,
+        title: str,
+        body: str,
+        *,
+        poll: Optional[ForumPoll] = None,
+    ) -> CreateForumTopicResponse:
         """
         https://osu.ppy.sh/docs/index.html#create-topic
         """
         data = {
             "body": body,
             "forum_id": forum_id,
             "title": title,
@@ -1892,18 +2096,18 @@
             data["forum_topic_poll[hide_results]"] = poll.hide_results
             data["forum_topic_poll[length_days]"] = poll.length_days
             data["forum_topic_poll[max_options]"] = poll.max_options
             data["forum_topic_poll[options]"] = "\r\n".join(poll.options)
             data["forum_topic_poll[title]"] = poll.title
             data["forum_topic_poll[vote_change]"] = poll.vote_change
 
-        return self._post(CreateForumTopicResponse, "/forums/topics", data=data)
+        return await self._post(CreateForumTopicResponse, "/forums/topics", data=data)
 
     @request(Scope.FORUM_WRITE, category="forums")
-    def forum_reply(self, topic_id: int, body: str) -> ForumPost:
+    async def forum_reply(self, topic_id: int, body: str) -> ForumPost:
         """
         Reply to a forum topic.
 
         Parameters
         ----------
         topic_id
             The topic to reply to.
@@ -1912,18 +2116,18 @@
 
         Notes
         -----
         Implements the `Reply Topic
         <https://osu.ppy.sh/docs/index.html#reply-topic>`__ endpoint.
         """
         data = {"body": body}
-        return self._post(ForumPost, f"/forums/topics/{topic_id}/reply", data)
+        return await self._post(ForumPost, f"/forums/topics/{topic_id}/reply", data)
 
     @request(Scope.FORUM_WRITE, category="forums")
-    def forum_edit_topic(self, topic_id: int, title: str) -> ForumTopic:
+    async def forum_edit_topic(self, topic_id: int, title: str) -> ForumTopic:
         """
         Edit a forum topic.
 
         Parameters
         ---------
         topic_id
             The topic to edit.
@@ -1932,18 +2136,18 @@
 
         Notes
         -----
         Implements the `Edit Topic
         <https://osu.ppy.sh/docs/index.html#edit-topic>`__ endpoint.
         """
         data = {"forum_topic[topic_title]": title}
-        return self._put(ForumTopic, f"/forums/topics/{topic_id}", data)
+        return await self._put(ForumTopic, f"/forums/topics/{topic_id}", data)
 
     @request(Scope.FORUM_WRITE, category="forums")
-    def forum_edit_post(self, post_id: int, body: str) -> ForumPost:
+    async def forum_edit_post(self, post_id: int, body: str) -> ForumPost:
         """
         Edit a forum post.
 
         Parameters
         ----------
         post_id
             The post to edit.
@@ -1952,25 +2156,26 @@
 
         Notes
         -----
         Implements the `Edit Post
         <https://osu.ppy.sh/docs/index.html#edit-post>`__ endpoint.
         """
         data = {"body": body}
-        return self._put(ForumPost, f"/forums/posts/{post_id}", data)
+        return await self._put(ForumPost, f"/forums/posts/{post_id}", data)
 
     @request(Scope.PUBLIC, category="forums")
-    def forum_topic(self,
+    async def forum_topic(
+        self,
         topic_id: int,
         *,
         cursor_string: Optional[str] = None,
         sort: Optional[ForumTopicSortT] = None,
         limit: Optional[int] = None,
         start: Optional[int] = None,
-        end: Optional[int] = None
+        end: Optional[int] = None,
     ) -> ForumTopicAndPosts:
         """
         Get a forum topic and its posts.
 
         Parameters
         ----------
         topic_id
@@ -1991,45 +2196,48 @@
             Ignored otherwise.
 
         Notes
         -----
         Implements the `Get Topic and Posts
         <https://osu.ppy.sh/docs/index.html#get-topic-and-posts>`__ endpoint.
         """
-        params = {"cursor_string": cursor_string, "sort": sort, "limit": limit,
-            "start": start, "end": end}
-        return self._get(ForumTopicAndPosts, f"/forums/topics/{topic_id}",
-            params)
-
+        params = {
+            "cursor_string": cursor_string,
+            "sort": sort,
+            "limit": limit,
+            "start": start,
+            "end": end,
+        }
+        return await self._get(ForumTopicAndPosts, f"/forums/topics/{topic_id}", params)
 
     # /friends
     # --------
 
     @request(Scope.FRIENDS_READ, category="friends")
-    def friends(self) -> List[UserCompact]:
+    async def friends(self) -> List[UserCompact]:
         """
         Get the friends of the authenticated user.
 
         Notes
         -----
         Implements the `Get Friends
         <https://osu.ppy.sh/docs/index.html#friends>`__ endpoint.
         """
-        return self._get(List[UserCompact], "/friends")
-
+        return await self._get(List[UserCompact], "/friends")
 
     # / ("home")
     # ----------
 
     @request(Scope.PUBLIC, category="home")
-    def search(self,
+    async def search(
+        self,
         query: str,
         *,
         mode: Optional[SearchModeT] = None,
-        page: Optional[int] = None
+        page: Optional[int] = None,
     ) -> Search:
         """
         Search users and wiki pages. If you want to search beatmapsets, see
         :meth:`search_beatmapsets`.
 
         Parameters
         ----------
@@ -2042,91 +2250,88 @@
 
         Notes
         -----
         Implements the `Search
         <https://osu.ppy.sh/docs/index.html#search>`__ endpoint.
         """
         params = {"mode": mode, "query": query, "page": page}
-        return self._get(Search, "/search", params)
-
+        return await self._get(Search, "/search", params)
 
     # /matches
     # --------
 
     @request(Scope.PUBLIC, category="matches")
-    def matches(self) -> Matches:
+    async def matches(self) -> Matches:
         """
         Get current matches. If you want to get a specific match, see
         :meth:`match`.
 
         Notes
         -----
         Implements the `Get Matches
         <https://osu.ppy.sh/docs/index.html#matches>`__ endpoint.
         """
-        return self._get(Matches, "/matches")
+        return await self._get(Matches, "/matches")
 
     @request(Scope.PUBLIC, category="matches")
-    def match(self,
+    def match(
+        self,
         match_id: MatchIdT,
         *,
-        after: Optional[int] = None,
-        before: Optional[int] = None,
-        limit: Optional[int] = None
+        after_id: Optional[int] = None,
+        before_id: Optional[int] = None,
+        limit: Optional[int] = None,
     ) -> MatchResponse:
         """
         Get a match (eg https://osu.ppy.sh/community/matches/97947404).
 
         Parameters
         ----------
         match_id
             The match to get.
 
         Notes
         -----
         Implements the `Get Match
         <https://osu.ppy.sh/docs/index.html#matchesmatch>`__ endpoint.
         """
-        params = {"after": after, "before": before, "limit": limit}
+        params = {"after": after_id, "before": before_id, "limit": limit}
         return self._get(MatchResponse, f"/matches/{match_id}", params=params)
 
-
     # /me
     # ---
 
     @request(Scope.IDENTIFY, category="me")
-    def get_me(self,
-        mode: Optional[GameModeT] = None
-    ) -> User:
+    async def get_me(self, mode: Optional[GameModeT] = None):
         """
         Get data about the authenticated user.
 
         Parameters
         ----------
         mode
             Get data about the specified mode. Defaults to the user's default
             mode.
 
         Notes
         -----
         Implements the `Get Own Data
         <https://osu.ppy.sh/docs/index.html#get-own-data>`__ endpoint.
         """
-        return self._get(User, f"/me/{mode.value if mode else ''}")
-
+        return await self._get(User, f"/me/{mode.value if mode else ''}")
 
     # /news
     # -----
 
     @request(scope=None, category="news")
-    def news_listing(self,
+    async def news_listing(
+        self,
         *,
         limit: Optional[int] = None,
         year: Optional[int] = None,
-        cursor_string: Optional[str] = None
+        cursor_string: Optional[str] = None,
     ) -> NewsListing:
         """
         Get news posts.
 
         Parameters
         ----------
         limit
@@ -2138,21 +2343,19 @@
 
         Notes
         -----
         Implements the `Get News Listing
         <https://osu.ppy.sh/docs/index.html#get-news-listing>`__ endpoint.
         """
         params = {"limit": limit, "year": year, "cursor_string": cursor_string}
-        return self._get(NewsListing, "/news", params=params)
+        return await self._get(NewsListing, "/news", params=params)
 
     @request(scope=None, category="news")
-    def news_post(self,
-        news: str,
-        *,
-        key: Optional[NewsPostKeyT] = NewsPostKey.SLUG
+    async def news_post(
+        self, news: str, *, key: Optional[NewsPostKeyT] = NewsPostKey.SLUG
     ) -> NewsPost:
         """
         Get a news post by id or slug.
 
         Parameters
         ----------
         news
@@ -2165,48 +2368,47 @@
         Implements the `Get News Post
         <https://osu.ppy.sh/docs/index.html#get-news-post>`__ endpoint.
         """
         # docs state key should be "unset to query by slug"
         if key is NewsPostKey.SLUG:
             key = None
         params = {"key": key}
-        return self._get(NewsPost, f"/news/{news}", params=params)
-
+        return await self._get(NewsPost, f"/news/{news}", params=params)
 
     # /oauth
     # ------
 
     @request(scope=None, category="oauth")
-    def revoke_token(self):
+    async def revoke_token(self):
         """
         Revoke the current token. This will remove any authentication and leave
         you unable to make any more api calls until you re-authenticate.
 
         Notes
         -----
         Implements the `Revoke Current Token
         <https://osu.ppy.sh/docs/index.html#revoke-current-token>`__ endpoint.
         """
         self.session.delete(f"{self.base_url}/oauth/tokens/current")
         self.remove_token(self.token_key, self.token_directory)
 
-
     # /rankings
     # ---------
 
     @request(Scope.PUBLIC, category="rankings")
-    def ranking(self,
+    async def ranking(
+        self,
         mode: GameModeT,
         type: RankingTypeT,
         *,
         country: Optional[str] = None,
         cursor: Optional[Cursor] = None,
         filter_: RankingFilterT = RankingFilter.ALL,
         spotlight: Optional[int] = None,
-        variant: Optional[str] = None
+        variant: Optional[str] = None,
     ) -> Rankings:
         """
         Get current rankings for the specified game mode. Can specify ``type``
         to get different types of rankings (performance, score, country, etc).
 
         Parameters
         ----------
@@ -2230,33 +2432,39 @@
             mania. Only available for ``RankingType.PERFORMANCE``.
 
         Notes
         -----
         Implements the `Get Ranking
         <https://osu.ppy.sh/docs/index.html#get-ranking>`__ endpoint.
         """
-        params = {"country": country, "cursor": cursor, "filter": filter_,
-            "spotlight": spotlight, "variant": variant}
-        return self._get(Rankings, f"/rankings/{mode.value}/{type.value}",
-            params=params)
-
+        params = {
+            "country": country,
+            "cursor": cursor,
+            "filter": filter_,
+            "spotlight": spotlight,
+            "variant": variant,
+        }
+        return await self._get(
+            Rankings, f"/rankings/{mode.value}/{type.value}", params=params
+        )
 
     # /rooms
     # ------
 
     # TODO add test for this once I figure out values for room_id and
     # playlist_id that actually produce a response lol
     @request(Scope.PUBLIC, category="rooms")
-    def multiplayer_scores(self,
+    async def multiplayer_scores(
+        self,
         room_id: int,
         playlist_id: int,
         *,
         limit: Optional[int] = None,
         sort: Optional[MultiplayerScoresSortT] = None,
-        cursor_string: Optional[str] = None
+        cursor_string: Optional[str] = None,
     ) -> MultiplayerScores:
         """
         Get scores on a playlist item in a room.
 
         Parameters
         ----------
         room_id
@@ -2272,61 +2480,65 @@
 
         Notes
         -----
         Implements the `Get Scores
         <https://osu.ppy.sh/docs/index.html#get-scores>`__ endpoint.
         """
         params = {"limit": limit, "sort": sort, "cursor_string": cursor_string}
-        return self._get(MultiplayerScores,
-            f"/rooms/{room_id}/playlist/{playlist_id}/scores", params=params)
+        return await self._get(
+            MultiplayerScores,
+            f"/rooms/{room_id}/playlist/{playlist_id}/scores",
+            params=params,
+        )
 
     @request(Scope.PUBLIC, category="rooms")
-    def room(self, room_id: RoomIdT) -> Room:
+    async def room(self, room_id: RoomIdT) -> Room:
         """
         Get a room.
 
         Parameters
         ----------
         room_id
             The room to get.
 
         Notes
         -----
         Implements the `Get Room
         <https://osu.ppy.sh/docs/index.html#roomsroom>`__ endpoint.
         """
-        return self._get(Room, f"/rooms/{room_id}")
+        return await self._get(Room, f"/rooms/{room_id}")
 
     @request(Scope.PUBLIC, requires_user=True, category="rooms")
-    def room_leaderboard(self, room_id: RoomIdT) -> RoomLeaderboard:
+    async def room_leaderboard(self, room_id: RoomIdT) -> RoomLeaderboard:
         """
         Get the leaderboard of a room.
 
         Parameters
         ----------
         room_id
             The room to get the leaderboard of.
 
         Notes
         -----
         Implements the `Get Room Leaderboard
         <https://osu.ppy.sh/docs/index.html#roomsroomleaderboard>`__ endpoint.
         """
-        return self._get(RoomLeaderboard, f"/rooms/{room_id}/leaderboard")
+        return await self._get(RoomLeaderboard, f"/rooms/{room_id}/leaderboard")
 
     @request(Scope.PUBLIC, requires_user=True, category="rooms")
-    def rooms(self,
+    async def rooms(
+        self,
         *,
         limit: Optional[int] = None,
         mode: Optional[RoomSearchModeT] = None,
         season_id: Optional[int] = None,
         # TODO enumify
         sort: Optional[str] = None,
         # TODO enumify
-        type_group: Optional[str] = None
+        type_group: Optional[str] = None,
     ) -> List[Room]:
         """
         Get the list of current rooms.
 
         Parameters
         ----------
         limit
@@ -2341,140 +2553,193 @@
             "playlists" (default) or "realtime".
 
         Notes
         -----
         Implements the `Get Rooms
         <https://osu.ppy.sh/docs/index.html#roomsmode>`__ endpoint.
         """
-        params = {"limit": limit, "mode": mode, "season_id": season_id,
-            "sort": sort, "type_group": type_group}
-        return self._get(List[Room], "/rooms", params=params)
-
+        params = {
+            "limit": limit,
+            "mode": mode,
+            "season_id": season_id,
+            "sort": sort,
+            "type_group": type_group,
+        }
+        return await self._get(List[Room], "/rooms", params=params)
 
     # /scores
     # -------
 
     @request(Scope.PUBLIC, category="scores")
-    def score(self,
-        mode: GameModeT,
-        score_id: int
-    ) -> Score:
+    def score(self, score_id: int) -> Score:
         """
-        Get a score.
+        Get a score. This corresponds to urls of the form https://osu.ppy.sh/scores/1312718771
+        ("new id format").
+
+        If you have an old id which is per-gamemode, use api.score_mode.
 
         Parameters
         ----------
-        mode
-            The mode the score was set on.
         score_id
             The score to get.
 
         Notes
         -----
         Implements the `Get Score
         <https://osu.ppy.sh/docs/index.html#scoresmodescore>`__ endpoint.
         """
-        return self._get(Score, f"/scores/{mode.value}/{score_id}")
+        return self._get(Score, f"/scores/{score_id}")
 
-    @request(Scope.PUBLIC, requires_user=True, category="scores")
-    def download_score(self,
-        mode: GameModeT,
-        score_id: int,
-        *,
-        raw: bool = False
-    ) -> Replay:
+    @request(Scope.PUBLIC, category="scores")
+    def score_mode(self, mode: GameModeT, score_id: int) -> Score:
         """
-        Download the replay data of a score.
+        Get a score, where the score id is specific to the gamemode. This
+        corresponds to urls of the form https://osu.ppy.sh/scores/osu/4459998279
+        ("old id format").
+
+        If you have a new id which is global across gamemodes, use api.score.
 
         Parameters
         ----------
         mode
-            The mode of the score to download.
+            The mode the score was set on.
         score_id
-            The score to download.
-        raw
-            If ``True``, will return the raw string response from the api
-            instead of a :class:`~ossapi.replay.Replay` object.
+            The score to get.
 
         Notes
         -----
-        Implements the `Download Score
-        <https://osu.ppy.sh/docs/index.html#scoresmodescoredownload>`__
-        endpoint.
+        Implements the `Get Score
+        <https://osu.ppy.sh/docs/index.html#scoresmodescore>`__ endpoint.
         """
-        if self.domain is Domain.LAZER:
-            raise ValueError("Downloading scores using the lazer domain is not "
-                "currently supported, as lazer itself does not currently "
-                "support replay downloads. This may change in the future. To "
-                "download replays, use the osu domain (ie, a normal Ossapi "
-                "instance.)")
+        return self._get(Score, f"/scores/{mode.value}/{score_id}")
 
-        url = f"{self.base_url}/scores/{mode.value}/{score_id}/download"
-        r = self.session.get(url)
+    async def _download_score(self, *, url, raw):
+        from aiohttp import ClientSession, ContentTypeError
+
+        aiohttp_session = ClientSession()
+        r = await self.session.request_async("GET", url, session=aiohttp_session)
 
         # if the response above succeeded, it will return a raw string
         # instead of json. If it didn't succeed, it will return json with an
         # error.
         # So always try parsing as json to check if there's an error. If parsing
         # fails, just assume the request succeeded and move on.
+        # TODO we probably want to be checking headers here instead.
+        # Should be x-osu-replay for valid response.
         try:
-            json_ = r.json()
+            json_ = await r.json()
+            await aiohttp_session.close()
             self._check_response(json_, url)
-        except json.JSONDecodeError:
+        except ContentTypeError:
             pass
 
+        content = await r.read()
+        await aiohttp_session.close()
+
         if raw:
-            return r.content
+            return content
 
-        replay = osrparse.Replay.from_string(r.content)
+        replay = osrparse.Replay.from_string(content)
         return Replay(replay, self)
 
+    @request(Scope.PUBLIC, requires_user=True, category="scores")
+    async def download_score(self, score_id: int, *, raw: bool = False) -> Replay:
+        """
+        Download the replay data of a score.
+
+        This endpoint is for score ids which don't have a matching gamemode
+        (new id format). If you have an old score id, use api.download_score_mode.
+
+        Parameters
+        ----------
+        score_id
+            The score to download.
+        raw
+            If ``True``, will return the raw string response from the api
+            instead of a :class:`~ossapi.replay.Replay` object.
+
+        Notes
+        -----
+        Implements the `Download Score
+        <https://osu.ppy.sh/docs/index.html#scoresmodescoredownload>`__
+        endpoint.
+        """
+        url = f"{self.base_url}/scores/{score_id}/download"
+        return await self._download_score(url=url, raw=raw)
+
+    @request(Scope.PUBLIC, requires_user=True, category="scores")
+    async def download_score_mode(
+        self, mode: GameModeT, score_id: int, *, raw: bool = False
+    ) -> Replay:
+        """
+        Download the replay data of a score.
+
+        This endpoint is for score ids which have a matching gamemode
+        (old id format). If you have a new score id, use api.download_score.
+
+        Parameters
+        ----------
+        mode
+            The mode of the score to download.
+        score_id
+            The score to download.
+        raw
+            If ``True``, will return the raw string response from the api
+            instead of a :class:`~ossapi.replay.Replay` object.
+
+        Notes
+        -----
+        Implements the `Download Score
+        <https://osu.ppy.sh/docs/index.html#scoresmodescoredownload>`__
+        endpoint.
+        """
+        url = f"{self.base_url}/scores/{mode.value}/{score_id}/download"
+        return await self._download_score(url=url, raw=raw)
 
     # seasonal backgrounds
     # --------------------
 
     @request(scope=None, category="seasonal backgrounds")
-    def seasonal_backgrounds(self) -> SeasonalBackgrounds:
+    async def seasonal_backgrounds(self) -> SeasonalBackgrounds:
         """
         Get current seasonal backgrounds.
 
         Notes
         -----
         Implements the `Seasonal Backgrounds
         <https://osu.ppy.sh/docs/index.html#seasonal-backgrounds>`__ endpoint.
         """
-        return self._get(SeasonalBackgrounds, "/seasonal-backgrounds")
-
+        return await self._get(SeasonalBackgrounds, "/seasonal-backgrounds")
 
     # /spotlights
     # -----------
 
     @request(Scope.PUBLIC, category="spotlights")
-    def spotlights(self) -> List[Spotlight]:
+    async def spotlights(self) -> List[Spotlight]:
         """
         Get active spotlights.
 
         Notes
         -----
         Implements the `Get Spotlights
         <https://osu.ppy.sh/docs/index.html#get-spotlights>`__ endpoint.
         """
-        spotlights = self._get(Spotlights, "/spotlights")
+        spotlights = await self._get(Spotlights, "/spotlights")
         return spotlights.spotlights
 
-
     # /users
     # ------
 
     @request(Scope.PUBLIC, category="users")
-    def user_kudosu(self,
+    async def user_kudosu(
+        self,
         user_id: UserIdT,
         *,
         limit: Optional[int] = None,
-        offset: Optional[int] = None
+        offset: Optional[int] = None,
     ) -> List[KudosuHistory]:
         """
         Get user kudosu history.
 
         Parameters
         ----------
         user_id
@@ -2486,26 +2751,26 @@
 
         Notes
         -----
         Implements the `Get User Kudosu
         <https://osu.ppy.sh/docs/index.html#get-user-kudosu>`__ endpoint.
         """
         params = {"limit": limit, "offset": offset}
-        return self._get(List[KudosuHistory], f"/users/{user_id}/kudosu",
-            params)
+        return await self._get(List[KudosuHistory], f"/users/{user_id}/kudosu", params)
 
     @request(Scope.PUBLIC, category="users")
-    def user_scores(self,
+    async def user_scores(
+        self,
         user_id: UserIdT,
         type: ScoreTypeT,
         *,
         include_fails: Optional[bool] = None,
         mode: Optional[GameModeT] = None,
         limit: Optional[int] = None,
-        offset: Optional[int] = None
+        offset: Optional[int] = None,
     ) -> List[Score]:
         """
         Get scores of a user.
 
         user_id
             The user to get scores of.
         type
@@ -2528,26 +2793,32 @@
         # require a bool to be passed, and just do the conversion behind the
         # scenes.
         if include_fails is False:
             include_fails = 0
         if include_fails is True:
             include_fails = 1
 
-        params = {"include_fails": include_fails, "mode": mode, "limit": limit,
-            "offset": offset}
-        return self._get(List[Score], f"/users/{user_id}/scores/{type.value}",
-            params)
+        params = {
+            "include_fails": include_fails,
+            "mode": mode,
+            "limit": limit,
+            "offset": offset,
+        }
+        return await self._get(
+            List[Score], f"/users/{user_id}/scores/{type.value}", params
+        )
 
     @request(Scope.PUBLIC, category="users")
-    def user_beatmaps(self,
+    async def user_beatmaps(
+        self,
         user_id: UserIdT,
         type: UserBeatmapTypeT,
         *,
         limit: Optional[int] = None,
-        offset: Optional[int] = None
+        offset: Optional[int] = None,
     ) -> Union[List[Beatmapset], List[BeatmapPlaycount]]:
         """
         Get beatmaps of a user.
 
         Parameters
         ----------
         user_id
@@ -2571,23 +2842,25 @@
         """
         params = {"limit": limit, "offset": offset}
 
         return_type = List[Beatmapset]
         if type is UserBeatmapType.MOST_PLAYED:
             return_type = List[BeatmapPlaycount]
 
-        return self._get(return_type,
-            f"/users/{user_id}/beatmapsets/{type.value}", params)
+        return await self._get(
+            return_type, f"/users/{user_id}/beatmapsets/{type.value}", params
+        )
 
     @request(Scope.PUBLIC, category="users")
-    def user_recent_activity(self,
+    async def user_recent_activity(
+        self,
         user_id: UserIdT,
         *,
         limit: Optional[int] = None,
-        offset: Optional[int] = None
+        offset: Optional[int] = None,
     ) -> List[Event]:
         """
         Get recent activity of a user.
 
         Parameters
         ----------
         user_id
@@ -2600,23 +2873,25 @@
         Notes
         -----
         Implements the `Get User Recent Activity
         <https://osu.ppy.sh/docs/index.html#get-user-recent-activity>`__
         endpoint.
         """
         params = {"limit": limit, "offset": offset}
-        return self._get(List[_Event], f"/users/{user_id}/recent_activity/",
-            params)
+        return await self._get(
+            List[_Event], f"/users/{user_id}/recent_activity/", params
+        )
 
     @request(Scope.PUBLIC, category="users")
-    def user(self,
+    async def user(
+        self,
         user: Union[UserIdT, str],
         *,
         mode: Optional[GameModeT] = None,
-        key: Optional[UserLookupKeyT] = None
+        key: Optional[UserLookupKeyT] = None,
     ) -> User:
         """
         Get a user by id or username.
 
         user
             The user id or username of the user to get.
         mode
@@ -2628,21 +2903,20 @@
 
         Notes
         -----
         Implements the `Get User
         <https://osu.ppy.sh/docs/index.html#get-user>`__ endpoint.
         """
         params = {"key": key}
-        return self._get(User, f"/users/{user}/{mode.value if mode else ''}",
-            params)
+        return await self._get(
+            User, f"/users/{user}/{mode.value if mode else ''}", params
+        )
 
     @request(Scope.PUBLIC, category="users")
-    def users(self,
-        user_ids: List[int]
-    ) -> List[UserCompact]:
+    async def users(self, user_ids: List[int]) -> List[UserCompact]:
         """
         Batch get users by id. If you only want to retrieve a single user, or
         want to retrieve users by username instead of id, see :meth:`user`.
 
         Parameters
         ---------
         user_ids
@@ -2650,24 +2924,22 @@
 
         Notes
         -----
         Implements the `Get Users
         <https://osu.ppy.sh/docs/index.html#get-users>`__ endpoint.
         """
         params = {"ids": user_ids}
-        return self._get(Users, "/users", params).users
+        users = await self._get(Users, "/users", params)
+        return users.users
 
     # /wiki
     # -----
 
     @request(scope=None, category="wiki")
-    def wiki_page(self,
-        locale: str,
-        path: str
-    ) -> WikiPage:
+    async def wiki_page(self, locale: str, path: str) -> WikiPage:
         """
         Get a wiki page.
 
         Parameters
         ----------
         locale
             two letter language code of the wiki page.
@@ -2675,8 +2947,8 @@
             The path name of the wiki page.
 
         Notes
         -----
         Implements the `Get Wiki Page
         <https://osu.ppy.sh/docs/index.html#get-wiki-page>`__ endpoint.
         """
-        return self._get(WikiPage, f"/wiki/{locale}/{path}")
+        return await self._get(WikiPage, f"/wiki/{locale}/{path}")
```

### Comparing `ossapi-3.4.4/ossapi/ossapiv2_async.py` & `ossapi-4.0.0b1/ossapi/ossapiv2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-# This file has been copied wholesale from ossapiv2.py, with minor adjustments
-# to make functions async and work around aiohttp vs requests differences.
-# No changes should be made here without changing ossapiv2 as well (the
-# converse may not necessarily be true, as I consider the sync part of the
-# library more important than the async).
-# I may eventually write a code generator to copy ossapiv2.py and automatically
-# adjust for async. I'm not sure it's worthwhile just yet given how finnicky it
-# will be to hardcode the insertion points of all the particular changes I've
-# made.
-
 from typing import Union, TypeVar, Optional, List, _GenericAlias
 import logging
 import webbrowser
 import socket
 import pickle
 from pathlib import Path
 from datetime import datetime
@@ -20,120 +10,133 @@
 import inspect
 import json
 import hashlib
 import functools
 import sys
 
 from requests_oauthlib import OAuth2Session
-from requests_oauthlib.oauth2_session import TokenUpdated
-from oauthlib.oauth2 import (BackendApplicationClient, TokenExpiredError,
-    AccessDeniedError, InsecureTransportError, is_secure_transport, OAuth2Error)
+from oauthlib.oauth2 import (
+    BackendApplicationClient,
+    TokenExpiredError,
+    AccessDeniedError,
+    OAuth2Error,
+)
 from oauthlib.oauth2.rfc6749.errors import InsufficientScopeError
 from oauthlib.oauth2.rfc6749.tokens import OAuth2Token
 import osrparse
 from typing_utils import issubtype, get_type_hints, get_origin, get_args
 
 import ossapi
-from ossapi.models import (Beatmap, BeatmapCompact, BeatmapUserScore,
-    ForumTopicAndPosts, Search, CommentBundle, Cursor, Score,
-    BeatmapsetSearchResult, ModdingHistoryEventsBundle, User, Rankings,
-    BeatmapScores, KudosuHistory, Beatmapset, BeatmapPlaycount, Spotlight,
-    Spotlights, WikiPage, _Event, Event, BeatmapsetDiscussionPosts, Build,
-    ChangelogListing, MultiplayerScores,
-    BeatmapsetDiscussionVotes, CreatePMResponse, BeatmapsetDiscussions,
-    UserCompact, NewsListing, NewsPost, SeasonalBackgrounds, BeatmapsetCompact,
-    BeatmapUserScores, DifficultyAttributes, Users, Beatmaps,
-    CreateForumTopicResponse, ForumPoll, ForumPost, ForumTopic, Room,
-    RoomLeaderboard, Matches, Match, MatchResponse, ChatChannel, Events,
-    BeatmapPack, BeatmapPacks)
-from ossapi.enums import (GameMode, ScoreType, RankingFilter, RankingType,
-    UserBeatmapType, BeatmapDiscussionPostSort, UserLookupKey,
-    BeatmapsetEventType, CommentableType, CommentSort, ForumTopicSort,
-    SearchMode, MultiplayerScoresSort, BeatmapsetDiscussionVote,
-    BeatmapsetDiscussionVoteSort, BeatmapsetStatus, MessageType,
-    BeatmapsetSearchCategory, BeatmapsetSearchMode,
-    BeatmapsetSearchExplicitContent, BeatmapsetSearchGenre,
-    BeatmapsetSearchLanguage, NewsPostKey, BeatmapsetSearchSort, RoomSearchMode,
-    ChangelogMessageFormat, EventsSort, BeatmapPackType)
-from ossapi.utils import (is_primitive_type, is_optional, is_base_model_type,
-    is_model_type, is_high_model_type, Field, convert_primitive_type)
+from ossapi.models import (
+    Beatmap,
+    BeatmapCompact,
+    BeatmapUserScore,
+    ForumTopicAndPosts,
+    Search,
+    CommentBundle,
+    Cursor,
+    Score,
+    BeatmapsetSearchResult,
+    ModdingHistoryEventsBundle,
+    User,
+    Rankings,
+    BeatmapScores,
+    KudosuHistory,
+    Beatmapset,
+    BeatmapPlaycount,
+    Spotlight,
+    Spotlights,
+    WikiPage,
+    _Event,
+    Event,
+    BeatmapsetDiscussionPosts,
+    Build,
+    ChangelogListing,
+    MultiplayerScores,
+    BeatmapsetDiscussionVotes,
+    CreatePMResponse,
+    BeatmapsetDiscussions,
+    UserCompact,
+    NewsListing,
+    NewsPost,
+    SeasonalBackgrounds,
+    BeatmapsetCompact,
+    BeatmapUserScores,
+    DifficultyAttributes,
+    Users,
+    Beatmaps,
+    CreateForumTopicResponse,
+    ForumPoll,
+    ForumPost,
+    ForumTopic,
+    Room,
+    RoomLeaderboard,
+    Matches,
+    Match,
+    MatchResponse,
+    ChatChannel,
+    Events,
+    BeatmapPack,
+    BeatmapPacks,
+    _NonLegacyBeatmapScores,
+)
+from ossapi.enums import (
+    GameMode,
+    ScoreType,
+    RankingFilter,
+    RankingType,
+    UserBeatmapType,
+    BeatmapDiscussionPostSort,
+    UserLookupKey,
+    BeatmapsetEventType,
+    CommentableType,
+    CommentSort,
+    ForumTopicSort,
+    SearchMode,
+    MultiplayerScoresSort,
+    BeatmapsetDiscussionVote,
+    BeatmapsetDiscussionVoteSort,
+    BeatmapsetStatus,
+    MessageType,
+    BeatmapsetSearchCategory,
+    BeatmapsetSearchMode,
+    BeatmapsetSearchExplicitContent,
+    BeatmapsetSearchGenre,
+    BeatmapsetSearchLanguage,
+    NewsPostKey,
+    BeatmapsetSearchSort,
+    RoomSearchMode,
+    ChangelogMessageFormat,
+    EventsSort,
+    BeatmapPackType,
+)
+from ossapi.utils import (
+    is_primitive_type,
+    is_optional,
+    is_base_model_type,
+    is_model_type,
+    is_high_model_type,
+    Field,
+    convert_primitive_type,
+)
 from ossapi.mod import Mod
 from ossapi.replay import Replay
 
-
-class Oauth2SessionAsync(OAuth2Session):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        headers = {"User-Agent": f"ossapi (v{ossapi.__version__})"}
-        self.headers.update(headers)
-
-    # this method is shamelessly copied from `OAuth2Session.request`, modified
-    # to call `self.session.request` instead of `super().request`.
-    # Any OAuth2Session code which calls `request` will remain sync, but we have
-    # control over the vast majority of code which interacts with the session
-    # object and can switch to calling this async function instead.
-    # This means things like refreshing the token will still be sync. A
-    # negligible hit for a huge maintainability increase.
-    async def request_async(
-        self,
-        method,
-        url,
-        *,
-        session,
-        data=None,
-        headers=None,
-        withhold_token=False,
-        client_id=None,
-        client_secret=None,
-        **kwargs
-    ):
-        import aiohttp
-        if not is_secure_transport(url):
-            raise InsecureTransportError()
-        if self.token and not withhold_token:
-            for hook in self.compliance_hook["protected_request"]:
-                url, headers, data = hook(url, headers, data)
-
-            try:
-                url, headers, data = self._client.add_token(
-                    url, http_method=method, body=data, headers=headers
-                )
-            except TokenExpiredError:
-                if self.auto_refresh_url:
-                    auth = kwargs.pop("auth", None)
-                    if client_id and client_secret and (auth is None):
-                        auth = aiohttp.BasicAuth(client_id, client_secret)
-                    token = self.refresh_token(
-                        self.auto_refresh_url, auth=auth, **kwargs
-                    )
-                    if self.token_updater:
-                        self.token_updater(token)
-                        url, headers, data = self._client.add_token(
-                            url, http_method=method, body=data, headers=headers
-                        )
-                    else:
-                        raise TokenUpdated(token)
-                else:
-                    raise
-
-        return await session.request(
-            method, url, headers=headers, data=data, **kwargs
-        )
-
 # our `request` function below relies on the ordering of these types. The
 # base type must come first, with any auxiliary types that the base type accepts
 # coming after.
 # These types are intended to provide better type hinting for consumers. We
 # want to support the ability to pass `"osu"` instead of `GameMode.STD`,
 # for instance. We automatically convert any value to its base class if the
 # relevant parameter has a type hint of the form below (see `request` for
 # details).
 GameModeT = Union[GameMode, str]
 ScoreTypeT = Union[ScoreType, str]
+# XXX this cannot be recursively typed without breaking our runtime type hint
+# inspection.
 ModT = Union[Mod, str, int, List[Union[Mod, str, int]]]
 RankingFilterT = Union[RankingFilter, str]
 RankingTypeT = Union[RankingType, str]
 UserBeatmapTypeT = Union[UserBeatmapType, str]
 BeatmapDiscussionPostSortT = Union[BeatmapDiscussionPostSort, str]
 UserLookupKeyT = Union[UserLookupKey, str]
 BeatmapsetEventTypeT = Union[BeatmapsetEventType, str]
@@ -159,14 +162,15 @@
 
 BeatmapIdT = Union[int, BeatmapCompact]
 UserIdT = Union[int, UserCompact]
 BeatmapsetIdT = Union[int, BeatmapCompact, BeatmapsetCompact]
 RoomIdT = Union[int, Room]
 MatchIdT = Union[int, Match]
 
+
 def request(scope, *, requires_user=False, category):
     """
     Handles various validation and preparation tasks for any endpoint request
     method.
 
     This method does the following things:
     * makes sure the client has the requuired scope to access the endpoint in
@@ -191,39 +195,44 @@
     requires_user: bool
         Whether this endpoint requires a user to be associated with the grant.
         Currently, only authtorization code grants can access these endpoints.
     category: str
         What category of endpoints this endpoint belongs to. Used for grouping
         in the docs.
     """
+
     def decorator(function):
         instantiate = {}
         for name, type_ in function.__annotations__.items():
             origin = get_origin(type_)
             args = get_args(type_)
             if origin is Union and is_base_model_type(args[0]):
                 instantiate[name] = type_
 
         arg_names = list(inspect.signature(function).parameters)
 
         @functools.wraps(function)
         def wrapper(*args, **kwargs):
             self = args[0]
             if scope is not None and scope not in self.scopes:
-                raise InsufficientScopeError(f"A scope of {scope} is required "
+                raise InsufficientScopeError(
+                    f"A scope of {scope} is required "
                     "for this endpoint. Your client's current scopes are "
-                    f"{self.scopes}")
+                    f"{self.scopes}"
+                )
 
             if requires_user and self.grant is Grant.CLIENT_CREDENTIALS:
-                raise AccessDeniedError("To access this endpoint you must be "
+                raise AccessDeniedError(
+                    "To access this endpoint you must be "
                     "authorized using the authorization code grant. You are "
                     "currently authorized with the client credentials grant."
                     "\n\n"
                     "For more details, see "
-                    "https://tybug.github.io/ossapi/grants.html.")
+                    "https://tybug.github.io/ossapi/grants.html."
+                )
 
             # we may need to edit this later so convert from tuple
             args = list(args)
 
             def id_from_id_type(arg_name, arg):
                 annotations = function.__annotations__
                 if arg_name not in annotations:
@@ -281,68 +290,83 @@
             return function(*args, **kwargs)
 
         # for docs generation
         wrapper.__ossapi_category__ = category
         wrapper.__ossapi_scope__ = scope
 
         return wrapper
+
     return decorator
 
 
 class ReauthenticationRequired(Exception):
     """
     Indicates that either the user has revoked this application from their
     account, or osu-web itself has invalidated the refresh token associated with
     this application.
+
     This exception is only raised when a manual access_token is passed to
     Ossapi, to bypass Ossapi's default authentication methods. The expectation
     is that in these cases, the consumer has their own way of authenticating
     with the user. That method should be used here to handle the
     reauthentication.
     """
+
     pass
 
+
 class Grant(Enum):
     """
     The grant types used by the api.
     """
+
     CLIENT_CREDENTIALS = "client"
     AUTHORIZATION_CODE = "authorization"
 
+
 class Scope(Enum):
     """
     The OAuth scopes used by the api.
     """
+
     CHAT_WRITE = "chat.write"
     CHAT_WRITE_MANAGE = "chat.write_manage"
     CHAT_READ = "chat.read"
     DELEGATE = "delegate"
     FORUM_WRITE = "forum.write"
     FRIENDS_READ = "friends.read"
     IDENTIFY = "identify"
     PUBLIC = "public"
 
+
 class Domain(Enum):
     """
     Different possible api domains. These correspond to different deployments of
-    the osu server: osu.ppy.sh, lazer.ppy.sh, and dev.ppy.sh respectively.
+    the osu server, such as osu.ppy.sh or dev.ppy.sh.
 
     The default domain, and the one the vast majority of users want, is
     :data:`Domain.OSU <ossapi.ossapiv2.Domain.OSU>`, and corresponds to the
-    main website. To retrieve information from the lazer website or the dev
-    website, use the corresponding domain.
+    main website.
     """
+
     OSU = "osu"
-    LAZER = "lazer"
     DEV = "dev"
 
-class OssapiAsync:
+
+class Oauth2SessionOssapi(OAuth2Session):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        headers = {"User-Agent": f"ossapi (v{ossapi.__version__})"}
+        self.headers.update(headers)
+
+
+class Ossapi:
     """
-    Async equivalent of :class:`~ossapi.ossapiv2.Ossapi`. Main (async) entry
-    point into osu! api v2.
+    A wrapper around osu! api v2. The main entry point for ossapi.
 
     Parameters
     ----------
     client_id: int
         The id of the client to authenticate with.
     client_secret: str
         The secret of the client to authenticate with.
@@ -401,43 +425,43 @@
         osu! api. Optional if using :data:`Grant.CLIENT_CREDENTIALS
         <ossapi.ossapiv2.Grant.CLIENT_CREDENTIALS>`.
     domain: Domain or str
         The domain to retrieve information from. This defaults to
         :data:`Domain.OSU <ossapi.ossapiv2.Domain.OSU>`, which corresponds to
         osu.ppy.sh, the main website.
         |br|
-        To retrieve information from lazer.ppy.sh - for instance, the
-        leaderboards on lazer, or a user's best score on lazer - specify
-        :data:`Domain.LAZER <ossapi.ossapiv2.Domain.LAZER>`. To retureve
-        information from dev.ppy.sh, specify
+        To retrieve information from dev.ppy.sh, specify
         :data:`Domain.DEV <ossapi.ossapiv2.Domain.DEV>`.
         |br|
         See :doc:`Domains <domains>` for more about domains.
     """
+
     TOKEN_URL = "https://{domain}.ppy.sh/oauth/token"
     AUTH_CODE_URL = "https://{domain}.ppy.sh/oauth/authorize"
     BASE_URL = "https://{domain}.ppy.sh/api/v2"
 
-    def __init__(self,
+    def __init__(
+        self,
         client_id: int,
         client_secret: str,
         redirect_uri: Optional[str] = None,
         scopes: List[Union[str, Scope]] = [Scope.PUBLIC],
         *,
         grant: Optional[Union[Grant, str]] = None,
         strict: bool = False,
         token_directory: Optional[str] = None,
         token_key: Optional[str] = None,
         access_token: Optional[str] = None,
         refresh_token: Optional[str] = None,
-        domain: Union[str, Domain] = Domain.OSU
+        domain: Union[str, Domain] = Domain.OSU,
     ):
         if not grant:
-            grant = (Grant.AUTHORIZATION_CODE if redirect_uri else
-                Grant.CLIENT_CREDENTIALS)
+            grant = (
+                Grant.AUTHORIZATION_CODE if redirect_uri else Grant.CLIENT_CREDENTIALS
+            )
         grant = Grant(grant)
 
         domain = Domain(domain)
 
         self.token_url = self.TOKEN_URL.format(domain=domain.value)
         self.auth_code_url = self.AUTH_CODE_URL.format(domain=domain.value)
         self.base_url = self.BASE_URL.format(domain=domain.value)
@@ -447,57 +471,64 @@
         self.client_secret = client_secret
         self.redirect_uri = redirect_uri
         self.scopes = [Scope(scope) for scope in scopes]
         self.strict = strict
         self.domain = domain
 
         self.log = logging.getLogger(__name__)
-        self.token_key = token_key or self.gen_token_key(self.grant,
-            self.client_id, self.client_secret, self.scopes, self.domain.value)
+        self.token_key = token_key or self.gen_token_key(
+            self.grant,
+            self.client_id,
+            self.client_secret,
+            self.scopes,
+            self.domain.value,
+        )
         self._type_hints_cache = {}
 
         # support saving tokens when being run from pyinstaller
-        if hasattr(sys, '_MEIPASS') and not token_directory:
-            token_directory = sys._MEIPASS # pylint: disable=no-member
+        if hasattr(sys, "_MEIPASS") and not token_directory:
+            token_directory = sys._MEIPASS  # pylint: disable=no-member
 
         self.token_directory = (
             Path(token_directory) if token_directory else Path(__file__).parent
         )
         self.token_file = self.token_directory / f"{self.token_key}.pickle"
 
         if self.grant is Grant.CLIENT_CREDENTIALS:
             if self.scopes != [Scope.PUBLIC]:
-                raise ValueError(f"`scopes` must be ['public'] if the "
-                    f"client credentials grant is used. Got {self.scopes}")
+                raise ValueError(
+                    f"`scopes` must be ['public'] if the "
+                    f"client credentials grant is used. Got {self.scopes}"
+                )
 
         if self.grant is Grant.AUTHORIZATION_CODE and not self.redirect_uri:
-            raise ValueError("`redirect_uri` must be passed if the "
-                "authorization code grant is used.")
+            raise ValueError(
+                "`redirect_uri` must be passed if the "
+                "authorization code grant is used."
+            )
 
         # whether the consumer passed a token to ossapi to bypass authentication
         self.access_token_passed = False
         token = None
         if access_token is not None:
             # allow refresh_token to be null for the case of client credentials
             # grant from access token, which does not have an associated refresh
             # token.
             params = {
                 "token_type": "Bearer",
                 "access_token": access_token,
-                "refresh_token": refresh_token
+                "refresh_token": refresh_token,
             }
             token = OAuth2Token(params)
             self.access_token_passed = True
 
         self.session = self.authenticate(token=token)
 
     @staticmethod
-    def gen_token_key(grant, client_id, client_secret, scopes,
-        domain=Domain.OSU
-    ):
+    def gen_token_key(grant, client_id, client_secret, scopes, domain=Domain.OSU):
         """
         The unique key / hash for the given set of parameters. This is intended
         to provide a way to allow multiple OssapiV2's to live at the same time,
         by eg saving their tokens to different files based on their key.
 
         This function is also deterministic, to eg allow tokens to be reused if
         OssapiV2 is instantiated twice with the same parameters. This avoids the
@@ -514,16 +545,14 @@
 
         for scope in scopes:
             m.update(scope.value.encode("utf-8"))
 
         # for backwards compatability, only hash the domain when it's
         # non-default. This ensures keys from before and after domains were
         # introduced coincide.
-        # This intentionally treats Domain.OSU and Domain.LAZER as the same key,
-        # as those domains share account and oauth credentials.
         if domain is Domain.DEV:
             m.update(domain.value.encode("utf-8"))
 
         return m.hexdigest()
 
     @staticmethod
     def remove_token(key, token_directory=None):
@@ -551,226 +580,217 @@
         # try saved token file first
         if self.token_file.exists() or token is not None:
             if token is None:
                 with open(self.token_file, "rb") as f:
                     token = pickle.load(f)
 
             if self.grant is Grant.CLIENT_CREDENTIALS:
-                return Oauth2SessionAsync(self.client_id, token=token)
+                return Oauth2SessionOssapi(self.client_id, token=token)
 
             if self.grant is Grant.AUTHORIZATION_CODE:
                 auto_refresh_kwargs = {
                     "client_id": self.client_id,
-                    "client_secret": self.client_secret
+                    "client_secret": self.client_secret,
                 }
-                return Oauth2SessionAsync(self.client_id, token=token,
+                return Oauth2SessionOssapi(
+                    self.client_id,
+                    token=token,
                     redirect_uri=self.redirect_uri,
                     auto_refresh_url=self.token_url,
                     auto_refresh_kwargs=auto_refresh_kwargs,
                     token_updater=self._save_token,
-                    scope=[scope.value for scope in self.scopes])
+                    scope=[scope.value for scope in self.scopes],
+                )
 
         # otherwise, authorize from scratch
         return self._new_grant()
 
     def _new_grant(self):
         if self.grant is Grant.CLIENT_CREDENTIALS:
             return self._new_client_grant(self.client_id, self.client_secret)
 
-        return self._new_authorization_grant(self.client_id, self.client_secret,
-            self.redirect_uri, self.scopes)
+        return self._new_authorization_grant(
+            self.client_id, self.client_secret, self.redirect_uri, self.scopes
+        )
 
     def _new_client_grant(self, client_id, client_secret):
         """
         Authenticates with the api from scratch on the client grant.
         """
         self.log.info("initializing client credentials grant")
         client = BackendApplicationClient(client_id=client_id, scope=["public"])
-        session = Oauth2SessionAsync(client=client)
-        token = session.fetch_token(token_url=self.token_url,
-            client_id=client_id, client_secret=client_secret)
+        session = Oauth2SessionOssapi(client=client)
+        token = session.fetch_token(
+            token_url=self.token_url, client_id=client_id, client_secret=client_secret
+        )
 
         self._save_token(token)
         return session
 
-    def _new_authorization_grant(self, client_id, client_secret, redirect_uri,
-        scopes):
+    def _new_authorization_grant(self, client_id, client_secret, redirect_uri, scopes):
         """
         Authenticates with the api from scratch on the authorization code grant.
         """
         self.log.info("initializing authorization code")
 
-        auto_refresh_kwargs = {
-            "client_id": client_id,
-            "client_secret": client_secret
-        }
-        session = Oauth2SessionAsync(client_id, redirect_uri=redirect_uri,
+        auto_refresh_kwargs = {"client_id": client_id, "client_secret": client_secret}
+        session = OAuth2Session(
+            client_id,
+            redirect_uri=redirect_uri,
             auto_refresh_url=self.token_url,
             auto_refresh_kwargs=auto_refresh_kwargs,
             token_updater=self._save_token,
-            scope=[scope.value for scope in scopes])
-
-        authorization_url, _state = (
-            session.authorization_url(self.auth_code_url)
+            scope=[scope.value for scope in scopes],
         )
+
+        authorization_url, _state = session.authorization_url(self.auth_code_url)
         webbrowser.open(authorization_url)
 
         # open up a temporary socket so we can receive the GET request to the
         # callback url
         port = int(redirect_uri.rsplit(":", 1)[1].split("/")[0])
         serversocket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         serversocket.bind(("localhost", port))
         serversocket.listen(1)
         connection, _ = serversocket.accept()
         # arbitrary "large enough" byte receive size
         data = str(connection.recv(8192))
         connection.send(b"HTTP/1.0 200 OK\n")
         connection.send(b"Content-Type: text/html\n")
         connection.send(b"\n")
-        connection.send(b"""<html><body>
+        connection.send(
+            b"""<html><body>
             <h2>Ossapi has received your authentication.</h2> You
             may now close this tab safely.
             </body></html>
-        """)
+        """
+        )
         connection.close()
         serversocket.close()
 
         code = data.split("code=")[1].split("&state=")[0]
-        token = session.fetch_token(self.token_url, client_id=client_id,
-            client_secret=client_secret, code=code)
+        token = session.fetch_token(
+            self.token_url, client_id=client_id, client_secret=client_secret, code=code
+        )
         self._save_token(token)
 
         return session
 
     def _save_token(self, token):
         """
         Saves the token to this OssapiV2's associated token file.
         """
         self.log.info(f"saving token to {self.token_file}")
         with open(self.token_file, "wb+") as f:
             pickle.dump(token, f)
 
-    async def _request(self, type_, method, url, params={}, data={}):
-        from aiohttp import ClientSession
-
+    def _request(self, type_, method, url, params={}, data={}):
         # I don't *think* type hints should change over the lifetime of a
         # program, but clear them every request out of an abundance of caution.
         # This costs us almost nothing and may avoid bugs when eg a consumer
         # changes type hints of a custom model dynamically at some point.
         # They should certainly not be doing so in the middle of a request,
         # however.
         self._clear_type_hints_cache()
-
         params = self._format_params(params)
         # also format data for post requests
         data = self._format_params(data)
 
-        # No, we should not be using a session for every request. Yes, we are
-        # not achieving 100% performance by doing this. The benefit is that we
-        # don't require `async with OssapiAsync(...) as api:` syntax in order to
-        # use ossapi.
-        aiohttp_session = ClientSession()
-
-        async def make_request():
-            return await self.session.request_async(method,
-                f"{self.base_url}{url}", session=aiohttp_session,
-                params=params, data=data)
+        def make_request():
+            return self.session.request(
+                method, f"{self.base_url}{url}", params=params, data=data
+            )
 
-        async def reauthenticate_and_retry():
+        def reauthenticate_and_retry():
             # don't automatically re-authenticate if the user passed an access
             # token. They should handle re-authentication with the user
             # manually (since they may have a bespoke system, like a website).
             if self.access_token_passed:
-                self.log.info("refresh token is invalid. raising for consumer "
-                    "to handle since access token was passed originally.")
+                self.log.info(
+                    "refresh token is invalid. raising for consumer "
+                    "to handle since access token was passed originally."
+                )
                 raise ReauthenticationRequired()
 
-            self.log.info("refresh token invalid, re-authenticating (grant: "
-                f"{self.grant})")
+            self.log.info(
+                "refresh token invalid, re-authenticating (grant: " f"{self.grant})"
+            )
             # don't use .authenticate, that falls back to cached tokens. go
             # straight to authenticating from scratch.
             self.session = self._new_grant()
             # redo the request now that we have a valid session
-            return await make_request()
+            return make_request()
 
         try:
-            r = await make_request()
+            r = make_request()
         except TokenExpiredError:
             # provide "auto refreshing" for client credentials grant. The client
             # grant doesn't actually provide a refresh token, so we can't hook
             # onto OAuth2Session's auto_refresh functionality like we do for the
             # authorization code grant. But we can do something effectively
             # equivalent: whenever we make a request with an expired client
             # grant token, just request a new one.
             if self.grant is not Grant.CLIENT_CREDENTIALS:
                 raise
-            self.session = self._new_client_grant(self.client_id,
-                self.client_secret)
+            self.session = self._new_client_grant(self.client_id, self.client_secret)
             # redo the request now that we have a valid token
-            r = await make_request()
+            r = make_request()
         except OAuth2Error as e:
             if e.description != "The refresh token is invalid.":
                 raise
 
-            r = await reauthenticate_and_retry()
+            r = reauthenticate_and_retry()
+
+        self.log.info(f"made {method} request to {r.request.url}, data {data}")
+        json_ = r.json()
 
-        # aiohttp annoyingly differentiates between url (no url fragments, for
-        # some reason) and real_url (actual url). They also use a URL object
-        # here instead of a string.
-        # XXX don't overwrite url passed in function, used in
-        # authenticate_and_retry
-        url_ = str(r.real_url)
-        self.log.info(f"made {method} request to {url_}, data {data}")
-
-        # aiohttp throws on unexpected encoding (non-json mimetype). Match
-        # requests behavior by automatically detecting encoding.
-        # See https://github.com/tybug/ossapi/issues/60.
-        json_ = await r.json(encoding=None)
         # occurs if a client gets revoked and the token hasn't officially
         # expired yet (so it doesn't error earlier up in the chain with
         # Oauth2Error).
         if json_ == {"authentication": "basic"}:
-            r = await reauthenticate_and_retry()
-            json_ = await r.json(encoding=None)
-
-        # aiohttp sessions have to live as long as any responses returned via
-        # the session. Wait to close it until we're done with the response `r`.
-        # Make sure we close this before we call _check_response, or any errors
-        # there will result in the session not being closed. We should probably
-        # move this to a try/finally block at some point for safety.
-        await aiohttp_session.close()
+            r = reauthenticate_and_retry()
+            json_ = r.json()
 
         self.log.debug(f"received json: \n{json.dumps(json_, indent=4)}")
-        self._check_response(json_, url_)
+        self._check_response(json_, r.url)
 
         return self._instantiate_type(type_, json_)
 
     def _check_response(self, json_, url):
         # TODO this should just be `if "error" in json`, but for some reason
         # `self.search_beatmaps` always returns an error in the response...
         # open an issue on osu-web?
         if len(json_) == 1 and "error" in json_:
-            raise ValueError(f"api returned an error of `{json_['error']}` for "
-                f"a request to {unquote(url)}")
+            raise ValueError(
+                f"api returned an error of `{json_['error']}` for "
+                f"a request to {unquote(url)}"
+            )
+
+        # some endpoints only require authorization grant for some endpoints.
+        # e.g. normally api.match only requires client credentials grant, but for
+        # private matches like api.match(111632899), it will return this error.
+        if json_ == {"authentication": "basic"}:
+            raise ValueError(
+                "Permission denied for a request to "
+                f"{unquote(url)}. This request may require "
+                "Grant.AUTHORIZATION_CODE."
+            )
 
-    async def _get(self, type_, url, params={}):
-        return await self._request(type_, "GET", url, params=params)
+    def _get(self, type_, url, params={}):
+        return self._request(type_, "GET", url, params=params)
 
-    async def _post(self, type_, url, data={}):
-        return await self._request(type_, "POST", url, data=data)
+    def _post(self, type_, url, data={}):
+        return self._request(type_, "POST", url, data=data)
 
-    async def _put(self, type_, url, data={}):
-        return await self._request(type_, "PUT", url, data=data)
+    def _put(self, type_, url, data={}):
+        return self._request(type_, "PUT", url, data=data)
 
     def _format_params(self, params):
         for key, value in params.copy().items():
-            # requests ignores None values, but aiohttp doesn't. Make compliant.
-            if value is None:
-                del params[key]
-            elif isinstance(value, list):
+            if isinstance(value, list):
                 # we need to pass multiple values for this key, so make its
                 # value a list https://stackoverflow.com/a/62042144
                 params[f"{key}[]"] = []
                 for v in value:
                     params[f"{key}[]"].append(self._format_value(v))
                 del params[key]
             elif isinstance(value, Cursor):
@@ -853,15 +873,15 @@
             # skipping fields that are null which aren't supposed to be, and
             # prevent that error from being caught.
             if value is None and is_optional(type_):
                 continue
             self.log.debug(f"resolving attribute {attr}")
 
             value = self._instantiate_type(type_, value, obj, attr_name=attr)
-            if not value:
+            if value is None:
                 continue
             setattr(obj, attr, value)
         self.log.debug(f"resolved annotations for type {type(obj)}")
         return obj
 
     def _instantiate_type(self, type_, value, obj=None, attr_name=None):
         # `attr_name` is purely for debugging, it's the name of the attribute
@@ -886,29 +906,32 @@
         def _check_primitive_type():
             # The osu api occasionally makes attributes optional, so allow null
             # values even for non-optional fields if we're not in
             # strict mode.
             if not self.strict and value is None:
                 return
             if not isinstance(value, type_):
-                raise TypeError(f"expected type {type_} for value {value}, got "
+                raise TypeError(
+                    f"expected type {type_} for value {value}, got "
                     f"type {type(value)}"
-                    f" (for attribute: {attr_name})" if attr_name else "")
+                    f" (for attribute: {attr_name})"
+                    if attr_name
+                    else ""
+                )
 
         if is_primitive_type(type_):
             value = convert_primitive_type(value, type_)
             _check_primitive_type()
             return value
 
         if is_base_model_type(type_):
             self.log.debug(f"instantiating base type {type_}")
             return type_(value)
 
-        if origin is list and (is_model_type(args[0]) or
-            isinstance(args[0], TypeVar)):
+        if origin is list and (is_model_type(args[0]) or isinstance(args[0], TypeVar)):
             assert len(args) == 1
             # check if the list has been instantiated generically; if so,
             # use the concrete type backing the generic type.
             if isinstance(args[0], TypeVar):
                 # `__orig_class__` is how we can get the concrete type of
                 # a generic. See https://stackoverflow.com/a/60984681 and
                 # https://www.python.org/dev/peps/pep-0560/#mro-entries.
@@ -940,27 +963,29 @@
             new_value = None
             # purely for debugging. errors for each arg are shown when we can't
             # deserialize any of them.
             fail_reasons = []
             for arg in args:
                 try:
                     import copy
+
                     v = copy.deepcopy(value)
                     # _instantiate_type implicitly mutates the passed value.
                     # this is probably something we should change - but for now,
                     # fix it here, as we may reuse `value`.
-                    new_value = self._instantiate_type(arg, v, obj,
-                        attr_name)
+                    new_value = self._instantiate_type(arg, v, obj, attr_name)
                 except Exception as e:
                     fail_reasons.append(str(e))
                     continue
 
             if new_value is None:
-                raise ValueError(f"Failed to satisfy union: no type in {args} "
-                    f"satisfied {attr_name} (fail reasons: {fail_reasons})")
+                raise ValueError(
+                    f"Failed to satisfy union: no type in {args} "
+                    f"satisfied {attr_name} (fail reasons: {fail_reasons})"
+                )
             return new_value
 
         # either we ourself are a model type (eg `Search`), or we are
         # a special indexed type (eg `type_ == SearchResult[UserCompact]`,
         # `origin == UserCompact`). In either case we want to instantiate
         # `type_`.
         if not is_model_type(type_) and not is_model_type(origin):
@@ -992,30 +1017,37 @@
             type_hints = self._get_type_hints(type_)
         except TypeError:
             assert type(type_) is _GenericAlias
 
             signature_type = get_origin(type_)
             type_hints = self._get_type_hints(signature_type)
 
+        # field override name to existing attribute name
         field_names = {}
+        # existing attribute name to field deserialize type
+        field_deserialize_types = {}
+        # process Field attributes.
         for name in type_hints:
             # any inherited attributes will be present in the annotations
             # (type_hints) but not actually an attribute of the type. Just skip
             # them for now. TODO I'm pretty sure this is going to cause issues
             # if we ever have a field on a model and then another model
             # inheriting from it; the inheriting model won't have the field
             # picked up here and the override name won't come into play.
             # probably just traverse the mro?
             if not hasattr(type_, name):
                 continue
             value = getattr(type_, name)
             if not isinstance(value, Field):
                 continue
-            if value.name:
+
+            if value.name is not None:
                 field_names[value.name] = name
+            if value.deserialize_type is not None:
+                field_deserialize_types[name] = value.deserialize_type
 
         # make a copy so we can modify while iterating
         for key in list(kwargs):
             value = kwargs.pop(key)
             if key in field_names:
                 key = field_names[key]
             kwargs[key] = value
@@ -1047,33 +1079,44 @@
         kwargs_ = {}
 
         for k, v in kwargs.items():
             if k in parameters:
                 kwargs_[k] = v
             else:
                 if self.strict:
-                    raise TypeError(f"unexpected parameter `{k}` for type "
-                        f"{type_}")
+                    raise TypeError(f"unexpected parameter `{k}` for type " f"{type_}")
                 # this is an INFO log in spirit, but can be spammy with Union
                 # type resolution where the first union case hits nonfatal
                 # errors like this before a fatal error causes it to backtrack.
                 # In practice, it makes no difference for developing ossapi,
                 # as tests and local development are all done in strict mode.
-                self.log.debug(f"ignoring unexpected parameter `{k}` from "
-                    f"api response for type {type_}")
+                self.log.debug(
+                    f"ignoring unexpected parameter `{k}` from "
+                    f"api response for type {type_}"
+                )
 
         # every model gets a special `_api` parameter, which is the
         # `OssapiV2` instance which loaded it (aka us).
         kwargs_["_api"] = self
 
         try:
             val = type_(**kwargs_)
         except TypeError as e:
-            raise TypeError(f"type error while instantiating class {type_}: "
-                f"{e}") from e
+            raise TypeError(
+                f"type error while instantiating class {type_}: " f"{e}"
+            ) from e
+
+        for name, deserialize_type in field_deserialize_types.items():
+            val.__annotations__[name] = deserialize_type
+
+        # modifying the type hints of an object dynamically invalidates its
+        # cache. Avoid looking up stale type hints if we had looked up its
+        # previous value before modifying it here.
+        if field_deserialize_types:
+            del self._type_hints_cache[type(val)]
 
         return val
 
     def _get_type_hints(self, obj):
         # type hints are expensive to compute. Our models should never change
         # their type hints, so cache them.
         if obj in self._type_hints_cache:
@@ -1082,27 +1125,26 @@
         type_hints = get_type_hints(obj)
         self._type_hints_cache[obj] = type_hints
         return type_hints
 
     def _clear_type_hints_cache(self):
         self._type_hints_cache = {}
 
-
     # =========
     # Endpoints
     # =========
 
-
     # /beatmaps/packs
     # ---------------
 
     @request(Scope.PUBLIC, category="beatmap packs")
-    async def beatmap_packs(self,
+    def beatmap_packs(
+        self,
         type: Optional[BeatmapPackTypeT] = None,
-        cursor_string: Optional[str] = None
+        cursor_string: Optional[str] = None,
     ) -> BeatmapPacks:
         """
         Get a list of beatmap packs. If you want to retrieve a specific pack,
         see :meth:`beatmap_pack`.
 
         Parameters
         ----------
@@ -1112,43 +1154,41 @@
         Notes
         -----
         Implements the `Beatmap Packs
         <https://osu.ppy.sh/docs/index.html#get-beatmap-packs>`__
         endpoint.
         """
         params = {"type": type, "cursor_string": cursor_string}
-        return await self._get(BeatmapPacks, "/beatmaps/packs", params)
+        return self._get(BeatmapPacks, "/beatmaps/packs", params)
 
     @request(Scope.PUBLIC, category="beatmap packs")
-    async def beatmap_pack(self,
-        pack: str
-    ) -> BeatmapPack:
+    def beatmap_pack(self, pack: str) -> BeatmapPack:
         """
         Get a beatmap pack. If you want to retrieve a list of beatmap packs, see
         see :meth:`beatmap_packs`.
 
         Notes
         -----
         Implements the `Beatmap Pack
         <https://osu.ppy.sh/docs/index.html#get-beatmap-pack>`__
         endpoint.
         """
-        return await self._get(BeatmapPack, f"/beatmaps/packs/{pack}")
-
+        return self._get(BeatmapPack, f"/beatmaps/packs/{pack}")
 
     # /beatmaps
     # ---------
 
     @request(Scope.PUBLIC, category="beatmaps")
-    async def beatmap_user_score(self,
+    def beatmap_user_score(
+        self,
         beatmap_id: BeatmapIdT,
         user_id: UserIdT,
         *,
         mode: Optional[GameModeT] = None,
-        mods: Optional[ModT] = None
+        mods: Optional[ModT] = None,
     ) -> BeatmapUserScore:
         """
         Get a user's best score on a beatmap. If you want to retrieve all
         scores, see :meth:`beatmap_user_scores`.
 
         Parameters
         ----------
@@ -1164,23 +1204,25 @@
         Notes
         -----
         Implements the `User Beatmap Score
         <https://osu.ppy.sh/docs/index.html#get-a-user-beatmap-score>`__
         endpoint.
         """
         params = {"mode": mode, "mods": mods}
-        return await self._get(BeatmapUserScore,
-            f"/beatmaps/{beatmap_id}/scores/users/{user_id}", params)
+        return self._get(
+            BeatmapUserScore, f"/beatmaps/{beatmap_id}/scores/users/{user_id}", params
+        )
 
     @request(Scope.PUBLIC, category="beatmaps")
-    async def beatmap_user_scores(self,
+    def beatmap_user_scores(
+        self,
         beatmap_id: BeatmapIdT,
         user_id: UserIdT,
         *,
-        mode: Optional[GameModeT] = None
+        mode: Optional[GameModeT] = None,
     ) -> List[Score]:
         """
         Get all of a user's scores on a beatmap. If you only want the top user
         score, see :meth:`beatmap_user_score`.
 
         Parameters
         ----------
@@ -1194,26 +1236,30 @@
         Notes
         -----
         Implements to `User Beatmap Scores
         <https://osu.ppy.sh/docs/index.html#get-a-user-beatmap-scores>`__
         endpoint.
         """
         params = {"mode": mode}
-        scores = await self._get(BeatmapUserScores,
-            f"/beatmaps/{beatmap_id}/scores/users/{user_id}/all", params)
+        scores = self._get(
+            BeatmapUserScores,
+            f"/beatmaps/{beatmap_id}/scores/users/{user_id}/all",
+            params,
+        )
         return scores.scores
 
     @request(Scope.PUBLIC, category="beatmaps")
-    async def beatmap_scores(self,
+    def beatmap_scores(
+        self,
         beatmap_id: BeatmapIdT,
         *,
         mode: Optional[GameModeT] = None,
         mods: Optional[ModT] = None,
         type: Optional[RankingTypeT] = None,
-        limit: Optional[int] = None
+        limit: Optional[int] = None,
     ) -> BeatmapScores:
         """
         Get the top scores of a beatmap.
 
         Parameters
         ----------
         beatmap_id
@@ -1230,19 +1276,48 @@
 
         Notes
         -----
         Implements the `Get Beatmap Scores
         <https://osu.ppy.sh/docs/index.html#get-beatmap-scores>`__ endpoint.
         """
         params = {"mode": mode, "mods": mods, "type": type, "limit": limit}
-        return await self._get(BeatmapScores, f"/beatmaps/{beatmap_id}/scores",
-            params)
+        return self._get(BeatmapScores, f"/beatmaps/{beatmap_id}/scores", params)
+
+    def _beatmap_scores_non_legacy(
+        self,
+        beatmap_id: BeatmapIdT,
+        *,
+        mode: Optional[GameModeT] = None,
+        mods: Optional[ModT] = None,
+        type: Optional[RankingTypeT] = None,
+        limit: Optional[int] = None,
+        legacy_only: Optional[bool] = None,
+    ) -> _NonLegacyBeatmapScores:
+        """
+        This is a provisional method. It may change or disappear in the future.
+        Feel free to use it, but don't expect ossapi to maintain backwards
+        compatability here.
+
+        I'll decide what to do about these provisional methods once the lazer
+        migration settles down.
+        """
+        params = {
+            "mode": mode,
+            "mods": mods,
+            "type": type,
+            "limit": limit,
+            "legacy_only": legacy_only,
+        }
+        return self._get(
+            _NonLegacyBeatmapScores, f"/beatmaps/{beatmap_id}/solo-scores", params
+        )
 
     @request(Scope.PUBLIC, category="beatmaps")
-    async def beatmap(self,
+    def beatmap(
+        self,
         beatmap_id: Optional[BeatmapIdT] = None,
         *,
         checksum: Optional[str] = None,
         filename: Optional[str] = None,
     ) -> Beatmap:
         """
         Get a beatmap from an id, checksum, or filename.
@@ -1260,23 +1335,22 @@
         -----
         Combines the
         `Get Beatmap <https://osu.ppy.sh/docs/index.html#get-beatmap>`_ and
         `Lookup Beatmap <https://osu.ppy.sh/docs/index.html#lookup-beatmap>`_
         endpoints.
         """
         if not (beatmap_id or checksum or filename):
-            raise ValueError("at least one of beatmap_id, checksum, or "
-                "filename must be passed")
+            raise ValueError(
+                "at least one of beatmap_id, checksum, or " "filename must be passed"
+            )
         params = {"checksum": checksum, "filename": filename, "id": beatmap_id}
-        return await self._get(Beatmap, "/beatmaps/lookup", params)
+        return self._get(Beatmap, "/beatmaps/lookup", params)
 
     @request(Scope.PUBLIC, category="beatmaps")
-    async def beatmaps(self,
-        beatmap_ids: List[BeatmapIdT]
-    ) -> List[Beatmap]:
+    def beatmaps(self, beatmap_ids: List[BeatmapIdT]) -> List[Beatmap]:
         """
         Batch get beatmaps by id. If you only want to retrieve a single beatmap,
         or want to retrieve beatmaps by something other than id (eg checksum),
         see :meth:`beatmap`.
 
         Parameters
         ----------
@@ -1285,24 +1359,24 @@
 
         Notes
         -----
         Implements the `Get Beatmaps
         <https://osu.ppy.sh/docs/index.html#get-beatmaps>`__ endpoint.
         """
         params = {"ids": beatmap_ids}
-        beatmaps = await self._get(Beatmaps, "/beatmaps", params)
-        return beatmaps.beatmaps
+        return self._get(Beatmaps, "/beatmaps", params).beatmaps
 
     @request(Scope.PUBLIC, category="beatmaps")
-    async def beatmap_attributes(self,
+    def beatmap_attributes(
+        self,
         beatmap_id: int,
         *,
         mods: Optional[ModT] = None,
         ruleset: Optional[GameModeT] = None,
-        ruleset_id: Optional[int] = None
+        ruleset_id: Optional[int] = None,
     ) -> DifficultyAttributes:
         """
         Get the difficult attributes of a beatmap. Used for pp calculation.
 
         Parameters
         ----------
         beatmap_id
@@ -1317,30 +1391,31 @@
 
         Notes
         -----
         Implements the `Get Beatmap Attributes
         <https://osu.ppy.sh/docs/index.html#get-beatmap-attributes>`__ endpoint.
         """
         data = {"mods": mods, "ruleset": ruleset, "ruleset_id": ruleset_id}
-        return await self._post(DifficultyAttributes,
-            f"/beatmaps/{beatmap_id}/attributes", data=data)
-
+        return self._post(
+            DifficultyAttributes, f"/beatmaps/{beatmap_id}/attributes", data=data
+        )
 
     # /beatmapsets
     # ------------
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    async def beatmapset_discussion_posts(self,
+    def beatmapset_discussion_posts(
+        self,
         beatmapset_discussion_id: Optional[int] = None,
         *,
         limit: Optional[int] = None,
         page: Optional[int] = None,
         sort: Optional[BeatmapDiscussionPostSortT] = None,
         user_id: Optional[UserIdT] = None,
-        with_deleted: Optional[bool] = None
+        with_deleted: Optional[bool] = None,
     ) -> BeatmapsetDiscussionPosts:
         """
         Get the posts of a beatmapset discussion.
 
         Parameters
         ----------
         beatmapset_discussion_id
@@ -1359,31 +1434,38 @@
 
         Notes
         -----
         Implements the `Get Beatmapset Discussion Posts
         <https://osu.ppy.sh/docs/index.html#get-beatmapset-discussion-posts>`__
         endpoint.
         """
-        params = {"beatmapset_discussion_id": beatmapset_discussion_id,
-            "limit": limit, "page": page, "sort": sort, "user": user_id,
-            "with_deleted": with_deleted}
-        return await self._get(BeatmapsetDiscussionPosts,
-            "/beatmapsets/discussions/posts", params)
+        params = {
+            "beatmapset_discussion_id": beatmapset_discussion_id,
+            "limit": limit,
+            "page": page,
+            "sort": sort,
+            "user": user_id,
+            "with_deleted": with_deleted,
+        }
+        return self._get(
+            BeatmapsetDiscussionPosts, "/beatmapsets/discussions/posts", params
+        )
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    async def beatmapset_discussion_votes(self,
+    def beatmapset_discussion_votes(
+        self,
         *,
         beatmapset_discussion_id: Optional[int] = None,
         limit: Optional[int] = None,
         page: Optional[int] = None,
         receiver_id: Optional[int] = None,
         vote: Optional[BeatmapsetDiscussionVoteT] = None,
         sort: Optional[BeatmapsetDiscussionVoteSortT] = None,
         user_id: Optional[UserIdT] = None,
-        with_deleted: Optional[bool] = None
+        with_deleted: Optional[bool] = None,
     ) -> BeatmapsetDiscussionVotes:
         """
         Get beatmapset discussion votes.
 
         Parameters
         ----------
         beatmapset_discussion_id
@@ -1406,23 +1488,31 @@
 
         Notes
         -----
         Implements the `Get Beatmapset Discussion Posts
         <https://osu.ppy.sh/docs/index.html#get-beatmapset-discussion-posts>`__
         endpoint.
         """
-        params = {"beatmapset_discussion_id": beatmapset_discussion_id,
-            "limit": limit, "page": page, "receiver": receiver_id,
-            "score": vote, "sort": sort, "user": user_id,
-            "with_deleted": with_deleted}
-        return await self._get(BeatmapsetDiscussionVotes,
-            "/beatmapsets/discussions/votes", params)
+        params = {
+            "beatmapset_discussion_id": beatmapset_discussion_id,
+            "limit": limit,
+            "page": page,
+            "receiver": receiver_id,
+            "score": vote,
+            "sort": sort,
+            "user": user_id,
+            "with_deleted": with_deleted,
+        }
+        return self._get(
+            BeatmapsetDiscussionVotes, "/beatmapsets/discussions/votes", params
+        )
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    async def beatmapset_discussions(self,
+    def beatmapset_discussions(
+        self,
         *,
         beatmapset_id: Optional[BeatmapsetIdT] = None,
         beatmap_id: Optional[BeatmapIdT] = None,
         beatmapset_status: Optional[BeatmapsetStatusT] = None,
         limit: Optional[int] = None,
         message_types: Optional[List[MessageTypeT]] = None,
         only_unresolved: Optional[bool] = None,
@@ -1460,44 +1550,49 @@
 
         Notes
         -----
         Implements the `Get Beatmapset Discussion Posts
         <https://osu.ppy.sh/docs/index.html#get-beatmapset-discussion-posts>`__
         endpoint.
         """
-        params = {"beatmapset_id": beatmapset_id, "beatmap_id": beatmap_id,
-            "beatmapset_status": beatmapset_status, "limit": limit,
-            "message_types": message_types, "only_unresolved": only_unresolved,
-            "page": page, "sort": sort, "user": user_id,
-            "with_deleted": with_deleted}
-        return await self._get(BeatmapsetDiscussions,
-            "/beatmapsets/discussions", params)
+        params = {
+            "beatmapset_id": beatmapset_id,
+            "beatmap_id": beatmap_id,
+            "beatmapset_status": beatmapset_status,
+            "limit": limit,
+            "message_types": message_types,
+            "only_unresolved": only_unresolved,
+            "page": page,
+            "sort": sort,
+            "user": user_id,
+            "with_deleted": with_deleted,
+        }
+        return self._get(BeatmapsetDiscussions, "/beatmapsets/discussions", params)
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    async def search_beatmapsets(self,
+    def search_beatmapsets(
+        self,
         query: Optional[str] = None,
         *,
         mode: BeatmapsetSearchModeT = BeatmapsetSearchMode.ANY,
-        category: BeatmapsetSearchCategoryT =
-            BeatmapsetSearchCategory.HAS_LEADERBOARD,
-        explicit_content: BeatmapsetSearchExplicitContentT =
-            BeatmapsetSearchExplicitContent.HIDE,
+        category: BeatmapsetSearchCategoryT = BeatmapsetSearchCategory.HAS_LEADERBOARD,
+        explicit_content: BeatmapsetSearchExplicitContentT = BeatmapsetSearchExplicitContent.HIDE,
         genre: BeatmapsetSearchGenreT = BeatmapsetSearchGenre.ANY,
         language: BeatmapsetSearchLanguageT = BeatmapsetSearchLanguage.ANY,
         # "Extra"
         force_video: bool = False,
         force_storyboard: bool = False,
         # "General"
         force_recommended_difficulty: bool = False,
         include_converts: bool = False,
         force_followed_mappers: bool = False,
         force_spotlights: bool = False,
         force_featured_artists: bool = False,
         cursor: Optional[Cursor] = None,
-        sort: Optional[BeatmapsetSearchSortT] = None
+        sort: Optional[BeatmapsetSearchSortT] = None,
     ) -> BeatmapsetSearchResult:
         """
         Search beatmapsets. Equivalent to the beatmapset search page on the
         website (https://osu.ppy.sh/beatmapsets).
 
         Parameters
         ----------
@@ -1563,34 +1658,44 @@
             generals.append("follows")
         if force_spotlights:
             generals.append("spotlights")
         if force_featured_artists:
             generals.append("featured_artists")
         general = ".".join(generals)
 
-        params = {"cursor": cursor, "q": query, "s": category, "m": mode,
-            "g": genre, "l": language, "nsfw": explicit_content, "e": extra,
-            "c": general, "sort": sort}
+        params = {
+            "cursor": cursor,
+            "q": query,
+            "s": category,
+            "m": mode,
+            "g": genre,
+            "l": language,
+            "nsfw": explicit_content,
+            "e": extra,
+            "c": general,
+            "sort": sort,
+        }
 
         # BeatmapsetSearchGenre.ANY is the default and doesn't have a correct
         # corresponding value
         if genre is BeatmapsetSearchGenre.ANY:
             del params["g"]
 
         # same for BeatmapsetSearchLanguage.ANY
         if language is BeatmapsetSearchLanguage.ANY:
             del params["l"]
 
-        return await self._get(BeatmapsetSearchResult, "/beatmapsets/search/", params)
+        return self._get(BeatmapsetSearchResult, "/beatmapsets/search/", params)
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    async def beatmapset(self,
+    def beatmapset(
+        self,
         beatmapset_id: Optional[BeatmapsetIdT] = None,
         *,
-        beatmap_id: Optional[BeatmapIdT] = None
+        beatmap_id: Optional[BeatmapIdT] = None,
     ) -> Beatmapset:
         """
         Get a beatmapset from a beatmapset id or a beatmap id.
 
         Parameters
         ----------
         beatmapset_id
@@ -1602,30 +1707,32 @@
         -----
         Combines the `Get Beatmapset
         <https://osu.ppy.sh/docs/index.html#beatmapsetsbeatmapset>`__ and
         `Beatmapset Lookup
         <https://osu.ppy.sh/docs/index.html#beatmapsetslookup>`__ endpoints.
         """
         if not bool(beatmap_id) ^ bool(beatmapset_id):
-            raise ValueError("exactly one of beatmap_id and beatmapset_id must "
-                "be passed.")
+            raise ValueError(
+                "exactly one of beatmap_id and beatmapset_id must " "be passed."
+            )
         if beatmap_id:
             params = {"beatmap_id": beatmap_id}
-            return await self._get(Beatmapset, "/beatmapsets/lookup", params)
-        return await self._get(Beatmapset, f"/beatmapsets/{beatmapset_id}")
+            return self._get(Beatmapset, "/beatmapsets/lookup", params)
+        return self._get(Beatmapset, f"/beatmapsets/{beatmapset_id}")
 
     @request(Scope.PUBLIC, category="beatmapsets")
-    async def beatmapset_events(self,
+    def beatmapset_events(
+        self,
         *,
         limit: Optional[int] = None,
         page: Optional[int] = None,
         user_id: Optional[UserIdT] = None,
         types: Optional[List[BeatmapsetEventTypeT]] = None,
         min_date: Optional[datetime] = None,
-        max_date: Optional[datetime] = None
+        max_date: Optional[datetime] = None,
     ) -> ModdingHistoryEventsBundle:
         """
         Get beatmapset events. Equivalent to the events search page on the
         website (https://osu.ppy.sh/beatmapsets/events).
 
         Parameters
         ----------
@@ -1644,28 +1751,29 @@
 
         Notes
         -----
         Implements the `Beatmapset Events
         <https://osu.ppy.sh/docs/index.html#beatmapsetsevents>`__ endpoint.
         """
         # limit is 5-50
-        params = {"limit": limit, "page": page, "user": user_id,
-            "min_date": min_date, "max_date": max_date, "types": types}
-        return await self._get(ModdingHistoryEventsBundle, "/beatmapsets/events",
-            params)
-
+        params = {
+            "limit": limit,
+            "page": page,
+            "user": user_id,
+            "min_date": min_date,
+            "max_date": max_date,
+            "types": types,
+        }
+        return self._get(ModdingHistoryEventsBundle, "/beatmapsets/events", params)
 
     # /changelog
     # ----------
 
     @request(scope=None, category="changelog")
-    async def changelog_build(self,
-        stream: str,
-        build: str
-    ) -> Build:
+    def changelog_build(self, stream: str, build: str) -> Build:
         """
         Get changelog build details.
 
         Parameters
         ----------
         stream
             The changelog stream name (eg ``stable40``).
@@ -1673,25 +1781,28 @@
             The changelog build name (eg ``20230121.1``)
 
         Notes
         -----
         Implements the `Get Changelog Build
         <https://osu.ppy.sh/docs/index.html#get-changelog-build>`__ endpoint.
         """
-        return await self._get(Build, f"/changelog/{stream}/{build}")
+        return self._get(Build, f"/changelog/{stream}/{build}")
 
     @request(scope=None, category="changelog")
-    async def changelog_listing(self,
+    def changelog_listing(
+        self,
         *,
         from_: Optional[str] = None,
         to: Optional[str] = None,
         max_id: Optional[int] = None,
         stream: Optional[str] = None,
-        message_formats: List[ChangelogMessageFormat] =
-            [ChangelogMessageFormat.HTML, ChangelogMessageFormat.MARKDOWN]
+        message_formats: List[ChangelogMessageFormat] = [
+            ChangelogMessageFormat.HTML,
+            ChangelogMessageFormat.MARKDOWN,
+        ],
     ) -> ChangelogListing:
         """
         Get list of changelogs.
 
         Parameters
         ----------
         from_
@@ -1706,27 +1817,35 @@
             Format to return text of changelog entries in.
 
         Notes
         -----
         Implements the `Get Changelog Listing
         <https://osu.ppy.sh/docs/index.html#get-changelog-listing>`__ endpoint.
         """
-        params = {"from": from_, "to": to, "max_id": max_id, "stream": stream,
-            "message_formats": message_formats}
-        return await self._get(ChangelogListing, "/changelog", params)
+        params = {
+            "from": from_,
+            "to": to,
+            "max_id": max_id,
+            "stream": stream,
+            "message_formats": message_formats,
+        }
+        return self._get(ChangelogListing, "/changelog", params)
 
     # TODO can almost certainly be combined with changelog_build endpoint, in
     # line with other get/lookup endpoint combinations (beatmap, beatmapset)
     @request(scope=None, category="changelog")
-    async def changelog_build_lookup(self,
+    def changelog_build_lookup(
+        self,
         changelog: str,
         *,
         key: Optional[str] = None,
-        message_formats: List[ChangelogMessageFormat] =
-            [ChangelogMessageFormat.HTML, ChangelogMessageFormat.MARKDOWN]
+        message_formats: List[ChangelogMessageFormat] = [
+            ChangelogMessageFormat.HTML,
+            ChangelogMessageFormat.MARKDOWN,
+        ],
     ) -> Build:
         """
         Look up a changelog build by version, update stream name, or id.
 
         Parameters
         ----------
         changelog
@@ -1740,26 +1859,22 @@
         Notes
         -----
         Implements the `Lookup Changelog Build
         <https://osu.ppy.sh/docs/index.html#lookup-changelog-build>`__ endpoint.
 
         """
         params = {"key": key, "message_formats": message_formats}
-        return await self._get(Build, f"/changelog/{changelog}", params)
-
+        return self._get(Build, f"/changelog/{changelog}", params)
 
     # /chat
     # -----
 
     @request(Scope.CHAT_WRITE, category="chat")
-    async def send_pm(self,
-        user_id: UserIdT,
-        message: str,
-        *,
-        is_action: Optional[bool] = False
+    def send_pm(
+        self, user_id: UserIdT, message: str, *, is_action: Optional[bool] = False
     ) -> CreatePMResponse:
         """
         Send a pm to a user.
 
         Parameters
         ----------
         user_id
@@ -1769,22 +1884,22 @@
         is_action
 
         Notes
         -----
         Implements the `Create New PM
         <https://osu.ppy.sh/docs/index.html#create-new-pm>`__ endpoint.
         """
-        data = {"target_id": user_id, "message": message,
-            "is_action": is_action}
-        return await self._post(CreatePMResponse, "/chat/new", data=data)
+        data = {"target_id": user_id, "message": message, "is_action": is_action}
+        return self._post(CreatePMResponse, "/chat/new", data=data)
 
     # this method requires a user in the announce group, so I've never tested
     # it.
     @request(Scope.CHAT_WRITE_MANAGE, category="chat")
-    async def send_announcement(self,
+    def send_announcement(
+        self,
         channel_name: str,
         channel_description: str,
         message: str,
         # TODO need to add support to automatic conversion for lists of id types
         # instead of just bare types (: UserIdT)
         target_ids: List[UserIdT],
     ) -> ChatChannel:
@@ -1818,34 +1933,34 @@
         dm me on discord (tybug#8490)!
         """
         data = {
             "channel.name": channel_name,
             "channel.description": channel_description,
             "message": message,
             "target_ids": target_ids,
-            "type": "ANNOUNCE"
+            "type": "ANNOUNCE",
         }
-        return await self._post(ChatChannel, "/chat/channels", data=data)
-
+        return self._post(ChatChannel, "/chat/channels", data=data)
 
     # /comments
     # ---------
 
     @request(Scope.PUBLIC, category="comments")
-    async def comments(self,
+    def comments(
+        self,
         *,
         commentable_type: Optional[CommentableTypeT] = None,
         commentable_id: Optional[int] = None,
         cursor: Optional[Cursor] = None,
         parent_id: Optional[int] = None,
-        sort: Optional[CommentSortT] = None
+        sort: Optional[CommentSortT] = None,
     ) -> CommentBundle:
         """
-        Get comments and their replies (up to 2 levels deep). If you only want
-        to retrieve a single comment, see :meth:`comment`.
+        Get recent comments and their replies (up to 2 levels deep). If you only
+        want to retrieve a single comment, see :meth:`comment`.
 
         Parameters
         ----------
         commentable_type
             The type of resource to get comments for.
         commentable_id
             The id of the resource to get comments for.
@@ -1858,47 +1973,46 @@
             the user-specified default when authenticated.
 
         Notes
         -----
         Implements the `Get Comments
         <https://osu.ppy.sh/docs/index.html#get-comments>`__ endpoint.
         """
-        params = {"commentable_type": commentable_type,
-            "commentable_id": commentable_id, "cursor": cursor,
-            "parent_id": parent_id, "sort": sort}
-        return await self._get(CommentBundle, "/comments", params)
+        params = {
+            "commentable_type": commentable_type,
+            "commentable_id": commentable_id,
+            "cursor": cursor,
+            "parent_id": parent_id,
+            "sort": sort,
+        }
+        return self._get(CommentBundle, "/comments", params)
 
     @request(scope=None, category="comments")
-    async def comment(self,
-        comment_id: int
-    ) -> CommentBundle:
+    def comment(self, comment_id: int) -> CommentBundle:
         """
         Get a comment and its replies (up to 2 levels deep).
 
         Parameters
         ----------
         comment_id
             The comment to get.
 
         Notes
         -----
         Implements the `Get a Comment
         <https://osu.ppy.sh/docs/index.html#get-a-comment>`__ endpoint.
         """
-        return await self._get(CommentBundle, f"/comments/{comment_id}")
-
+        return self._get(CommentBundle, f"/comments/{comment_id}")
 
     # /events
     # -------
 
     @request(Scope.PUBLIC, category="events")
-    async def events(self,
-        *,
-        sort: Optional[EventsSortT] = None,
-        cursor_string: Optional[str] = None
+    def events(
+        self, *, sort: Optional[EventsSortT] = None, cursor_string: Optional[str] = None
     ) -> Events:
         """
         Get most recent events, in order of creation time.
 
         Parameters
         ----------
         sort
@@ -1908,28 +2022,28 @@
 
         Notes
         -----
         Implements the `Get Events
         <https://osu.ppy.sh/docs/index.html#get-events>`__ endpoint.
         """
         params = {"cursor_string": cursor_string, "sort": sort}
-        return await self._get(Events, "/events", params)
-
+        return self._get(Events, "/events", params)
 
     # /forums
     # -------
 
     @request(Scope.FORUM_WRITE, category="forums")
-    async def forum_create_topic(self,
-       forum_id: int,
-       title: str,
-       body: str,
-       *,
-       poll: Optional[ForumPoll] = None,
-   ) -> CreateForumTopicResponse:
+    def forum_create_topic(
+        self,
+        forum_id: int,
+        title: str,
+        body: str,
+        *,
+        poll: Optional[ForumPoll] = None,
+    ) -> CreateForumTopicResponse:
         """
         https://osu.ppy.sh/docs/index.html#create-topic
         """
         data = {
             "body": body,
             "forum_id": forum_id,
             "title": title,
@@ -1939,18 +2053,18 @@
             data["forum_topic_poll[hide_results]"] = poll.hide_results
             data["forum_topic_poll[length_days]"] = poll.length_days
             data["forum_topic_poll[max_options]"] = poll.max_options
             data["forum_topic_poll[options]"] = "\r\n".join(poll.options)
             data["forum_topic_poll[title]"] = poll.title
             data["forum_topic_poll[vote_change]"] = poll.vote_change
 
-        return await self._post(CreateForumTopicResponse, "/forums/topics", data=data)
+        return self._post(CreateForumTopicResponse, "/forums/topics", data=data)
 
     @request(Scope.FORUM_WRITE, category="forums")
-    async def forum_reply(self, topic_id: int, body: str) -> ForumPost:
+    def forum_reply(self, topic_id: int, body: str) -> ForumPost:
         """
         Reply to a forum topic.
 
         Parameters
         ----------
         topic_id
             The topic to reply to.
@@ -1959,18 +2073,18 @@
 
         Notes
         -----
         Implements the `Reply Topic
         <https://osu.ppy.sh/docs/index.html#reply-topic>`__ endpoint.
         """
         data = {"body": body}
-        return await self._post(ForumPost, f"/forums/topics/{topic_id}/reply", data)
+        return self._post(ForumPost, f"/forums/topics/{topic_id}/reply", data)
 
     @request(Scope.FORUM_WRITE, category="forums")
-    async def forum_edit_topic(self, topic_id: int, title: str) -> ForumTopic:
+    def forum_edit_topic(self, topic_id: int, title: str) -> ForumTopic:
         """
         Edit a forum topic.
 
         Parameters
         ---------
         topic_id
             The topic to edit.
@@ -1979,18 +2093,18 @@
 
         Notes
         -----
         Implements the `Edit Topic
         <https://osu.ppy.sh/docs/index.html#edit-topic>`__ endpoint.
         """
         data = {"forum_topic[topic_title]": title}
-        return await self._put(ForumTopic, f"/forums/topics/{topic_id}", data)
+        return self._put(ForumTopic, f"/forums/topics/{topic_id}", data)
 
     @request(Scope.FORUM_WRITE, category="forums")
-    async def forum_edit_post(self, post_id: int, body: str) -> ForumPost:
+    def forum_edit_post(self, post_id: int, body: str) -> ForumPost:
         """
         Edit a forum post.
 
         Parameters
         ----------
         post_id
             The post to edit.
@@ -1999,25 +2113,26 @@
 
         Notes
         -----
         Implements the `Edit Post
         <https://osu.ppy.sh/docs/index.html#edit-post>`__ endpoint.
         """
         data = {"body": body}
-        return await self._put(ForumPost, f"/forums/posts/{post_id}", data)
+        return self._put(ForumPost, f"/forums/posts/{post_id}", data)
 
     @request(Scope.PUBLIC, category="forums")
-    async def forum_topic(self,
+    def forum_topic(
+        self,
         topic_id: int,
         *,
         cursor_string: Optional[str] = None,
         sort: Optional[ForumTopicSortT] = None,
         limit: Optional[int] = None,
         start: Optional[int] = None,
-        end: Optional[int] = None
+        end: Optional[int] = None,
     ) -> ForumTopicAndPosts:
         """
         Get a forum topic and its posts.
 
         Parameters
         ----------
         topic_id
@@ -2038,45 +2153,48 @@
             Ignored otherwise.
 
         Notes
         -----
         Implements the `Get Topic and Posts
         <https://osu.ppy.sh/docs/index.html#get-topic-and-posts>`__ endpoint.
         """
-        params = {"cursor_string": cursor_string, "sort": sort, "limit": limit,
-            "start": start, "end": end}
-        return await self._get(ForumTopicAndPosts, f"/forums/topics/{topic_id}",
-            params)
-
+        params = {
+            "cursor_string": cursor_string,
+            "sort": sort,
+            "limit": limit,
+            "start": start,
+            "end": end,
+        }
+        return self._get(ForumTopicAndPosts, f"/forums/topics/{topic_id}", params)
 
     # /friends
     # --------
 
     @request(Scope.FRIENDS_READ, category="friends")
-    async def friends(self) -> List[UserCompact]:
+    def friends(self) -> List[UserCompact]:
         """
         Get the friends of the authenticated user.
 
         Notes
         -----
         Implements the `Get Friends
         <https://osu.ppy.sh/docs/index.html#friends>`__ endpoint.
         """
-        return await self._get(List[UserCompact], "/friends")
-
+        return self._get(List[UserCompact], "/friends")
 
     # / ("home")
     # ----------
 
     @request(Scope.PUBLIC, category="home")
-    async def search(self,
+    def search(
+        self,
         query: str,
         *,
         mode: Optional[SearchModeT] = None,
-        page: Optional[int] = None
+        page: Optional[int] = None,
     ) -> Search:
         """
         Search users and wiki pages. If you want to search beatmapsets, see
         :meth:`search_beatmapsets`.
 
         Parameters
         ----------
@@ -2089,84 +2207,88 @@
 
         Notes
         -----
         Implements the `Search
         <https://osu.ppy.sh/docs/index.html#search>`__ endpoint.
         """
         params = {"mode": mode, "query": query, "page": page}
-        return await self._get(Search, "/search", params)
-
+        return self._get(Search, "/search", params)
 
     # /matches
     # --------
 
     @request(Scope.PUBLIC, category="matches")
-    async def matches(self) -> Matches:
+    def matches(self) -> Matches:
         """
         Get current matches. If you want to get a specific match, see
         :meth:`match`.
 
         Notes
         -----
         Implements the `Get Matches
         <https://osu.ppy.sh/docs/index.html#matches>`__ endpoint.
         """
-        return await self._get(Matches, "/matches")
+        return self._get(Matches, "/matches")
 
     @request(Scope.PUBLIC, category="matches")
-    async def match(self, match_id: MatchIdT) -> MatchResponse:
+    def match(
+        self,
+        match_id: MatchIdT,
+        *,
+        after_id: Optional[int] = None,
+        before_id: Optional[int] = None,
+        limit: Optional[int] = None,
+    ) -> MatchResponse:
         """
         Get a match (eg https://osu.ppy.sh/community/matches/97947404).
 
         Parameters
         ----------
         match_id
             The match to get.
 
         Notes
         -----
         Implements the `Get Match
         <https://osu.ppy.sh/docs/index.html#matchesmatch>`__ endpoint.
         """
-        return await self._get(MatchResponse, f"/matches/{match_id}")
-
+        params = {"after": after_id, "before": before_id, "limit": limit}
+        return self._get(MatchResponse, f"/matches/{match_id}", params=params)
 
     # /me
     # ---
 
     @request(Scope.IDENTIFY, category="me")
-    async def get_me(self,
-        mode: Optional[GameModeT] = None
-    ):
+    def get_me(self, mode: Optional[GameModeT] = None) -> User:
         """
         Get data about the authenticated user.
 
         Parameters
         ----------
         mode
             Get data about the specified mode. Defaults to the user's default
             mode.
 
         Notes
         -----
         Implements the `Get Own Data
         <https://osu.ppy.sh/docs/index.html#get-own-data>`__ endpoint.
         """
-        return await self._get(User, f"/me/{mode.value if mode else ''}")
-
+        return self._get(User, f"/me/{mode.value if mode else ''}")
 
     # /news
     # -----
 
     @request(scope=None, category="news")
-    async def news_listing(self,
+    def news_listing(
+        self,
         *,
         limit: Optional[int] = None,
         year: Optional[int] = None,
-        cursor_string: Optional[str] = None
+        cursor_string: Optional[str] = None,
     ) -> NewsListing:
         """
         Get news posts.
 
         Parameters
         ----------
         limit
@@ -2178,21 +2300,19 @@
 
         Notes
         -----
         Implements the `Get News Listing
         <https://osu.ppy.sh/docs/index.html#get-news-listing>`__ endpoint.
         """
         params = {"limit": limit, "year": year, "cursor_string": cursor_string}
-        return await self._get(NewsListing, "/news", params=params)
+        return self._get(NewsListing, "/news", params=params)
 
     @request(scope=None, category="news")
-    async def news_post(self,
-        news: str,
-        *,
-        key: Optional[NewsPostKeyT] = NewsPostKey.SLUG
+    def news_post(
+        self, news: str, *, key: Optional[NewsPostKeyT] = NewsPostKey.SLUG
     ) -> NewsPost:
         """
         Get a news post by id or slug.
 
         Parameters
         ----------
         news
@@ -2205,48 +2325,47 @@
         Implements the `Get News Post
         <https://osu.ppy.sh/docs/index.html#get-news-post>`__ endpoint.
         """
         # docs state key should be "unset to query by slug"
         if key is NewsPostKey.SLUG:
             key = None
         params = {"key": key}
-        return await self._get(NewsPost, f"/news/{news}", params=params)
-
+        return self._get(NewsPost, f"/news/{news}", params=params)
 
     # /oauth
     # ------
 
     @request(scope=None, category="oauth")
-    async def revoke_token(self):
+    def revoke_token(self):
         """
         Revoke the current token. This will remove any authentication and leave
         you unable to make any more api calls until you re-authenticate.
 
         Notes
         -----
         Implements the `Revoke Current Token
         <https://osu.ppy.sh/docs/index.html#revoke-current-token>`__ endpoint.
         """
         self.session.delete(f"{self.base_url}/oauth/tokens/current")
         self.remove_token(self.token_key, self.token_directory)
 
-
     # /rankings
     # ---------
 
     @request(Scope.PUBLIC, category="rankings")
-    async def ranking(self,
+    def ranking(
+        self,
         mode: GameModeT,
         type: RankingTypeT,
         *,
         country: Optional[str] = None,
         cursor: Optional[Cursor] = None,
         filter_: RankingFilterT = RankingFilter.ALL,
         spotlight: Optional[int] = None,
-        variant: Optional[str] = None
+        variant: Optional[str] = None,
     ) -> Rankings:
         """
         Get current rankings for the specified game mode. Can specify ``type``
         to get different types of rankings (performance, score, country, etc).
 
         Parameters
         ----------
@@ -2270,33 +2389,39 @@
             mania. Only available for ``RankingType.PERFORMANCE``.
 
         Notes
         -----
         Implements the `Get Ranking
         <https://osu.ppy.sh/docs/index.html#get-ranking>`__ endpoint.
         """
-        params = {"country": country, "cursor": cursor, "filter": filter_,
-            "spotlight": spotlight, "variant": variant}
-        return await self._get(Rankings, f"/rankings/{mode.value}/{type.value}",
-            params=params)
-
+        params = {
+            "country": country,
+            "cursor": cursor,
+            "filter": filter_,
+            "spotlight": spotlight,
+            "variant": variant,
+        }
+        return self._get(
+            Rankings, f"/rankings/{mode.value}/{type.value}", params=params
+        )
 
     # /rooms
     # ------
 
     # TODO add test for this once I figure out values for room_id and
     # playlist_id that actually produce a response lol
     @request(Scope.PUBLIC, category="rooms")
-    async def multiplayer_scores(self,
+    def multiplayer_scores(
+        self,
         room_id: int,
         playlist_id: int,
         *,
         limit: Optional[int] = None,
         sort: Optional[MultiplayerScoresSortT] = None,
-        cursor_string: Optional[str] = None
+        cursor_string: Optional[str] = None,
     ) -> MultiplayerScores:
         """
         Get scores on a playlist item in a room.
 
         Parameters
         ----------
         room_id
@@ -2312,61 +2437,65 @@
 
         Notes
         -----
         Implements the `Get Scores
         <https://osu.ppy.sh/docs/index.html#get-scores>`__ endpoint.
         """
         params = {"limit": limit, "sort": sort, "cursor_string": cursor_string}
-        return await self._get(MultiplayerScores,
-            f"/rooms/{room_id}/playlist/{playlist_id}/scores", params=params)
+        return self._get(
+            MultiplayerScores,
+            f"/rooms/{room_id}/playlist/{playlist_id}/scores",
+            params=params,
+        )
 
     @request(Scope.PUBLIC, category="rooms")
-    async def room(self, room_id: RoomIdT) -> Room:
+    def room(self, room_id: RoomIdT) -> Room:
         """
         Get a room.
 
         Parameters
         ----------
         room_id
             The room to get.
 
         Notes
         -----
         Implements the `Get Room
         <https://osu.ppy.sh/docs/index.html#roomsroom>`__ endpoint.
         """
-        return await self._get(Room, f"/rooms/{room_id}")
+        return self._get(Room, f"/rooms/{room_id}")
 
     @request(Scope.PUBLIC, requires_user=True, category="rooms")
-    async def room_leaderboard(self, room_id: RoomIdT) -> RoomLeaderboard:
+    def room_leaderboard(self, room_id: RoomIdT) -> RoomLeaderboard:
         """
         Get the leaderboard of a room.
 
         Parameters
         ----------
         room_id
             The room to get the leaderboard of.
 
         Notes
         -----
         Implements the `Get Room Leaderboard
         <https://osu.ppy.sh/docs/index.html#roomsroomleaderboard>`__ endpoint.
         """
-        return await self._get(RoomLeaderboard, f"/rooms/{room_id}/leaderboard")
+        return self._get(RoomLeaderboard, f"/rooms/{room_id}/leaderboard")
 
     @request(Scope.PUBLIC, requires_user=True, category="rooms")
-    async def rooms(self,
+    def rooms(
+        self,
         *,
         limit: Optional[int] = None,
         mode: Optional[RoomSearchModeT] = None,
         season_id: Optional[int] = None,
         # TODO enumify
         sort: Optional[str] = None,
         # TODO enumify
-        type_group: Optional[str] = None
+        type_group: Optional[str] = None,
     ) -> List[Room]:
         """
         Get the list of current rooms.
 
         Parameters
         ----------
         limit
@@ -2381,151 +2510,183 @@
             "playlists" (default) or "realtime".
 
         Notes
         -----
         Implements the `Get Rooms
         <https://osu.ppy.sh/docs/index.html#roomsmode>`__ endpoint.
         """
-        params = {"limit": limit, "mode": mode, "season_id": season_id,
-            "sort": sort, "type_group": type_group}
-        return await self._get(List[Room], "/rooms", params=params)
-
+        params = {
+            "limit": limit,
+            "mode": mode,
+            "season_id": season_id,
+            "sort": sort,
+            "type_group": type_group,
+        }
+        return self._get(List[Room], "/rooms", params=params)
 
     # /scores
     # -------
 
     @request(Scope.PUBLIC, category="scores")
-    async def score(self,
-        mode: GameModeT,
-        score_id: int
-    ) -> Score:
+    def score(self, score_id: int) -> Score:
         """
-        Get a score.
+        Get a score. This corresponds to urls of the form https://osu.ppy.sh/scores/1312718771
+        ("new id format").
+
+        If you have an old id which is per-gamemode, use api.score_mode.
 
         Parameters
         ----------
-        mode
-            The mode the score was set on.
         score_id
             The score to get.
 
         Notes
         -----
         Implements the `Get Score
         <https://osu.ppy.sh/docs/index.html#scoresmodescore>`__ endpoint.
         """
-        return await self._get(Score, f"/scores/{mode.value}/{score_id}")
+        return self._get(Score, f"/scores/{score_id}")
 
-    @request(Scope.PUBLIC, requires_user=True, category="scores")
-    async def download_score(self,
-        mode: GameModeT,
-        score_id: int,
-        *,
-        raw: bool = False
-    ) -> Replay:
+    @request(Scope.PUBLIC, category="scores")
+    def score_mode(self, mode: GameModeT, score_id: int) -> Score:
         """
-        Download the replay data of a score.
+        Get a score, where the score id is specific to the gamemode. This
+        corresponds to urls of the form https://osu.ppy.sh/scores/osu/4459998279
+        ("old id format").
+
+        If you have a new id which is global across gamemodes, use api.score.
 
         Parameters
         ----------
         mode
-            The mode of the score to download.
+            The mode the score was set on.
         score_id
-            The score to download.
-        raw
-            If ``True``, will return the raw string response from the api
-            instead of a :class:`~ossapi.replay.Replay` object.
+            The score to get.
 
         Notes
         -----
-        Implements the `Download Score
-        <https://osu.ppy.sh/docs/index.html#scoresmodescoredownload>`__
-        endpoint.
+        Implements the `Get Score
+        <https://osu.ppy.sh/docs/index.html#scoresmodescore>`__ endpoint.
         """
-        from aiohttp import ClientSession, ContentTypeError
-
-        if self.domain is Domain.LAZER:
-            raise ValueError("Downloading scores using the lazer domain is not "
-                "currently supported, as lazer itself does not currently "
-                "support replay downloads. This may change in the future. To "
-                "download replays, use the osu domain (ie, a normal Ossapi "
-                "instance.)")
-
-        url = f"{self.base_url}/scores/{mode.value}/{score_id}/download"
-
-        aiohttp_session = ClientSession()
-        r = await self.session.request_async("GET", url,
-            session=aiohttp_session)
+        return self._get(Score, f"/scores/{mode.value}/{score_id}")
 
+    def _download_score(self, *, url, raw):
+        r = self.session.get(url)
         # if the response above succeeded, it will return a raw string
         # instead of json. If it didn't succeed, it will return json with an
         # error.
         # So always try parsing as json to check if there's an error. If parsing
         # fails, just assume the request succeeded and move on.
-        # TODO we probably want to be checking headers here instead.
-        # Should be x-osu-replay for valid response.
         try:
-            json_ = await r.json()
-            await aiohttp_session.close()
+            json_ = r.json()
             self._check_response(json_, url)
-        except ContentTypeError:
+        except json.JSONDecodeError:
             pass
 
-        content = await r.read()
-        await aiohttp_session.close()
-
         if raw:
-            return content
+            return r.content
 
-        replay = osrparse.Replay.from_string(content)
+        replay = osrparse.Replay.from_string(r.content)
         return Replay(replay, self)
 
+    @request(Scope.PUBLIC, requires_user=True, category="scores")
+    def download_score(self, score_id: int, *, raw: bool = False) -> Replay:
+        """
+        Download the replay data of a score.
+
+        This endpoint is for score ids which don't have a matching gamemode
+        (new id format). If you have an old score id, use api.download_score_mode.
+
+        Parameters
+        ----------
+        score_id
+            The score to download.
+        raw
+            If ``True``, will return the raw string response from the api
+            instead of a :class:`~ossapi.replay.Replay` object.
+
+        Notes
+        -----
+        Implements the `Download Score
+        <https://osu.ppy.sh/docs/index.html#scoresmodescoredownload>`__
+        endpoint.
+        """
+        url = f"{self.base_url}/scores/{score_id}/download"
+        return self._download_score(url=url, raw=raw)
+
+    @request(Scope.PUBLIC, requires_user=True, category="scores")
+    def download_score_mode(
+        self, mode: GameModeT, score_id: int, *, raw: bool = False
+    ) -> Replay:
+        """
+        Download the replay data of a score.
+
+        This endpoint is for score ids which have a matching gamemode
+        (old id format). If you have a new score id, use api.download_score.
+
+        Parameters
+        ----------
+        mode
+            The mode of the score to download.
+        score_id
+            The score to download.
+        raw
+            If ``True``, will return the raw string response from the api
+            instead of a :class:`~ossapi.replay.Replay` object.
+
+        Notes
+        -----
+        Implements the `Download Score
+        <https://osu.ppy.sh/docs/index.html#scoresmodescoredownload>`__
+        endpoint.
+        """
+        url = f"{self.base_url}/scores/{mode.value}/{score_id}/download"
+        return self._download_score(url=url, raw=raw)
 
     # seasonal backgrounds
     # --------------------
 
     @request(scope=None, category="seasonal backgrounds")
-    async def seasonal_backgrounds(self) -> SeasonalBackgrounds:
+    def seasonal_backgrounds(self) -> SeasonalBackgrounds:
         """
         Get current seasonal backgrounds.
 
         Notes
         -----
         Implements the `Seasonal Backgrounds
         <https://osu.ppy.sh/docs/index.html#seasonal-backgrounds>`__ endpoint.
         """
-        return await self._get(SeasonalBackgrounds, "/seasonal-backgrounds")
-
+        return self._get(SeasonalBackgrounds, "/seasonal-backgrounds")
 
     # /spotlights
     # -----------
 
     @request(Scope.PUBLIC, category="spotlights")
-    async def spotlights(self) -> List[Spotlight]:
+    def spotlights(self) -> List[Spotlight]:
         """
         Get active spotlights.
 
         Notes
         -----
         Implements the `Get Spotlights
         <https://osu.ppy.sh/docs/index.html#get-spotlights>`__ endpoint.
         """
-        spotlights = await self._get(Spotlights, "/spotlights")
+        spotlights = self._get(Spotlights, "/spotlights")
         return spotlights.spotlights
 
-
     # /users
     # ------
 
     @request(Scope.PUBLIC, category="users")
-    async def user_kudosu(self,
+    def user_kudosu(
+        self,
         user_id: UserIdT,
         *,
         limit: Optional[int] = None,
-        offset: Optional[int] = None
+        offset: Optional[int] = None,
     ) -> List[KudosuHistory]:
         """
         Get user kudosu history.
 
         Parameters
         ----------
         user_id
@@ -2537,26 +2698,26 @@
 
         Notes
         -----
         Implements the `Get User Kudosu
         <https://osu.ppy.sh/docs/index.html#get-user-kudosu>`__ endpoint.
         """
         params = {"limit": limit, "offset": offset}
-        return await self._get(List[KudosuHistory], f"/users/{user_id}/kudosu",
-            params)
+        return self._get(List[KudosuHistory], f"/users/{user_id}/kudosu", params)
 
     @request(Scope.PUBLIC, category="users")
-    async def user_scores(self,
+    def user_scores(
+        self,
         user_id: UserIdT,
         type: ScoreTypeT,
         *,
         include_fails: Optional[bool] = None,
         mode: Optional[GameModeT] = None,
         limit: Optional[int] = None,
-        offset: Optional[int] = None
+        offset: Optional[int] = None,
     ) -> List[Score]:
         """
         Get scores of a user.
 
         user_id
             The user to get scores of.
         type
@@ -2579,26 +2740,30 @@
         # require a bool to be passed, and just do the conversion behind the
         # scenes.
         if include_fails is False:
             include_fails = 0
         if include_fails is True:
             include_fails = 1
 
-        params = {"include_fails": include_fails, "mode": mode, "limit": limit,
-            "offset": offset}
-        return await self._get(List[Score], f"/users/{user_id}/scores/{type.value}",
-            params)
+        params = {
+            "include_fails": include_fails,
+            "mode": mode,
+            "limit": limit,
+            "offset": offset,
+        }
+        return self._get(List[Score], f"/users/{user_id}/scores/{type.value}", params)
 
     @request(Scope.PUBLIC, category="users")
-    async def user_beatmaps(self,
+    def user_beatmaps(
+        self,
         user_id: UserIdT,
         type: UserBeatmapTypeT,
         *,
         limit: Optional[int] = None,
-        offset: Optional[int] = None
+        offset: Optional[int] = None,
     ) -> Union[List[Beatmapset], List[BeatmapPlaycount]]:
         """
         Get beatmaps of a user.
 
         Parameters
         ----------
         user_id
@@ -2622,23 +2787,25 @@
         """
         params = {"limit": limit, "offset": offset}
 
         return_type = List[Beatmapset]
         if type is UserBeatmapType.MOST_PLAYED:
             return_type = List[BeatmapPlaycount]
 
-        return await self._get(return_type,
-            f"/users/{user_id}/beatmapsets/{type.value}", params)
+        return self._get(
+            return_type, f"/users/{user_id}/beatmapsets/{type.value}", params
+        )
 
     @request(Scope.PUBLIC, category="users")
-    async def user_recent_activity(self,
+    def user_recent_activity(
+        self,
         user_id: UserIdT,
         *,
         limit: Optional[int] = None,
-        offset: Optional[int] = None
+        offset: Optional[int] = None,
     ) -> List[Event]:
         """
         Get recent activity of a user.
 
         Parameters
         ----------
         user_id
@@ -2651,23 +2818,23 @@
         Notes
         -----
         Implements the `Get User Recent Activity
         <https://osu.ppy.sh/docs/index.html#get-user-recent-activity>`__
         endpoint.
         """
         params = {"limit": limit, "offset": offset}
-        return await self._get(List[_Event], f"/users/{user_id}/recent_activity/",
-            params)
+        return self._get(List[_Event], f"/users/{user_id}/recent_activity/", params)
 
     @request(Scope.PUBLIC, category="users")
-    async def user(self,
+    def user(
+        self,
         user: Union[UserIdT, str],
         *,
         mode: Optional[GameModeT] = None,
-        key: Optional[UserLookupKeyT] = None
+        key: Optional[UserLookupKeyT] = None,
     ) -> User:
         """
         Get a user by id or username.
 
         user
             The user id or username of the user to get.
         mode
@@ -2679,21 +2846,18 @@
 
         Notes
         -----
         Implements the `Get User
         <https://osu.ppy.sh/docs/index.html#get-user>`__ endpoint.
         """
         params = {"key": key}
-        return await self._get(User, f"/users/{user}/{mode.value if mode else ''}",
-            params)
+        return self._get(User, f"/users/{user}/{mode.value if mode else ''}", params)
 
     @request(Scope.PUBLIC, category="users")
-    async def users(self,
-        user_ids: List[int]
-    ) -> List[UserCompact]:
+    def users(self, user_ids: List[int]) -> List[UserCompact]:
         """
         Batch get users by id. If you only want to retrieve a single user, or
         want to retrieve users by username instead of id, see :meth:`user`.
 
         Parameters
         ---------
         user_ids
@@ -2701,25 +2865,21 @@
 
         Notes
         -----
         Implements the `Get Users
         <https://osu.ppy.sh/docs/index.html#get-users>`__ endpoint.
         """
         params = {"ids": user_ids}
-        users = await self._get(Users, "/users", params)
-        return users.users
+        return self._get(Users, "/users", params).users
 
     # /wiki
     # -----
 
     @request(scope=None, category="wiki")
-    async def wiki_page(self,
-        locale: str,
-        path: str
-    ) -> WikiPage:
+    def wiki_page(self, locale: str, path: str) -> WikiPage:
         """
         Get a wiki page.
 
         Parameters
         ----------
         locale
             two letter language code of the wiki page.
@@ -2727,8 +2887,8 @@
             The path name of the wiki page.
 
         Notes
         -----
         Implements the `Get Wiki Page
         <https://osu.ppy.sh/docs/index.html#get-wiki-page>`__ endpoint.
         """
-        return await self._get(WikiPage, f"/wiki/{locale}/{path}")
+        return self._get(WikiPage, f"/wiki/{locale}/{path}")
```

### Comparing `ossapi-3.4.4/ossapi/replay.py` & `ossapi-4.0.0b1/ossapi/replay.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from osrparse import GameMode as OsrparseGameMode, Replay as OsrparseReplay
 
 from ossapi.models import GameMode, User, Beatmap
 from ossapi.mod import Mod
 from ossapi.enums import UserLookupKey
 
 game_mode_map = {
-    OsrparseGameMode.STD:   GameMode.OSU,
+    OsrparseGameMode.STD: GameMode.OSU,
     OsrparseGameMode.TAIKO: GameMode.TAIKO,
-    OsrparseGameMode.CTB:   GameMode.CATCH,
+    OsrparseGameMode.CTB: GameMode.CATCH,
     OsrparseGameMode.MANIA: GameMode.MANIA,
 }
 
+
 class Replay(OsrparseReplay):
     """
     A replay played by a player.
 
     Notes
     -----
     This is a thin wrapper around an :class:`osrparse.replay.Replay` instance.
     It converts some attributes to more appropriate types and adds :meth:`.user`
     and :meth:`.beatmap` to retrieve api-related objects.
     """
+
     def __init__(self, replay, api):
         super().__init__(
             mode=game_mode_map[replay.mode],
             game_version=replay.game_version,
             beatmap_hash=replay.beatmap_hash,
             username=replay.username,
             replay_hash=replay.replay_hash,
@@ -38,15 +40,15 @@
             max_combo=replay.max_combo,
             perfect=replay.perfect,
             mods=Mod(replay.mods.value),
             life_bar_graph=replay.life_bar_graph,
             timestamp=replay.timestamp,
             replay_data=replay.replay_data,
             replay_id=replay.replay_id,
-            rng_seed=replay.rng_seed
+            rng_seed=replay.rng_seed,
         )
 
         self._osrparse_mode = replay.mode
         self._osrparse_mods = replay.mods
         self._api = api
         self._beatmap = None
         self._user = None
@@ -100,10 +102,10 @@
             max_combo=self.max_combo,
             perfect=self.perfect,
             mods=self._osrparse_mods,
             life_bar_graph=self.life_bar_graph,
             timestamp=self.timestamp,
             replay_data=self.replay_data,
             replay_id=self.replay_id,
-            rng_seed=self.rng_seed
+            rng_seed=self.rng_seed,
         )
         return r.pack(dict_size=dict_size, mode=mode)
```

### Comparing `ossapi-3.4.4/ossapi/utils.py` & `ossapi-4.0.0b1/ossapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from enum import Enum, IntFlag
 from datetime import datetime, timezone
 from typing import Any, Union
 from dataclasses import dataclass
 
 from typing_utils import issubtype, get_origin, get_args
 
+
 def is_high_model_type(type_):
     """
     Whether ``type_`` is both a model type and not a base model type.
 
     "high" here is meant to indicate that it is not at the bottom of the model
     hierarchy, ie not a "base" model.
     """
     return is_model_type(type_) and not is_base_model_type(type_)
 
+
 def is_model_type(type_):
     """
     Whether ``type_`` is a subclass of ``Model``.
     """
     if not isinstance(type_, type):
         return False
     return issubclass(type_, Model)
 
+
 def is_base_model_type(type_):
     """
     Whether ``type_`` is a subclass of ``BaseModel``.
     """
     if not isinstance(type_, type):
         return False
     return issubclass(type_, BaseModel)
@@ -42,20 +45,22 @@
         # For instance, events should deserialize as _Event, but have a runtime
         # type of Event.
         #
         # This field allows setting the runtime type via annotations and the
         # deserialize type via passing this field.
         self.deserialize_type = deserialize_type
 
+
 class _Model:
     """
     Base class for all models in ``ossapi``. If you want a model which handles
     its own members and cleanup after instantion, subclass ``BaseModel``
     instead.
     """
+
     def override_types(self):
         """
         Sometimes, the types of attributes in models depends on the value of
         other fields in that model. By overriding this method, models can return
         "override types", which overrides the static annotation of attributes
         and tells ossapi to use the returned type to instantiate the attribute
         instead.
@@ -95,14 +100,15 @@
 
         ``preprocess_data`` is called before ``override_class`` and
         ``override_types``, so changes to the data in ``preprocess_data`` will
         affect the data passed to those methods.
         """
         return data
 
+
 class ModelMeta(type):
     def __new__(cls, name, bases, dct):
         model = super().__new__(cls, name, bases, dct)
         field_names = []
         for name, value in model.__dict__.items():
             if name.startswith("__") and name.endswith("__"):
                 continue
@@ -117,18 +123,20 @@
         # @dataclass will automatically define a str/repr if it can't find one
         # we defined ourselves. We *do* define one on Model, but I guess because
         # we're doing weird stuff with metaclasses it can't find it sometimes?
         # not sure. but we can fix it by telling @dataclass to never generate
         # a repr for us.
         return dataclass(model, repr=False)
 
+
 class Model(_Model, metaclass=ModelMeta):
     """
     A dataclass-style model. Provides an ``_api`` attribute.
     """
+
     # This is the ``OssapiV2`` instance that loaded this model.
     # can't annotate with OssapiV2 or we get a circular import error, this is
     # good enough.
     _api: Any
 
     def _foreign_key(self, fk, func, existing):
         if existing:
@@ -149,20 +157,21 @@
         func = lambda: self._api.beatmapset(beatmapset_id)
         return self._foreign_key(beatmapset_id, func, existing)
 
     def __str__(self):
         # don't print internal values
         blacklisted_keys = ["_api"]
         items = [
-            f"{k}={v!r}" for k, v in self.__dict__.items()
-            if k not in blacklisted_keys
+            f"{k}={v!r}" for k, v in self.__dict__.items() if k not in blacklisted_keys
         ]
         return "{}({})".format(type(self).__name__, ", ".join(items))
+
     __repr__ = __str__
 
+
 class BaseModel(_Model):
     """
     A model which promises to take care of its own members and cleanup, after we
     instantiate it.
 
     Normally, for a high (non-base) model type, we recurse down its members to
     look for more model types after we instantiate it. We also resolve
@@ -171,29 +180,33 @@
 
     A commonly used example of a base model type is an ``Enum``. Enums have
     their own magic that takes care of cleaning the data upon instantiation
     (taking a string and converting it into one of a finite set of enum members,
     for instance). We don't need or want to do anything else with an enum after
     instantiating it, hence it's defined as a base type.
     """
+
     pass
 
+
 class EnumModel(BaseModel, Enum):
     pass
 
+
 class IntFlagModel(BaseModel, IntFlag):
     pass
 
 
 class Datetime(datetime, BaseModel):
     """
     Our replacement for the ``datetime`` object that deals with the various
     datetime formats the api returns.
     """
-    def __new__(cls, value): # pylint: disable=signature-differs
+
+    def __new__(cls, value):
         if value is None:
             raise ValueError("cannot instantiate a Datetime with a null value")
         # the api returns a bunch of different timestamps: two ISO 8601
         # formats (eg "2018-09-11T08:45:49.000000Z" and
         # "2014-05-18T17:22:23+00:00"), a unix timestamp (eg
         # 1615385278000), and others. We handle each case below.
         # Fully compliant ISO 8601 parsing is apparently a pain, and
@@ -225,18 +238,18 @@
         try:
             _ = datetime.strptime(value, format_)
         except ValueError:
             return False
         return True
 
 
-
 # typing utils
 # ------------
 
+
 def is_optional(type_):
     """
     Whether ``type(None)`` is a valid instance of ``type_``. eg,
     ``is_optional(Union[str, int, NoneType]) == True``.
 
     Exception: when ``type_`` is any, we return false. Strictly speaking, if
     ``Any`` is a subtype of ``type_`` then we return false, since
@@ -266,19 +279,21 @@
     # Union[int, NoneType].
     if get_origin(type_) is Union:
         if get_args(type_)[1] is type(None):
             return True
 
     return issubtype(type(None), type_) and not issubtype(Any, type_)
 
+
 def is_primitive_type(type_):
     if not isinstance(type_, type):
         return False
     return type_ in [int, float, str, bool]
 
+
 def convert_primitive_type(value, type_):
     # In the json we receive, eg ``pp`` can have a value of ``15833``, which is
     # interpreted as an int by our json parser even though ``pp`` is a float.
     # Convert back to the correct typing here.
     # This is important as some consumers may rely on float-specific methods
     # (`#is_integer`)
     if type_ is float and isinstance(value, int):
```

### Comparing `ossapi-3.4.4/ossapi.egg-info/PKG-INFO` & `ossapi-4.0.0b1/ossapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.4.4
+Version: 4.0.0b1
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/tybug/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,14 @@
 ossapi is the definitive python wrapper for the osu! api. ossapi has complete coverage of [api v2](https://osu.ppy.sh/docs/index.html) and [api v1](https://github.com/ppy/osu-api/wiki), and provides both sync (`Ossapi`) and async (`OssapiAsync`) versions for api v2.
 
 If you need support or would like to contribute, feel free to ask in the `#ossapi` channel of the [circleguard discord](https://discord.gg/e84qxkQ).
 
 * [Installation](#installation)
 * [Quickstart](#quickstart)
 * [Async](#async)
-* [Lazer](#lazer)
 * [Endpoints](#endpoints)
   * [Beatmap Packs](#endpoints-beatmap-packs)
   * [Beatmaps](#endpoints-beatmaps)
   * [Beatmapsets](#endpoints-beatmapsets)
   * [Changelog](#endpoints-changelog)
   * [Chat](#endpoints-chat)
   * [Comments](#endpoints-comments)
@@ -45,14 +44,15 @@
   * [Rankings](#endpoints-rankings)
   * [Rooms](#endpoints-rooms)
   * [Scores](#endpoints-scores)
   * [Seasonal Backgrounds](#endpoints-seasonal-backgrounds)
   * [Spotlights](#endpoints-spotlights)
   * [Users](#endpoints-users)
   * [Wiki](#endpoints-wiki)
+* [Other domains](#other-domains)
 * [API v1 Usage](#api-v1-usage)
 
 
 ## Installation
 
 To install:
 
@@ -100,26 +100,26 @@
     await api.user("tybug")
 
 asyncio.run(main())
 ```
 
 [Read more about OssapiAsync on the docs.](https://tybug.github.io/ossapi/async.html)
 
-## Lazer
+## Other domains
 
-You can retrieve lazer-specific data (scores, leaderboards, etc) with ossapi:
+You can use ossapi to interact with the api of other deployments of the osu website, such as https://dev.ppy.sh.
 
 ```python
 from ossapi import Ossapi
 
-api_lazer = Ossapi(client_id, client_secret, domain="lazer")
-
-# best score on the lazer server (lazer + osu scores combined)
-scores = api_lazer.user_scores(12092800, "best")
-print(scores[0].pp)
+api = Ossapi(client_id, client_secret, domain="dev")
+# get the dev server pp leaderboards
+ranking = api.ranking("osu", "performance").ranking
+# pearline06, as of 2023
+print(ranking[0].user.username)
 ```
 
 [Read more about domains on the docs.](https://tybug.github.io/ossapi/domains.html)
 
 ## Endpoints
 
 All endpoints for api v2.
@@ -179,14 +179,15 @@
   * [`api.multiplayer_scores`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.multiplayer_scores)
   * [`api.room`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.room)
   * [`api.room_leaderboard`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.room_leaderboard)
   * [`api.rooms`](https://tybug.github.io/ossapi/rooms.html#ossapi.ossapiv2.Ossapi.rooms)
 * Scores<a name="endpoints-scores"></a>
   * [`api.download_score`](https://tybug.github.io/ossapi/scores.html#ossapi.ossapiv2.Ossapi.download_score)
   * [`api.score`](https://tybug.github.io/ossapi/scores.html#ossapi.ossapiv2.Ossapi.score)
+  * [`api.score_mode`](https://tybug.github.io/ossapi/scores.html#ossapi.ossapiv2.Ossapi.score_mode)
 * Seasonal Backgrounds<a name="endpoints-seasonal-backgrounds"></a>
   * [`api.seasonal_backgrounds`](https://tybug.github.io/ossapi/seasonal%20backgrounds.html#ossapi.ossapiv2.Ossapi.seasonal_backgrounds)
 * Spotlights<a name="endpoints-spotlights"></a>
   * [`api.spotlights`](https://tybug.github.io/ossapi/spotlights.html#ossapi.ossapiv2.Ossapi.spotlights)
 * Users<a name="endpoints-users"></a>
   * [`api.user`](https://tybug.github.io/ossapi/users.html#ossapi.ossapiv2.Ossapi.user)
   * [`api.user_beatmaps`](https://tybug.github.io/ossapi/users.html#ossapi.ossapiv2.Ossapi.user_beatmaps)
```

### Comparing `ossapi-3.4.4/pyproject.toml` & `ossapi-4.0.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ossapi"
-version = "3.4.4"
+version = "4.0.0beta1"
 description = "Complete python wrapper for osu! api v2 and v1."
 readme = "README.md"
 keywords = ["osu!", "wrapper", "api", "python"]
 authors = [
   {name = "Liam DeVoe", email = "orionldevoe@gmail.com" }
 ]
 classifiers = [
```

### Comparing `ossapi-3.4.4/tests/test_cursor.py` & `ossapi-4.0.0b1/tests/test_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest import TestCase
 
 from ossapi import RankingType, Cursor
 
 from tests import api_v2 as api
 
+
 class TestCursor(TestCase):
     def test_nullable_cursor(self):
         cursor = Cursor(page=199)
         r = api.ranking("osu", RankingType.SCORE, cursor=cursor)
         self.assertIsNotNone(r.cursor)
 
         # 200 is the last page of results so we expect a null cursor in response
```

### Comparing `ossapi-3.4.4/tests/test_endpoints.py` & `ossapi-4.0.0b1/tests/test_endpoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,332 +1,379 @@
 from datetime import datetime
 from unittest import TestCase
 
-from ossapi import (RankingType, BeatmapsetEventType, AccessDeniedError,
-    InsufficientScopeError, Mod, GameMode, ForumPoll, RoomSearchMode,
-    EventsSort)
+from ossapi import (
+    RankingType,
+    BeatmapsetEventType,
+    InsufficientScopeError,
+    Mod,
+    GameMode,
+    ForumPoll,
+    RoomSearchMode,
+    EventsSort,
+)
 
 from tests import (
-    TestCaseAuthorizationCode, TestCaseDevServer, UNIT_TEST_MESSAGE,
+    TestCaseAuthorizationCode,
+    TestCaseDevServer,
+    UNIT_TEST_MESSAGE,
     api_v2 as api,
     api_v2_full as api_full,
-    api_v2_lazer as api_lazer,
-    api_v2_dev as api_dev
+    api_v2_dev as api_dev,
 )
 
 
 class TestBeatmapsetDiscussionPosts(TestCase):
     def test_deserialize(self):
         api.beatmapset_discussion_posts()
 
+
 class TestUserRecentActivity(TestCase):
     def test_deserialize(self):
         api.user_recent_activity(12092800)
 
+
 class TestSpotlights(TestCase):
     def test_deserialize(self):
         api.spotlights()
 
+
 class TestUserBeatmaps(TestCase):
     def test_deserialize(self):
         api.user_beatmaps(user_id=12092800, type="most_played")
 
+
 class TestUserKudosu(TestCase):
     def test_deserialize(self):
         api.user_kudosu(user_id=3178418)
 
+
 class TestBeatmapScores(TestCase):
     def test_deserialize(self):
         api.beatmap_scores(beatmap_id=1981090)
 
+
 class TestBeatmap(TestCase):
     def test_deserialize(self):
         api.beatmap(beatmap_id=221777)
 
         # beatmap with a diff owner
         bm = api.beatmap(beatmap_id=1604098)
         # might need to be updated when
         # https://github.com/ppy/osu-web/issues/9784 is addressed.
         self.assertIsNone(bm.owner)
 
+
 class TestBeatmapset(TestCase):
     def test_deserialize(self):
         api.beatmapset(beatmap_id=3207950)
 
+
 class TestBeatmapsetEvents(TestCase):
     def test_deserialize(self):
         api.beatmapset_events()
 
     def test_all_types(self):
         # beatmapset_events is a really complicated endpoint in terms of return
         # types. We want to make sure both that we're not doing anything wrong,
         # and the osu! api isn't doing anything wrong by returning something
         # that doesn't match their documentation.
         for event_type in BeatmapsetEventType:
             api.beatmapset_events(types=[event_type])
 
+
 class TestRanking(TestCase):
     def test_deserialize(self):
         api.ranking("osu", RankingType.PERFORMANCE, country="US")
         api.ranking("osu", type="country")
         api.ranking("osu", type="charts")
 
         api.ranking("mania", "performance")
         api.ranking("mania", "performance", variant="4k")
         api.ranking("mania", "performance", variant="7k")
 
         api.ranking("fruits", "performance")
         api.ranking("taiko", "performance")
 
+
 class TestUserScores(TestCase):
     def test_deserialize(self):
         api.user_scores(12092800, "best")
 
+
 class TestBeatmapUserScore(TestCase):
     def test_deserialize(self):
         api.beatmap_user_score(beatmap_id=221777, user_id=2757689, mode="osu")
 
+
 class TestBeatmapUserScores(TestCase):
     def test_deserialize(self):
         api.beatmap_user_scores(beatmap_id=221777, user_id=2757689, mode="osu")
 
+
 class TestSearch(TestCase):
     def test_deserialize(self):
         api.search(query="peppy")
 
+
 class TestComment(TestCase):
     def test_deserialize(self):
         # normal comments
         api.comment(1)
         api.comment(1123123)
 
         # comment on a deleted object
         api.comment(3)
 
-class TestDownloadScore(TestCase):
-    def test_deserialize(self):
-        # api instance is using client credentials which doesn't have access to
-        # downloading replays
-        self.assertRaises(AccessDeniedError,
-            lambda: api.download_score(mode="osu", score_id=2797309065))
 
 class TestSearchBeatmaps(TestCase):
     def test_deserialize(self):
         api.search_beatmapsets(query="the big black")
 
+
 class TestUser(TestCase):
     def test_deserialize(self):
         api.user(12092800)
         # user with an account_history (tournament ban)
         api.user(9997093)
 
     def test_key(self):
         # make sure it automatically falls back to username if not specified
         api.user("tybug")
         api.user("tybug", key="username")
 
         self.assertRaises(Exception, lambda: api.user("tybug", key="id"))
 
+
 class TestMe(TestCase):
     def test_insufficient_scope(self):
         # client credentials grant can't request `Scope.IDENTIFY` and so can't
         # access /me
         self.assertRaises(InsufficientScopeError, api.get_me)
 
+
 class TestWikiPage(TestCase):
     def test_deserialize(self):
         api.wiki_page("en", "Welcome")
 
+
 class TestChangelogBuild(TestCase):
     def test_deserialize(self):
         api.changelog_build("stable40", "20210520.2")
 
+
 class TestChangelogListing(TestCase):
     def test_deserialize(self):
         api.changelog_listing()
 
+
 class TestChangelogLookup(TestCase):
     def test_deserialize(self):
         api.changelog_build_lookup("lazer")
 
+
 class TestForumTopic(TestCase):
     def test_deserialize(self):
         # normal topic
         # https://osu.ppy.sh/community/forums/topics/141240?n=1
         api.forum_topic(141240)
         # topic with a poll
         # https://osu.ppy.sh/community/forums/topics/1781998?n=1
         api.forum_topic(1781998)
 
+
 class TestBeatmapsetDiscussionVotes(TestCase):
     def test_deserialize(self):
         api.beatmapset_discussion_votes().votes[0].score
 
+
 class TestBeatmapsetDiscussions(TestCase):
     def test_deserialize(self):
         api.beatmapset_discussions()
 
+
 class TestNewsListing(TestCase):
     def test_deserialize(self):
         api.news_listing(year=2021)
 
+
 class TestNewsPost(TestCase):
     def test_deserialize(self):
         # querying the same post by id or slug should give the same result.
         post1 = api.news_post(1025, key="id")
         post2 = api.news_post("2021-10-04-halloween-fanart-contest", key="slug")
 
         self.assertEqual(post1.id, post2.id)
         self.assertEqual(post1, post2)
 
+
 class TestSeasonalBackgrounds(TestCase):
     def test_deserialize(self):
         api.seasonal_backgrounds()
 
+
 class TestBeatmapAttributes(TestCase):
     def test_deserialize(self):
         api.beatmap_attributes(221777, ruleset="osu")
         api.beatmap_attributes(221777, mods=Mod.HDDT)
         api.beatmap_attributes(221777, mods="HR")
         api.beatmap_attributes(221777, ruleset_id=0)
 
+
 class TestUsers(TestCase):
     def test_deserialize(self):
         api.users([12092800])
 
+
 class TestBeatmaps(TestCase):
     def test_deserialize(self):
         api.beatmaps([221777])
 
+
 class TestScore(TestCase):
     def test_deserialize(self):
         # downloadable
-        api.score(GameMode.OSU, 2243145877)
+        api.score(429915881)
         # downloadable, my score
-        api.score(GameMode.OSU, 3685255338)
+        api.score(1262758549)
         # not downloadable, my score
-        api.score(GameMode.OSU, 3772000814)
+        api.score(1312718771)
 
         # other gamemodes
-        api.score(GameMode.TAIKO, 176904666)
-        api.score(GameMode.MANIA, 524674141)
-        api.score(GameMode.CATCH, 211167989)
+        api.score(1874611010)
+        api.score(2238254261)
+        api.score(1958862711)
+
+
+class TestScoreMode(TestCase):
+    def test_deserialize(self):
+        # downloadable
+        api.score_mode(GameMode.OSU, 2243145877)
+        # downloadable, my score
+        api.score_mode(GameMode.OSU, 3685255338)
+        # not downloadable, my score
+        api.score_mode(GameMode.OSU, 3772000814)
+
+        # other gamemodes
+        api.score_mode(GameMode.TAIKO, 176904666)
+        api.score_mode(GameMode.MANIA, 524674142)
+        api.score_mode(GameMode.CATCH, 211167989)
+
 
 class TestFriends(TestCase):
     def test_access_denied(self):
         self.assertRaises(InsufficientScopeError, api.friends)
 
+
 class TestRoom(TestCase):
     def test_deserialize(self):
         # https://osu.ppy.sh/multiplayer/rooms/257524
         api.room(257524)
 
+
 class TestMatches(TestCase):
     def test_deserialize(self):
         api.matches()
 
+
 class TestMatch(TestCase):
     def test_deserialize(self):
         # https://osu.ppy.sh/community/matches/97947404, tournament match
         api.match(97947404)
         # https://osu.ppy.sh/community/matches/103721175, deleted beatmap
         api.match(103721175)
 
+
 class TestComments(TestCase):
     def test_deserialize(self):
         api.comments()
 
+
 class TestEvents(TestCase):
     def test_deserialize(self):
         events = api.events()
         api.events(cursor_string=events.cursor_string)
         api.events(sort=EventsSort.NEW)
 
+
 class TestBeatmapPacks(TestCase):
     def test_deserialize(self):
         api.beatmap_packs()
         api.beatmap_packs("artist")
 
+
 class TestBeatmapPack(TestCase):
     def test_deserialize(self):
         api.beatmap_pack("S100")
         api.beatmap_pack("A1")
 
 
 # ======================
 # api_full test cases
 # ======================
 
+
 class TestCreateNewPM(TestCaseAuthorizationCode):
     def test_deserialize(self):
         # test_account https://osu.ppy.sh/users/14212521
         api_full.send_pm(14212521, UNIT_TEST_MESSAGE)
 
+
 class TestMeAuth(TestCaseAuthorizationCode):
     def test_deserialize(self):
         api_full.get_me()
 
+
 class TestFriendsAuth(TestCaseAuthorizationCode):
     def test_deserialize(self):
         api_full.friends()
 
+
 class TestRoomLeaderboard(TestCaseAuthorizationCode):
     def test_deserialize(self):
         # https://osu.ppy.sh/multiplayer/rooms/232594
         api_full.room_leaderboard(232594)
 
+
 class TestRooms(TestCaseAuthorizationCode):
     def test_deserialize(self):
         api_full.rooms()
         api_full.rooms(mode=RoomSearchMode.OWNED)
 
 
-# ====================
-# api_lazer test cases
-# ====================
-class TestLazerUser(TestCase):
-    def test_lazer_different_from_osu(self):
-        # make sure the lazer domain returns something different than the osu
-        # domain. ie, we're actually hitting a different db.
-
-        statistics = api.user("tybug").statistics
-        pp_osu = statistics.pp
-        pp_exp_osu = statistics.pp_exp
-
-        statistics = api_lazer.user("tybug").statistics
-        pp_lazer = statistics.pp
-        pp_exp_lazer = statistics.pp_exp
-
-        # pp_exp is 0 in lazer
-        self.assertEqual(pp_exp_lazer, 0)
-        # not necessarily an invariant, but happens to be true for my account
-        self.assertNotEqual(pp_osu, pp_lazer)
-        # this is the real invariant relating pp_exp and pp on the two domains.
-        self.assertEqual(pp_lazer, pp_exp_osu)
+class TestDownloadScore(TestCaseAuthorizationCode):
+    def test_deserialize(self):
+        api_full.download_score(429915881)
+
+
+class TestDownloadScoreMode(TestCaseAuthorizationCode):
+    def test_deserialize(self):
+        api_full.download_score_mode("osu", score_id=2243145877)
 
 
 # ==================
 # api_dev test cases
 # ==================
 
+
 class TestForum(TestCaseDevServer):
     def test_forum(self):
         # test creating both a topic and posting a reply in that topic.
         # be careful to post to one of the forums in
         # `double_post_allowed_forum_ids`, or else we'll be rejected for double
         # posting.
         # https://github.com/ppy/osu-web/blob/3d1586392102b05f2a3b264905c4dbb7b
         # 2d430a2/config/osu.php#L107.
 
         # create and edit a topic
-        response = api_dev.forum_create_topic(85, UNIT_TEST_MESSAGE,
-            UNIT_TEST_MESSAGE)
+        response = api_dev.forum_create_topic(85, UNIT_TEST_MESSAGE, UNIT_TEST_MESSAGE)
         topic_id = response.topic.id
-        api_dev.forum_edit_topic(topic_id,
-            f"This title was last updated at {datetime.now()}")
+        api_dev.forum_edit_topic(
+            topic_id, f"This title was last updated at {datetime.now()}"
+        )
 
         # unfortunately, 85 (help and technical support) is not one of the
         # whitelisted double posting allowed forums, so we can't create a reply
         # right after our post.
         # We could switch to another forum which does allow double posting
         # (off-topic), but then we can only make as many topics as we have
         # playcount, requiring me to constantly play on my dev account to make
@@ -348,19 +395,20 @@
             vote_change=True,
             max_options=1,
         )
         api_dev.forum_create_topic(
             title=f"{UNIT_TEST_MESSAGE}",
             body=f"{UNIT_TEST_MESSAGE} ({datetime.now()})",
             forum_id=85,
-            poll=poll
+            poll=poll,
         )
 
 
 # ==========================
 # provisional api test cases
 # ==========================
 
+
 class TestBeatmapScoresNonLegacy(TestCase):
     def test_deserialize(self):
         api._beatmap_scores_non_legacy(221777)
         api._beatmap_scores_non_legacy(221777, legacy_only=True)
```

### Comparing `ossapi-3.4.4/tests/test_models.py` & `ossapi-4.0.0b1/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from unittest import TestCase
 
-from ossapi import (User, BeatmapsetCompact, UserCompact, GameMode,
-    BeatmapCompact)
+from ossapi import User, BeatmapsetCompact, UserCompact, GameMode, BeatmapCompact
 
 from tests import api_v2 as api
 
 
 class TestMethodTypeConversion(TestCase):
     def test_beatmap_as_parameter(self):
         # make sure we can pass the full model in place of an id
         beatmap = api.beatmap(221777)
-        self.assertEqual(api.beatmap_scores(beatmap),
-            api.beatmap_scores(beatmap.id))
+        self.assertEqual(api.beatmap_scores(beatmap), api.beatmap_scores(beatmap.id))
 
     def test_room_as_parameter(self):
         room1 = api.room(257524)
         room2 = api.room(room1)
         self.assertEqual(room1, room2)
 
+
 class TestExpandableModels(TestCase):
     def test_expand_user(self):
         user = api.search(query="tybug").users.data[0]
         # `statistics` is only available on User models, so make sure it's not
         # present before expanding and is present afterwards
         self.assertIsNone(user.statistics)
 
@@ -41,14 +40,15 @@
 
         beatmapset_new = beatmapset.expand()
         self.assertIs(beatmapset_new, beatmapset)
 
     # TODO add test_expand_beatmap when I find a good endpoint that returns
     # BeatmapCompacts and not full Beatmaps.
 
+
 class TestFollowingForeignKeys(TestCase):
     def test_beatmap_fks(self):
         beatmap = api.beatmap(221777)
 
         user = beatmap.user()
         self.assertIsInstance(user, User)
         self.assertEqual(user.id, 1047883)
@@ -62,15 +62,15 @@
         beatmapset = api.beatmapset(beatmap_id=3207950)
 
         user = beatmapset.user()
         self.assertIsInstance(user, UserCompact)
         self.assertEqual(user.id, 4693052)
 
     def test_score_fks(self):
-        score = api.score(GameMode.OSU, 3685255338)
+        score = api.score_mode(GameMode.OSU, 3685255338)
 
         user = score.user()
         self.assertIsInstance(user, UserCompact)
         self.assertEqual(user.id, 12092800)
 
     def test_comment_fks(self):
         comment = api.comment(1533934).comments[0]
```

### Comparing `ossapi-3.4.4/tests/test_v1.py` & `ossapi-4.0.0b1/tests/test_v1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 from unittest import TestCase
 
 from tests import api_v1 as api
 
+
 class TestGetUser(TestCase):
     def test_deserialize(self):
         r = api.get_user("tybug")
 
         self.assertEqual(r.username, "tybug")
         self.assertEqual(api.get_user(12092800).username, "tybug")
 
+
 class TestGetBeatmaps(TestCase):
     def test_deserialize(self):
         api.get_beatmaps(beatmapset_id=1051305)
         api.get_beatmaps(beatmap_id=221777)
 
+
 class TestGetUserBest(TestCase):
     def test_deserialize(self):
         api.get_user_best(12092800)
 
+
 class TestGetReplay(TestCase):
     def test_deserialize(self):
         r1 = api.get_replay(beatmap_id=221777, user=2757689)
         r2 = api.get_replay(score_id=2828620518)
 
         self.assertEqual(len(r1), 155328)
         self.assertEqual(len(r2), 141068)
 
+
 class TestGetScores(TestCase):
     def test_deserialize(self):
         api.get_scores(221777)
         api.get_scores(221777, user="tybug")
 
+
 class TestGetUserRecent(TestCase):
     def test_deserialize(self):
         api.get_user_recent(12092800)
 
+
 class TestGetMatch(TestCase):
     def test_deserialize(self):
         api.get_match(69063884)
```

