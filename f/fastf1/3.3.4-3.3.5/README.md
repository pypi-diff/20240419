# Comparing `tmp/fastf1-3.3.4.tar.gz` & `tmp/fastf1-3.3.5.tar.gz`

## Comparing `fastf1-3.3.4.tar` & `fastf1-3.3.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/README.rst
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/example_fastf1_signalrclient.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_annotate_corners.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_annotate_speed_trace.py
--rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_driver_laptimes.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_gear_shifts_on_track.py
--rwxr-xr-x   0        0        0     3163 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_laptimes_distribution.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_position_changes.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_qualifying_results.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_results_tracker.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_speed_on_track.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_speed_traces.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_strategy.py
--rwxr-xr-x   0        0        0     2053 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_team_pace_ranking.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fastf1-3.3.4/examples/plot_who_can_still_win_wdc.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/__init__.py
--rw-r--r--   0        0        0    74642 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/_api.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/_version.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/api.py
--rw-r--r--   0        0        0   153144 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/core.py
--rw-r--r--   0        0        0    41549 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/events.py
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/legacy.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/logger.py
--rw-r--r--   0        0        0    16355 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/plotting.py
--rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/req.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/utils.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/__init__.py
--rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/interface.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/legacy.py
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/sphinx.py
--rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/ergast/structure.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/internals/__init__.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/internals/pandas_base.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/internals/pandas_extensions.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/livetiming/__init__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/livetiming/__main__.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/livetiming/client.py
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/livetiming/data.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/mvapi/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/mvapi/api.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/mvapi/data.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/mvapi/internals.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/LICENSE
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/_connection.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/events/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/events/_events.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/hubs/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/hubs/_hub.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/_exceptions.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/_parameters.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/_queue_events.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.3.4/fastf1/signalr_aio/transports/_transport.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 fastf1-3.3.4/requirements/dev.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.3.4/requirements/minver.txt
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastf1-3.3.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.3.4/LICENSE
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.3.4/README.md
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastf1-3.3.4/pyproject.toml
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fastf1-3.3.4/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/README.rst
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/example_fastf1_signalrclient.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_annotate_corners.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_annotate_speed_trace.py
+-rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_driver_laptimes.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_gear_shifts_on_track.py
+-rwxr-xr-x   0        0        0     3163 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_laptimes_distribution.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_position_changes.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_qualifying_results.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_results_tracker.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_speed_on_track.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_speed_traces.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_strategy.py
+-rwxr-xr-x   0        0        0     2053 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_team_pace_ranking.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fastf1-3.3.5/examples/plot_who_can_still_win_wdc.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/__init__.py
+-rw-r--r--   0        0        0    74642 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/_api.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/_version.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/api.py
+-rw-r--r--   0        0        0   154780 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/core.py
+-rw-r--r--   0        0        0    41549 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/events.py
+-rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/legacy.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/logger.py
+-rw-r--r--   0        0        0    16355 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/plotting.py
+-rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/req.py
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/utils.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/__init__.py
+-rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/interface.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/legacy.py
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/sphinx.py
+-rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/ergast/structure.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/internals/__init__.py
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/internals/pandas_base.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/internals/pandas_extensions.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/livetiming/__init__.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/livetiming/__main__.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/livetiming/client.py
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/livetiming/data.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/mvapi/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/mvapi/api.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/mvapi/data.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/mvapi/internals.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/LICENSE
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/_connection.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/events/_events.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/hubs/_hub.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.3.5/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 fastf1-3.3.5/requirements/dev.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.3.5/requirements/minver.txt
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastf1-3.3.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.3.5/LICENSE
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.3.5/README.md
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastf1-3.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fastf1-3.3.5/PKG-INFO
```

### Comparing `fastf1-3.3.4/examples/plot_annotate_corners.py` & `fastf1-3.3.5/examples/plot_annotate_corners.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_annotate_speed_trace.py` & `fastf1-3.3.5/examples/plot_annotate_speed_trace.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_driver_laptimes.py` & `fastf1-3.3.5/examples/plot_driver_laptimes.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_gear_shifts_on_track.py` & `fastf1-3.3.5/examples/plot_gear_shifts_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_laptimes_distribution.py` & `fastf1-3.3.5/examples/plot_laptimes_distribution.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_position_changes.py` & `fastf1-3.3.5/examples/plot_position_changes.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_qualifying_results.py` & `fastf1-3.3.5/examples/plot_qualifying_results.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_results_tracker.py` & `fastf1-3.3.5/examples/plot_results_tracker.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_speed_on_track.py` & `fastf1-3.3.5/examples/plot_speed_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_speed_traces.py` & `fastf1-3.3.5/examples/plot_speed_traces.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_strategy.py` & `fastf1-3.3.5/examples/plot_strategy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_team_pace_ranking.py` & `fastf1-3.3.5/examples/plot_team_pace_ranking.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/examples/plot_who_can_still_win_wdc.py` & `fastf1-3.3.5/examples/plot_who_can_still_win_wdc.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/__init__.py` & `fastf1-3.3.5/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/_api.py` & `fastf1-3.3.5/fastf1/_api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/api.py` & `fastf1-3.3.5/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/core.py` & `fastf1-3.3.5/fastf1/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,14 @@
      [5, 'VET', 'Aston Martin'], [18, 'STR', 'Aston Martin'],
      [14, 'ALO', 'Alpine'], [31, 'OCO', 'Alpine'],
      [22, 'TSU', 'AlphaTauri'], [10, 'GAS', 'AlphaTauri'],
      [47, 'MSC', 'Haas F1 Team'], [9, 'MAZ', 'Haas F1 Team'],
      [7, 'RAI', 'Alfa Romeo'], [99, 'GIO', 'Alfa Romeo'],
      [6, 'LAT', 'Williams'], [63, 'RUS', 'Williams']]
 
-_RACE_LIKE_SESSIONS = ('Race', 'Sprint', 'Sprint Qualifying')
-_QUALI_LIKE_SESSIONS = ('Qualifying', 'Sprint Shootout')
-
 
 class Telemetry(pd.DataFrame):
     """Multi-channel time series telemetry data
 
     The object can contain multiple telemetry channels. Multiple telemetry
     objects with different channels can be merged on time. Each telemetry
     channel is one dataframe column. Partial telemetry (e.g. for one lap only)
@@ -1197,14 +1194,26 @@
         self.api_path = api.make_path(
             self.event['EventName'],
             self.event['EventDate'].strftime('%Y-%m-%d'),
             self.name, _api_date.strftime('%Y-%m-%d')
         )
         """str: API base path for this session"""
 
+        if self.date.year <= 2023:
+            self._RACE_LIKE_SESSIONS = ('Race', 'Sprint', 'Sprint Qualifying')
+            # in 2021, 'Sprint Qualifying' was used as the name for a race-like
+            # session that set the grid for the main race
+            self._QUALI_LIKE_SESSIONS = ('Qualifying', 'Sprint Shootout')
+        else:
+            self._RACE_LIKE_SESSIONS = ('Race', 'Sprint')
+            self._QUALI_LIKE_SESSIONS = ('Qualifying', 'Sprint Qualifying')
+            # starting from 2024, 'Sprint Qualifying' is the name for the
+            # qualifying-like session that sets the grid for the Sprint
+            # (previously, this was called 'Sprint Shootout')
+
         self._ergast = ergast.Ergast()
 
         self._session_info: dict
 
         self._session_status: pd.DataFrame
         self._race_control_messages: pd.DataFrame
 
@@ -1493,15 +1502,15 @@
             if d2.shape[0] != len(d2['Stint'].unique()):
                 # tyre info includes correction messages that need to be
                 # applied before continuing
                 d2 = self.__fix_tyre_info(d2)
 
             is_generated = False
             if not len(d1):
-                if self.name in _RACE_LIKE_SESSIONS and len(d2):
+                if self.name in self._RACE_LIKE_SESSIONS and len(d2):
                     # add data for drivers who crashed on the very first lap
                     # as a downside, this potentially adds a nonexistent lap
                     # for drivers who could not start the race
                     is_generated = True
                     result = d1.copy()
                     result.reset_index(drop=True, inplace=True)
                     result['Driver'] = [driver, ]
@@ -1532,15 +1541,15 @@
             # add flag that indicates if the data for this lap was generated
             # by FastF1
             result['FastF1Generated'] = is_generated
 
             # calculate lap start time by setting it to the 'Time' of the
             # previous lap
             laps_start_time = list(result['Time'])[:-1]
-            if self.name in _RACE_LIKE_SESSIONS:
+            if self.name in self._RACE_LIKE_SESSIONS:
                 # assumption that the first lap started when the session was
                 # started can only be made for the race
                 laps_start_time.insert(0, self.session_start_time)
             else:
                 laps_start_time.insert(0, pd.NaT)
             laps_start_time = pd.Series(laps_start_time)
 
@@ -1558,15 +1567,15 @@
                         try:
                             restart_index = result.loc[
                                 result['PitOutTime'] > row['Time'],
                                 'PitOutTime'
                             ].index[0]
                         except IndexError:
                             continue  # no pit out, car did not restart
-                        if self.name in _RACE_LIKE_SESSIONS:
+                        if self.name in self._RACE_LIKE_SESSIONS:
                             # If this is a race-like session, we can assume the
                             # session restart time as lap start time.
                             # But only set from session status, if it is
                             # actually missing or incorrect (is correct in
                             # case backmarkers are allowed to unlap themselves
                             # at the end of the red flag by completing missing
                             # laps or if there is a formation lap for standing
@@ -1620,15 +1629,15 @@
         laps['Team'] = laps['DriverNumber'].map(t_map)
         d_map = {r['DriverNumber']: r['Abbreviation']
                  for _, r in self.results.iterrows()}
         laps['Driver'] = laps['DriverNumber'].map(d_map)
 
         # add Position based on lap timing
         laps['Position'] = np.NaN  # create empty column
-        if self.name in _RACE_LIKE_SESSIONS:
+        if self.name in self._RACE_LIKE_SESSIONS:
             for lap_n in laps['LapNumber'].unique():
                 # get each drivers lap for the current lap number, sorted by
                 # the time when each lap was set
                 laps_eq_n = laps.loc[
                     laps['LapNumber'] == lap_n, ('Time', 'Position')
                 ].reset_index(drop=True).sort_values(by='Time')
 
@@ -1776,24 +1785,45 @@
 
         # set all to False, then selectively set to True if actually deleted
         self._laps['Deleted'] = False
 
         msg_pattern = re.compile(
             r"CAR (\d{1,2}) .* TIME (\d:\d\d\.\d\d\d) DELETED - (.*)"
         )
+        msg_pattern_reinstated = re.compile(
+            r"CAR (\d{1,2}) .* TIME (\d:\d\d\.\d\d\d) .*REINSTATED.*"
+        )
         timestamp_pattern = re.compile(r"\d\d:\d\d:\d\d")
 
+        # Do a look-ahead pass to find laps that later were reinstated.
+        # This way, the deletion message can be ignored on the main pass which
+        # means that we do not need to preserve the state of a lap (e.g.
+        # 'IsPersonalBest') in case we'd need to reinstate it again.
+        reinstated_laps = list()
+        for _, row in self._race_control_messages.iterrows():
+            reinstated_match = msg_pattern_reinstated.match(row['Message'])
+            if reinstated_match:
+                drv = reinstated_match[1]
+                deleted_time = to_timedelta(reinstated_match[2])
+                reinstated_laps.append((drv, deleted_time))
+
+        # do the main pass where laps are marked as deleted
         for _, row in self._race_control_messages.iterrows():
             match = msg_pattern.match(row['Message'])
             if match:
                 drv = match[1]
                 deleted_time = to_timedelta(match[2])
+                if (drv, deleted_time) in reinstated_laps:
+                    # ignore this lap because it was reinstated later
+                    continue
+
                 # remove timestamp from reasons because confusingly it is given
                 # as local time at the track
                 reason = timestamp_pattern.sub("", match[3])
+
                 self._laps.loc[
                     (self._laps['DriverNumber'] == drv)
                     & (self._laps['LapTime'] == deleted_time),
                     ('Deleted', 'IsPersonalBest', 'DeletedReason')
                 ] = (True, False, reason)
 
     @soft_exceptions("quali results",
@@ -1803,15 +1833,15 @@
         """Try to calculate quali results from lap times if no results are
         available
 
         Args:
             force (bool): Force calculation of quali results even if
             results are already available, (default: False)"""
 
-        if self.name not in _QUALI_LIKE_SESSIONS:
+        if self.name not in self._QUALI_LIKE_SESSIONS:
             return
 
         if not hasattr(self, '_laps'):
             return
 
         if not self.results['Position'].isna().all() and not force:
             # Don't do anything if results are already available
@@ -1965,15 +1995,15 @@
                             "information!")
 
     @soft_exceptions("total lap count", "Failed to load total lap count!",
                      _logger)
     def _load_total_lap_count(self, livedata=None):
         # Get the number of originally scheduled laps
         # Lap count data only exists for race-like sessions.
-        if self.name in _RACE_LIKE_SESSIONS:
+        if self.name in self._RACE_LIKE_SESSIONS:
             try:
                 lap_count = api.lap_count(self.api_path, livedata=livedata)
                 # A race-like session can have multiple intended total laps,
                 # the first one being the original schedule
                 self._total_laps = lap_count['TotalLaps'][0]
             except IndexError:
                 self._total_laps = None
@@ -2232,15 +2262,15 @@
                                        driver_info['LastName']):
                     driver_info['FullName'].append(f"{first} {last}")
         return pd.DataFrame(driver_info, index=driver_info['DriverNumber'])
 
     def _drivers_results_from_ergast(
             self, *, load_drivers=False, load_results=False
     ) -> Optional[pd.DataFrame]:
-        if self.name in _RACE_LIKE_SESSIONS + _QUALI_LIKE_SESSIONS:
+        if self.name in self._RACE_LIKE_SESSIONS + self._QUALI_LIKE_SESSIONS:
             session_name = self.name
         else:
             # this is a practice session, use drivers from race session but
             # don't load results
             session_name = 'Race'
             load_results = False
 
@@ -2291,24 +2321,24 @@
             })
 
         if load_results:
             rename_return.update({
                 'position': 'Position',
             })
 
-            if session_name in _RACE_LIKE_SESSIONS:
+            if session_name in self._RACE_LIKE_SESSIONS:
                 rename_return.update({
                     'positionText': 'ClassifiedPosition',
                     'grid': 'GridPosition',
                     'status': 'Status',
                     'points': 'Points',
                     'totalRaceTime': 'Time'
                 })
 
-            if session_name in _QUALI_LIKE_SESSIONS:
+            if session_name in self._QUALI_LIKE_SESSIONS:
                 rename_return.update({
                     'Q1': 'Q1',
                     'Q2': 'Q2',
                     'Q3': 'Q3',
                 })
 
         # ergast does not provide all data for old sessions
@@ -3241,15 +3271,15 @@
 
             q1, q2, q3 = laps.split_qualifying_sessions()
 
         Returns: Three :class:`Laps` objects, one for Q1, Q2 and Q3
             each. If any of these sessions was cancelled, ``None`` will be
             returned instead of :class:`Laps`.
         """
-        if self.session.name not in _QUALI_LIKE_SESSIONS:
+        if self.session.name not in self.session._QUALI_LIKE_SESSIONS:
             raise ValueError("Session is not a qualifying session!")
         elif self.session.session_status is None:
             raise ValueError("Session status data is unavailable!")
 
         if self.session._session_split_times:
             # prefer using the split times that were generated by the timing
             # data parser, those are more reliable
```

### Comparing `fastf1-3.3.4/fastf1/events.py` & `fastf1-3.3.5/fastf1/events.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/legacy.py` & `fastf1-3.3.5/fastf1/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/logger.py` & `fastf1-3.3.5/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/plotting.py` & `fastf1-3.3.5/fastf1/plotting.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/req.py` & `fastf1-3.3.5/fastf1/req.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/utils.py` & `fastf1-3.3.5/fastf1/utils.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/ergast/interface.py` & `fastf1-3.3.5/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/ergast/legacy.py` & `fastf1-3.3.5/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/ergast/sphinx.py` & `fastf1-3.3.5/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/ergast/structure.py` & `fastf1-3.3.5/fastf1/ergast/structure.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/internals/pandas_base.py` & `fastf1-3.3.5/fastf1/internals/pandas_base.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/internals/pandas_extensions.py` & `fastf1-3.3.5/fastf1/internals/pandas_extensions.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/livetiming/__init__.py` & `fastf1-3.3.5/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/livetiming/__main__.py` & `fastf1-3.3.5/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/livetiming/client.py` & `fastf1-3.3.5/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/livetiming/data.py` & `fastf1-3.3.5/fastf1/livetiming/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/mvapi/api.py` & `fastf1-3.3.5/fastf1/mvapi/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/mvapi/data.py` & `fastf1-3.3.5/fastf1/mvapi/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/signalr_aio/LICENSE` & `fastf1-3.3.5/fastf1/signalr_aio/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/signalr_aio/_connection.py` & `fastf1-3.3.5/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/signalr_aio/hubs/_hub.py` & `fastf1-3.3.5/fastf1/signalr_aio/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/signalr_aio/transports/_parameters.py` & `fastf1-3.3.5/fastf1/signalr_aio/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/fastf1/signalr_aio/transports/_transport.py` & `fastf1-3.3.5/fastf1/signalr_aio/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/.gitignore` & `fastf1-3.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/LICENSE` & `fastf1-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/README.md` & `fastf1-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/pyproject.toml` & `fastf1-3.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.4/PKG-INFO` & `fastf1-3.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastf1
-Version: 3.3.4
+Version: 3.3.5
 Summary: Python package for accessing and analyzing Formula 1 results, schedules, timing data and telemetry.
 Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev
 Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: fastf1 Version: 3.3.4 Summary: Python package for
+Metadata-Version: 2.3 Name: fastf1 Version: 3.3.5 Summary: Python package for
 accessing and analyzing Formula 1 results, schedules, timing data and
 telemetry. Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org License: MIT License Copyright (c) 2024
 Philipp SchÃ¤fer Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
```

