# Comparing `tmp/bdmc-0.1.1.tar.gz` & `tmp/bdmc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.1.tar", last modified: Thu Apr 18 10:14:00 2024, max compression
+gzip compressed data, was "bdmc-0.1.2.tar", last modified: Fri Apr 19 15:42:42 2024, max compression
```

## Comparing `bdmc-0.1.1.tar` & `bdmc-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3857 2024-04-18 10:13:39.436645 bdmc-0.1.1/README.md
--rw-r--r--   0        0        0      545 2024-04-18 10:14:00.025063 bdmc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      526 2024-04-18 10:13:39.436645 bdmc-0.1.1/src/bdmc/__init__.py
--rw-r--r--   0        0        0      133 2024-04-18 10:13:39.436645 bdmc-0.1.1/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0     5789 2024-04-18 10:13:39.436645 bdmc-0.1.1/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2257 2024-04-18 10:13:39.436645 bdmc-0.1.1/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-04-18 10:13:39.436645 bdmc-0.1.1/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-04-18 10:13:39.436645 bdmc-0.1.1/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7404 2024-04-18 10:13:39.436645 bdmc-0.1.1/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0       64 2024-04-18 10:13:39.436645 bdmc-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1357 2024-04-18 10:13:39.436645 bdmc-0.1.1/tests/tests.py
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 bdmc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5296 2024-04-19 15:42:23.082585 bdmc-0.1.2/README.md
+-rw-r--r--   0        0        0      545 2024-04-19 15:42:42.478595 bdmc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      526 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      133 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0     8896 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7404 2024-04-19 15:42:23.082585 bdmc-0.1.2/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0       64 2024-04-19 15:42:23.082585 bdmc-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1983 2024-04-19 15:42:23.082585 bdmc-0.1.2/tests/tests.py
+-rw-r--r--   0        0        0     5610 1970-01-01 00:00:00.000000 bdmc-0.1.2/PKG-INFO
```

### Comparing `bdmc-0.1.1/README.md` & `bdmc-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -49,37 +49,75 @@
 # Supports chain calls
 # In this case, these 3 cmds will be sent to the motors at almost the same time, only the [0]*4 will take effect as a result
 (con
  .set_motors_speed([100, 200, 300, 400])
  .set_motors_speed([1000] * 4)  # move all 4 motors with the speed of 1000
  .set_motors_speed([0] * 4))
 
-# Chain call with a delay
+# Chain call with delay
 # In this case, these 3 cmds will be sent to motors with the specified interval
 (con
  .set_motors_speed([100, 200, 300, 400])
  .delay(1.2)  # delay 1.2 sec
  .set_motors_speed([1000] * 4)
  .delay(3)  # delay 3.0 sec
  .set_motors_speed([0] * 4))
 
-# Chain call with a delay_b
+# Chain call with delay_b
 # In this case, these 3 cmds will be sent to motors with specified interval,but with a break checker
 # NOTE1: you can't set check_interval bigger than delay_sec
 from random import random
 
 (con
  .set_motors_speed([100, 200, 300, 400])
  .delay_b(delay_sec=1.2, breaker=lambda: random() > 0.8,
           check_interval=0.01)  # delay 1.2 sec, will skip the 1.2 sec on the breaker returns True, execute the checker every 0.01 sec
  .set_motors_speed([1000] * 4)
  .delay_b(3, breaker=lambda: random() > 0.5,
           check_interval=0.02)  # delay 3.0 sec, will skip the 1.2 sec on the breaker returns True, execute the checker every 0.02 sec
  .set_motors_speed([0] * 4))
 
+# Branched chain call with delay_b_match
+# In this case, a switch-case branch has been enforced.
+# Once the breaker returns a True during the 1.2 sec delay, a FULL_STOP cmd will be sent.
+# if the breaker never return a True, then the 1.2sec delay will be fully waited and the [500]*4 cmd will be sent.
+
+# NOTE1: delay_b_match has same delay logic as delay_b, the only difference is the return value:
+# delay_b       returns Self
+# delay_b_match returns breaker()
+
+
+match (con
+       .set_motors_speed([100] * 4)
+       .delay_b_match(1.2, breaker=lambda: random() > 0.8)):
+    case True:
+        con.send_cmd(CMD.FULL_STOP)
+    case False:
+        con.set_motors_speed([500] * 4)
+    case _:
+        raise ValueError("should never be here")
+
+# A more complex usage of delay_b_match
+# Note
+from random import choice
+
+match (con
+       .set_motors_speed([100] * 4)
+       .delay_b_match(1.2, breaker=lambda: choice([0, 0, 1, 2, 3]), check_interval=0.1)):
+    case 1:
+        con.send_cmd(CMD.FULL_STOP)  # Switch to this case once the breaker returns 1
+    case 2:
+        con.set_motors_speed([666] * 4)  # Switch to this case once the breaker returns 2
+    case 3:
+        con.set_motors_speed([777] * 4)  # Switch to this case once the breaker returns 3
+    case 0:
+        con.set_motors_speed([555] * 4)  # Switch to this case if the breaker has never returned a non-zero value
+    case _:
+        raise ValueError("should never be here")
+
 
 ```
 
 use `set_log_level` to silent the console, this should improve the performance in high pressure conditions
 
 ```python
 from bdmc import set_log_level
```

### Comparing `bdmc-0.1.1/pyproject.toml` & `bdmc-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.1"
+version = "0.1.2"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.1/src/bdmc/__init__.py` & `bdmc-0.1.2/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.1/src/bdmc/modules/debug.py` & `bdmc-0.1.2/src/bdmc/modules/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,9 +65,9 @@
 
         for i in range(speed_level):
             speed = i * 1000
             print(f"doing {speed}")
             con.set_motors_speed([speed] * motors)
             time.sleep(interval)
 
-    con.set_motors_speed([0])
+    con.set_motors_speed([0] * motors)
     print("over")
```

### Comparing `bdmc-0.1.1/src/bdmc/modules/logger.py` & `bdmc-0.1.2/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.1/src/bdmc/modules/port.py` & `bdmc-0.1.2/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.1/src/bdmc/modules/seriald.py` & `bdmc-0.1.2/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.1/tests/tests.py` & `bdmc-0.1.2/tests/tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+import time
 import unittest
 
 from viztracer import VizTracer
 
 from bdmc import set_log_level
 from bdmc.modules.controller import MotorInfo, CloseLoopController
 from bdmc.modules.debug import motor_speed_test
@@ -14,15 +15,15 @@
 class MyTestCase(unittest.TestCase):
     def setUp(self):
         self.test_port = "COM3"
         self.tracer = VizTracer()
 
     def test_send(self):
         set_log_level(10)
-        m = [MotorInfo(code_sign=1, direction=-1)]
+        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
         self.tracer.start()
         motor_speed_test(port=self.test_port, motor_infos=m, interval=0.01)
         self.tracer.stop()
         self.tracer.save(output_file=(VIZ_OUTPUT_DIR / "test_send.json").as_posix())
 
     def test_unique_motor_check(self):
         m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=1, direction=-1)]
@@ -33,10 +34,23 @@
     def test_cmds_align(self):
         m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
         con = CloseLoopController(port=self.test_port, motor_infos=m)
         con.set_motors_speed([1000, 2000])
         with self.assertRaises(ValueError):
             con.set_motors_speed([100] * 3)
 
+    def test_delays(self):
+        m = [MotorInfo(code_sign=1, direction=-1), MotorInfo(code_sign=2, direction=-1)]
+        con = CloseLoopController(port=self.test_port, motor_infos=m)
+        start = time.time()
+        con.delay(1)
+        self.assertAlmostEqual(start + 1, time.time(), delta=0.02)
+        start = time.time()
+        con.delay_b(1, lambda: False)
+        self.assertAlmostEqual(start + 1, time.time(), delta=0.02)
+        start = time.time()
+        print(con.delay_b(1, lambda: False))
+        self.assertAlmostEqual(start + 1, time.time(), delta=0.02)
+
 
 if __name__ == "__main__":
     pass
```

