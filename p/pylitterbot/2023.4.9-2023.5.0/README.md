# Comparing `tmp/pylitterbot-2023.4.9.tar.gz` & `tmp/pylitterbot-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylitterbot-2023.4.9.tar", max compression
+gzip compressed data, was "pylitterbot-2023.5.0.tar", max compression
```

## Comparing `pylitterbot-2023.4.9.tar` & `pylitterbot-2023.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1076 2023-10-02 17:29:25.010079 pylitterbot-2023.4.9/LICENSE
--rw-r--r--   0        0        0     3168 2023-10-02 17:29:25.010079 pylitterbot-2023.4.9/README.md
--rw-r--r--   0        0        0      403 2023-10-02 17:29:45.826167 pylitterbot-2023.4.9/pylitterbot/__init__.py
--rw-r--r--   0        0        0     8594 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/account.py
--rw-r--r--   0        0        0     1118 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/activity.py
--rw-r--r--   0        0        0     4597 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/enums.py
--rw-r--r--   0        0        0     1149 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/event.py
--rw-r--r--   0        0        0      348 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/exceptions.py
--rw-r--r--   0        0        0        0 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/py.typed
--rw-r--r--   0        0        0     6170 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/__init__.py
--rw-r--r--   0        0        0    10446 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/feederrobot.py
--rw-r--r--   0        0        0     7187 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/litterrobot.py
--rw-r--r--   0        0        0    11704 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/litterrobot3.py
--rw-r--r--   0        0        0    25838 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/litterrobot4.py
--rw-r--r--   0        0        0     2364 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/robot/models.py
--rw-r--r--   0        0        0     9337 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/session.py
--rw-r--r--   0        0        0     4170 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/utils.py
--rw-r--r--   0        0        0     5148 2023-10-02 17:29:25.014079 pylitterbot-2023.4.9/pylitterbot/ws_monitor.py
--rw-r--r--   0        0        0     1176 2023-10-02 17:29:45.826167 pylitterbot-2023.4.9/pyproject.toml
--rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pylitterbot-2023.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/LICENSE
+-rw-r--r--   0        0        0     3168 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/README.md
+-rw-r--r--   0        0        0      436 2024-04-19 16:20:10.180045 pylitterbot-2023.5.0/pylitterbot/__init__.py
+-rw-r--r--   0        0        0     9640 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/account.py
+-rw-r--r--   0        0        0     1119 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/activity.py
+-rw-r--r--   0        0        0     4598 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/enums.py
+-rw-r--r--   0        0        0     1150 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/event.py
+-rw-r--r--   0        0        0      348 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/exceptions.py
+-rw-r--r--   0        0        0    10063 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/pet.py
+-rw-r--r--   0        0        0        0 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/py.typed
+-rw-r--r--   0        0        0     6199 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/robot/__init__.py
+-rw-r--r--   0        0        0    10447 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/robot/feederrobot.py
+-rw-r--r--   0        0        0     7206 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/robot/litterrobot.py
+-rw-r--r--   0        0        0    11705 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/robot/litterrobot3.py
+-rw-r--r--   0        0        0    26318 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/robot/litterrobot4.py
+-rw-r--r--   0        0        0     2419 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/robot/models.py
+-rw-r--r--   0        0        0     9338 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/session.py
+-rw-r--r--   0        0        0     4197 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/utils.py
+-rw-r--r--   0        0        0     5149 2024-04-19 16:19:56.707969 pylitterbot-2023.5.0/pylitterbot/ws_monitor.py
+-rw-r--r--   0        0        0     1505 2024-04-19 16:20:10.180045 pylitterbot-2023.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4139 1970-01-01 00:00:00.000000 pylitterbot-2023.5.0/PKG-INFO
```

### Comparing `pylitterbot-2023.4.9/LICENSE` & `pylitterbot-2023.5.0/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2023 Nathan Spencer
+Copyright (c) 2020-2024 Nathan Spencer
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pylitterbot-2023.4.9/README.md` & `pylitterbot-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pylitterbot-2023.4.9/pylitterbot/account.py` & `pylitterbot-2023.5.0/pylitterbot/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Account access and data handling for Litter-Robot endpoint."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 from collections.abc import Callable
 from typing import TypeVar, cast
 
@@ -11,14 +12,15 @@
     ClientResponseError,
     ClientSession,
     ClientWebSocketResponse,
 )
 
 from .event import EVENT_UPDATE
 from .exceptions import LitterRobotException, LitterRobotLoginException
+from .pet import Pet
 from .robot import Robot
 from .robot.feederrobot import FEEDER_ENDPOINT, FEEDER_ROBOT_MODEL, FeederRobot
 from .robot.litterrobot3 import DEFAULT_ENDPOINT, DEFAULT_ENDPOINT_KEY, LitterRobot3
 from .robot.litterrobot4 import LITTER_ROBOT_4_MODEL, LR4_ENDPOINT, LitterRobot4
 from .session import LitterRobotSession
 from .utils import decode, urljoin
 from .ws_monitor import WebSocketMonitor
@@ -40,20 +42,21 @@
         self._session = LitterRobotSession(token=token, websession=websession)
         self._session._custom_args[DEFAULT_ENDPOINT] = {
             "headers": {"x-api-key": decode(DEFAULT_ENDPOINT_KEY)}
         }
         self._user_id = self._session.get_user_id() if token else None
         self._user: dict = {}
         self._robots: list[Robot] = []
+        self._pets: list[Pet] = []
         self._monitors: dict[type[Robot], WebSocketMonitor] = {}
 
         if token_update_callback:
             self._session.on(
                 EVENT_UPDATE,
-                lambda session=self._session: token_update_callback(session.tokens),  # type: ignore
+                lambda session=self._session: token_update_callback(session.tokens),
             )
 
     @property
     def user_id(self) -> str | None:
         """Return the logged in user's id."""
         if not self._user_id and self.session:
             self._user_id = self.session.get_user_id()
@@ -61,14 +64,19 @@
 
     @property
     def robots(self) -> list[Robot]:
         """Return the set of robots for the logged in account."""
         return self._robots
 
     @property
+    def pets(self) -> list[Pet]:
+        """Return the set of pets for the logged in account."""
+        return self._pets
+
+    @property
     def session(self) -> LitterRobotSession:
         """Return the associated session on the account."""
         return self._session
 
     def get_robot(self, robot_id: str | int | None) -> Robot | None:
         """If found, return the robot with the specified id."""
         return next(
@@ -76,20 +84,28 @@
             None,
         )
 
     def get_robots(self, robot_class: type[_RobotT]) -> list[_RobotT]:
         """If found, return the specified class of robots."""
         return [robot for robot in self._robots if isinstance(robot, robot_class)]
 
+    def get_pet(self, pet_id: str) -> Pet | None:
+        """If found, return the pet with the specified id."""
+        return next(
+            (pet for pet in self._pets if pet.id == pet_id),
+            None,
+        )
+
     async def connect(
         self,
         username: str | None = None,
         password: str | None = None,
         load_robots: bool = False,
         subscribe_for_updates: bool = False,
+        load_pets: bool = False,
     ) -> None:
         """Connect to the Litter-Robot API."""
         try:
             if not self.session.is_token_valid():
                 if self.session.has_refresh_token():
                     await self.session.refresh_token()
                 elif username and password:
@@ -97,14 +113,18 @@
                 else:
                     raise LitterRobotLoginException(
                         "Username and password are required to login to Litter-Robot."
                     )
 
             if load_robots:
                 await self.load_robots(subscribe_for_updates)
+
+            if load_pets:
+                await self.load_pets()
+
         except ClientResponseError as ex:
             _LOGGER.error(ex)
             if ex.status == 401:
                 raise LitterRobotLoginException(
                     "Unable to login to Litter-Robot with the supplied credentials."
                 ) from ex
             raise LitterRobotException("Unable to login to Litter-Robot.") from ex
@@ -122,14 +142,27 @@
         """Refresh the logged in user's info."""
         data = cast(
             dict,
             await self.session.get(urljoin(DEFAULT_ENDPOINT, f"users/{self.user_id}")),
         )
         self._user.update(data.get("user", {}))
 
+    async def load_pets(self) -> None:
+        """Get information about the pets connected to the account."""
+        assert self.user_id
+        pets = await Pet.fetch_pets_for_user(self._session, self.user_id)
+        if not self._pets:
+            self._pets = pets
+        else:
+            for pet in pets:
+                if existing_pet := self.get_pet(pet.id):
+                    existing_pet._update_data(pet._data)
+                else:
+                    self._pets.append(pet)
+
     async def load_robots(self, subscribe_for_updates: bool = False) -> None:
         """Get information about robots connected to the account."""
         robots: list[Robot] = []
         try:
             all_robots = [
                 self.session.get(
                     urljoin(DEFAULT_ENDPOINT, f"users/{self.user_id}/robots")
@@ -173,19 +206,19 @@
                     robot._update_data(data)
                 else:
                     robot = robot_cls(data=data, account=self)
                     if subscribe_for_updates:
                         await robot.subscribe()
                 robots.append(robot)
 
-            for robot_data in resp[0]:
+            for robot_data in resp[0]:  # type: ignore
                 await update_or_create_robot(LitterRobot3, robot_data)
-            for robot_data in resp[1].get("data").get("getLitterRobot4ByUser") or []:
+            for robot_data in resp[1].get("data").get("getLitterRobot4ByUser") or []:  # type: ignore
                 await update_or_create_robot(LitterRobot4, robot_data)
-            for robot_data in resp[2].get("data").get("feeder_unit") or []:
+            for robot_data in resp[2].get("data", {}).get("feeder_unit") or []:  # type: ignore
                 await update_or_create_robot(FeederRobot, robot_data)
 
             self._robots = robots
         except (LitterRobotException, ClientResponseError, ClientConnectorError) as ex:
             _LOGGER.error("Unable to retrieve your robots: %s", ex)
 
     async def refresh_robots(self) -> None:
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/activity.py` & `pylitterbot-2023.5.0/pylitterbot/activity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pylitterbot activity and insight classes."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import date, datetime
 
 from .enums import LitterBoxStatus
 from .utils import pluralize
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/enums.py` & `pylitterbot-2023.5.0/pylitterbot/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pylitterbot enums."""
+
 from __future__ import annotations
 
 import logging
 from enum import Enum
 from typing import Any
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/event.py` & `pylitterbot-2023.5.0/pylitterbot/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Event handling class for pylitterbot."""
+
 from __future__ import annotations
 
 from collections.abc import Callable
 from dataclasses import dataclass, field
 from typing import Any
 
 EVENT_UPDATE = "update"
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/robot/__init__.py` & `pylitterbot-2023.5.0/pylitterbot/robot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Robot base class."""
+
 from __future__ import annotations
 
 import logging
 from abc import abstractmethod
 from collections.abc import Callable
 from datetime import datetime
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, cast
 
 from aiohttp import ClientWebSocketResponse
 from deepdiff import DeepDiff
 
 from ..event import EVENT_UPDATE, Event
 from ..utils import to_timestamp, urljoin
 
@@ -65,15 +66,15 @@
     def model(self) -> str:
         """Return the robot model."""
         return self._attr_model
 
     @property
     def name(self) -> str:
         """Return the name of the robot, if any."""
-        return self._data.get(self._data_name, "")
+        return cast(str, self._data.get(self._data_name, ""))
 
     @property
     @abstractmethod
     def night_light_mode_enabled(self) -> bool:
         """Return `True` if night light mode is enabled."""
 
     @property
@@ -90,15 +91,15 @@
         `DC` = battery backup
         `NC` = unknown, not connected or off
         """
 
     @property
     def serial(self) -> str:
         """Return the serial of the robot, if any."""
-        return self._data.get(self._data_serial, "")
+        return cast(str, self._data.get(self._data_serial, ""))
 
     @property
     def setup_date(self) -> datetime | None:
         """Return the datetime the robot was onboarded, if any."""
         return to_timestamp(self._data.get(self._data_setup_date))
 
     @abstractmethod
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/robot/feederrobot.py` & `pylitterbot-2023.5.0/pylitterbot/robot/feederrobot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Feeder-Robot."""
+
 from __future__ import annotations
 
 import logging
 from copy import deepcopy
 from typing import TYPE_CHECKING, Any, TypeVar, cast
 from uuid import uuid4
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/robot/litterrobot.py` & `pylitterbot-2023.5.0/pylitterbot/robot/litterrobot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Litter-Robot base class."""
+
 from __future__ import annotations
 
 import logging
 from abc import abstractmethod
 from collections.abc import Callable
 from datetime import datetime, time
-from typing import Any
+from typing import Any, cast
 
 from ..activity import Activity, Insight
 from ..enums import LitterBoxCommand, LitterBoxStatus
 from ..utils import to_timestamp
 from . import Robot
 
 _LOGGER = logging.getLogger(__name__)
@@ -71,15 +72,15 @@
     @abstractmethod
     def is_drawer_full_indicator_triggered(self) -> bool:
         """Return `True` if the drawer full indicator has been triggered."""
 
     @property
     def is_onboarded(self) -> bool:
         """Return `True` if the Litter-Robot is onboarded."""
-        return self._data.get("isOnboarded", False)
+        return self._data.get("isOnboarded") is True
 
     @property
     @abstractmethod
     def is_sleeping(self) -> bool:
         """Return `True` if the Litter-Robot is currently "sleeping" and won't automatically perform a clean cycle."""
 
     @property
@@ -96,15 +97,15 @@
     def power_status(self) -> str:
         """Return the power status.
 
         `AC` = normal/mains
         `DC` = battery backup
         `NC` = unknown, not connected or off
         """
-        return self._data.get(self._data_power_status, "NC")
+        return cast(str, self._data.get(self._data_power_status, "NC"))
 
     @property
     @abstractmethod
     def sleep_mode_enabled(self) -> bool:
         """Return `True` if sleep mode is enabled."""
 
     @property
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/robot/litterrobot3.py` & `pylitterbot-2023.5.0/pylitterbot/robot/litterrobot3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Litter-Robot 3."""
+
 from __future__ import annotations
 
 import logging
 from datetime import datetime, time, timedelta, timezone
 from typing import TYPE_CHECKING, Any, cast
 
 from ..activity import Activity, Insight
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/robot/litterrobot4.py` & `pylitterbot-2023.5.0/pylitterbot/robot/litterrobot4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Litter-Robot 4."""
+
 from __future__ import annotations
 
 import logging
 from datetime import datetime, time, timedelta, timezone
 from enum import Enum, IntEnum, unique
 from json import dumps
 from typing import TYPE_CHECKING, Any, Dict, Union, cast
@@ -49,14 +50,15 @@
     "robotCycleStatusIdle": LitterBoxStatus.CLEAN_CYCLE_COMPLETE,
     "robotStatusCatDetect": LitterBoxStatus.CAT_DETECTED,
 }
 CYCLE_STATE_STATUS_MAP = {
     "CYCLE_STATE_CAT_DETECT": LitterBoxStatus.CAT_SENSOR_INTERRUPTED,
     "CYCLE_STATE_PAUSE": LitterBoxStatus.PAUSED,
 }
+DISPLAY_CODE_STATUS_MAP = {"DC_CAT_DETECT": LitterBoxStatus.CAT_DETECTED}
 
 LITTER_LEVEL_EMPTY = 500
 
 
 @unique
 class BrightnessLevel(IntEnum):
     """Brightness level of a Litter-Robot 4 unit."""
@@ -113,54 +115,54 @@
         """Initialize a Litter-Robot 4."""
         super().__init__(data, account)
         self._path = LR4_ENDPOINT
 
     @property
     def clean_cycle_wait_time_minutes(self) -> int:
         """Return the number of minutes after a cat uses the Litter-Robot to begin an automatic clean cycle."""
-        return self._data.get("cleanCycleWaitTime", 7)
+        return cast(int, self._data.get("cleanCycleWaitTime", 7))
 
     @property
     def firmware(self) -> str:
         """Return the firmware version."""
         return (
             f"ESP: {self._data.get('espFirmware')} / "
             f"PIC: {self._data.get('picFirmwareVersion')} / "
             f"TOF: {self._data.get('laserBoardFirmwareVersion')}"
         )
 
     @property
     def firmware_update_status(self) -> str:
         """Return the firmware update status."""
-        return self._data.get("firmwareUpdateStatus", "UNKNOWN")
+        return cast(str, self._data.get("firmwareUpdateStatus", "UNKNOWN"))
 
     @property
     def firmware_update_triggered(self) -> bool:
         """Return `True` if a firmware update has been triggered."""
-        return self._data.get("isFirmwareUpdateTriggered", False)
+        return self._data.get("isFirmwareUpdateTriggered") is True
 
     @property
     def is_drawer_full_indicator_triggered(self) -> bool:
         """Return `True` if the drawer full indicator has been triggered."""
-        return self._data.get("isDFIFull", False)
+        return self._data.get("isDFIFull") is True
 
     @property
     def is_online(self) -> bool:
         """Return `True` if the robot is online."""
-        return self._data.get("isOnline", False)
+        return self._data.get("isOnline") is True
 
     @property
     def is_sleeping(self) -> bool:
         """Return `True` if the Litter-Robot is currently "sleeping" and won't automatically perform a clean cycle."""
         return bool(self._data.get("sleepStatus", "WAKE") != "WAKE")
 
     @property
     def is_waste_drawer_full(self) -> bool:
         """Return `True` if the Litter-Robot is reporting that the waste drawer is full."""
-        return self._data.get("isDFIFull", False)
+        return self._data.get("isDFIFull") is True
 
     @property
     def litter_level(self) -> float:
         """Return the litter level.
 
         The litterLevel field from the API is a millimeter distance to the
         top center time of flight (ToF) sensor and is interpreted as:
@@ -214,20 +216,20 @@
         if brightness in list(BrightnessLevel):
             return BrightnessLevel(brightness)
         return None
 
     @property
     def panel_lock_enabled(self) -> bool:
         """Return `True` if the buttons on the robot are disabled."""
-        return self._data.get("isKeypadLockout", False)
+        return self._data.get("isKeypadLockout") is True
 
     @property
     def pet_weight(self) -> float:
         """Return the last recorded pet weight in pounds (lbs)."""
-        return self._data.get("catWeight", 0)
+        return cast(float, self._data.get("catWeight", 0))
 
     @property
     def sleep_mode_enabled(self) -> bool:
         """Return `True` if sleep mode is enabled."""
         sleep_schedule = self._data["weekdaySleepModeEnabled"]
         return any(day["isEnabled"] for day in sleep_schedule.values())
 
@@ -241,38 +243,48 @@
     def sleep_mode_end_time(self) -> datetime | None:
         """Return the sleep mode end time, if any."""
         self._revalidate_sleep_info()
         return self._sleep_mode_end_time
 
     @property
     def status(self) -> LitterBoxStatus:
-        """Return the status of the Litter-Robot."""
+        """Return the status of the Litter-Robot.
+
+        The Litter-Robot 4's status is determined based on the values of:
+          - `displayCode`
+          - `robotCycleState`
+          - `robotStatus`
+          - `isDFIFull`
+          - `isOnline`
+        """
         if not self.is_online:
             return LitterBoxStatus.OFFLINE
-        cycle_state = self._data["robotCycleState"]
-        status = self._data["robotStatus"]
-        if status == "ROBOT_IDLE" and self.is_waste_drawer_full:
-            return LitterBoxStatus.DRAWER_FULL
-        return CYCLE_STATE_STATUS_MAP.get(
-            cycle_state, LR4_STATUS_MAP.get(status, LitterBoxStatus.UNKNOWN)
-        )
+        if status := CYCLE_STATE_STATUS_MAP.get(self._data["robotCycleState"]):
+            return status
+        status = LR4_STATUS_MAP.get(self._data["robotStatus"], LitterBoxStatus.UNKNOWN)
+        if status == LitterBoxStatus.READY:
+            if display_code := DISPLAY_CODE_STATUS_MAP.get(self._data["displayCode"]):
+                return display_code
+            if self.is_waste_drawer_full:
+                return LitterBoxStatus.DRAWER_FULL
+        return status
 
     @property
     def status_code(self) -> str | None:
         """Return the status code of the Litter-Robot."""
         return (
             self.status.value
             if self.status != LitterBoxStatus.UNKNOWN
             else self._data.get("robotStatus")
         )
 
     @property
     def waste_drawer_level(self) -> float:
         """Return the approximate waste drawer level."""
-        return self._data.get("DFILevelPercent", 0)
+        return cast(float, self._data.get("DFILevelPercent", 0))
 
     def _revalidate_sleep_info(self) -> None:
         """Revalidate sleep info."""
         if (
             self.sleep_mode_enabled
             and (now := utcnow()) > (self._sleep_mode_start_time or now)
             and now > (self._sleep_mode_end_time or now)
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/robot/models.py` & `pylitterbot-2023.5.0/pylitterbot/robot/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pylitterbot robot models."""
+
 FEEDER_ROBOT_MODEL = """
 {
     id
     name
     serial
     timezone
     isEighthCupEnabled
@@ -112,9 +113,12 @@
     isFirmwareUpdateTriggered
     firmwareUpdateStatus
     wifiModeStatus
     isUSBPowerOn
     USBFaultStatus
     isDFIPartialFull
     isLaserDirty
+    surfaceType
+    hopperStatus
+    scoopsSavedCount
 }}
 """
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/session.py` & `pylitterbot-2023.5.0/pylitterbot/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Session handling for litter-robot endpoint."""
+
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from asyncio import Lock
 from types import TracebackType
 from typing import Any, TypeVar, cast
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/utils.py` & `pylitterbot-2023.5.0/pylitterbot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities module."""
+
 from __future__ import annotations
 
 import json
 import logging
 import re
 from base64 import b64decode, b64encode
 from collections.abc import Iterable, Mapping
@@ -29,14 +30,15 @@
     "oneSignalPlayerId",
     "deviceId",
     "id",
     "litterRobotId",
     "unitId",
     "litterRobotSerial",
     "serial",
+    "s3ImageURL",
 ]
 
 
 def decode(value: str) -> str:
     """Decode a value."""
     return b64decode(value).decode(ENCODING)
 
@@ -100,21 +102,20 @@
     """Log a deprecation warning message."""
     message = f"{old_name} has been deprecated{'' if new_name is None else f' in favor of {new_name}'} and will be removed in a future release"
     warn(message, DeprecationWarning, stacklevel=2)
     _LOGGER.warning(message)
 
 
 @overload
-def redact(data: Mapping) -> dict:  # type: ignore[misc]
+def redact(data: Mapping) -> dict:  # type: ignore[overload-overlap]
     ...
 
 
 @overload
-def redact(data: _T) -> _T:
-    ...
+def redact(data: _T) -> _T: ...
 
 
 def redact(data: _T) -> _T:
     """Redact sensitive data in a dict."""
     if not isinstance(data, (Mapping, list)):
         return data
```

### Comparing `pylitterbot-2023.4.9/pylitterbot/ws_monitor.py` & `pylitterbot-2023.5.0/pylitterbot/ws_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Websocket monitor."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
 from datetime import datetime
 from json import loads
 from random import uniform
```

### Comparing `pylitterbot-2023.4.9/pyproject.toml` & `pylitterbot-2023.5.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylitterbot"
-version = "2023.4.9"
+version = "2023.5.0"
 description = "Python package for controlling Whisker automatic robots."
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/natekspencer/pylitterbot"
 repository = "https://github.com/natekspencer/pylitterbot"
 keywords = ["Whisker", "Litter-Robot", "Feeder-Robot", "litter box", "pet feeder", "asynchronous"]
@@ -14,29 +14,43 @@
 python = "^3.8.1"
 aiohttp = "^3.8.1"
 deepdiff = "^6.2.1"
 PyJWT = "^2.7.0"
 "backports.zoneinfo" = {version = "^0.2.1", python = "<3.9"}
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
-pytest-asyncio = "^0.21.0"
+pytest = ">=7.3.1,<9.0.0"
+pytest-asyncio = ">=0.21,<0.24"
 pytest-cov = "^4.1.0"
-pytest-freezegun = "^0.4.2"
 aioresponses = "^0.7.4"
-black = "^23.3.0"
-isort = "^5.11.5"
 mypy = "^1.3"
-flake8 = ">=5.0.4,<7.0.0"
-pylint = "^2.17.4"
 tox = ">=3.28,<5.0"
-pydocstyle = "^6.3.0"
 pytest-timeout = "^2.1.0"
+ruff = "^0.3"
+pytest-freezer = "^0.4.8"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
+[tool.ruff.lint]
+select = [
+    "D", # pydocstyle
+    "E", # pycodestyle Error
+    "F", # Pyflakes
+    "I", # isort
+    "W", # pycodestyle Warning
+]
+ignore = [
+    "D203", # 1 blank line required before class docstring
+    "D213", # Multi-line docstring summary should start at the second line
+    "E501", # Line too long
+]
+
+[tool.ruff.lint.isort]
+combine-as-imports = true
+split-on-trailing-comma = false
+
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `pylitterbot-2023.4.9/PKG-INFO` & `pylitterbot-2023.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pylitterbot
-Version: 2023.4.9
+Version: 2023.5.0
 Summary: Python package for controlling Whisker automatic robots.
 Home-page: https://github.com/natekspencer/pylitterbot
 License: MIT
 Keywords: Whisker,Litter-Robot,Feeder-Robot,litter box,pet feeder,asynchronous
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyJWT (>=2.7.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: backports.zoneinfo (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: deepdiff (>=6.2.1,<7.0.0)
 Project-URL: Repository, https://github.com/natekspencer/pylitterbot
 Description-Content-Type: text/markdown
```

