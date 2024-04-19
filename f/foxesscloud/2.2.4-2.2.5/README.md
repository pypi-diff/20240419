# Comparing `tmp/foxesscloud-2.2.4.tar.gz` & `tmp/foxesscloud-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-i2tqbp31\foxesscloud-2.2.4.tar", last modified: Wed Apr 17 10:07:31 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-7nf_8d0n\foxesscloud-2.2.5.tar", last modified: Fri Apr 19 13:59:24 2024, max compression
```

## Comparing `foxesscloud-2.2.4.tar` & `foxesscloud-2.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.4/LICENCE
--rw-rw-rw-   0        0        0    39688 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    39133 2024-04-17 10:00:06.000000 foxesscloud-2.2.4/README.md
--rw-rw-rw-   0        0        0      635 2024-04-17 09:50:25.000000 foxesscloud-2.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud/
--rw-rw-rw-   0        0        0   175961 2024-04-17 10:05:41.000000 foxesscloud-2.2.4/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   170165 2024-04-17 10:05:34.000000 foxesscloud-2.2.4/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    39688 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 10:07:31.000000 foxesscloud-2.2.4/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.5/LICENCE
+-rw-rw-rw-   0        0        0    39749 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    39194 2024-04-19 13:43:40.000000 foxesscloud-2.2.5/README.md
+-rw-rw-rw-   0        0        0      635 2024-04-17 17:44:34.000000 foxesscloud-2.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud/
+-rw-rw-rw-   0        0        0   174707 2024-04-19 13:41:14.000000 foxesscloud-2.2.5/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   168871 2024-04-19 13:41:14.000000 foxesscloud-2.2.5/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    39749 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-19 13:59:24.000000 foxesscloud-2.2.5/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.2.4/LICENCE` & `foxesscloud-2.2.5/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.2.4/PKG-INFO` & `foxesscloud-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.4
+Version: 2.2.5
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -666,15 +666,17 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.4<br>
+2.2.5<br>
+Refactor debug messaging.
+Simplify charge_needed() output.
 Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
 Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.4 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.5 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -458,21 +458,22 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.4
-Added 'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
-temperatures when API returns 0 instead of -50 where there is no battery Fix
-key error when accessing cell volts and temps using an agent / installer
-account. Ensure output is generated if get_battery() fails using battery_info
-(). Update f.avg() to include calculation of averages in lists containng None
-values. Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.5
+Refactor debug messaging. Simplify charge_needed() output. Added 'target_soc'
+to charge_needed() settings Fix bat_info() giving incorrect temperatures when
+API returns 0 instead of -50 where there is no battery Fix key error when
+accessing cell volts and temps using an agent / installer account. Ensure
+output is generated if get_battery() fails using battery_info(). Update f.avg()
+to include calculation of averages in lists containng None values. Added
+'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.4/README.md` & `foxesscloud-2.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -652,15 +652,17 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.4<br>
+2.2.5<br>
+Refactor debug messaging.
+Simplify charge_needed() output.
 Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
 Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
```

#### html2text {}

```diff
@@ -451,21 +451,22 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.4
-Added 'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
-temperatures when API returns 0 instead of -50 where there is no battery Fix
-key error when accessing cell volts and temps using an agent / installer
-account. Ensure output is generated if get_battery() fails using battery_info
-(). Update f.avg() to include calculation of averages in lists containng None
-values. Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.5
+Refactor debug messaging. Simplify charge_needed() output. Added 'target_soc'
+to charge_needed() settings Fix bat_info() giving incorrect temperatures when
+API returns 0 instead of -50 where there is no battery Fix key error when
+accessing cell volts and temps using an agent / installer account. Ensure
+output is generated if get_battery() fails using battery_info(). Update f.avg()
+to include calculation of averages in lists containng None values. Added
+'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.4/pyproject.toml` & `foxesscloud-2.2.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.2.4"
+version = "2.2.5"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.2.4/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.2.5/src/foxesscloud/foxesscloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud
-Updated:  17 April 2024
+Updated:  19 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.3.6"
+version = "1.3.7"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -116,33 +116,31 @@
     headers['Token'] = token
     headers['Lang'] = lang
     headers['User-Agent'] = token_store['user_agent']
     headers['Timezone'] = token_store['time_zone']
     headers['Timestamp'] = timestamp
     headers['Content-Type'] = 'application/json;charset=UTF-8'
     headers['Signature'] = hashlib.md5(fr"{path}\r\n{headers['Token']}\r\n{headers['Lang']}\r\n{headers['Timestamp']}".encode('UTF-8')).hexdigest() + '.' + token_store['client_id']
-    if debug_setting > 2:
-        output(f"path = {path}")
-        output(f"headers = {headers}")
+    output(f"path = {path}", 3)
+    output(f"headers = {headers}", 3)
     return headers
 
 def signed_get(path, params = None, login = 0):
     global fox_domain, http_timeout, http_tries, response_time
     message = None
     for i in range(0, http_tries):
         headers = signed_header(path, login)
         try:
             t_now = time.time()
             response = requests.get(url=fox_domain + path, headers=headers, params=params, timeout=http_timeout)
             response_time[path] = time.time() - t_now
             return response
         except Exception as e:
             message = str(e)
-            if debug_setting > 0:
-                output(f"** signed_get(): {message}\n  path = {path}\n  headers = {headers}")
+            output(f"** signed_get(): {message}\n  path = {path}\n  headers = {headers}")
             continue
     return MockResponse(999, message)
 
 def signed_post(path, data = None, login = 0):
     global fox_domain, http_timeout, http_tries, response_time
     message = None
     for i in range(0, http_tries):
@@ -150,31 +148,29 @@
         try:
             t_now = time.time()
             response = requests.post(url=fox_domain + path, headers=headers, data=json.dumps(data), timeout=http_timeout)
             response_time[path] = time.time() - t_now
             return response
         except Exception as e:
             message = str(e)
-            if debug_setting > 0:
-                output(f"** signed_post(): {message}\n  path = {path}\n  headers = {headers}")
+            output(f"** signed_post(): {message}\n  path = {path}\n  headers = {headers}")
             continue
     return MockResponse(999, message)
 
 
 ##################################################################################################
 # get error messages
 ##################################################################################################
 
 messages = None
 user_agent = None
 
 def get_messages():
     global debug_setting, messages, fox_user_agent
-    if debug_setting > 1:
-        output(f"getting messages")
+    output(f"getting messages", 2)
     headers = {'User-Agent': fox_user_agent, 'Content-Type': 'application/json;charset=UTF-8', 'Connection': 'keep-alive'}
     response = signed_get(path="/c/v0/errors/message", login=1)
     if response.status_code != 200:
         output(f"** get_messages() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -219,19 +215,17 @@
         if token_store.get('client_id') is None:
             token_store['client_id'] = fox_client_id
     if messages is None:
         get_messages()
     time_now = datetime.now()
     if token_store.get('token') is not None and token_store['valid_from'] is not None:
         if time_now < datetime.fromisoformat(token_store['valid_from']) + timedelta(seconds=token_store['valid_for']):
-            if debug_setting > 2:
-                output(f"token is still valid")
+            output(f"token is still valid", 3)
             return token_store['token']
-    if debug_setting > 1:
-        output(f"loading new token")
+    output(f"loading new token", 2)
     device_list = None
     device = None
     if username is None or password is None or username == 'my.fox_username' or password == 'my.fox_password':
         output(f"** please configure your Fox ESS Cloud username and password")
         return None
     credentials = {'user': username, 'password': hashlib.md5(password.encode()).hexdigest()}
     response = signed_post(path="/c/v0/user/login", data=credentials, login=1)
@@ -259,16 +253,15 @@
 
 info = None
 
 def get_info():
     global token, debug_setting, info, messages
     if get_token() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting access")
+    output(f"getting access", 2)
     response = signed_get(path="/c/v0/user/info")
     if response.status_code != 200:
         output(f"** get_info() got info response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
         errno = response.json().get('errno')
@@ -292,16 +285,15 @@
 
 status = None
 
 def get_status(station=0):
     global token, debug_setting, info, messages, status
     if get_token() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting status")
+    output(f"getting status", 2)
     path = "/c/v0/device/status/all" if station == 0 else "/c/v0/plant/status/all"
     response = signed_get(path=path)
     if response.status_code != 200:
         output(f"** get_status() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -323,16 +315,15 @@
 
 def get_site(name=None):
     global token, site_list, site, debug_setting, messages, station_id
     if get_token() is None:
         return None
     if site is not None and name is None:
         return site
-    if debug_setting > 1:
-        output(f"getting sites")
+    output(f"getting sites", 2)
     site = None
     station_id = None
     query = {'pageSize': 10, 'currentPage': 1, 'total': 0, 'condition': {'status': 0, 'contentType': 2, 'content': ''} }
     response = signed_post(path="/c/v1/plant/list", data=query)
     if response.status_code != 200:
         output(f"** get_sites() got response code {response.status_code}: {response.reason}")
         return None
@@ -373,16 +364,15 @@
 
 def get_logger(sn=None):
     global token, logger_list, logger, debug_setting, messages
     if get_token() is None:
         return None
     if logger is not None and sn is None:
         return logger
-    if debug_setting > 1:
-        output(f"getting loggers")
+    output(f"getting loggers", 2)
     query = {'pageSize': 100, 'currentPage': 1, 'total': 0, 'condition': {'communication': 0, 'moduleSN': '', 'moduleType': ''} }
     response = signed_post(path="/c/v0/module/list", data=query)
     if response.status_code != 200:
         output(f"** get_logger() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -427,16 +417,15 @@
     if get_token() is None:
         return None
     if device is not None:
         if sn is None:
             return device
         if device_sn[:len(sn)].upper() == sn.upper():
             return device
-    if debug_setting > 1:
-        output(f"getting device")
+    output(f"getting device", 2)
     if sn is None and device_sn is not None and len(device_sn) == 15:
         sn = device_sn
     # get device list
     query = {'pageSize': 100, 'currentPage': 1, 'total': 0, 'condition': {'queryDate': {'begin': 0, 'end':0}}}
     response = signed_post(path="/c/v0/device/list", data=query)
     if response.status_code != 200:
         output(f"** get_device() get device list, got response code {response.status_code}: {response.reason}")
@@ -514,16 +503,15 @@
 # get list of raw_data variables for selected device
 ##################################################################################################
 
 def get_vars():
     global token, device_id, debug_setting, messages
     if get_device() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting variables")
+    output(f"getting variables", 2)
     params = {'deviceID': device_id}
     # v1 api required for full list with {name, variable, unit}
     response = signed_get(path="/c/v1/device/variables", params=params)
     if response.status_code != 200:
         output(f"** get_vars() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
@@ -543,16 +531,15 @@
 
 firmware = None
 
 def get_firmware():
     global token, device_id, firmware, debug_setting, messages
     if get_device() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting firmware")
+    output(f"getting firmware", 2)
     params = {'deviceID': device_id}
     response = signed_get(path="/c/v0/device/addressbook", params=params)
     if response.status_code != 200:
         output(f"** get_firmware() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -572,16 +559,15 @@
 battery = None
 battery_settings = None
 
 def get_battery():
     global token, device_id, battery, debug_setting, messages
     if get_device() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting battery")
+    output(f"getting battery", 2)
     params = {'id': device_id}
     response = signed_get(path="/c/v0/device/battery/info", params=params)
     if response.status_code != 200:
         output(f"** get_battery() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -599,16 +585,15 @@
 
 def get_charge():
     global token, device_sn, battery_settings, debug_setting, messages
     if get_device() is None:
         return None
     if battery_settings is None:
         battery_settings = {}
-    if debug_setting > 1:
-        output(f"getting charge times")
+    output(f"getting charge times", 2)
     params = {'sn': device_sn}
     response = signed_get(path="/c/v0/device/battery/time/get", params=params)
     if response.status_code != 200:
         output(f"** get_charge() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -678,47 +663,45 @@
             en2 = round_time(time_hours(en2) + adjust)
         battery_settings['times'][1]['enableCharge'] = True
         battery_settings['times'][1]['enableGrid'] = True if ch2 == True or ch2 == 1 else False
         battery_settings['times'][1]['startTime']['hour'] = int(st2)
         battery_settings['times'][1]['startTime']['minute'] = int(60 * (st2 - int(st2)) + 0.5)
         battery_settings['times'][1]['endTime']['hour'] = int(en2)
         battery_settings['times'][1]['endTime']['minute'] = int(60 * (en2 - int(en2)) + 0.5)
-    if debug_setting > 0:
-        output(f"\nSetting time periods:")
-        output(f"   Time Period 1 = {time_period(battery_settings['times'][0])}")
-        output(f"   Time Period 2 = {time_period(battery_settings['times'][1])}")
+    output(f"\nSetting time periods:", 1)
+    output(f"   Time Period 1 = {time_period(battery_settings['times'][0])}", 1)
+    output(f"   Time Period 2 = {time_period(battery_settings['times'][1])}", 1)
     # set charge times
     data = {'sn': device_sn, 'times': battery_settings.get('times')}
     response = signed_post(path="/c/v0/device/battery/time/set", data=data)
     if response.status_code != 200:
         output(f"** set_charge() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
             output(f"** set_charge(), cannot update settings when schedule is active")
         else:
             output(f"** set_charge(), {errno_message(errno)}")
         return None
-    elif debug_setting > 1:
-        output(f"success") 
+    else:
+        output(f"success", 2) 
     return battery_settings
 
 ##################################################################################################
 # get min soc settings and save in battery_settings
 ##################################################################################################
 
 def get_min():
     global token, device_sn, battery_settings, debug_setting, messages
     if get_device() is None:
         return None
     if battery_settings is None:
         battery_settings = {}
-    if debug_setting > 1:
-        output(f"getting min soc")
+    output(f"getting min soc", 2)
     params = {'sn': device_sn}
     response = signed_get(path="/c/v0/device/battery/soc/get", params=params)
     if response.status_code != 200:
         output(f"** get_min() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -747,19 +730,17 @@
         battery_settings = {}
     if minGridSoc is not None:
         data['minGridSoc'] = minGridSoc
         battery_settings['minGridSoc'] = minGridSoc
     if minSoc is not None:
         data['minSoc'] = minSoc
         battery_settings['minSoc'] = minSoc
-    if debug_setting > 1:
-        output(f"set_min(): {battery_settings}")
+        output(f"set_min(): {battery_settings}", 2)
         return None
-    if debug_setting > 0:
-        output(f"\nSetting minSoc = {battery_settings.get('minSoc')}, minGridSoc = {battery_settings.get('minGridSoc')}")
+    output(f"\nSetting minSoc = {battery_settings.get('minSoc')}, minGridSoc = {battery_settings.get('minGridSoc')}", 1)
     response = signed_post(path="/c/v0/device/battery/soc/set", data=data)
     if response.status_code != 200:
         output(f"** set_min() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
@@ -808,40 +789,42 @@
 }
 
 def get_ui():
     global device_id, debug_setting, messages, remote_settings, named_settings, merge_settings
     if get_device() is None:
         return None
     if remote_settings is None:
-        if debug_setting > 1:
-            output(f"getting ui settings")
+        output(f"getting ui settings", 2)
         params = {'id': device_id}
         response = signed_get(path="/generic/v0/device/setting/ui", params=params)
         if response.status_code != 200:
             output(f"** get_ui() got response code {response.status_code}: {response.reason}")
             return None
         result = response.json().get('result')
         if result is None:
             errno = response.json().get('errno')
             output(f"** get_ui(), no result data, {errno_message(errno)}")
             return None
         remote_settings = result
         protocol = remote_settings['protocol'].lower().replace('xx','__')
         named_settings = {'_protocol': protocol}
+        output(f"  protocol = {protocol}", 2)
         volt_n = 0
         volt_keys = []
         for p in remote_settings['parameters']:
             if p['name'][:11] == 'BatteryVolt':    # merge BatteryVolts
+                output(f"  found {p['name']} with key {p['key']}", 2)
                 volt_n += 1
                 volt_keys.append(p['key'])
                 if volt_n == 3:
                     named_settings['BatteryVolt'] = {'keys': volt_keys, 'type': 'list', 'valueType': 'float', 'unit': p['properties'][0]['unit']}
                 elif volt_n > 3:
-                    print(f"** get_ui(): more than 3 groups found for BatteryVolt")
+                    print(f"** get_ui(): more than 3 groups found for BatteryVolt, n={volt_n}")
             elif p['name'][:11] == 'BatteryTemp':
+                output(f"  found {p['name']} with key {p['key']}", 2)
                 named_settings['BatteryTemp'] = {'keys': p['key'], 'type': 'list', 'valueType': 'int', 'unit': p['properties'][0]['unit']}
             else:
                 items = []
                 block = p['block'] and len(p['properties']) > 1
                 for e in p['properties']:
                     valueType = e['elemType']['valueType']
                     item = {'name': e['key'].replace(protocol,'')} if block else {'key': e['key']} #, 'group': p['name']}
@@ -868,16 +851,15 @@
                         named_settings[name][k] = merge_settings[name][k]
     return remote_settings
 
 def get_remote_settings(key):
     global token, device_id, debug_setting, messages
     if get_device() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting remote settings")
+    output(f"getting remote settings", 2)
     if key is None:
         return None
     if type(key) is list:
         values = {}
         for k in key:
             v = get_remote_settings(k)
             if v is None:
@@ -911,14 +893,15 @@
     if named_settings is None or named_settings.get(name) is None:
         output(f"** get_named_settings(): {name} was not recognised")
         return None
     keys = named_settings[name].get('keys')
     if keys is None:
         output(f"** get_named_settings(): no keys for name: {name}")
         return None
+    output(f"getting named_settings for {name} using {keys}", 2)
     result = get_remote_settings(keys)
     if result is None:
         output(f"** get_named_settings(): no result for {name} using key: {keys}")
         return None
     result_type = named_settings[name].get('type')
     value_type = named_settings[name].get('valueType')
     if result_type is None:
@@ -1024,16 +1007,15 @@
 # get the current enable flag
 def get_flag():
     global token, device_id, schedule, debug_setting, messages
     if get_device() is None:
         return None
     if schedule is not None and schedule.get('support') is not None:
         return schedule
-    if debug_setting > 1:
-        output(f"getting flag")
+    output(f"getting flag", 2)
     params = {'deviceSN': device_sn}
     response = signed_get(path="/generic/v0/device/scheduler/get/flag", params=params)
     if response.status_code != 200:
         output(f"** get_flag() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -1054,16 +1036,15 @@
 def get_schedule():
     global token, device_id, schedule, debug_setting, messages
     if get_flag() is None:
         return None
     if schedule.get('support') == False:
         output(f"** get_schedule(), not supported on this device")
         return None
-    if debug_setting > 1:
-        output(f"getting schedule")
+    output(f"getting schedule", 2)
     params = {'deviceSN': device_sn}
     response = signed_get(path="/generic/v0/device/scheduler/list", params=params)
     if response.status_code != 200:
         output(f"** get_schedule() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -1139,18 +1120,17 @@
     find = '' if name is None else name.replace(' ','').lower()
     found = [k for k in templates.keys() if templates[k]['templateName'][:len(find)].lower() == find]
     if len(found) == 0:
         output(f"** find_template(): no templates found with {name}")
         return None
     if len(found) == 1:
         return found[0]
-    if debug_setting > 0:
-        output(f"** find_template(): found multiple templates with {name}")
-        for k in found:
-            output(f"  {templates[k]['templateName']}")
+    output(f"** find_template(): found multiple templates with {name}")
+    for k in found:
+        output(f"  {templates[k]['templateName']}")
     return None
 
 
 ##################################################################################################
 # set schedule
 ##################################################################################################
 
@@ -1185,16 +1165,16 @@
     if get_flag() is None:
         return None
     if schedule.get('support') == False:
         output(f"** set_schedule(), not supported on this device")
         return None
     if schedule is None:
         schedule = get_schedule()
+    output(f"set_schedule(): enable = {enable}, periods = {periods}, template={template}", 2)
     if debug_setting > 1:
-        output(f"set_schedule(): enable = {enable}, periods = {periods}, template={template}")
         return None
     params = {'deviceSN': device_sn}
     if enable == 0:
         if debug_setting > 0:
             output(f"\nDisabling schedule")
         response = signed_get(path="/generic/v0/device/scheduler/disable", params=params)
         if response.status_code != 200:
@@ -1289,16 +1269,15 @@
     elif type(v) is not list:
         v = [v]
     for var in v:
         if var not in [x['variable'] for x in raw_vars]:
             output(f"** get_raw(): invalid variable '{var}'")
             output(f"{[x['variable'] for x in raw_vars]}")
             return None
-    if debug_setting > 1:
-        output(f"getting raw data")
+    output(f"getting raw data", 2)
     if load is None:
         d_begin = query_date(d)
         if d_begin is None:
             return None
         query = {id_name: id_code, 'variables': v, 'timespan': time_span, 'beginDate': d_begin}
         response = signed_post(path="/c/v0/device/history/raw", data=query)
         if response.status_code != 200:
@@ -1334,16 +1313,15 @@
                 v['value'] = v['data'][-1]['value']
                 del v['data']
 #                del v['date']
         elif plot > 0:
             plot_raw(result, plot)
         return result
     # integrate kW to kWh based on 5 minute samples
-    if debug_setting > 2:
-        output(f"calculating summary data")
+    output(f"calculating summary data", 3)
     # copy generationPower to produce inputPower data
     input_name = None
     if 'generationPower' in v:
         input_name = energy_vars[-1]
         input_result = deepcopy(result[v.index('generationPower')])
         input_result['name'] = input_name
         for y in input_result['data']:
@@ -1358,30 +1336,28 @@
             kwh_off = 0.0   # kwh during off peak time (02:00-05:00)
             kwh_peak = 0.0  # kwh during peak time (16:00-19:00)
             kwh_neg = 0.0
             if len(var['data']) > 1:
                 sample_time = round(60 * sample_rounding * (time_hours(var['data'][-1]['time'][11:]) - time_hours(var['data'][0]['time'][11:])) / (len(var['data']) - 1), 0) / sample_rounding
             else:
                 sample_time = 5.0
-            if debug_setting > 1:
-                output(f"{var['variable']}: samples = {len(var['data'])}, sample_time = {sample_time} minutes")
+            output(f"{var['variable']}: samples = {len(var['data'])}, sample_time = {sample_time} minutes", 2)
         sum = 0.0
         count = 0
         max = None
         max_time = None
         min = None
         min_time = None
         if summary == 3 and energy:
             var['state'] = [{}]
         for y in var['data']:
             h = time_hours(y['time'][11:19]) # time
             value = y['value']
             if value is None:
-                if debug_setting > 0:
-                    output(f"** get_raw(), warning: missing data for {var['variable']} at {y['time']}")
+                output(f"** get_raw(), warning: missing data for {var['variable']} at {y['time']}", 1)
                 continue
             sum += value
             count += 1
             max = value if max is None or value > max else max
             min = value if min is None or value < min else min
             if energy:
                 e = value * sample_time / 60      # convert kW samples to kWh energy
@@ -1536,16 +1512,15 @@
     elif type(v) is not list:
         v = [v]
     for var in v:
         if var not in report_vars:
             output(f"** get_report(): invalid variable '{var}'")
             output(f"{report_vars}")
             return None
-    if debug_setting > 1:
-        output(f"getting report data")
+    output(f"getting report data", 2)
     current_date = query_date(None)
     main_date = query_date(d)
     if main_date is None:
         return None
     side_result = None
     if report_type in ('day', 'week') and summary > 0:
         # side report needed
@@ -1630,16 +1605,15 @@
         count = 0
         sum = 0.0
         max = None
         min = None
         for j, y in enumerate(var['data']):
             value = y['value']
             if value is None:
-                if debug_setting > 0:
-                    output(f"** get_report(), warning: missing data for {var['variable']} on {d} at index {j}")
+                output(f"** get_report(), warning: missing data for {var['variable']} on {d} at index {j}", 1)
                 continue
             count += 1
             sum += value
             max = value if max is None or value > max else max
             min = value if min is None or value < min else min
         # correct day total from side report
         var['total'] = sum if report_type != 'day' else side_result[i]['data'][int(main_date['day'])-1]['value']
@@ -1675,16 +1649,15 @@
             if v['type'] not in types:
                 types.append(v['type'])
             if v['date'] not in dates:
                 dates.append(v['date'])
             for i in [x['index'] for x in v['data']]:
                 if i not in index:
                     index.append(i)
-    if debug_setting > 2:
-        output(f"vars = {vars}, dates = {dates}, types = {types}, index = {index}")
+    output(f"vars = {vars}, dates = {dates}, types = {types}, index = {index}", 3)
     if len(vars) == 0:
         return
     # plot variables by date with the same units on the same charts
     lines = 0
     width = 0.8 / (len(dates) if plot == 1 else len(vars) if len(dates) == 1 else len(dates))
     align = 0.0
     for var in vars:
@@ -1738,16 +1711,15 @@
 
 def get_earnings():
     global token, device_id, station_id, var_list, debug_setting, messages
     if get_device() is None:
         return None
     id_name = 'deviceID'
     id_code = device_id
-    if debug_setting > 1:
-        output(f"getting earnings")
+    output(f"getting earnings", 2)
     params = {id_name: id_code}
     response = signed_get(path="/c/v0/device/earnings", params=params)
     if response.status_code != 200:
         output(f"** get_earnings() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json()
     if result is None:
@@ -2023,33 +1995,31 @@
     # adjust system to get local time now
     now = system_time + timedelta(hours=time_offset)
     hour_now = now.hour + now.minute / 60
     update_time = tariff_config['update_time']
     update_time = time_hours(update_time) if type(update_time) is str else 17 if update_time is None else update_time
     today = datetime.strftime(now + timedelta(days=0 if hour_now >= update_time else -1), '%Y-%m-%d')
     tomorrow = datetime.strftime(now + timedelta(days=1 if hour_now >= update_time else 0), '%Y-%m-%d')
-    if debug_setting > 1:
-        output(f"  datetime = {today} {hours_time(hour_now)}")
+    output(f"  datetime = {today} {hours_time(hour_now)}", 2)
     # get product and region
     product = tariff_config['product'].upper()
     region = tariff_config['region'].upper()
     if region not in regions:
         output(f"** region {region} not recognised, valid regions are {regions}")
         return None
     # get prices from 11pm today to 11pm tomorrow
     output(f"\nProduct: {product}")
     output(f"Region:  {regions[region]}")
     zulu_hour = "T" + hours_time(23 - time_offset - time_shift, ss=True) + "Z"
     url = octopus_api_url.replace("%PRODUCT%", product).replace("%REGION%", region)
     period_from = today + zulu_hour
     period_to = tomorrow + zulu_hour
     params = {'period_from': period_from, 'period_to': period_to }
-    if debug_setting > 1:
-        output(f"time_offset = {time_offset}, time_shift = {time_shift}")
-        output(f"period_from = {period_from}, period_to = {period_to}")
+    output(f"time_offset = {time_offset}, time_shift = {time_shift}", 2)
+    output(f"period_from = {period_from}, period_to = {period_to}", 2)
     response = requests.get(url, params=params)
     if response.status_code != 200:
         output(f"** get_agile_period() response code from Octopus API {response.status_code}: {response.reason}")
         return None
     # results are in reverse chronological order...
     results = response.json().get('results')[::-1]
     # extract times and prices
@@ -2061,16 +2031,15 @@
         prices.append(r['value_inc_vat'])
     # work out start and end times for charging
     start_at = time_hours(start_at) if type(start_at) is str else 23.0 if start_at is None else start_at
     end_by = time_hours(end_by) if type(end_by) is str else 8.0 if end_by is None else end_by
     start_i = int(round_time(start_at - 23) * 2)
     end_i = int(round_time(end_by - 23) * 2)
     end_i = 48 if end_i == 0 or end_i > 48 else end_i
-    if debug_setting > 1:
-        output(f"start_at = {start_at}, end_by = {end_by}, start_i = {start_i}, end_i = {end_i}, duration = {duration}, span = {span}")
+    output(f"start_at = {start_at}, end_by = {end_by}, start_i = {start_i}, end_i = {end_i}, duration = {duration}, span = {span}", 2)
     if (start_i + span) > 48 or start_i > end_i:
         output(f"** get_agile_period(): invalid times {hours_time(start_at)} - {hours_time(end_by)}. Must start from 23:00 today and end by 23:00 tomorrow")
         return None
     if len(results) < (start_i + span):
         output(f"** get_agile_period(): prices not available for {tomorrow}")
         return None
     # work out weighted average for each period and track lowest price
@@ -2177,68 +2146,68 @@
     args = locals()
     s = ""
     for k in [k for k in args.keys() if args[k] is not None and k != 'settings']:
         s += f"\n  {k} = {args[k]}"
     # store settings:
     for key, value in settings.items():
         if key not in tariff_config:
-            print(f"** unknown configuration parameter: {key}")
+            output(f"** unknown configuration parameter: {key}")
         else:
             tariff_config[key] = value
             s += f"\n  {key} = {value}"
-    if len(s) > 0 and debug_setting > 1:
-        print(f"Parameters: {s}")
+    if len(s) > 0:
+        output(f"Parameters: {s}", 2)
     found = []
     if find in tariff_list:
         found = [find]
     elif type(find) is str:
         for dict in tariff_list:
             if find.lower() in dict['name'].lower():
                 found.append(dict)
     if len(found) != 1:
-        print(f"** set_tariff(): {find} must identify one of the available tariffs:")
+        output(f"** set_tariff(): {find} must identify one of the available tariffs:")
         for x in tariff_list:
             print(f"  {x['name']}")
         return None
     use = found[0]
     if times is None:
         times = [(start_at, end_by, duration)] if start_at is not None or end_by is not None or duration is not None else [(None, None, 3)]
     elif type(times) is not list:
         times = [times]
     if len(times) > 2:
-        print(f"** set_tariff(): one AM (11pm - 11am) and one PM (11am - 11pm) charge time can be set. times = {times}")
+        output(f"** set_tariff(): one AM (11pm - 11am) and one PM (11am - 11pm) charge time can be set. times = {times}")
         return None
     set_proc = set_agile_period if use == agile_octopus else set_tariff_period
     for t in times:
         result = set_proc(period={'start': t[0], 'end': t[1], 'duration': t[2]}, tariff=use, d=d)
         if result is None:
             return None
     if forecast_times is not None:
         if type(forecast_times) is not list:
             forecast_times = [forecast_times]
         forecast_hours = []
         for i, t in enumerate(forecast_times):
             forecast_times[i] = hours_time(t)
             forecast_hours.append(time_hours(t))
         use['forecast_times'] = forecast_hours
-        print(f"\nForecast times set to {forecast_times}")
+        output(f"\nForecast times set to {forecast_times}")
     if work_times is not None:
         if type(work_times) is not None:
             work_times = [work_times]
         work_hours = []
         for d in work_times:
             (mode, start, end) = d
             work_hours.append({'mode': mode, 'start': time_hours(start), 'end': time_hours(end)})
         use['work_hours'] = work_hours
-        print(f"\nWork mode times set to {work_hours}")
+        output(f"\nWork mode times set to {work_hours}")
     if update == 1:
         tariff = use
-        print(f"\nTariff set to {tariff['name']}")
-    elif debug_setting > 0:
-        print(f"\nNo changes made to current tariff")
+        output(f"\nTariff set to {tariff['name']}")
+    else:
+        output(f"\nNo changes made to current tariff", 1)
     return None
 
 # get work mode for a time of day based on the tariff:
 def timed_work_mode(h, default = 'SelfUse'):
     if tariff is None or tariff.get('work_hours') is None:
         return default
     for d in tariff['work_hours']:
@@ -2395,18 +2364,18 @@
     # store settings:
     for key, value in settings.items():
         if key not in charge_config:
             print(f"** unknown configuration parameter: {key}")
         else:
             charge_config[key] = value
             s += f"\n  {key} = {value}"
-    if len(s) > 0 and debug_setting > 1:
-        print(f"Parameters: {s}")
-    if tariff is not None and debug_setting > 1:
-        print(f"  tariff = {tariff['name']}")
+    if len(s) > 0:
+        output(f"Parameters: {s}", 2)
+    if tariff is not None:
+        output(f"  tariff = {tariff['name']}", 2)
     # set default parameters
     show_data = 1 if show_data is None or show_data == True else 0 if show_data == False else show_data
     show_plot = 3 if show_plot is None or show_plot == True else 0 if show_plot == False else show_plot
     run_after = 1 if run_after is None else run_after 
     timed_mode = 1 if timed_mode is None and tariff is not None and tariff.get('work_hours') is not None else 0 if timed_mode is None else timed_mode
     if forecast_times is None:
         forecast_times = tariff['forecast_times'] if tariff is not None and tariff.get('forecast_times') is not None else [22,23]
@@ -2415,16 +2384,15 @@
     # get dates and times
     system_time = (datetime.now(tz=timezone.utc) + timedelta(hours=time_shift)) if test_time is None else datetime.strptime(test_time, '%Y-%m-%d %H:%M')
     time_offset = daylight_saving(system_time) if daylight_saving is not None else 0
     now = system_time + timedelta(hours=time_offset)
     today = datetime.strftime(now, '%Y-%m-%d')
     base_hour = now.hour
     hour_now = now.hour + now.minute / 60
-    if debug_setting > 1:
-        print(f"  datetime = {today} {hours_time(hour_now)}")
+    output(f"  datetime = {today} {hours_time(hour_now)}", 2)
     yesterday = datetime.strftime(now - timedelta(days=1), '%Y-%m-%d')
     tomorrow = datetime.strftime(now + timedelta(days=1), '%Y-%m-%d')
     day_tomorrow = day_names[(now.weekday() + 1) % 7]
     day_after_tomorrow = datetime.strftime(now + timedelta(days=2), '%Y-%m-%d')
     # work out if we lose 1 hour if clocks go forward or gain 1 hour if clocks go back
     change_hour = 0
     hour_adjustment = 0 if daylight_saving is None else daylight_changes(system_time, system_time + timedelta(days=2))
@@ -2444,15 +2412,15 @@
     start_pm = time_hours(tariff['off_peak2']['start'] if tariff is not None else 0.0)
     end_pm = time_hours(tariff['off_peak2']['end'] if tariff is not None else 0.0)
     force_charge_pm = 0 if tariff is not None and tariff['off_peak2']['force'] == 0 or force_charge == 0 else 1
     time_to_pm = round_time(start_pm - base_hour) if start_pm > 0 else None
     no_go1 = time_to_am is not None and hour_in(hour_now, {'start': round_time(start_am - 0.25), 'end': round_time(end_am + 0.25)})
     no_go2 = time_to_pm is not None and hour_in(hour_now, {'start': round_time(start_pm - 0.25), 'end': round_time(end_pm + 0.25)})
     if (no_go1 or no_go2) and update_settings > 0:
-        print(f"\nInverter settings will not be changed less than 15 minutes before or after a charging period")
+        output(f"\nInverter settings will not be changed less than 15 minutes before or after a charging period")
         update_settings = 0
     # choose and configure parameters for next charge time period
     charge_pm = time_to_pm is not None and time_to_pm < time_to_am
     force_charge = force_charge_pm if charge_pm else force_charge_am
     start_at = start_pm if charge_pm else start_am
     end_by = end_pm if charge_pm else end_am
     charge_time = round_time(end_by - start_at)
@@ -2466,49 +2434,48 @@
     run_time = int((time_to_am if charge_pm else time_to_am + 24 if time_to_pm is None else time_to_pm) + 0.99) + 1 + hour_adjustment
     # if we need to do a full charge, full_charge is the date, otherwise None
     full_charge = charge_config['full_charge'] if not charge_pm else None
     if type(full_charge) is int:            # value = day of month
         full_charge = tomorrow if full_charge is not None and int(tomorrow[-2:]) == full_charge else None
     elif type(full_charge) is str:          # value = daily or day of week
         full_charge = tomorrow if full_charge.lower() == 'daily' or full_charge.title() == day_tomorrow[:3] else None
-    if debug_setting > 2:
-        print(f"\ntoday = {today}, tomorrow = {tomorrow}, time_shift = {time_shift}")
-        print(f"start_am = {start_am}, end_am = {end_am}, force_am = {force_charge_am}, time_to_am = {time_to_am}")
-        print(f"start_pm = {start_pm}, end_pm = {end_pm}, force_pm = {force_charge_pm}, time_to_pm = {time_to_pm}")
-        print(f"start_at = {start_at}, end_by = {end_by}, force_charge = {force_charge}")
-        print(f"base_hour = {base_hour}, hour_adjustment = {hour_adjustment}, change_hour = {change_hour}")
-        print(f"time_to_start = {time_to_start}, run_time = {run_time}, charge_pm = {charge_pm}")
-        print(f"start_hour = {start_hour}, time_to_next = {time_to_next}, full_charge = {full_charge}")
+    output(f"\ntoday = {today}, tomorrow = {tomorrow}, time_shift = {time_shift}", 3)
+    output(f"start_am = {start_am}, end_am = {end_am}, force_am = {force_charge_am}, time_to_am = {time_to_am}", 3)
+    output(f"start_pm = {start_pm}, end_pm = {end_pm}, force_pm = {force_charge_pm}, time_to_pm = {time_to_pm}", 3)
+    output(f"start_at = {start_at}, end_by = {end_by}, force_charge = {force_charge}", 3)
+    output(f"base_hour = {base_hour}, hour_adjustment = {hour_adjustment}, change_hour = {change_hour}", 3)
+    output(f"time_to_start = {time_to_start}, run_time = {run_time}, charge_pm = {charge_pm}", 3)
+    output(f"start_hour = {start_hour}, time_to_next = {time_to_next}, full_charge = {full_charge}", 3)
     # get device and battery info from inverter
     if test_soc is None:
         if charge_config.get('min_soc') is not None:
             min_soc = charge_config['min_soc']
         else:
             get_min()
             if battery_settings.get('minGridSoc') is not None:
                 min_soc = battery_settings['minGridSoc']
             else:
                 print(f"\nMin SoC is not available. Please provide % via 'min_soc' parameter")
                 return None
         get_battery()
         if battery['status'] != 1:
-            print(f"\nBattery status is not available")
+            output(f"\nBattery status is not available")
             return None
         current_soc = battery['soc']
         bat_volt = battery['volt']
         bat_power = battery['power']
         bat_current = battery['current']
         temperature = battery['temperature']
         residual = battery['residual']
         if charge_config.get('capacity') is not None:
             capacity = charge_config['capacity']
         elif residual is not None and residual > 0.2 and current_soc is not None and current_soc > 1:
             capacity = residual * 100 / current_soc
         else:
-            print(f"Battery capacity could not be estimated. Please add the parameter 'capacity=xx' in kWh")
+            output(f"Battery capacity could not be estimated. Please add the parameter 'capacity=xx' in kWh")
             return None
     else:
         current_soc = test_soc
         capacity = 8.2
         residual = test_soc * capacity / 100
         min_soc = 10
         bat_volt = 122 / (1 + 0.03 * (100 - test_soc) / 90)
@@ -2517,56 +2484,56 @@
         bat_current = 0.0
     volt_curve = charge_config['volt_curve']
     nominal_soc = charge_config['nominal_soc']
     volt_nominal = interpolate(nominal_soc / 10, volt_curve)
     bat_resistance = charge_config['bat_resistance'] * bat_volt / volt_nominal
     bat_ocv = (bat_volt + bat_current * bat_resistance) * volt_nominal / interpolate(current_soc / 10, volt_curve)
     reserve = capacity * min_soc / 100
-    print(f"\nBattery Info:")
-    print(f"  Capacity:    {capacity:.1f}kWh")
-    print(f"  Residual:    {residual:.1f}kWh")
-    print(f"  Voltage:     {bat_volt:.1f}V")
-    print(f"  Current:     {bat_current:.1f}A")
-    print(f"  State:       {'Charging' if bat_power < 0 else 'Discharging'} ({abs(bat_power):.3f}kW)")
-    print(f"  Current SoC: {current_soc}%")
-    print(f"  Min SoC:     {min_soc}% ({reserve:.1f}kWh)")
-    print(f"  Temperature: {temperature:.1f}°C")
-    print(f"  Resistance:  {bat_resistance:.2f} ohms")
-    print(f"  Nominal OCV: {bat_ocv:.1f}V at {nominal_soc}% SoC")
+    output(f"\nBattery Info:")
+    output(f"  Capacity:    {capacity:.1f}kWh")
+    output(f"  Residual:    {residual:.1f}kWh")
+    output(f"  Voltage:     {bat_volt:.1f}V")
+    output(f"  Current:     {bat_current:.1f}A")
+    output(f"  State:       {'Charging' if bat_power < 0 else 'Discharging'} ({abs(bat_power):.3f}kW)")
+    output(f"  Current SoC: {current_soc}%")
+    output(f"  Min SoC:     {min_soc}% ({reserve:.1f}kWh)")
+    output(f"  Temperature: {temperature:.1f}°C")
+    output(f"  Resistance:  {bat_resistance:.2f} ohms")
+    output(f"  Nominal OCV: {bat_ocv:.1f}V at {nominal_soc}% SoC")
     # get power and charge current for device
     device_power = device.get('power')
     device_current = device.get('max_charge_current')
     model = device.get('deviceType') if device.get('deviceType') is not None else 'unknown'
     if device_power is None or device_current is None:
-        print(f"** could not get parameters for {model} inverter, using default rating of 3.68kW")
+        output(f"** could not get parameters for {model} inverter, using default rating of 3.68kW")
         device_power = 3.68
         device_current = 26
     # charge times are derated based on temperature
     charge_current = device_current if charge_config['charge_current'] is None else charge_config['charge_current']
     derate_temp = charge_config['derate_temp']
     if temperature > 36:
-        print(f"\nHigh battery temperature may affect the charge rate")
+        output(f"\nHigh battery temperature may affect the charge rate")
     elif round(temperature, 0) <= derate_temp:
-        print(f"\nLow battery temperature may affect the charge rate")
+        output(f"\nLow battery temperature may affect the charge rate")
         derating = charge_config['derating']
         derate_step = charge_config['derate_step']
         i = int((derate_temp - temperature) / (derate_step if derate_step is not None and derate_step > 0 else 1))
         if derating is not None and type(derating) is list and i < len(derating):
             derated_current = derating[i]
             if derated_current < charge_current:
-                print(f"  Charge current reduced from {charge_current:.0f}A to {derated_current:.0f}A" )
+                output(f"  Charge current reduced from {charge_current:.0f}A to {derated_current:.0f}A" )
                 charge_current = derated_current
         else:
             force_charge = 2
-            print(f"  Full charge set")
+            output(f"  Full charge set")
     # work out charge limit = max power going into the battery after ac conversion losses
     charge_limit = device_power * charge_config['grid_loss']
     charge_power = charge_current * (bat_ocv + charge_current * bat_resistance) / 1000
     if charge_power < 0.1:
-        print(f"** charge_current is too low ({charge_current:.1f}A)")
+        output(f"** charge_current is too low ({charge_current:.1f}A)")
     elif charge_power < charge_limit:
         charge_limit = charge_power
     # work out losses when charging / force discharging
     inverter_power = charge_config['inverter_power'] if charge_config['inverter_power'] is not None else round(device_power, 0) * 20
     operating_loss = inverter_power / 1000
     bms_power = charge_config['bms_power']
     bms_loss = bms_power / 1000
@@ -2579,152 +2546,147 @@
     discharge_current = device_current if charge_config['discharge_current'] is None else charge_config['discharge_current']
     discharge_power = discharge_current * bat_ocv / 1000
     discharge_limit = discharge_power if discharge_power < discharge_limit else discharge_limit
     # charging happens if generation exceeds export limit in feedin work mode
     export_power = device_power if charge_config['export_limit'] is None else charge_config['export_limit']
     export_limit = export_power / discharge_loss
     current_mode = get_work_mode()
-    if debug_setting > 2:
-        print(f"\ncharge_config = {json.dumps(charge_config, indent=2)}")
-    print(f"\nDevice Info:")
-    print(f"  Model:     {model}")
-    print(f"  Rating:    {device_power:.2f}kW")
-    print(f"  Export:    {export_power:.2f}kW")
-    print(f"  Charge:    {charge_current:.1f}A, {charge_limit:.2f}kW, {charge_loss * 100:.1f}% efficient")
-    print(f"  Discharge: {discharge_current:.1f}A, {discharge_limit:.2f}kW, {discharge_loss * 100:.1f}% efficient")
-    print(f"  Inverter:  {inverter_power:.0f}W power consumption")
-    print(f"  BMS:       {bms_power:.0f}W power consumption")
+    output(f"\ncharge_config = {json.dumps(charge_config, indent=2)}", 3)
+    output(f"\nDevice Info:")
+    output(f"  Model:     {model}")
+    output(f"  Rating:    {device_power:.2f}kW")
+    output(f"  Export:    {export_power:.2f}kW")
+    output(f"  Charge:    {charge_current:.1f}A, {charge_limit:.2f}kW, {charge_loss * 100:.1f}% efficient")
+    output(f"  Discharge: {discharge_current:.1f}A, {discharge_limit:.2f}kW, {discharge_loss * 100:.1f}% efficient")
+    output(f"  Inverter:  {inverter_power:.0f}W power consumption")
+    output(f"  BMS:       {bms_power:.0f}W power consumption")
     if current_mode is not None:
-        print(f"  Work Mode: {current_mode}")
+        output(f"  Work Mode: {current_mode}")
     # get consumption data
     annual_consumption = charge_config['annual_consumption']
     if annual_consumption is not None:
         consumption = annual_consumption / 365 * seasonality[now.month - 1] / sum(seasonality) * 12
         consumption_by_hour = daily_consumption
-        print(f"\nEstimated consumption: {consumption:.1f}kWh")
+        output(f"\nEstimated consumption: {consumption:.1f}kWh")
     else:
         consumption_days = charge_config['consumption_days']
         consumption_days = 3 if consumption_days > 7 or consumption_days < 1 else consumption_days
         consumption_span = charge_config['consumption_span']
         if consumption_span == 'weekday':
             history = get_report('day', d=date_list(span='weekday', e=tomorrow, today=2)[-consumption_days-1:-1], v='loads')
         else:
             last_date = today if hour_now >= charge_config['use_today'] else yesterday
             history = get_report('day', d=date_list(span='week', e=last_date, today=1)[-consumption_days:], v='loads')
         (consumption, consumption_by_hour) = report_value_profile(history)
         if consumption is None:
             print(f"No consumption data available")
             return None
-        print(f"\nConsumption (kWh):")
+        output(f"\nConsumption (kWh):")
         s = ""
         for h in history:
             s += f"  {h['date']}: {h['total']:4.1f},"
-        print(s[:-1])
-        print(f"  Average of last {consumption_days} {day_tomorrow if consumption_span=='weekday' else 'day'}s: {consumption:.1f}kWh")
+        output(s[:-1])
+        output(f"  Average of last {consumption_days} {day_tomorrow if consumption_span=='weekday' else 'day'}s: {consumption:.1f}kWh")
     # time line has 1 hour buckets of consumption
     daily_sum = sum(consumption_by_hour)
     consumption_timed = timed_list([consumption * x / daily_sum for x in consumption_by_hour], hour_now, run_time)
     # get Solcast data and produce time line
     solcast_value = None
     solcast_profile = None
     if forecast is None and solcast_api_key is not None and solcast_api_key != 'my.solcast_api_key' and (base_hour in forecast_times or run_after == 0):
         fsolcast = Solcast(quiet=True, estimated=1 if charge_pm else 0)
         if fsolcast is not None and hasattr(fsolcast, 'daily') and fsolcast.daily.get(forecast_day) is not None:
             solcast_value = fsolcast.daily[forecast_day]['kwh']
             solcast_timed = forecast_value_timed(fsolcast, today, tomorrow, hour_now, run_time, time_offset)
             if charge_pm:
-                print(f"\nSolcast forecast for {today} = {fsolcast.daily[today]['kwh']:.1f}, {tomorrow} = {fsolcast.daily[tomorrow]['kwh']:.1f}")
+                output(f"\nSolcast forecast for {today} = {fsolcast.daily[today]['kwh']:.1f}, {tomorrow} = {fsolcast.daily[tomorrow]['kwh']:.1f}")
             else:
-                print(f"\nSolcast forecast for {forecast_day} = {solcast_value:.1f}kWh")
+                output(f"\nSolcast forecast for {forecast_day} = {solcast_value:.1f}kWh")
             adjust = charge_config['solcast_adjust']
             if adjust != 100:
                 solcast_value = solcast_value * adjust / 100
                 solcast_timed = [v * adjust / 100 for v in solcast_timed]
-                print(f"  Adjusted forecast: {solcast_value:.1f}kWh ({adjust}%)")
+                output(f"  Adjusted forecast: {solcast_value:.1f}kWh ({adjust}%)")
     # get forecast.solar data and produce time line
     solar_value = None
     solar_profile = None
     if forecast is None and solar_arrays is not None and (base_hour in forecast_times or run_after == 0):
         fsolar = Solar(quiet=True)
         if fsolar is not None and hasattr(fsolar, 'daily') and fsolar.daily.get(forecast_day) is not None:
             solar_value = fsolar.daily[forecast_day]['kwh']
             solar_timed = forecast_value_timed(fsolar, today, tomorrow, hour_now, run_time, time_offset)
             if charge_pm:
-                print(f"\nSolar forecast for {today} = {fsolar.daily[today]['kwh']:.1f}, {tomorrow} = {fsolar.daily[tomorrow]['kwh']:.1f}")
+                output(f"\nSolar forecast for {today} = {fsolar.daily[today]['kwh']:.1f}, {tomorrow} = {fsolar.daily[tomorrow]['kwh']:.1f}")
             else:
-                print(f"\nSolar forecast for {forecast_day} = {solar_value:.1f}kWh")
+                output(f"\nSolar forecast for {forecast_day} = {solar_value:.1f}kWh")
             adjust = charge_config['solar_adjust']
             if adjust != 100:
                 solar_value = solar_value * adjust / 100
                 solar_timed = [v * adjust / 100 for v in solar_timed]
-                print(f"  Adjusted forecast: {solar_value:.1f}kWh ({adjust}%)")
+                output(f"  Adjusted forecast: {solar_value:.1f}kWh ({adjust}%)")
     if solcast_value is None and solar_value is None and debug_setting > 1:
-        print(f"\nNo forecasts available at this time")
+        output(f"\nNo forecasts available at this time")
     # get generation data
     generation = None
     last_date = today if hour_now >= charge_config['use_today'] else yesterday
     gen_days = charge_config['generation_days']
     history = get_raw('week', d=last_date, v=['pvPower','meterPower2'], summary=2)
     pv_history = {}
     if history is not None and len(history) > 0:
         for day in history:
             date = day['date']
             if pv_history.get(date) is None:
                 pv_history[date] = 0.0
             if day.get('kwh') is not None and day.get('kwh_neg') is not None:
                 pv_history[date] += day['kwh_neg'] / 0.92 if day['variable'] == 'meterPower2' else day['kwh']
         pv_sum = sum([pv_history[d] for d in sorted(pv_history.keys())[-gen_days:]])
-        print(f"\nGeneration (kWh):")
+        output(f"\nGeneration (kWh):")
         s = ""
         for d in sorted(pv_history.keys())[-gen_days:]:
             s += f"  {d}: {pv_history[d]:4.1f},"
-        print(s[:-1])
+        output(s[:-1])
         generation = pv_sum / gen_days
-        print(f"  Average of last {gen_days} days: {generation:.1f}kWh")
+        output(f"  Average of last {gen_days} days: {generation:.1f}kWh")
     # choose expected value and produce generation time line
+    output_spool(charge_needed_app_key)
     quarter = now.month // 3 % 4
     sun_name = seasonal_sun[quarter]['name']
     sun_profile = seasonal_sun[quarter]['sun']
     sun_sum = sum(sun_profile)
     sun_timed = timed_list(sun_profile, hour_now, run_time)
     if forecast is not None:
         expected = forecast
         generation_timed = [expected * x / sun_sum for x in sun_timed]
-        output(f"\nUsing {expected:.1f}kWh manual forecast with {sun_name} sun and {consumption:.1f}kWh consumption")
     elif solcast_value is not None:
         expected = solcast_value
         generation_timed = solcast_timed
-        output(f"\nUsing {expected:.1f}kWh Solcast forecast and {consumption:.1f}kWh consumption for {forecast_day}")
     elif solar_value is not None:
         expected = solar_value
         generation_timed = solar_timed
-        output(f"\nUsing {expected:.1f}kWh Solar forecast and {consumption:.1f}kWh consumption for {forecast_day}")
     elif generation is None or generation == 0.0:
         output(f"\nNo generation data available")
         output_close()
         return None
     else:
         expected = generation
         generation_timed = [expected * x / sun_sum for x in sun_timed]
-        output(f"\nUsing {expected:.1f}kWh generation with {sun_name} sun and {consumption:.1f}kWh consumption")
         if charge_config['forecast_selection'] == 1 and update_settings > 0:
-            output(f"  Settings will not be updated when forecast is not available")
+            output(f"\nSettings will not be updated when forecast is not available")
             update_settings = 2 if update_settings == 3 else 0
     # produce time lines for main charge and discharge (after losses)
     charge_timed = [x * charge_config['pv_loss'] for x in generation_timed]
     discharge_timed = [x / charge_config['discharge_loss'] for x in consumption_timed]
     # adjust charge and discharge time lines for work mode, force charge and power limits
     work_mode = current_mode
     for i in range(0, run_time):
         h = base_hour + i
         # get work mode and check for changes
         new_work_mode = timed_work_mode(h, current_mode) if timed_mode == 1 else current_mode
         if new_work_mode is not None and new_work_mode != work_mode:
-            if debug_setting > 0:
-                output(f"  {hours_time(h)}: {new_work_mode} work mode")
+            output(f"  {hours_time(h)}: {new_work_mode} work mode", 2)
             work_mode = new_work_mode
         # cap charge / discharge power
         charge_timed[i] = charge_limit if charge_timed[i] > charge_limit else charge_timed[i]
         discharge_timed[i] = discharge_limit if discharge_timed[i] > discharge_limit else discharge_timed[i]
         if force_charge_am == 1 and hour_in(h, {'start': start_am, 'end': end_am}):
             discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
         elif force_charge_pm == 1 and hour_in(h, {'start': start_pm, 'end': end_pm}):
@@ -2761,35 +2723,34 @@
         bat_timed.append(kwh_current)
         if kwh_current < kwh_min:       # track minimum and time
             kwh_min = kwh_current
             min_hour = h
         kwh_current += kwh_timed[i]
         h += 1
     # work out what we need to add to stay above reserve and provide contingency or to hit target_soc
-    output_spool(charge_needed_app_key)
     contingency = charge_config['special_contingency'] if tomorrow[-5:] in charge_config['special_days'] else charge_config['contingency']
     kwh_contingency = consumption * contingency / 100
     kwh_needed = reserve + kwh_contingency - kwh_min
     start_residual = interpolate(time_to_start, bat_timed)      # residual when charging starts
     target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 0
     target_kwh = capacity if target_soc > 100 else target_soc / 100 * capacity
     if target_kwh > (start_residual + kwh_needed):
         kwh_needed = target_kwh - start_residual
     day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     if kwh_min > reserve and kwh_needed < charge_config['min_kwh'] and full_charge is None and test_charge is None:
-        output(f"\nNo charging is needed")
+        output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
     else:
         charge_message = "with charge added"
         if test_charge is None:
             min_hour_adjust = min_hour - hour_adjustment if min_hour >= change_hour else 0
-            output(f"\nCharge of {kwh_needed:.2f}kWh is needed")
+            output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
         else:
             output(f"\nTest charge of {test_charge}kWh")
             charge_message = "** test charge **"
             kwh_needed = test_charge
         # work out time to add kwh_needed to battery
         taper_time = 10/60 if (start_residual + kwh_needed) >= (capacity * 0.95) else 0
         hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
@@ -2798,15 +2759,15 @@
             kwh_needed = capacity - start_residual
             hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
             if full_charge is not None or force_charge == 2 or hours > charge_time:
                 hours = charge_time
                 output(f"  Full charge time used")
         elif hours < charge_config['min_hours']:
             hours = charge_config['min_hours']
-            output(f"  Minimum charge time used")
+#            output(f"  Minimum charge time used")
         end1 = round_time(start_at + hours)
         # rework charge and discharge and work out grid consumption
         start_timed = time_to_start      # relative start and end time 
         end_timed = start_timed + hours
         charge_timed_old = [x for x in charge_timed]
         discharge_timed_old = [x for x in discharge_timed]
         for i in range(time_to_next, int(time_to_next + hours + 2)):
@@ -2852,15 +2813,15 @@
             h += 1
         time_to_end = int(start_timed + hours) + 1
         kwh_added = bat_timed[time_to_end] - bat_timed_old[time_to_end]
         end_part_hour = end_timed - int(end_timed)
         old_residual = interpolate(end_timed, bat_timed_old)
         new_residual = capacity if old_residual + kwh_added > capacity else old_residual + kwh_added
         net_added = new_residual - start_residual
-        output(f"  Charging for {int(hours * 60)} minutes adds {net_added:.2f}kWh")
+#        output(f"  Charging for {int(hours * 60)} minutes adds {net_added:.2f}kWh")
         output(f"  Start SoC: {start_residual / capacity * 100:3.0f}% at {hours_time(start_at)} ({start_residual:.2f}kWh)")
         output(f"  End SoC:   {new_residual / capacity * 100:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
     if show_data > 2:
         output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh")
         for i in range(0, run_time):
             h = base_hour + i
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
@@ -2882,18 +2843,18 @@
         output(s[:-1])
     if show_plot > 0:
         print()
         plt.figure(figsize=(figure_width, figure_width/2))
         x_timed = [i for i in range(0, run_time)]
         plt.xticks(ticks=x_timed, labels=[hours_time(base_hour + x - (hour_adjustment if (base_hour + x) >= change_hour else 0), day=False) for x in x_timed], rotation=90, fontsize=8, ha='center')
         if show_plot == 1:
-            title = f"Battery SoC % ({charge_message}, forecast={expected:.1f}kWh, consumption={consumption:.1f}kWh)"
+            title = f"Battery SoC % ({charge_message})"
             plt.plot(x_timed, [round(bat_timed[x] * 100 / capacity,1) for x in x_timed], label='Battery', color='blue')
         else:
-            title = f"Energy Flow kWh ({charge_message}, forecast={expected:.1f}kWh, consumption={consumption:.1f}kWh)"
+            title = f"Energy Flow kWh ({charge_message})"
             plt.plot(x_timed, bat_timed, label='Battery', color='blue')
             plt.plot(x_timed, generation_timed, label='Generation', color='green')
             plt.plot(x_timed, consumption_timed, label='Consumption', color='red')
 #            if kwh_needed > 0:
 #                plt.plot(x_timed, bat_timed_old, label='Battery (before charging)', color='blue', linestyle='dotted')
             if show_plot == 3:
                 plt.plot(x_timed, charge_timed, label='Charge', color='orange', linestyle='dotted')
@@ -3824,16 +3785,18 @@
 # simple push message
 def output_message(app_key=None, message=None, plot=0):
     output_spool(app_key, message)
     output_close(plot=plot)
     return None
 
 # add to spooled_output
-def output(s=""):
-    global spool_mode, spooled_output
+def output(s="", log_level=None):
+    global spool_mode, spooled_output, debug_setting
+    if log_level is not None and debug_setting < log_level:
+        return
     # keep output stream up to date in case of problem / exception
     print(s)
     # spool output for pushover if needed
     if spool_mode is not None:
         if ((len(spooled_output) if spooled_output is not None else 0) + len(s)) > 1024:
             # more than 1024 chars, re-start spooling to avoid data loss
             output_spool(spool_mode)
```

### Comparing `foxesscloud-2.2.4/src/foxesscloud/openapi.py` & `foxesscloud-2.2.5/src/foxesscloud/openapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud using Open API
-Updated:  17 April 2024
+Updated:  19 April 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.2.4"
+version = "2.2.5"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -151,69 +151,63 @@
     headers['Lang'] = lang
     headers['User-Agent'] = user_agent
     headers['Timezone'] = time_zone
     headers['Timestamp'] = timestamp
     headers['Content-Type'] = 'application/json'
     if login == 0:
         headers['Signature'] = hashlib.md5(fr"{path}\r\n{headers['Token']}\r\n{headers['Timestamp']}".encode('UTF-8')).hexdigest()
-    if debug_setting > 2:
-        output(f"path = {path}")
-        output(f"headers = {headers}")
+    output(f"path = {path}", 3)
+    output(f"headers = {headers}", 3)
     return headers
 
 def signed_get(path, params = None, login = 0):
     global fox_domain, debug_setting, http_timeout, http_tries, response_time
-    if debug_setting > 2:
-        output(f"params = {params}")
+    output(f"params = {params}", 3)
     message = None
     for i in range(0, http_tries):
         headers = signed_header(path, login)
         try:
             t_now = time.time()
             response = requests.get(url=fox_domain + path, headers=headers, params=params, timeout=http_timeout)
             response_time[path] = time.time() - t_now
             return response
         except Exception as e:
             message = str(e)
-            if debug_setting > 0:
-                output(f"** signed_get(): {message}\n  path = {path}\n  headers = {headers}")
+            output(f"** signed_get(): {message}\n  path = {path}\n  headers = {headers}")
             continue
     return MockResponse(999, message)
 
 def signed_post(path, body = None, login = 0):
     global fox_domain, debug_setting, http_timeout, http_tries, response_time
     data = json.dumps(body)
-    if debug_setting > 2:
-        output(f"body = {data}")
+    output(f"body = {data}", 3)
     message = None
     for i in range(0, http_tries):
         headers = signed_header(path, login)
         try:
             t_now = time.time()
             response = requests.post(url=fox_domain + path, headers=headers, data=data, timeout=http_timeout)
             response_time[path] = time.time() - t_now
             return response
         except Exception as e:
             message = str(e)
-            if debug_setting > 0:
-                output(f"** signed_post(): {message}\n  path = {path}\n  headers = {headers}")
+            output(f"** signed_post(): {message}\n  path = {path}\n  headers = {headers}")
             continue
     return MockResponse(999, message)
 
 
 ##################################################################################################
 # get error messages / error handling
 ##################################################################################################
 
 messages = None
 
 def get_messages():
     global debug_setting, messages, user_agent
-    if debug_setting > 1:
-        output(f"getting messages")
+    output(f"getting messages", 2)
     headers = {'User-Agent': user_agent, 'Content-Type': 'application/json;charset=UTF-8', 'Connection': 'keep-alive'}
     response = signed_get(path="/c/v0/errors/message", login=1)
     if response.status_code != 200:
         output(f"** get_messages() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -239,16 +233,15 @@
 ##################################################################################################
 
 def get_access_count():
     global debug_setting, messages, lang
     if api_key is None:
         output(f"** please generate an API Key at foxesscloud.com and provide this (f.api_key='your API key')")
         return None
-    if debug_setting > 1:
-        output(f"getting access info")
+    output(f"getting access info", 2)
     response = signed_get(path="/op/v0/user/getAccessCount")
     if response.status_code != 200:
         output(f"** get_access_count() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
         output(f"** get_access_count(), no result data, {errno_message(response)}")
@@ -267,16 +260,15 @@
     if api_key is None:
         output(f"** please generate an API Key at foxesscloud.com and provide this (f.api_key='your API key')")
         return None
     if messages is None:
         get_messages()
     if var_list is not None:
         return var_list
-    if debug_setting > 1:
-        output(f"getting variables")
+    output(f"getting variables", 2)
     response = signed_get(path="/op/v0/device/variable/get")
     if response.status_code != 200:
         output(f"** get_vars() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
         output(f"** get_vars(), no result data, {errno_message(response)}")
@@ -298,16 +290,15 @@
 
 def get_site(name=None):
     global site_list, site, debug_setting, station_id
     if get_vars() is None:
         return None
     if site is not None and name is None:
         return site
-    if debug_setting > 1:
-        output(f"getting sites")
+    output(f"getting sites", 2)
     site = None
     station_id = None
     body = {'currentPage': 1, 'pageSize': 100 }
     response = signed_post(path="/op/v0/plant/list", body=body)
     if response.status_code != 200:
         output(f"** get_sites() got list response code {response.status_code}: {response.reason}")
         return None
@@ -358,16 +349,15 @@
 
 def get_logger(sn=None):
     global logger_list, logger, debug_setting
     if get_vars() is None:
         return None
     if logger is not None and sn is None:
         return logger
-    if debug_setting > 1:
-        output(f"getting loggers")
+    output(f"getting loggers", 2)
     body = {'pageSize': 100, 'currentPage': 1}
     response = signed_post(path="/op/v0/module/list", body=body)
     if response.status_code != 200:
         output(f"** get_logger() got list response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -408,16 +398,15 @@
     if get_vars() is None:
         return None
     if device is not None:
         if sn is None:
             return device
         if device_sn[:len(sn)].upper() == sn.upper():
             return device
-    if debug_setting > 1:
-        output(f"getting device")
+    output(f"getting device", 2)
     if sn is None and device_sn is not None and len(device_sn) == 15:
         sn = device_sn
     # get device list
     body = {'pageSize': 100, 'currentPage': 1}
     response = signed_post(path="/op/v0/device/list", body=body)
     if response.status_code != 200:
         output(f"** get_device() list got response code {response.status_code}: {response.reason}")
@@ -500,16 +489,15 @@
 # get generation info and save to device
 ##################################################################################################
 
 def get_generation(update=1):
     global device_sn, device
     if get_device() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting generation")
+    output(f"getting generation", 2)
     params = {'sn': device_sn}
     response = signed_get(path="/op/v0/device/generation", params=params)
     if response.status_code != 200:
         output(f"** get_generation() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -531,16 +519,15 @@
 battery_vars = ['SoC', 'invBatVolt', 'invBatCurrent', 'invBatPower', 'batTemperature', 'ResidualEnergy' ]
 battery_data = ['soc', 'volt', 'current', 'power', 'temperature', 'residual']
 
 def get_battery(v = None):
     global device_sn, battery, debug_setting, residual_scaling
     if get_device() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting battery")
+    output(f"getting battery", 2)
     if v is None:
         v = battery_vars
     result = get_real(v)
     if battery is None:
         battery = {}
     for i in range(0, len(battery_vars)):
         battery[battery_data[i]] = result[i].get('value')
@@ -552,16 +539,15 @@
 
 def get_charge():
     global token, device_sn, battery_settings, debug_setting
     if get_device() is None:
         return None
     if battery_settings is None:
         battery_settings = {}
-    if debug_setting > 1:
-        output(f"getting charge times")
+    output(f"getting charge times", 2)
     params = {'sn': device_sn}
     response = signed_get(path="/op/v0/device/battery/forceChargeTime/get", params=params)
     if response.status_code != 200:
         output(f"** get_charge() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -626,18 +612,17 @@
             st2 = round_time(time_hours(st2) + adjust)
             en2 = round_time(time_hours(en2) + adjust)
         battery_settings['times']['enable2'] = True if ch2 == True or ch2 == 1 else False
         battery_settings['times']['startTime2']['hour'] = int(st2)
         battery_settings['times']['startTime2']['minute'] = int(60 * (st2 - int(st2)) + 0.5)
         battery_settings['times']['endTime2']['hour'] = int(en2)
         battery_settings['times']['endTime2']['minute'] = int(60 * (en2 - int(en2)) + 0.5)
-    if debug_setting > 0:
-        output(f"\nSetting time periods:")
-        output(f"   Time Period 1 = {time_period(battery_settings['times'], 1)}")
-        output(f"   Time Period 2 = {time_period(battery_settings['times'], 2)}")
+    output(f"\nSetting time periods:", 1)
+    output(f"   Time Period 1 = {time_period(battery_settings['times'], 1)}", 1)
+    output(f"   Time Period 2 = {time_period(battery_settings['times'], 2)}", 1)
     # set charge times
     body = {'sn': device_sn}
     for k in ['enable1', 'startTime1', 'endTime1', 'enable2', 'startTime2', 'endTime2']:
         body[k] = battery_settings['times'][k]          # try forcing order of items?
     response = signed_post(path="/op/v0/device/battery/forceChargeTime/set", body=body)
     if response.status_code != 200:
         output(f"** set_charge() got response code {response.status_code}: {response.reason}")
@@ -645,30 +630,29 @@
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
             output(f"** set_charge(), cannot update settings when schedule is active")
         else:
             output(f"** set_charge(), {errno_message(response)}")
         return None
-    elif debug_setting > 1:
-        output(f"success") 
+    else:
+        output(f"success", 2) 
     return battery_settings
 
 ##################################################################################################
 # get min soc settings and save in battery_settings
 ##################################################################################################
 
 def get_min():
     global token, device_sn, battery_settings, debug_setting
     if get_device() is None:
         return None
     if battery_settings is None:
         battery_settings = {}
-    if debug_setting > 1:
-        output(f"getting min soc")
+    output(f"getting min soc", 2)
     params = {'sn': device_sn}
     response = signed_get(path="/op/v0/device/battery/soc/get", params=params)
     if response.status_code != 200:
         output(f"** get_min() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -707,16 +691,15 @@
         output(f"set_min(): {battery_settings}")
         return None
     body = {'sn': device_sn}
     if battery_settings.get('minSocOnGrid') is not None:
         body['minSocOnGrid'] = battery_settings['minSocOnGrid']
     if battery_settings.get('minSoc') is not None:
         body['minSoc'] = battery_settings['minSoc']
-    if debug_setting > 0:
-        output(f"\nSetting minSoc = {battery_settings.get('minSoc')}, minSocOnGrid = {battery_settings.get('minSocOnGrid')}")
+    output(f"\nSetting minSoc = {battery_settings.get('minSoc')}, minSocOnGrid = {battery_settings.get('minSocOnGrid')}", 1)
     response = signed_post(path="/op/v0/device/battery/soc/set", body=body)
     if response.status_code != 200:
         output(f"** set_min() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
         if errno == 44096:
@@ -765,16 +748,15 @@
 }
 
 def get_ui():
     global device_id, debug_setting, messages, remote_settings, named_settings, merge_settings
     if get_device() is None:
         return None
     if remote_settings is None:
-        if debug_setting > 1:
-            output(f"getting ui settings")
+        output(f"getting ui settings", 2)
         params = {'id': device_id}
         response = signed_get(path="/generic/v0/device/setting/ui", params=params)
         if response.status_code != 200:
             output(f"** get_ui() got response code {response.status_code}: {response.reason}")
             return None
         result = response.json().get('result')
         if result is None:
@@ -784,21 +766,23 @@
         remote_settings = result
         protocol = remote_settings['protocol'].lower().replace('xx','__')
         named_settings = {'_protocol': protocol}
         volt_n = 0
         volt_keys = []
         for p in remote_settings['parameters']:
             if p['name'][:11] == 'BatteryVolt':    # merge BatteryVolts
+                output(f"  found {p['name']} with key {p['key']}", 2)
                 volt_n += 1
                 volt_keys.append(p['key'])
                 if volt_n == 3:
                     named_settings['BatteryVolt'] = {'keys': volt_keys, 'type': 'list', 'valueType': 'float', 'unit': p['properties'][0]['unit']}
                 elif volt_n > 3:
-                    print(f"** get_ui(): more than 3 groups found for BatteryVolt")
+                    print(f"** get_ui(): more than 3 groups found for BatteryVolt, n={volt_n}")
             elif p['name'][:11] == 'BatteryTemp':
+                output(f"  found {p['name']} with key {p['key']}", 2)
                 named_settings['BatteryTemp'] = {'keys': p['key'], 'type': 'list', 'valueType': 'int', 'unit': p['properties'][0]['unit']}
             else:
                 items = []
                 block = p['block'] and len(p['properties']) > 1
                 for e in p['properties']:
                     valueType = e['elemType']['valueType']
                     item = {'name': e['key'].replace(protocol,'')} if block else {'key': e['key']} #, 'group': p['name']}
@@ -825,16 +809,15 @@
                         named_settings[name][k] = merge_settings[name][k]
     return remote_settings
 
 def get_remote_settings(key):
     global token, device_id, debug_setting, messages
     if get_device() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting remote settings")
+    output(f"getting remote settings", 2)
     if key is None:
         return None
     if type(key) is list:
         values = {}
         for k in key:
             v = get_remote_settings(k)
             if v is None:
@@ -868,14 +851,15 @@
     if named_settings is None or named_settings.get(name) is None:
         output(f"** get_named_settings(): {name} was not recognised")
         return None
     keys = named_settings[name].get('keys')
     if keys is None:
         output(f"** get_named_settings(): no keys for name: {name}")
         return None
+    output(f"getting named_settings for {name} using {keys}", 2)
     result = get_remote_settings(keys)
     if result is None:
         output(f"** get_named_settings(): no result for {name} using key: {keys}")
         return None
     result_type = named_settings[name].get('type')
     value_type = named_settings[name].get('valueType')
     if result_type is None:
@@ -952,16 +936,15 @@
         if force == 0:
             output(f"** set_work_mode(): cannot set work mode when a schedule is enabled")
             return None
         set_schedule(enable=0)
     if debug_setting > 1:
         output(f"set_work_mode(): {mode}")
         return None
-    if debug_setting > 0:
-        output(f"\nSetting work mode: {mode}")
+    output(f"\nSetting work mode: {mode}", 1)
     body = {'sn': device_sn, 'key': 'operation_mode__work_mode', 'values': {'operation_mode__work_mode': mode}, 'raw': ''}
     response = signed_post(path="/op/v0/device/setting/set", body=body)
     if response.status_code != 200:
         output(f"** set_work_mode() got response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
@@ -984,16 +967,15 @@
 def get_flag():
     global device_sn, schedule, debug_setting
     if get_device() is None:
         return None
     if device.get('function') is None or device['function'].get('scheduler') is None or device['function']['scheduler'] == False:
         output(f"** get_schedule() schedules are not supported")
         return None
-    if debug_setting > 1:
-        output(f"getting flag")
+    output(f"getting flag", 2)
     body = {'deviceSN': device_sn}
     response = signed_post(path="/op/v0/device/scheduler/get/flag", body=body)
     if response.status_code != 200:
         output(f"** get_flag() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -1010,16 +992,15 @@
 ##################################################################################################
 
 # get the current schedule
 def get_schedule():
     global device_sn, schedule, debug_setting, work_modes
     if get_flag() is None:
         return None
-    if debug_setting > 1:
-        output(f"getting schedule")
+    output(f"getting schedule", 2)
     body = {'deviceSN': device_sn}
     response = signed_post(path="/op/v0/device/scheduler/get", body=body)
     if response.status_code != 200:
         output(f"** get_schedule() got response code {response.status_code}: {response.reason}")
         return None
     result = response.json().get('result')
     if result is None:
@@ -1061,34 +1042,32 @@
     return group
 
 # set a schedule from a period or list of time segment groups
 def set_schedule(enable=1, groups=None):
     global token, device_sn, debug_setting, schedule
     if get_flag() is None:
         return None
+    output(f"set_schedule(): enable = {enable}, groups = {groups}", 2)
     if debug_setting > 1:
-        output(f"set_schedule(): enable = {enable}, groups = {groups}")
         return None
     if groups is not None:
         if type(groups) is not list:
             groups = [groups]
         body = {'deviceSN': device_sn, 'groups': groups}
-        if debug_setting > 0:
-            output(f"\nSaving schedule")
+        output(f"\nSaving schedule", 1)
         response = signed_post(path="/op/v0/device/scheduler/enable", body=body)
         if response.status_code != 200:
             output(f"** set_schedule() groups response code {response.status_code}: {response.reason}")
             return None
         errno = response.json().get('errno')
         if errno != 0:
             output(f"** set_schedule(), enable, {errno_message(response)}")
             return None
         schedule['groups'] = groups
-    if debug_setting > 0:
-        output(f"\nSetting schedule enable flag to {enable}")
+    output(f"\nSetting schedule enable flag to {enable}", 1)
     body = {'deviceSN': device_sn, 'enable': enable}
     response = signed_post(path="/op/v0/device/scheduler/set/flag", body=body)
     if response.status_code != 200:
         output(f"** set_schedule() flag response code {response.status_code}: {response.reason}")
         return None
     errno = response.json().get('errno')
     if errno != 0:
@@ -1111,16 +1090,15 @@
     if get_device() is None:
         return None
     if device['status'] > 1:
         status_code = device['status']
         state = 'fault' if status_code == 2 else 'off-line' if status_code == 3 else 'unknown'
         output(f"** get_real(): device {device_sn} is not on-line, status = {state} ({device['status']})")
         return None
-    if debug_setting > 1:
-        output(f"getting real-time data")
+    output(f"getting real-time data", 2)
     body = {'deviceSN': device_sn}
     if v is not None:
         body['variables'] = v if type(v) is list else [v]
     response = signed_post(path="/op/v0/device/real/query", body=body)
     if response.status_code != 200:
         output(f"** get_real() got response code {response.status_code}: {response.reason}")
         return None
@@ -1191,16 +1169,15 @@
     elif type(v) is not list:
         v = [v]
     for var in v:
         if var not in var_list:
             output(f"** get_history(): invalid variable '{var}'")
             output(f"var_list = {var_list}")
             return None
-    if debug_setting > 1:
-        output(f"getting history data")
+    output(f"getting history data", 2)
     if load is None:
         (t_begin, t_end) = query_time(d, time_span)
         if t_begin is None:
             return None
         body = {'sn': device_sn, 'variables': v, 'begin': t_begin, 'end': t_end}
         response = signed_post(path="/op/v0/device/history/query", body=body)
         if response.status_code != 200:
@@ -1236,16 +1213,15 @@
         elif var.get('unit') is None:
             var['unit'] = ''
     if summary <= 0 or time_span == 'hour':
         if plot > 0:
             plot_history(result, plot)
         return result
     # integrate kW to kWh based on 5 minute samples
-    if debug_setting > 2:
-        output(f"calculating summary data")
+    output(f"calculating summary data", 3)
     # copy generationPower to produce inputPower data
     input_name = None
     if 'generationPower' in v:
         input_name = energy_vars[-1]
         input_result = deepcopy(result[v.index('generationPower')])
         input_result['name'] = input_name
         for y in input_result['data']:
@@ -1259,30 +1235,28 @@
             kwh_off = 0.0   # kwh during off peak time (02:00-05:00)
             kwh_peak = 0.0  # kwh during peak time (16:00-19:00)
             kwh_neg = 0.0
             if len(var['data']) > 1:
                 sample_time = round(60 * sample_rounding * (time_hours(var['data'][-1]['time'][11:]) - time_hours(var['data'][0]['time'][11:])) / (len(var['data']) - 1), 0) / sample_rounding
             else:
                 sample_time = 5.0
-            if debug_setting > 1:
-                output(f"{var['variable']}: samples = {len(var['data'])}, sample_time = {sample_time} minutes")
+            output(f"{var['variable']}: samples = {len(var['data'])}, sample_time = {sample_time} minutes", 2)
         sum = 0.0
         count = 0
         max = None
         max_time = None
         min = None
         min_time = None
         if summary == 3 and energy:
             var['state'] = [{}]
         for y in var['data']:
             h = time_hours(y['time'][11:19]) # time
             value = y['value']
             if value is None:
-                if debug_setting > 0:
-                    output(f"** get_history(), warning: missing data for {var['variable']} at {y['time']}")
+                output(f"** get_history(), warning: missing data for {var['variable']} at {y['time']}", 1)
                 continue
             sum += value
             count += 1
             max = value if max is None or value > max else max
             min = value if min is None or value < min else min
             if energy:
                 e = value * sample_time / 60      # convert kW samples to kWh energy
@@ -1431,16 +1405,15 @@
     elif type(v) is not list:
         v = [v]
     for var in v:
         if var not in report_vars:
             output(f"** get_report(): invalid variable '{var}'")
             output(f"{report_vars}")
             return None
-    if debug_setting > 1:
-        output(f"getting report data")
+    output(f"getting report data", 2)
     current_date = query_date(None)
     main_date = query_date(d)
     if main_date is None:
         return None
     side_result = None
     if dimension in ('day', 'week') and summary > 0:
         # side report needed
@@ -1524,16 +1497,15 @@
     for i, var in enumerate(result):
         count = 0
         sum = 0.0
         max = None
         min = None
         for j, value in enumerate(var['values']):
             if value is None:
-                if debug_setting > 0:
-                    output(f"** get_report(), warning: missing data for {var['variable']} on {d} at index {j}")
+                output(f"** get_report(), warning: missing data for {var['variable']} on {d} at index {j}", 1)
                 continue
             count += 1
             sum += value
             max = value if max is None or value > max else max
             min = value if min is None or value < min else min
         # correct day total from side report
         var['total'] = sum if dimension != 'day' else side_result[i]['values'][int(main_date['day'])-1]
@@ -1569,16 +1541,15 @@
             if v['type'] not in types:
                 types.append(v['type'])
             if v['date'] not in dates:
                 dates.append(v['date'])
             for i in range(1, len(v['values'])+1):
                 if i not in index:
                     index.append(i)
-    if debug_setting > 2:
-        output(f"vars = {vars}, dates = {dates}, types = {types}, index = {index}")
+    output(f"vars = {vars}, dates = {dates}, types = {types}, index = {index}", 2)
     if len(vars) == 0:
         return
     # plot variables by date with the same units on the same charts
     lines = 0
     width = 0.8 / (len(dates) if plot == 1 else len(vars) if len(dates) == 1 else len(dates))
     align = 0.0
     for var in vars:
@@ -1893,33 +1864,31 @@
     # adjust system to get local time now
     now = system_time + timedelta(hours=time_offset)
     hour_now = now.hour + now.minute / 60
     update_time = tariff_config['update_time']
     update_time = time_hours(update_time) if type(update_time) is str else 17 if update_time is None else update_time
     today = datetime.strftime(now + timedelta(days=0 if hour_now >= update_time else -1), '%Y-%m-%d')
     tomorrow = datetime.strftime(now + timedelta(days=1 if hour_now >= update_time else 0), '%Y-%m-%d')
-    if debug_setting > 1:
-        output(f"  datetime = {today} {hours_time(hour_now)}")
+    output(f"  datetime = {today} {hours_time(hour_now)}", 2)
     # get product and region
     product = tariff_config['product'].upper()
     region = tariff_config['region'].upper()
     if region not in regions:
         output(f"** region {region} not recognised, valid regions are {regions}")
         return None
     # get prices from 11pm today to 11pm tomorrow
     output(f"\nProduct: {product}")
     output(f"Region:  {regions[region]}")
     zulu_hour = "T" + hours_time(23 - time_offset - time_shift, ss=True) + "Z"
     url = octopus_api_url.replace("%PRODUCT%", product).replace("%REGION%", region)
     period_from = today + zulu_hour
     period_to = tomorrow + zulu_hour
     params = {'period_from': period_from, 'period_to': period_to }
-    if debug_setting > 1:
-        output(f"time_offset = {time_offset}, time_shift = {time_shift}")
-        output(f"period_from = {period_from}, period_to = {period_to}")
+    output(f"time_offset = {time_offset}, time_shift = {time_shift}", 2)
+    output(f"period_from = {period_from}, period_to = {period_to}", 2)
     response = requests.get(url, params=params)
     if response.status_code != 200:
         output(f"** get_agile_period() response code from Octopus API {response.status_code}: {response.reason}")
         return None
     # results are in reverse chronological order...
     results = response.json().get('results')[::-1]
     # extract times and prices
@@ -1931,16 +1900,15 @@
         prices.append(r['value_inc_vat'])
     # work out start and end times for charging
     start_at = time_hours(start_at) if type(start_at) is str else 23.0 if start_at is None else start_at
     end_by = time_hours(end_by) if type(end_by) is str else 8.0 if end_by is None else end_by
     start_i = int(round_time(start_at - 23) * 2)
     end_i = int(round_time(end_by - 23) * 2)
     end_i = 48 if end_i == 0 or end_i > 48 else end_i
-    if debug_setting > 1:
-        output(f"start_at = {start_at}, end_by = {end_by}, start_i = {start_i}, end_i = {end_i}, duration = {duration}, span = {span}")
+    output(f"start_at = {start_at}, end_by = {end_by}, start_i = {start_i}, end_i = {end_i}, duration = {duration}, span = {span}", 2)
     if (start_i + span) > 48 or start_i > end_i:
         output(f"** get_agile_period(): invalid times {hours_time(start_at)} - {hours_time(end_by)}. Must start from 23:00 today and end by 23:00 tomorrow")
         return None
     if len(results) < (start_i + span):
         output(f"** get_agile_period(): prices not available for {tomorrow}")
         return None
     # work out weighted average for each period and track lowest price
@@ -2265,18 +2233,18 @@
     # store settings:
     for key, value in settings.items():
         if key not in charge_config:
             print(f"** unknown configuration parameter: {key}")
         else:
             charge_config[key] = value
             s += f"\n  {key} = {value}"
-    if len(s) > 0 and debug_setting > 1:
-        print(f"Parameters: {s}")
-    if tariff is not None and debug_setting > 1:
-        print(f"  tariff = {tariff['name']}")
+    if len(s) > 0:
+        output(f"Parameters: {s}", 2)
+    if tariff is not None:
+        output(f"  tariff = {tariff['name']}", 2)
     # set default parameters
     show_data = 1 if show_data is None or show_data == True else 0 if show_data == False else show_data
     show_plot = 3 if show_plot is None or show_plot == True else 0 if show_plot == False else show_plot
     run_after = 1 if run_after is None else run_after 
     timed_mode = 1 if timed_mode is None and tariff is not None and tariff.get('work_hours') is not None else 0 if timed_mode is None else timed_mode
     if forecast_times is None:
         forecast_times = tariff['forecast_times'] if tariff is not None and tariff.get('forecast_times') is not None else [22,23]
@@ -2285,16 +2253,15 @@
     # get dates and times
     system_time = (datetime.now(tz=timezone.utc) + timedelta(hours=time_shift)) if test_time is None else datetime.strptime(test_time, '%Y-%m-%d %H:%M')
     time_offset = daylight_saving(system_time) if daylight_saving is not None else 0
     now = system_time + timedelta(hours=time_offset)
     today = datetime.strftime(now, '%Y-%m-%d')
     base_hour = now.hour
     hour_now = now.hour + now.minute / 60
-    if debug_setting > 1:
-        print(f"  datetime = {today} {hours_time(hour_now)}")
+    output(f"  datetime = {today} {hours_time(hour_now)}", 2)
     yesterday = datetime.strftime(now - timedelta(days=1), '%Y-%m-%d')
     tomorrow = datetime.strftime(now + timedelta(days=1), '%Y-%m-%d')
     day_tomorrow = day_names[(now.weekday() + 1) % 7]
     day_after_tomorrow = datetime.strftime(now + timedelta(days=2), '%Y-%m-%d')
     # work out if we lose 1 hour if clocks go forward or gain 1 hour if clocks go back
     change_hour = 0
     hour_adjustment = 0 if daylight_saving is None else daylight_changes(system_time, system_time + timedelta(days=2))
@@ -2336,46 +2303,45 @@
     run_time = int((time_to_am if charge_pm else time_to_am + 24 if time_to_pm is None else time_to_pm) + 0.99) + 1 + hour_adjustment
     # if we need to do a full charge, full_charge is the date, otherwise None
     full_charge = charge_config['full_charge'] if not charge_pm else None
     if type(full_charge) is int:            # value = day of month
         full_charge = tomorrow if full_charge is not None and int(tomorrow[-2:]) == full_charge else None
     elif type(full_charge) is str:          # value = daily or day of week
         full_charge = tomorrow if full_charge.lower() == 'daily' or full_charge.title() == day_tomorrow[:3] else None
-    if debug_setting > 2:
-        print(f"\ntoday = {today}, tomorrow = {tomorrow}, time_shift = {time_shift}")
-        print(f"start_am = {start_am}, end_am = {end_am}, force_am = {force_charge_am}, time_to_am = {time_to_am}")
-        print(f"start_pm = {start_pm}, end_pm = {end_pm}, force_pm = {force_charge_pm}, time_to_pm = {time_to_pm}")
-        print(f"start_at = {start_at}, end_by = {end_by}, force_charge = {force_charge}")
-        print(f"base_hour = {base_hour}, hour_adjustment = {hour_adjustment}, change_hour = {change_hour}")
-        print(f"time_to_start = {time_to_start}, run_time = {run_time}, charge_pm = {charge_pm}")
-        print(f"start_hour = {start_hour}, time_to_next = {time_to_next}, full_charge = {full_charge}")
+    output(f"\ntoday = {today}, tomorrow = {tomorrow}, time_shift = {time_shift}", 3)
+    output(f"start_am = {start_am}, end_am = {end_am}, force_am = {force_charge_am}, time_to_am = {time_to_am}", 3)
+    output(f"start_pm = {start_pm}, end_pm = {end_pm}, force_pm = {force_charge_pm}, time_to_pm = {time_to_pm}", 3)
+    output(f"start_at = {start_at}, end_by = {end_by}, force_charge = {force_charge}", 3)
+    output(f"base_hour = {base_hour}, hour_adjustment = {hour_adjustment}, change_hour = {change_hour}", 3)
+    output(f"time_to_start = {time_to_start}, run_time = {run_time}, charge_pm = {charge_pm}", 3)
+    output(f"start_hour = {start_hour}, time_to_next = {time_to_next}, full_charge = {full_charge}", 3)
     # get device and battery info from inverter
     if test_soc is None:
         if charge_config.get('min_soc') is not None:
             min_soc = charge_config['min_soc']
         else:
             get_min()
             if battery_settings.get('minSocOnGrid') is not None:
                 min_soc = battery_settings['minSocOnGrid']
             else:
-                print(f"\nMin SoC On Grid is not available. Please provide % via 'min_soc' parameter")
+                output(f"\nMin SoC On Grid is not available. Please provide % via 'min_soc' parameter")
                 return None
         get_battery()
         current_soc = battery['soc']
         bat_volt = battery['volt']
         bat_power = battery['power']
         bat_current = battery['current']
         temperature = battery['temperature']
         residual = battery['residual']
         if charge_config.get('capacity') is not None:
             capacity = charge_config['capacity']
         elif residual is not None and residual > 0.2 and current_soc is not None and current_soc > 1:
             capacity = residual * 100 / current_soc
         else:
-            print(f"Battery capacity could not be estimated. Please add the parameter 'capacity=xx' in kWh")
+            output(f"Battery capacity could not be estimated. Please add the parameter 'capacity=xx' in kWh")
             return None
     else:
         current_soc = test_soc
         capacity = 8.2
         residual = test_soc * capacity / 100
         min_soc = 10
         bat_volt = 122 / (1 + 0.03 * (100 - test_soc) / 90)
@@ -2384,56 +2350,56 @@
         bat_current = 0.0
     volt_curve = charge_config['volt_curve']
     nominal_soc = charge_config['nominal_soc']
     volt_nominal = interpolate(nominal_soc / 10, volt_curve)
     bat_resistance = charge_config['bat_resistance'] * bat_volt / volt_nominal
     bat_ocv = (bat_volt + bat_current * bat_resistance) * volt_nominal / interpolate(current_soc / 10, volt_curve)
     reserve = capacity * min_soc / 100
-    print(f"\nBattery Info:")
-    print(f"  Capacity:    {capacity:.1f}kWh")
-    print(f"  Residual:    {residual:.1f}kWh")
-    print(f"  Voltage:     {bat_volt:.1f}V")
-    print(f"  Current:     {bat_current:.1f}A")
-    print(f"  State:       {'Charging' if bat_power < 0 else 'Discharging'} ({abs(bat_power):.3f}kW)")
-    print(f"  Current SoC: {current_soc}%")
-    print(f"  Min SoC:     {min_soc}% ({reserve:.1f}kWh)")
-    print(f"  Temperature: {temperature:.1f}°C")
-    print(f"  Resistance:  {bat_resistance:.2f} ohms")
-    print(f"  Nominal OCV: {bat_ocv:.1f}V at {nominal_soc}% SoC")
+    output(f"\nBattery Info:")
+    output(f"  Capacity:    {capacity:.1f}kWh")
+    output(f"  Residual:    {residual:.1f}kWh")
+    output(f"  Voltage:     {bat_volt:.1f}V")
+    output(f"  Current:     {bat_current:.1f}A")
+    output(f"  State:       {'Charging' if bat_power < 0 else 'Discharging'} ({abs(bat_power):.3f}kW)")
+    output(f"  Current SoC: {current_soc}%")
+    output(f"  Min SoC:     {min_soc}% ({reserve:.1f}kWh)")
+    output(f"  Temperature: {temperature:.1f}°C")
+    output(f"  Resistance:  {bat_resistance:.2f} ohms")
+    output(f"  Nominal OCV: {bat_ocv:.1f}V at {nominal_soc}% SoC")
     # get power and charge current for device
     device_power = device.get('power')
     device_current = device.get('max_charge_current')
     model = device.get('deviceType') if device.get('deviceType') is not None else 'unknown'
     if device_power is None or device_current is None:
-        print(f"** could not get parameters for {model} inverter, using default rating of 3.68kW")
+        output(f"** could not get parameters for {model} inverter, using default rating of 3.68kW")
         device_power = 3.68
         device_current = 26
     # charge times are derated based on temperature
     charge_current = device_current if charge_config['charge_current'] is None else charge_config['charge_current']
     derate_temp = charge_config['derate_temp']
     if temperature > 36:
-        print(f"\nHigh battery temperature may affect the charge rate")
+        output(f"\nHigh battery temperature may affect the charge rate")
     elif round(temperature, 0) <= derate_temp:
-        print(f"\nLow battery temperature may affect the charge rate")
+        output(f"\nLow battery temperature may affect the charge rate")
         derating = charge_config['derating']
         derate_step = charge_config['derate_step']
         i = int((derate_temp - temperature) / (derate_step if derate_step is not None and derate_step > 0 else 1))
         if derating is not None and type(derating) is list and i < len(derating):
             derated_current = derating[i]
             if derated_current < charge_current:
-                print(f"  Charge current reduced from {charge_current:.0f}A to {derated_current:.0f}A" )
+                output(f"  Charge current reduced from {charge_current:.0f}A to {derated_current:.0f}A" )
                 charge_current = derated_current
         else:
             force_charge = 2
-            print(f"  Full charge set")
+            output(f"  Full charge set")
     # work out charge limit = max power going into the battery after ac conversion losses
     charge_limit = device_power * charge_config['grid_loss']
     charge_power = charge_current * (bat_ocv + charge_current * bat_resistance) / 1000
     if charge_power < 0.1:
-        print(f"** charge_current is too low ({charge_current:.1f}A)")
+        output(f"** charge_current is too low ({charge_current:.1f}A)")
     elif charge_power < charge_limit:
         charge_limit = charge_power
     # work out losses when charging / force discharging
     inverter_power = charge_config['inverter_power'] if charge_config['inverter_power'] is not None else round(device_power, 0) * 20
     operating_loss = inverter_power / 1000
     bms_power = charge_config['bms_power']
     bms_loss = bms_power / 1000
@@ -2446,46 +2412,45 @@
     discharge_current = device_current if charge_config['discharge_current'] is None else charge_config['discharge_current']
     discharge_power = discharge_current * bat_ocv / 1000
     discharge_limit = discharge_power if discharge_power < discharge_limit else discharge_limit
     # charging happens if generation exceeds export limit in feedin work mode
     export_power = device_power if charge_config['export_limit'] is None else charge_config['export_limit']
     export_limit = export_power / discharge_loss
     current_mode = get_work_mode()
-    if debug_setting > 2:
-        print(f"\ncharge_config = {json.dumps(charge_config, indent=2)}")
-    print(f"\nDevice Info:")
-    print(f"  Model:     {model}")
-    print(f"  Rating:    {device_power:.2f}kW")
-    print(f"  Export:    {export_power:.2f}kW")
-    print(f"  Charge:    {charge_current:.1f}A, {charge_limit:.2f}kW, {charge_loss * 100:.1f}% efficient")
-    print(f"  Discharge: {discharge_current:.1f}A, {discharge_limit:.2f}kW, {discharge_loss * 100:.1f}% efficient")
-    print(f"  Inverter:  {inverter_power:.0f}W power consumption")
-    print(f"  BMS:       {bms_power:.0f}W power consumption")
+    output(f"\ncharge_config = {json.dumps(charge_config, indent=2)}", 3)
+    output(f"\nDevice Info:")
+    output(f"  Model:     {model}")
+    output(f"  Rating:    {device_power:.2f}kW")
+    output(f"  Export:    {export_power:.2f}kW")
+    output(f"  Charge:    {charge_current:.1f}A, {charge_limit:.2f}kW, {charge_loss * 100:.1f}% efficient")
+    output(f"  Discharge: {discharge_current:.1f}A, {discharge_limit:.2f}kW, {discharge_loss * 100:.1f}% efficient")
+    output(f"  Inverter:  {inverter_power:.0f}W power consumption")
+    output(f"  BMS:       {bms_power:.0f}W power consumption")
     if current_mode is not None:
-        print(f"  Work Mode: {current_mode}")
+        output(f"  Work Mode: {current_mode}")
     # get consumption data
     annual_consumption = charge_config['annual_consumption']
     if annual_consumption is not None:
         consumption = annual_consumption / 365 * seasonality[now.month - 1] / sum(seasonality) * 12
         consumption_by_hour = daily_consumption
-        print(f"\nEstimated consumption: {consumption:.1f}kWh")
+        output(f"\nEstimated consumption: {consumption:.1f}kWh")
     else:
         consumption_days = charge_config['consumption_days']
         consumption_days = 3 if consumption_days > 7 or consumption_days < 1 else consumption_days
         consumption_span = charge_config['consumption_span']
         if consumption_span == 'weekday':
             history = get_report('day', d=date_list(span='weekday', e=tomorrow, today=2)[-consumption_days-1:-1], v='loads')
         else:
             last_date = today if hour_now >= charge_config['use_today'] else yesterday
             history = get_report('day', d=date_list(span='week', e=last_date, today=1)[-consumption_days:], v='loads')
         (consumption, consumption_by_hour) = report_value_profile(history)
         if consumption is None:
-            print(f"No consumption data available")
+            output(f"No consumption data available")
             return None
-        print(f"\nConsumption (kWh):")
+        output(f"\nConsumption (kWh):")
         s = ""
         for h in history:
             s += f"  {h['date']}: {h['total']:4.1f},"
         print(s[:-1])
         print(f"  Average of last {consumption_days} {day_tomorrow if consumption_span=='weekday' else 'day'}s: {consumption:.1f}kWh")
     # time line has 1 hour buckets of consumption
     daily_sum = sum(consumption_by_hour)
@@ -2495,103 +2460,99 @@
     solcast_profile = None
     if forecast is None and solcast_api_key is not None and solcast_api_key != 'my.solcast_api_key' and (base_hour in forecast_times or run_after == 0):
         fsolcast = Solcast(quiet=True, estimated=1 if charge_pm else 0)
         if fsolcast is not None and hasattr(fsolcast, 'daily') and fsolcast.daily.get(forecast_day) is not None:
             solcast_value = fsolcast.daily[forecast_day]['kwh']
             solcast_timed = forecast_value_timed(fsolcast, today, tomorrow, hour_now, run_time, time_offset)
             if charge_pm:
-                print(f"\nSolcast forecast for {today} = {fsolcast.daily[today]['kwh']:.1f}, {tomorrow} = {fsolcast.daily[tomorrow]['kwh']:.1f}")
+                output(f"\nSolcast forecast for {today} = {fsolcast.daily[today]['kwh']:.1f}, {tomorrow} = {fsolcast.daily[tomorrow]['kwh']:.1f}")
             else:
-                print(f"\nSolcast forecast for {forecast_day} = {solcast_value:.1f}kWh")
+                output(f"\nSolcast forecast for {forecast_day} = {solcast_value:.1f}kWh")
             adjust = charge_config['solcast_adjust']
             if adjust != 100:
                 solcast_value = solcast_value * adjust / 100
                 solcast_timed = [v * adjust / 100 for v in solcast_timed]
-                print(f"  Adjusted forecast: {solcast_value:.1f}kWh ({adjust}%)")
+                output(f"  Adjusted forecast: {solcast_value:.1f}kWh ({adjust}%)")
     # get forecast.solar data and produce time line
     solar_value = None
     solar_profile = None
     if forecast is None and solar_arrays is not None and (base_hour in forecast_times or run_after == 0):
         fsolar = Solar(quiet=True)
         if fsolar is not None and hasattr(fsolar, 'daily') and fsolar.daily.get(forecast_day) is not None:
             solar_value = fsolar.daily[forecast_day]['kwh']
             solar_timed = forecast_value_timed(fsolar, today, tomorrow, hour_now, run_time, time_offset)
             if charge_pm:
-                print(f"\nSolar forecast for {today} = {fsolar.daily[today]['kwh']:.1f}, {tomorrow} = {fsolar.daily[tomorrow]['kwh']:.1f}")
+                output(f"\nSolar forecast for {today} = {fsolar.daily[today]['kwh']:.1f}, {tomorrow} = {fsolar.daily[tomorrow]['kwh']:.1f}")
             else:
-                print(f"\nSolar forecast for {forecast_day} = {solar_value:.1f}kWh")
+                output(f"\nSolar forecast for {forecast_day} = {solar_value:.1f}kWh")
             adjust = charge_config['solar_adjust']
             if adjust != 100:
                 solar_value = solar_value * adjust / 100
                 solar_timed = [v * adjust / 100 for v in solar_timed]
-                print(f"  Adjusted forecast: {solar_value:.1f}kWh ({adjust}%)")
+                output(f"  Adjusted forecast: {solar_value:.1f}kWh ({adjust}%)")
     if solcast_value is None and solar_value is None and debug_setting > 1:
-        print(f"\nNo forecasts available at this time")
+        output(f"\nNo forecasts available at this time")
     # get generation data
     generation = None
     last_date = today if hour_now >= charge_config['use_today'] else yesterday
     gen_days = charge_config['generation_days']
     history = get_history('week', d=last_date, v=['pvPower','meterPower2'], summary=2)
     pv_history = {}
     if history is not None and len(history) > 0:
         for day in history:
             date = day['date']
             if pv_history.get(date) is None:
                 pv_history[date] = 0.0
             if day.get('kwh') is not None and day.get('kwh_neg') is not None:
                 pv_history[date] += day['kwh_neg'] / 0.92 if day['variable'] == 'meterPower2' else day['kwh']
         pv_sum = sum([pv_history[d] for d in sorted(pv_history.keys())[-gen_days:]])
-        print(f"\nGeneration (kWh):")
+        output(f"\nGeneration (kWh):")
         s = ""
         for d in sorted(pv_history.keys())[-gen_days:]:
             s += f"  {d}: {pv_history[d]:4.1f},"
         print(s[:-1])
         generation = pv_sum / gen_days
-        print(f"  Average of last {gen_days} days: {generation:.1f}kWh")
+        output(f"  Average of last {gen_days} days: {generation:.1f}kWh")
     # choose expected value and produce generation time line
     quarter = now.month // 3 % 4
     sun_name = seasonal_sun[quarter]['name']
     sun_profile = seasonal_sun[quarter]['sun']
     sun_sum = sum(sun_profile)
     sun_timed = timed_list(sun_profile, hour_now, run_time)
+    output_spool(charge_needed_app_key)
     if forecast is not None:
         expected = forecast
         generation_timed = [expected * x / sun_sum for x in sun_timed]
-        output(f"\nUsing {expected:.1f}kWh manual forecast with {sun_name} sun and {consumption:.1f}kWh consumption")
     elif solcast_value is not None:
         expected = solcast_value
         generation_timed = solcast_timed
-        output(f"\nUsing {expected:.1f}kWh Solcast forecast and {consumption:.1f}kWh consumption for {forecast_day}")
     elif solar_value is not None:
         expected = solar_value
         generation_timed = solar_timed
-        output(f"\nUsing {expected:.1f}kWh Solar forecast and {consumption:.1f}kWh consumption for {forecast_day}")
     elif generation is None or generation == 0.0:
         output(f"\nNo generation data available")
         output_close()
         return None
     else:
         expected = generation
         generation_timed = [expected * x / sun_sum for x in sun_timed]
-        output(f"\nUsing {expected:.1f}kWh generation with {sun_name} sun and {consumption:.1f}kWh consumption")
         if charge_config['forecast_selection'] == 1 and update_settings > 0:
-            output(f"  Settings will not be updated when forecast is not available")
+            output(f"\nSettings will not be updated when forecast is not available")
             update_settings = 2 if update_settings == 3 else 0
     # produce time lines for main charge and discharge (after losses)
     charge_timed = [x * charge_config['pv_loss'] for x in generation_timed]
     discharge_timed = [x / charge_config['discharge_loss'] for x in consumption_timed]
     # adjust charge and discharge time lines for work mode, force charge and power limits
     work_mode = current_mode
     for i in range(0, run_time):
         h = base_hour + i
         # get work mode and check for changes
         new_work_mode = timed_work_mode(h, current_mode) if timed_mode == 1 else current_mode
         if new_work_mode is not None and new_work_mode != work_mode:
-            if debug_setting > 1:
-                output(f"  {hours_time(h)}: {new_work_mode} work mode")
+            output(f"  {hours_time(h)}: {new_work_mode} work mode", 2)
             work_mode = new_work_mode
         # cap charge / discharge power
         charge_timed[i] = charge_limit if charge_timed[i] > charge_limit else charge_timed[i]
         discharge_timed[i] = discharge_limit if discharge_timed[i] > discharge_limit else discharge_timed[i]
         if force_charge_am == 1 and hour_in(h, {'start': start_am, 'end': end_am}):
             discharge_timed[i] = operating_loss if charge_timed[i] == 0.0 else 0.0
         elif force_charge_pm == 1 and hour_in(h, {'start': start_pm, 'end': end_pm}):
@@ -2628,35 +2589,34 @@
         bat_timed.append(kwh_current)
         if kwh_current < kwh_min:       # track minimum and time
             kwh_min = kwh_current
             min_hour = h
         kwh_current += kwh_timed[i]
         h += 1
     # work out what we need to add to stay above reserve and provide contingency or to hit target_soc
-    output_spool(charge_needed_app_key)
     contingency = charge_config['special_contingency'] if tomorrow[-5:] in charge_config['special_days'] else charge_config['contingency']
     kwh_contingency = consumption * contingency / 100
     kwh_needed = reserve + kwh_contingency - kwh_min
     start_residual = interpolate(time_to_start, bat_timed)      # residual when charging starts
     target_soc = charge_config['target_soc'] if charge_config.get('target_soc') is not None else 0
     target_kwh = capacity if target_soc > 100 else target_soc / 100 * capacity
     if target_kwh > (start_residual + kwh_needed):
         kwh_needed = target_kwh - start_residual
     day_when = 'today' if min_hour < 24 else 'tomorrow' if min_hour <= 48 else 'day after tomorrow'
     if kwh_min > reserve and kwh_needed < charge_config['min_kwh'] and full_charge is None and test_charge is None:
-        output(f"\nNo charging is needed")
+        output(f"\nNo charging is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
         charge_message = "no charge needed"
         kwh_needed = 0.0
         hours = 0.0
         end1 = start_at
     else:
         charge_message = "with charge added"
         if test_charge is None:
             min_hour_adjust = min_hour - hour_adjustment if min_hour >= change_hour else 0
-            output(f"\nCharge of {kwh_needed:.2f}kWh is needed")
+            output(f"\nCharge of {kwh_needed:.2f}kWh is needed (forecast = {expected:.1f}kWh, consumption = {consumption:.1f}kWh)")
         else:
             output(f"\nTest charge of {test_charge}kWh")
             charge_message = "** test charge **"
             kwh_needed = test_charge
         # work out time to add kwh_needed to battery
         taper_time = 10/60 if (start_residual + kwh_needed) >= (capacity * 0.95) else 0
         hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
@@ -2665,15 +2625,15 @@
             kwh_needed = capacity - start_residual
             hours = round_time(kwh_needed / (charge_limit * charge_loss + discharge_timed[time_to_next]) + taper_time)
             if full_charge is not None or force_charge == 2 or hours > charge_time:
                 hours = charge_time
                 output(f"  Full charge time used")
         elif hours < charge_config['min_hours']:
             hours = charge_config['min_hours']
-            output(f"  Minimum charge time used")
+#            output(f"  Minimum charge time used")
         end1 = round_time(start_at + hours)
         # rework charge and discharge and work out grid consumption
         start_timed = time_to_start      # relative start and end time 
         end_timed = start_timed + hours
         charge_timed_old = [x for x in charge_timed]
         discharge_timed_old = [x for x in discharge_timed]
         for i in range(time_to_next, int(time_to_next + hours + 2)):
@@ -2685,16 +2645,15 @@
                 t = j - start_timed                 # start this hour but not end
             elif end_timed > i and end_timed <= j and start_timed <= i:
                 t = end_timed - i                   # end this hour but not start
             elif start_timed <= i and end_timed > j:
                 t = 1.0                             # complete hour inside start and end
             else:
                 t = 0.0                             # complete hour before start or after end
-            if debug_setting > 2:
-                output(f"i = {i}, j = {j}, t = {t}")
+            output(f"i = {i}, j = {j}, t = {t}", 3)
             charge_added = charge_limit * t
             charge_timed[i] = charge_timed[i] + charge_added if charge_timed[i] + charge_added < charge_limit else charge_limit
             discharge_timed[i] *= (1-t)
         # rebuild the battery residual with the charge added
         # adjust residual from hour_now to what it was at the start of current hour
         h = base_hour
         kwh_timed = [charge * charge_loss - discharge for charge, discharge in zip(charge_timed, discharge_timed)]
@@ -2719,15 +2678,15 @@
             h += 1
         time_to_end = int(start_timed + hours) + 1
         kwh_added = bat_timed[time_to_end] - bat_timed_old[time_to_end]
         end_part_hour = end_timed - int(end_timed)
         old_residual = interpolate(end_timed, bat_timed_old)
         new_residual = capacity if old_residual + kwh_added > capacity else old_residual + kwh_added
         net_added = new_residual - start_residual
-        output(f"  Charging for {int(hours * 60)} minutes adds {net_added:.2f}kWh")
+#        output(f"  Charging for {int(hours * 60)} minutes adds {net_added:.2f}kWh")
         output(f"  Start SoC: {start_residual / capacity * 100:3.0f}% at {hours_time(start_at)} ({start_residual:.2f}kWh)")
         output(f"  End SoC:   {new_residual / capacity * 100:3.0f}% at {hours_time(end1)} ({new_residual:.2f}kWh)")
     if show_data > 2:
         output(f"\nTime, Generation, Charge, Consumption, Discharge, Residual, kWh")
         for i in range(0, run_time):
             h = base_hour + i
             output(f"  {hours_time(h)}, {generation_timed[i]:6.3f}, {charge_timed[i]:6.3f}, {consumption_timed[i]:6.3f}, {discharge_timed[i]:6.3f}, {bat_timed[i]:6.3f}")
@@ -2749,25 +2708,25 @@
         output(s[:-1])
     if show_plot > 0:
         print()
         plt.figure(figsize=(figure_width, figure_width/2))
         x_timed = [i for i in range(0, run_time)]
         plt.xticks(ticks=x_timed, labels=[hours_time(base_hour + x - (hour_adjustment if (base_hour + x) >= change_hour else 0), day=False) for x in x_timed], rotation=90, fontsize=8, ha='center')
         if show_plot == 1:
-            title = f"Battery SoC % ({charge_message}, forecast={expected:.1f}kWh, consumption={consumption:.1f}kWh)"
+            title = f"Battery SoC % ({charge_message})"
             plt.plot(x_timed, [round(bat_timed[x] * 100 / capacity,1) for x in x_timed], label='Battery', color='blue')
         else:
-            title = f"Energy Flow kWh ({charge_message}, forecast={expected:.1f}kWh, consumption={consumption:.1f}kWh)"
+            title = f"Energy Flow kWh ({charge_message})"
             plt.plot(x_timed, bat_timed, label='Battery', color='blue')
             plt.plot(x_timed, generation_timed, label='Generation', color='green')
             plt.plot(x_timed, consumption_timed, label='Consumption', color='red')
 #            if kwh_needed > 0:
 #                plt.plot(x_timed, bat_timed_old, label='Battery (before charging)', color='blue', linestyle='dotted')
             if show_plot == 3:
-                plt.plot(x_timed, charge_timed, label='Charge', color='orange', linestyle='dotted')
+                plt.plot(x_timed, charge_timed, label='Charge Avail.', color='orange', linestyle='dotted')
                 plt.plot(x_timed, discharge_timed, label='Discharge', color='brown', linestyle='dotted')
         plt.title(title, fontsize=10)
         plt.grid()
         if show_plot > 1:
             plt.legend(fontsize=8, loc="upper right")
         plot_show()
     if test_charge is not None:
@@ -3688,16 +3647,18 @@
 # simple push message
 def output_message(app_key=None, message=None, plot=0):
     output_spool(app_key, message)
     output_close(plot=plot)
     return None
 
 # add to spooled_output
-def output(s=""):
-    global spool_mode, spooled_output
+def output(s="", log_level=None):
+    global spool_mode, spooled_output, debug_setting
+    if log_level is not None and debug_setting < log_level:
+        return
     # keep output stream up to date in case of problem / exception
     print(s)
     # spool output for pushover if needed
     if spool_mode is not None:
         if ((len(spooled_output) if spooled_output is not None else 0) + len(s)) > 1024:
             # more than 1024 chars, re-start spooling to avoid data loss
             output_spool(spool_mode)
```

### Comparing `foxesscloud-2.2.4/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.2.5/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.4
+Version: 2.2.5
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -666,15 +666,17 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.4<br>
+2.2.5<br>
+Refactor debug messaging.
+Simplify charge_needed() output.
 Added 'target_soc' to charge_needed() settings
 Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50 where there is no battery
 Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.4 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.5 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -458,21 +458,22 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.4
-Added 'target_soc' to charge_needed() settings Fix bat_info() giving incorrect
-temperatures when API returns 0 instead of -50 where there is no battery Fix
-key error when accessing cell volts and temps using an agent / installer
-account. Ensure output is generated if get_battery() fails using battery_info
-(). Update f.avg() to include calculation of averages in lists containng None
-values. Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.5
+Refactor debug messaging. Simplify charge_needed() output. Added 'target_soc'
+to charge_needed() settings Fix bat_info() giving incorrect temperatures when
+API returns 0 instead of -50 where there is no battery Fix key error when
+accessing cell volts and temps using an agent / installer account. Ensure
+output is generated if get_battery() fails using battery_info(). Update f.avg()
+to include calculation of averages in lists containng None values. Added
+'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

