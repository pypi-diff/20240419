# Comparing `tmp/compal-0.5.1.tar.gz` & `tmp/compal-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compal-0.5.1.tar", last modified: Sat Feb 25 13:43:09 2023, max compression
+gzip compressed data, was "compal-0.6.0.tar", last modified: Fri Apr 19 14:40:49 2024, max compression
```

## Comparing `compal-0.5.1.tar` & `compal-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kockt      (501) staff       (20)        0 2023-02-25 13:43:09.420219 compal-0.5.1/
--rw-r--r--   0 kockt      (501) staff       (20)      119 2023-02-25 13:38:09.000000 compal-0.5.1/.flake8
--rw-r--r--   0 kockt      (501) staff       (20)      649 2023-02-25 13:38:09.000000 compal-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 kockt      (501) staff       (20)     1054 2023-02-25 13:38:09.000000 compal-0.5.1/LICENSE.txt
--rw-r--r--   0 kockt      (501) staff       (20)      544 2023-02-25 13:38:09.000000 compal-0.5.1/MANIFEST.in
--rw-r--r--   0 kockt      (501) staff       (20)     4206 2023-02-25 13:43:09.419620 compal-0.5.1/PKG-INFO
--rw-r--r--   0 kockt      (501) staff       (20)     3684 2023-02-25 13:38:09.000000 compal-0.5.1/README.md
--rw-r--r--   0 kockt      (501) staff       (20)     2365 2023-02-25 13:38:09.000000 compal-0.5.1/azure-pipelines.yml
-drwxr-xr-x   0 kockt      (501) staff       (20)        0 2023-02-25 13:43:09.408324 compal-0.5.1/compal/
--rw-r--r--   0 kockt      (501) staff       (20)    54918 2023-02-25 13:38:09.000000 compal-0.5.1/compal/__init__.py
--rwxr-xr-x   0 kockt      (501) staff       (20)     2138 2023-02-25 13:38:09.000000 compal-0.5.1/compal/functions.py
--rw-r--r--   0 kockt      (501) staff       (20)     3631 2023-02-25 13:38:09.000000 compal-0.5.1/compal/models.py
-drwxr-xr-x   0 kockt      (501) staff       (20)        0 2023-02-25 13:43:09.413746 compal-0.5.1/compal.egg-info/
--rw-r--r--   0 kockt      (501) staff       (20)     4206 2023-02-25 13:43:09.000000 compal-0.5.1/compal.egg-info/PKG-INFO
--rw-r--r--   0 kockt      (501) staff       (20)      504 2023-02-25 13:43:09.000000 compal-0.5.1/compal.egg-info/SOURCES.txt
--rw-r--r--   0 kockt      (501) staff       (20)        1 2023-02-25 13:43:09.000000 compal-0.5.1/compal.egg-info/dependency_links.txt
--rw-r--r--   0 kockt      (501) staff       (20)       14 2023-02-25 13:43:09.000000 compal-0.5.1/compal.egg-info/requires.txt
--rw-r--r--   0 kockt      (501) staff       (20)        7 2023-02-25 13:43:09.000000 compal-0.5.1/compal.egg-info/top_level.txt
-drwxr-xr-x   0 kockt      (501) staff       (20)        0 2023-02-25 13:43:09.414466 compal-0.5.1/docs/
--rw-r--r--   0 kockt      (501) staff       (20)    15349 2023-02-25 13:38:09.000000 compal-0.5.1/docs/notes.md
-drwxr-xr-x   0 kockt      (501) staff       (20)        0 2023-02-25 13:43:09.417259 compal-0.5.1/examples/
--rw-r--r--   0 kockt      (501) staff       (20)        0 2023-02-25 13:38:09.000000 compal-0.5.1/examples/__init__.py
--rw-r--r--   0 kockt      (501) staff       (20)     1480 2023-02-25 13:38:09.000000 compal-0.5.1/examples/guest_fun.py
--rw-r--r--   0 kockt      (501) staff       (20)     2977 2023-02-25 13:38:09.000000 compal-0.5.1/examples/modem_setup.py
--rw-r--r--   0 kockt      (501) staff       (20)     1895 2023-02-25 13:38:09.000000 compal-0.5.1/examples/wifi_fun.py
--rw-r--r--   0 kockt      (501) staff       (20)     1180 2023-02-25 13:38:09.000000 compal-0.5.1/pylintrc
--rw-r--r--   0 kockt      (501) staff       (20)       29 2023-02-25 13:38:09.000000 compal-0.5.1/pytest.ini
--rw-r--r--   0 kockt      (501) staff       (20)       38 2023-02-25 13:43:09.420429 compal-0.5.1/setup.cfg
--rw-r--r--   0 kockt      (501) staff       (20)      994 2023-02-25 13:40:07.000000 compal-0.5.1/setup.py
-drwxr-xr-x   0 kockt      (501) staff       (20)        0 2023-02-25 13:43:09.418705 compal-0.5.1/tests/
--rw-r--r--   0 kockt      (501) staff       (20)      509 2023-02-25 13:38:09.000000 compal-0.5.1/tests/test_function_ids_are_unique.py
--rw-r--r--   0 kockt      (501) staff       (20)      702 2023-02-25 13:38:09.000000 compal-0.5.1/tests/test_login_response_parsing.py
--rw-r--r--   0 kockt      (501) staff       (20)      818 2023-02-25 13:38:09.000000 compal-0.5.1/tox.ini
+drwxr-xr-x   0 kockt      (501) staff       (20)        0 2024-04-19 14:40:49.514866 compal-0.6.0/
+-rw-r--r--   0 kockt      (501) staff       (20)      119 2023-02-25 13:38:09.000000 compal-0.6.0/.flake8
+-rw-r--r--   0 kockt      (501) staff       (20)      649 2023-02-25 13:38:09.000000 compal-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 kockt      (501) staff       (20)     1054 2023-02-25 13:38:09.000000 compal-0.6.0/LICENSE.txt
+-rw-r--r--   0 kockt      (501) staff       (20)      544 2023-02-25 13:38:09.000000 compal-0.6.0/MANIFEST.in
+-rw-r--r--   0 kockt      (501) staff       (20)     4564 2024-04-19 14:40:49.513450 compal-0.6.0/PKG-INFO
+-rw-r--r--   0 kockt      (501) staff       (20)     3998 2024-04-19 14:40:18.000000 compal-0.6.0/README.md
+-rw-r--r--   0 kockt      (501) staff       (20)     2365 2023-02-25 13:38:09.000000 compal-0.6.0/azure-pipelines.yml
+drwxr-xr-x   0 kockt      (501) staff       (20)        0 2024-04-19 14:40:49.502869 compal-0.6.0/compal/
+-rw-r--r--   0 kockt      (501) staff       (20)    55811 2024-04-19 14:33:22.000000 compal-0.6.0/compal/__init__.py
+-rwxr-xr-x   0 kockt      (501) staff       (20)     2138 2023-02-25 13:38:09.000000 compal-0.6.0/compal/functions.py
+-rw-r--r--   0 kockt      (501) staff       (20)     3632 2024-04-19 14:33:22.000000 compal-0.6.0/compal/models.py
+drwxr-xr-x   0 kockt      (501) staff       (20)        0 2024-04-19 14:40:49.512336 compal-0.6.0/compal.egg-info/
+-rw-r--r--   0 kockt      (501) staff       (20)     4564 2024-04-19 14:40:49.000000 compal-0.6.0/compal.egg-info/PKG-INFO
+-rw-r--r--   0 kockt      (501) staff       (20)      504 2024-04-19 14:40:49.000000 compal-0.6.0/compal.egg-info/SOURCES.txt
+-rw-r--r--   0 kockt      (501) staff       (20)        1 2024-04-19 14:40:49.000000 compal-0.6.0/compal.egg-info/dependency_links.txt
+-rw-r--r--   0 kockt      (501) staff       (20)       14 2024-04-19 14:40:49.000000 compal-0.6.0/compal.egg-info/requires.txt
+-rw-r--r--   0 kockt      (501) staff       (20)        7 2024-04-19 14:40:49.000000 compal-0.6.0/compal.egg-info/top_level.txt
+drwxr-xr-x   0 kockt      (501) staff       (20)        0 2024-04-19 14:40:49.507033 compal-0.6.0/docs/
+-rw-r--r--   0 kockt      (501) staff       (20)    15349 2023-02-25 13:38:09.000000 compal-0.6.0/docs/notes.md
+drwxr-xr-x   0 kockt      (501) staff       (20)        0 2024-04-19 14:40:49.509777 compal-0.6.0/examples/
+-rw-r--r--   0 kockt      (501) staff       (20)        0 2023-02-25 13:38:09.000000 compal-0.6.0/examples/__init__.py
+-rw-r--r--   0 kockt      (501) staff       (20)     1480 2023-02-25 13:38:09.000000 compal-0.6.0/examples/guest_fun.py
+-rw-r--r--   0 kockt      (501) staff       (20)     2977 2023-02-25 13:38:09.000000 compal-0.6.0/examples/modem_setup.py
+-rw-r--r--   0 kockt      (501) staff       (20)     1895 2023-02-25 13:38:09.000000 compal-0.6.0/examples/wifi_fun.py
+-rw-r--r--   0 kockt      (501) staff       (20)     1180 2023-02-25 13:38:09.000000 compal-0.6.0/pylintrc
+-rw-r--r--   0 kockt      (501) staff       (20)       29 2023-02-25 13:38:09.000000 compal-0.6.0/pytest.ini
+-rw-r--r--   0 kockt      (501) staff       (20)       38 2024-04-19 14:40:49.515168 compal-0.6.0/setup.cfg
+-rw-r--r--   0 kockt      (501) staff       (20)      995 2024-04-19 14:40:18.000000 compal-0.6.0/setup.py
+drwxr-xr-x   0 kockt      (501) staff       (20)        0 2024-04-19 14:40:49.511448 compal-0.6.0/tests/
+-rw-r--r--   0 kockt      (501) staff       (20)      509 2023-02-25 13:38:09.000000 compal-0.6.0/tests/test_function_ids_are_unique.py
+-rw-r--r--   0 kockt      (501) staff       (20)      702 2023-02-25 13:38:09.000000 compal-0.6.0/tests/test_login_response_parsing.py
+-rw-r--r--   0 kockt      (501) staff       (20)      818 2023-02-25 13:38:09.000000 compal-0.6.0/tox.ini
```

### Comparing `compal-0.5.1/.pre-commit-config.yaml` & `compal-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/LICENSE.txt` & `compal-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/MANIFEST.in` & `compal-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/PKG-INFO` & `compal-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: compal
-Version: 0.5.1
+Version: 0.6.0
 Summary: Compal CH7465LG/Ziggo Connect Box client
 Home-page: https://github.com/ties/compal_CH7465LG_py
 Author: Ties de Kock
 Author-email: ties@tiesdekock.nl
 License: MIT
 Keywords: compal CH7465LG connect box cablemodem
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: lxml
 
 Compal CH7465LG (Ziggo Connect Box) tools
 =============================================
 
 This repository contains a simple api to wrap the web interface of the Ziggo Connect Box (i.e. the
 Compal CH7465LG). It is implemented in **Python >= 3.7**.
 
@@ -43,14 +45,17 @@
 [0]: https://fccid.io/UIDTG2492
 [1]: https://www.dslreports.com/forum/r31079834-ALL-SB6190-is-a-terrible-modem-Intel-Puma-6-MaxLinear-mistake
 [2]: https://blog.danman.eu/about-adding-a-static-route-to-my-docsis-modem/
 
 Changelog
 ---------
 
+### 0.6.0
+  * Support for static DHCP leases was added by @do3cc
+
 ### 0.5.1
   * Support for hashed (single-sha256) passwords was added by @7FM
 
 ### 0.5.0
   * Added support for get/create/disable/delete IPv6 filter rules by @7FM
 
 ### 0.4.0:
@@ -112,15 +117,23 @@
 print(settings)
 
 new_settings = settings._replace(radio_2g=settings.radio_2g._replace(ssid='api_works'))
 wifi.update_wifi_settings(new_settings)
 
 print(wifi.wifi_settings)
 
-# And/or DHCPSettings
+# And/or Make all dhcp adresses static:
+
+dhcp = DHCPSettings(modem)
+lan_table = LanTable(modem)
+for client in (*lan_table.get_lan(), *lan_table.get_wifi()):
+    dhcp.add_static_lease(
+        lease_ip=client["IPv4Addr"].split("/")[0], lease_mac=client["MACAddr"]
+    )
+
 
 # If you want to go back to 'normal':
 # modem.reboot() # or
 # modem.factory_reset()
 
 # And logout
 modem.logout()
```

### Comparing `compal-0.5.1/README.md` & `compal-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 [0]: https://fccid.io/UIDTG2492
 [1]: https://www.dslreports.com/forum/r31079834-ALL-SB6190-is-a-terrible-modem-Intel-Puma-6-MaxLinear-mistake
 [2]: https://blog.danman.eu/about-adding-a-static-route-to-my-docsis-modem/
 
 Changelog
 ---------
 
+### 0.6.0
+  * Support for static DHCP leases was added by @do3cc
+
 ### 0.5.1
   * Support for hashed (single-sha256) passwords was added by @7FM
 
 ### 0.5.0
   * Added support for get/create/disable/delete IPv6 filter rules by @7FM
 
 ### 0.4.0:
@@ -96,15 +99,23 @@
 print(settings)
 
 new_settings = settings._replace(radio_2g=settings.radio_2g._replace(ssid='api_works'))
 wifi.update_wifi_settings(new_settings)
 
 print(wifi.wifi_settings)
 
-# And/or DHCPSettings
+# And/or Make all dhcp adresses static:
+
+dhcp = DHCPSettings(modem)
+lan_table = LanTable(modem)
+for client in (*lan_table.get_lan(), *lan_table.get_wifi()):
+    dhcp.add_static_lease(
+        lease_ip=client["IPv4Addr"].split("/")[0], lease_mac=client["MACAddr"]
+    )
+
 
 # If you want to go back to 'normal':
 # modem.reboot() # or
 # modem.factory_reset()
 
 # And logout
 modem.logout()
```

### Comparing `compal-0.5.1/azure-pipelines.yml` & `compal-0.6.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/compal/__init__.py` & `compal-0.6.0/compal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 """
 Client for the Compal CH7465LG/Ziggo Connect box cable modem
 """
+
 import inspect
 import io
 import itertools
 import logging
 import re
 import time
 import urllib
 from collections import OrderedDict
 from datetime import timedelta
 from enum import Enum
-from xml.dom import minidom
 from hashlib import sha256
+from xml.dom import minidom
 
 import requests
 from lxml import etree
 
 from .functions import GetFunction, SetFunction
 from .models import (
     BandSetting,
     FilterAction,
     FilterIpRange,
     GuestNetworkEnabling,
     GuestNetworkProperties,
     GuestNetworkSettings,
-    NatMode,
     IPv6FilterRule,
     IPv6FilterRuleProto,
+    NatMode,
     PortForward,
     Proto,
     RadioSettings,
     RuleDir,
     SystemInfo,
     TimerMode,
 )
@@ -677,27 +678,31 @@
                 ("del", ""),
                 ("idd", ""),
                 (
                     "sIpRange",
                     int(
                         FilterIpRange.all
                         if src_addr == "::"
-                        else FilterIpRange.range
-                        if src_prefix != 128
-                        else FilterIpRange.single
+                        else (
+                            FilterIpRange.range
+                            if src_prefix != 128
+                            else FilterIpRange.single
+                        )
                     ),
                 ),
                 (
                     "dsIpRange",
                     int(
                         FilterIpRange.all
                         if dst_addr == "::"
-                        else FilterIpRange.range
-                        if dst_prefix != 128
-                        else FilterIpRange.single
+                        else (
+                            FilterIpRange.range
+                            if dst_prefix != 128
+                            else FilterIpRange.single
+                        )
                     ),
                 ),
                 ("PortRange", "2"),  # manual port selection
                 (
                     "TMode",
                     "0",
                 ),  # No timed rule
@@ -1279,24 +1284,46 @@
 class DHCPSettings:
     """
     Confgure the DHCP settings
     """
 
     def __init__(self, modem):
         self.modem = modem
+        self.parser = etree.XMLParser(recover=True)
 
     def add_static_lease(self, lease_ip, lease_mac):
         """
         Add a static DHCP lease
         """
         return self.modem.xml_setter(
             SetFunction.STATIC_DHCP_LEASE,
             {"data": "ADD,{ip},{mac};".format(ip=lease_ip, mac=lease_mac)},
         )
 
+    def del_static_lease(self, lease_ip, lease_mac):
+        """
+        Delete a static DHCP lease
+        """
+        return self.modem.xml_setter(
+            SetFunction.STATIC_DHCP_LEASE,
+            {"data": "DEL,{ip},{mac};".format(ip=lease_ip, mac=lease_mac)},
+        )
+
+    def get_static_leases(self):
+        """
+        Get all static leases
+        """
+        xml_content = self.modem.xml_getter(GetFunction.BASICDHCP, {}).content
+        tree = etree.fromstring(xml_content, parser=self.parser)
+        for host in tree.findall("ReserveIpadrr"):
+            yield {
+                "lease_ip": host.find("LeasedIP").text,
+                "lease_mac": host.find("MacAddress").text,
+            }
+
     def set_upnp_status(self, enabled):
         """
         Ensure that UPnP is set to the given value
         """
         return self.modem.xml_setter(
             SetFunction.UPNP_STATUS,
             OrderedDict(
```

### Comparing `compal-0.5.1/compal/functions.py` & `compal-0.6.0/compal/functions.py`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/compal/models.py` & `compal-0.6.0/compal/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Objects used by CH7465LG"""
+
 from dataclasses import dataclass
 from enum import IntEnum
-from typing import Optional, List
+from typing import List, Optional
 
 
 @dataclass
 class SystemInfo:
     docsis_mode: Optional[str] = None
     hardware_version: Optional[str] = None
     mac_address: Optional[str] = None
```

### Comparing `compal-0.5.1/compal.egg-info/PKG-INFO` & `compal-0.6.0/compal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: compal
-Version: 0.5.1
+Version: 0.6.0
 Summary: Compal CH7465LG/Ziggo Connect Box client
 Home-page: https://github.com/ties/compal_CH7465LG_py
 Author: Ties de Kock
 Author-email: ties@tiesdekock.nl
 License: MIT
 Keywords: compal CH7465LG connect box cablemodem
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: lxml
 
 Compal CH7465LG (Ziggo Connect Box) tools
 =============================================
 
 This repository contains a simple api to wrap the web interface of the Ziggo Connect Box (i.e. the
 Compal CH7465LG). It is implemented in **Python >= 3.7**.
 
@@ -43,14 +45,17 @@
 [0]: https://fccid.io/UIDTG2492
 [1]: https://www.dslreports.com/forum/r31079834-ALL-SB6190-is-a-terrible-modem-Intel-Puma-6-MaxLinear-mistake
 [2]: https://blog.danman.eu/about-adding-a-static-route-to-my-docsis-modem/
 
 Changelog
 ---------
 
+### 0.6.0
+  * Support for static DHCP leases was added by @do3cc
+
 ### 0.5.1
   * Support for hashed (single-sha256) passwords was added by @7FM
 
 ### 0.5.0
   * Added support for get/create/disable/delete IPv6 filter rules by @7FM
 
 ### 0.4.0:
@@ -112,15 +117,23 @@
 print(settings)
 
 new_settings = settings._replace(radio_2g=settings.radio_2g._replace(ssid='api_works'))
 wifi.update_wifi_settings(new_settings)
 
 print(wifi.wifi_settings)
 
-# And/or DHCPSettings
+# And/or Make all dhcp adresses static:
+
+dhcp = DHCPSettings(modem)
+lan_table = LanTable(modem)
+for client in (*lan_table.get_lan(), *lan_table.get_wifi()):
+    dhcp.add_static_lease(
+        lease_ip=client["IPv4Addr"].split("/")[0], lease_mac=client["MACAddr"]
+    )
+
 
 # If you want to go back to 'normal':
 # modem.reboot() # or
 # modem.factory_reset()
 
 # And logout
 modem.logout()
```

### Comparing `compal-0.5.1/docs/notes.md` & `compal-0.6.0/docs/notes.md`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/examples/guest_fun.py` & `compal-0.6.0/examples/guest_fun.py`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/examples/modem_setup.py` & `compal-0.6.0/examples/modem_setup.py`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/examples/wifi_fun.py` & `compal-0.6.0/examples/wifi_fun.py`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/pylintrc` & `compal-0.6.0/pylintrc`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/setup.py` & `compal-0.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """ Set up script """
+
 import os
 
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 with open(os.path.join(here, "README.md"), "rb") as f:
     long_descr = f.read().decode("utf-8")
 
 
 setup(
     name="compal",
-    version="0.5.1",
+    version="0.6.0",
     author="Ties de Kock",
     author_email="ties@tiesdekock.nl",
     description="Compal CH7465LG/Ziggo Connect Box client",
     long_description_content_type="text/markdown",
     long_description=long_descr,
     url="https://github.com/ties/compal_CH7465LG_py",
     entry_points={},
```

### Comparing `compal-0.5.1/tests/test_login_response_parsing.py` & `compal-0.6.0/tests/test_login_response_parsing.py`

 * *Files identical despite different names*

### Comparing `compal-0.5.1/tox.ini` & `compal-0.6.0/tox.ini`

 * *Files identical despite different names*

