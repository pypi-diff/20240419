# Comparing `tmp/zlsnasdisplay-1.0.0.tar.gz` & `tmp/zlsnasdisplay-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlsnasdisplay-1.0.0.tar", max compression
+gzip compressed data, was "zlsnasdisplay-1.0.1.tar", max compression
```

## Comparing `zlsnasdisplay-1.0.0.tar` & `zlsnasdisplay-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1071 2024-04-17 21:13:00.183050 zlsnasdisplay-1.0.0/LICENSE
--rw-r--r--   0        0        0     4775 2024-04-17 21:13:00.183050 zlsnasdisplay-1.0.0/README.md
--rw-r--r--   0        0        0     1365 2024-04-17 21:13:00.183050 zlsnasdisplay-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       66 2024-04-17 21:13:00.183050 zlsnasdisplay-1.0.0/zlsnasdisplay/__init__.py
--rwxr-xr-x   0        0        0      100 2024-04-17 21:13:00.187050 zlsnasdisplay-1.0.0/zlsnasdisplay/__main__.py
--rw-r--r--   0        0        0       18 2024-04-17 21:13:00.187050 zlsnasdisplay-1.0.0/zlsnasdisplay/_version.py
--rw-r--r--   0        0        0      561 2024-04-17 21:13:00.187050 zlsnasdisplay-1.0.0/zlsnasdisplay/display_controller.py
--rw-r--r--   0        0        0     9187 2024-04-17 21:13:00.187050 zlsnasdisplay-1.0.0/zlsnasdisplay/display_renderer.py
--rw-r--r--   0        0        0 11604276 2024-04-17 21:13:00.251050 zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/MaterialSymbolsRounded.ttf
--rw-r--r--   0        0        0   362552 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/Ubuntu-Light.ttf
--rw-r--r--   0        0        0   299684 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/Ubuntu-Regular.ttf
--rwxr-xr-x   0        0        0     2602 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/main.py
--rw-r--r--   0        0        0     3047 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/network_operations.py
--rw-r--r--   0        0        0        0 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/py.typed
--rw-r--r--   0        0        0     2330 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/system_operations.py
--rw-r--r--   0        0        0        0 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/__init__.py
--rw-r--r--   0        0        0    23799 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/epd2in9_V2.py
--rw-r--r--   0        0        0     8468 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/epdconfig.py
--rw-r--r--   0        0        0     5508 1970-01-01 00:00:00.000000 zlsnasdisplay-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-19 11:37:18.623481 zlsnasdisplay-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4775 2024-04-19 11:37:18.623481 zlsnasdisplay-1.0.1/README.md
+-rw-r--r--   0        0        0     1365 2024-04-19 11:37:18.623481 zlsnasdisplay-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-04-19 11:37:18.623481 zlsnasdisplay-1.0.1/zlsnasdisplay/__init__.py
+-rwxr-xr-x   0        0        0      100 2024-04-19 11:37:18.623481 zlsnasdisplay-1.0.1/zlsnasdisplay/__main__.py
+-rw-r--r--   0        0        0       18 2024-04-19 11:37:18.623481 zlsnasdisplay-1.0.1/zlsnasdisplay/_version.py
+-rw-r--r--   0        0        0      561 2024-04-19 11:37:18.623481 zlsnasdisplay-1.0.1/zlsnasdisplay/display_controller.py
+-rw-r--r--   0        0        0     9141 2024-04-19 11:37:18.623481 zlsnasdisplay-1.0.1/zlsnasdisplay/display_renderer.py
+-rw-r--r--   0        0        0 11604276 2024-04-19 11:37:18.691482 zlsnasdisplay-1.0.1/zlsnasdisplay/fonts/MaterialSymbolsRounded.ttf
+-rw-r--r--   0        0        0   362552 2024-04-19 11:37:18.695483 zlsnasdisplay-1.0.1/zlsnasdisplay/fonts/Ubuntu-Light.ttf
+-rw-r--r--   0        0        0   299684 2024-04-19 11:37:18.695483 zlsnasdisplay-1.0.1/zlsnasdisplay/fonts/Ubuntu-Regular.ttf
+-rwxr-xr-x   0        0        0     2602 2024-04-19 11:37:18.695483 zlsnasdisplay-1.0.1/zlsnasdisplay/main.py
+-rw-r--r--   0        0        0     3047 2024-04-19 11:37:18.695483 zlsnasdisplay-1.0.1/zlsnasdisplay/network_operations.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:37:18.695483 zlsnasdisplay-1.0.1/zlsnasdisplay/py.typed
+-rw-r--r--   0        0        0     2325 2024-04-19 11:37:18.695483 zlsnasdisplay-1.0.1/zlsnasdisplay/system_operations.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:37:18.695483 zlsnasdisplay-1.0.1/zlsnasdisplay/waveshare_epd/__init__.py
+-rw-r--r--   0        0        0    23799 2024-04-19 11:37:18.695483 zlsnasdisplay-1.0.1/zlsnasdisplay/waveshare_epd/epd2in9_V2.py
+-rw-r--r--   0        0        0     8468 2024-04-19 11:37:18.695483 zlsnasdisplay-1.0.1/zlsnasdisplay/waveshare_epd/epdconfig.py
+-rw-r--r--   0        0        0     5508 1970-01-01 00:00:00.000000 zlsnasdisplay-1.0.1/PKG-INFO
```

### Comparing `zlsnasdisplay-1.0.0/LICENSE` & `zlsnasdisplay-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-1.0.0/README.md` & `zlsnasdisplay-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-1.0.0/pyproject.toml` & `zlsnasdisplay-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zlsnasdisplay"
-version = "1.0.0"
+version = "1.0.1"
 description = "Eink display manager"
 authors = ["Ondrej Zalesky <o.zalesky@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/display_controller.py` & `zlsnasdisplay-1.0.1/zlsnasdisplay/display_controller.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/display_renderer.py` & `zlsnasdisplay-1.0.1/zlsnasdisplay/display_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #! /usr/bin/env python3
 
 import os
 
 from PIL import Image, ImageDraw, ImageFont
 
 from zlsnasdisplay.display_controller import DisplayController
-from zlsnasdisplay.network_operations import NetworkOperations
-from zlsnasdisplay.network_operations import TrafficMonitor
+from zlsnasdisplay.network_operations import NetworkOperations, TrafficMonitor
 from zlsnasdisplay.system_operations import SystemOperations
 
 
 class DisplayRenderer:
     def __init__(self, display_image_path, is_root):
         """Initialize the display renderer"""
         self.display_controller = DisplayController()
@@ -190,21 +189,21 @@
         self.update_display_and_save_image()
 
     def render_current_traffic(self):
         """Render current traffic"""
         self.draw.rectangle((204, 0, 296, 68), fill=255)
 
         network = TrafficMonitor().get_current_traffic()
-        self.draw.text((204, 0), f"down", font=self.font14, fill=0)
+        self.draw.text((204, 0), "down", font=self.font14, fill=0)
         self.draw.line([(242, 10), (261, 10)], fill=0, width=0)
         self.draw.text((263, 0), f"{network[1]}/s", font=self.font14, fill=0)
         self.draw.text((208, 10), "\uf090", font=self.nfont24, fill=0)  # Unicode icon download
         self.draw.text((233, 14), f"{round(network[0], 2)}", font=self.font20, fill=0)  # download
 
-        self.draw.text((204, 33), f"up", font=self.font14, fill=0)
+        self.draw.text((204, 33), "up", font=self.font14, fill=0)
         self.draw.line([(222, 43), (261, 43)], fill=0, width=0)
         self.draw.text((263, 33), f"{network[3]}/s", font=self.font14, fill=0)
         self.draw.text((208, 44), "\uf09b", font=self.nfont24, fill=0)  # Unicode icon for upload
         self.draw.text((233, 48), f"{round(network[2], 2)}", font=self.font20, fill=0)  # upload
 
         self.update_display_and_save_image()
```

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/MaterialSymbolsRounded.ttf` & `zlsnasdisplay-1.0.1/zlsnasdisplay/fonts/MaterialSymbolsRounded.ttf`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/Ubuntu-Light.ttf` & `zlsnasdisplay-1.0.1/zlsnasdisplay/fonts/Ubuntu-Light.ttf`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/Ubuntu-Regular.ttf` & `zlsnasdisplay-1.0.1/zlsnasdisplay/fonts/Ubuntu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/main.py` & `zlsnasdisplay-1.0.1/zlsnasdisplay/main.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 import logging
+import os
 import signal
 import sys
 import time
-import os
 
 import schedule
 
 from zlsnasdisplay.display_renderer import DisplayRenderer
 
 # GET ENVIRONMENT VARIABLES
 LOG_LEVEL = os.getenv("LOG_LEVEL", "INFO").upper()
@@ -52,34 +52,34 @@
 def main():
     """Main function to run the program."""
 
     signal.signal(signal.SIGINT, signal_handler)
     signal.signal(signal.SIGTERM, signal_handler)
     signal.signal(signal.SIGHUP, signal_handler)
 
+    # Render current traffic every 10 seconds
+    schedule.every(10).seconds.do(display_renderer.render_current_traffic)
+    # Render fan speed every 10 seconds
+    schedule.every(10).seconds.do(display_renderer.render_fan_speed)
     # Render CPU load every 30 seconds
     schedule.every(30).seconds.do(display_renderer.render_cpu_load)
-    # Get updates every 3 hours
-    schedule.every(3).hours.do(display_renderer.get_updates)
+    # Render current traffic every 30 seconds
+    schedule.every(30).seconds.do(display_renderer.check_net)
     # Render signal strength every minute
     schedule.every(1).minutes.do(display_renderer.render_signal_strength)
     # Render memory usage every minute
     schedule.every(1).minutes.do(display_renderer.render_mem)
     # Render NVMe stats every minute
     schedule.every(1).minutes.do(display_renderer.render_nvme_stats)
-    # Render fan speed every 10 seconds
-    schedule.every(10).seconds.do(display_renderer.render_fan_speed)
-    # Render IP address every hour
-    schedule.every(1).hours.do(display_renderer.render_ip_address)
     # Render uptime every minute
     schedule.every(1).minutes.do(display_renderer.render_uptime)
-    # Render current traffic every 10 seconds
-    schedule.every(10).seconds.do(display_renderer.render_current_traffic)
-    # Render current traffic every 30 seconds
-    schedule.every(30).seconds.do(display_renderer.check_net)
+    # Render IP address every hour
+    schedule.every(1).hours.do(display_renderer.render_ip_address)
+    # Get updates every 3 hours
+    schedule.every(3).hours.do(display_renderer.get_updates)
 
     schedule.run_all()
 
     while True:
         """ Run the scheduled tasks."""
         schedule.run_pending()
         time.sleep(1)
```

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/network_operations.py` & `zlsnasdisplay-1.0.1/zlsnasdisplay/network_operations.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/system_operations.py` & `zlsnasdisplay-1.0.1/zlsnasdisplay/system_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def get_cpu_temperature(self):
         """Get the CPU temperature in Celsius"""
         return int(self.cpu.temperature)
 
     @staticmethod
     def get_cpu_load():
         """Get the CPU load in percentage"""
-        return int(int(psutil.cpu_percent()))
+        return int(psutil.cpu_percent())
 
     @staticmethod
     def get_fan_speed():
         """Get the fan speed in RPM"""
         return psutil.sensors_fans()["pwmfan"][0].current
 
     @staticmethod
```

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/epd2in9_V2.py` & `zlsnasdisplay-1.0.1/zlsnasdisplay/waveshare_epd/epd2in9_V2.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/epdconfig.py` & `zlsnasdisplay-1.0.1/zlsnasdisplay/waveshare_epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-1.0.0/PKG-INFO` & `zlsnasdisplay-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlsnasdisplay
-Version: 1.0.0
+Version: 1.0.1
 Summary: Eink display manager
 License: MIT
 Author: Ondrej Zalesky
 Author-email: o.zalesky@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

