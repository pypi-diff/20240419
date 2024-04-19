# Comparing `tmp/eflips_eval-1.0.3.tar.gz` & `tmp/eflips_eval-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_eval-1.0.3.tar", max compression
+gzip compressed data, was "eflips_eval-1.0.4.tar", max compression
```

## Comparing `eflips_eval-1.0.3.tar` & `eflips_eval-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    34260 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     4658 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/input/__init__.py
--rw-r--r--   0        0        0     3291 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/input/prepare.py
--rw-r--r--   0        0        0     1321 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/input/visualize.py
--rw-r--r--   0        0        0        0 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/output/__init__.py
--rw-r--r--   0        0        0    15760 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/output/prepare.py
--rw-r--r--   0        0        0    10443 2024-04-17 13:29:32.016875 eflips_eval-1.0.3/eflips/eval/output/visualize.py
--rw-r--r--   0        0        0      781 2024-04-17 13:29:32.036875 eflips_eval-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 eflips_eval-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-04-19 16:21:20.484800 eflips_eval-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0     4658 2024-04-19 16:21:20.484800 eflips_eval-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 16:21:20.484800 eflips_eval-1.0.4/eflips/eval/input/__init__.py
+-rw-r--r--   0        0        0     3291 2024-04-19 16:21:20.484800 eflips_eval-1.0.4/eflips/eval/input/prepare.py
+-rw-r--r--   0        0        0     1321 2024-04-19 16:21:20.484800 eflips_eval-1.0.4/eflips/eval/input/visualize.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:21:20.484800 eflips_eval-1.0.4/eflips/eval/output/__init__.py
+-rw-r--r--   0        0        0    16194 2024-04-19 16:21:20.484800 eflips_eval-1.0.4/eflips/eval/output/prepare.py
+-rw-r--r--   0        0        0    10506 2024-04-19 16:21:20.484800 eflips_eval-1.0.4/eflips/eval/output/visualize.py
+-rw-r--r--   0        0        0      781 2024-04-19 16:21:20.504800 eflips_eval-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 eflips_eval-1.0.4/PKG-INFO
```

### Comparing `eflips_eval-1.0.3/LICENSE.md` & `eflips_eval-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.3/README.md` & `eflips_eval-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.3/eflips/eval/input/prepare.py` & `eflips_eval-1.0.4/eflips/eval/input/prepare.py`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.3/eflips/eval/input/visualize.py` & `eflips_eval-1.0.4/eflips/eval/input/visualize.py`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.3/eflips/eval/output/prepare.py` & `eflips_eval-1.0.4/eflips/eval/output/prepare.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import zoneinfo
 from datetime import datetime, timedelta
 from typing import Dict, List, Iterable, Tuple
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import sqlalchemy
@@ -309,29 +310,32 @@
                 "vehicle_type_name": trip.rotation.vehicle_type.name,
             }
         )
     return pd.DataFrame(result)
 
 
 def vehicle_soc(
-    vehicle_id: int, session: Session
+    vehicle_id: int,
+    session: Session,
+    timezone: zoneinfo.ZoneInfo = zoneinfo.ZoneInfo("UTC"),
 ) -> Tuple[pd.DataFrame, Dict[str, List[Tuple[str, datetime, datetime]]]]:
     """
     This function takes in a vehicle id and returns a description what happened to the vehicle over time.
     The dataframe contains the following columns:
     - time: the time at which the SoC was recorded
     - soc: the state of charge at the given time
 
     Additionally, a dictionary for the different kinds of events is returned. For each kind of event, a list of Tuples
     with a description of the event, the start time and the end time is returned.
 
     The kinds of events are:
     - "rotation": A list of rotation names and the time the rotation started and ended
     - "charging": A list of the location of the charging and the time the charging started and ended
 
+    :param timezone: Explicit timezone information to use for the visualization. Default is UTC
     :param vehicle_id: the unique identifier of the vehicle
     :param session: A :class:`sqlalchemy.orm.session.Session` object to an eflips-model database
     :return: A pandas DataFrame
     """
     events_from_db = (
         session.query(Event)
         .filter(Event.vehicle_id == vehicle_id)
@@ -343,45 +347,52 @@
         "rotation": [],
         "charging": [],
     }
 
     # Go through all events and connect the soc_start and soc_end and time_start and time_end
     all_times = []
     all_soc = []
+
     for event in events_from_db:
-        all_times.append(event.time_start)
-        all_times.append(event.time_end)
+        all_times.append(event.time_start.astimezone(timezone))
+        all_soc.append(event.soc_start)
 
         if event.timeseries is not None:
             this_event_times: List[datetime] = [
-                datetime.fromisoformat(t) for t in event.timeseries["time"]  # type: ignore
+                datetime.fromisoformat(t).astimezone(timezone) for t in event.timeseries["time"]  # type: ignore
             ]
             this_event_socs: List[float] = event.timeseries["soc"]  # type: ignore
             all_times.extend(this_event_times)
             all_soc.extend(this_event_socs)
 
-        all_soc.append(event.soc_start)
+        all_times.append(event.time_end.astimezone(timezone))
         all_soc.append(event.soc_end)
 
         if (
             event.event_type == EventType.CHARGING_DEPOT
             or event.event_type == EventType.CHARGING_OPPORTUNITY
         ):
             if event.area is not None:
                 name = event.area.name + " in " + event.area.depot.name
             else:
                 name = event.station.name
 
-            descriptions["charging"].append((name, event.time_start, event.time_end))
+            descriptions["charging"].append(
+                (
+                    name,
+                    event.time_start.astimezone(timezone),
+                    event.time_end.astimezone(timezone),
+                )
+            )
 
     for rotation in (
         session.query(Rotation).filter(Rotation.vehicle_id == vehicle_id).all()
     ):
         descriptions["rotation"].append(
             (
                 rotation.name,
-                rotation.trips[0].departure_time,
-                rotation.trips[-1].arrival_time,
+                rotation.trips[0].departure_time.astimezone(timezone),
+                rotation.trips[-1].arrival_time.astimezone(timezone),
             )
         )
 
     return (pd.DataFrame({"time": all_times, "soc": all_soc}), descriptions)
```

### Comparing `eflips_eval-1.0.3/eflips/eval/output/visualize.py` & `eflips_eval-1.0.4/eflips/eval/output/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             color = "event_type"
             color_discrete_map = {
                 "Charging Depot": "forestgreen",
                 "Charging Opportunity": "lightgreen",
                 "Driving": "skyblue",
                 "Service": "salmon",
                 "Standby Departure": "orange",
-                "Standby": "lightcoral",
+                "Standby": "yellow",
                 "Precondition": "lightgrey",
             }
             color_continuous_scale = ""
         case "soc":
             color = "soc_end"
             color_discrete_map = None
             color_continuous_scale = px.colors.sequential.Viridis
@@ -91,15 +91,17 @@
             "soc": "State of Charge (%)",
             "time": "Time",
             "rotation_name": "Rotation Name",
             "vehicle_type_name": "Vehicle Type",
             "event_type": "Event Type",
         },
     )
-    fig.update(layout_yaxis_range=[0, 100])
+
+    lower_range = min(prepared_data["soc"])
+    fig.update(layout_yaxis_range=[min(lower_range - 1, 0), 100])
     return fig
 
 
 def depot_event(
     prepared_data: pd.DataFrame, color_scheme: str = "event_type"
 ) -> go.Figure:
     """
```

### Comparing `eflips_eval-1.0.3/pyproject.toml` & `eflips_eval-1.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-eval"
-version = "1.0.3"
+version = "1.0.4"
 description = ""
 authors = [
     "Ludger Heide <ludger.heide@lhtechnologies.de>",
 	"Shuyao Guo <shuyao.guo@tu-berlin.de>"
 ]
 readme = "README.md"
 packages = [{ include = "eflips/eval" }]
```

### Comparing `eflips_eval-1.0.3/PKG-INFO` & `eflips_eval-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-eval
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: Ludger Heide
 Author-email: ludger.heide@lhtechnologies.de
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

