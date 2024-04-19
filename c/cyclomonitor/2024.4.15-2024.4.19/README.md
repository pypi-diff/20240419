# Comparing `tmp/cyclomonitor-2024.4.15.tar.gz` & `tmp/cyclomonitor-2024.4.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclomonitor-2024.4.15.tar", last modified: Mon Apr 15 01:52:36 2024, max compression
+gzip compressed data, was "cyclomonitor-2024.4.19.tar", last modified: Fri Apr 19 01:30:52 2024, max compression
```

## Comparing `cyclomonitor-2024.4.15.tar` & `cyclomonitor-2024.4.19.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-15 01:52:36.845573 cyclomonitor-2024.4.15/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.15/LICENSE
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.4.15/MANIFEST.in
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43113 2024-04-15 01:52:36.845573 cyclomonitor-2024.4.15/PKG-INFO
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1829 2024-04-15 01:44:33.000000 cyclomonitor-2024.4.15/README.md
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.15/privacy-policy.md
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1519 2024-04-15 01:29:25.000000 cyclomonitor-2024.4.15/pyproject.toml
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)       28 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/requirements.txt
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-04-15 01:52:36.845573 cyclomonitor-2024.4.15/setup.cfg
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1828 2024-04-14 22:24:58.000000 cyclomonitor-2024.4.15/setup.py
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-15 01:52:36.837573 cyclomonitor-2024.4.15/src/
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-15 01:52:36.841573 cyclomonitor-2024.4.15/src/cyclomonitor/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      189 2024-04-15 00:43:27.000000 cyclomonitor-2024.4.15/src/cyclomonitor/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    39144 2024-04-15 01:49:58.000000 cyclomonitor-2024.4.15/src/cyclomonitor/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10557 2024-04-14 12:51:51.000000 cyclomonitor-2024.4.15/src/cyclomonitor/atcf.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.15/src/cyclomonitor/dir_calc.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.15/src/cyclomonitor/errors.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/global_vars.py
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-15 01:52:36.841573 cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12661 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5062 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5070 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-15 01:52:36.841573 cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/locales/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/locales/C.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/locales/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/locales/en_US.json
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-15 01:52:36.841573 cyclomonitor-2024.4.15/src/cyclomonitor/locales/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12395 2024-04-15 01:00:29.000000 cyclomonitor-2024.4.15/src/cyclomonitor/locales/C.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     7200 2024-04-15 01:00:35.000000 cyclomonitor-2024.4.15/src/cyclomonitor/locales/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12395 2024-04-15 01:00:29.000000 cyclomonitor-2024.4.15/src/cyclomonitor/locales/en_US.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/server_vars.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.15/src/cyclomonitor/uptime.py
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-15 01:52:36.841573 cyclomonitor-2024.4.15/src/cyclomonitor.egg-info/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      710 2024-04-15 01:52:36.000000 cyclomonitor-2024.4.15/src/cyclomonitor.egg-info/SOURCES.txt
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.484628 cyclomonitor-2024.4.19/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.19/LICENSE
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.4.19/MANIFEST.in
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43192 2024-04-19 01:30:52.484628 cyclomonitor-2024.4.19/PKG-INFO
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1908 2024-04-19 01:01:12.000000 cyclomonitor-2024.4.19/README.md
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.19/privacy-policy.md
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1519 2024-04-15 01:29:25.000000 cyclomonitor-2024.4.19/pyproject.toml
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)       28 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/requirements.txt
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-04-19 01:30:52.484628 cyclomonitor-2024.4.19/setup.cfg
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1828 2024-04-19 00:44:11.000000 cyclomonitor-2024.4.19/setup.py
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.476628 cyclomonitor-2024.4.19/src/
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      189 2024-04-15 00:43:27.000000 cyclomonitor-2024.4.19/src/cyclomonitor/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    39238 2024-04-19 01:27:30.000000 cyclomonitor-2024.4.19/src/cyclomonitor/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10557 2024-04-14 12:51:51.000000 cyclomonitor-2024.4.19/src/cyclomonitor/atcf.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.19/src/cyclomonitor/dir_calc.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.19/src/cyclomonitor/errors.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/global_vars.py
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12661 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5062 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5070 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/C.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/en_US.json
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor/locales/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12395 2024-04-15 01:00:29.000000 cyclomonitor-2024.4.19/src/cyclomonitor/locales/C.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     7200 2024-04-15 01:00:35.000000 cyclomonitor-2024.4.19/src/cyclomonitor/locales/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12395 2024-04-15 01:00:29.000000 cyclomonitor-2024.4.19/src/cyclomonitor/locales/en_US.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/server_vars.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/uptime.py
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor.egg-info/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      710 2024-04-19 01:30:52.000000 cyclomonitor-2024.4.19/src/cyclomonitor.egg-info/SOURCES.txt
```

### Comparing `cyclomonitor-2024.4.15/LICENSE` & `cyclomonitor-2024.4.19/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/PKG-INFO` & `cyclomonitor-2024.4.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclomonitor
-Version: 2024.4.15
+Version: 2024.4.19
 Summary: Discord bot that helps you keep tabs on tropical cyclones.
 Home-page: https://github.com/ntvmb/cyclomonitor
 Author: Nathaniel Greenwell
 Author-email: Nathaniel Greenwell <nategreenwell@live.com>
 Maintainer-email: Nathaniel Greenwell <nategreenwell@live.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
@@ -727,8 +727,14 @@
 If you don't want to specify `-t` every time, paste your bot's token into a file called `TOKEN` in your working directory.  
 For full argument list: `python3 -m cyclomonitor -h` or run the module with no arguments.  
 Windows users: You might want to replace `python3` with `python`.
 
 If you're using a virtual environment, ensure it is active before running the bot.  
 CycloMonitor logs to stdout by default. To log to a file, specify the parameter `-l LOGFILE`, where `LOGFILE` is the path to the log file.
 
+## Configuring the bot 
+See CONFIGURATION.md for details.
+
+## CLI
+Coming soon
+
 Supports Python 3.8+, but Python 3.11+ is recommended.
```

### Comparing `cyclomonitor-2024.4.15/README.md` & `cyclomonitor-2024.4.19/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,8 +34,14 @@
 If you don't want to specify `-t` every time, paste your bot's token into a file called `TOKEN` in your working directory.  
 For full argument list: `python3 -m cyclomonitor -h` or run the module with no arguments.  
 Windows users: You might want to replace `python3` with `python`.
 
 If you're using a virtual environment, ensure it is active before running the bot.  
 CycloMonitor logs to stdout by default. To log to a file, specify the parameter `-l LOGFILE`, where `LOGFILE` is the path to the log file.
 
+## Configuring the bot 
+See CONFIGURATION.md for details.
+
+## CLI
+Coming soon
+
 Supports Python 3.8+, but Python 3.11+ is recommended.
```

### Comparing `cyclomonitor-2024.4.15/privacy-policy.md` & `cyclomonitor-2024.4.19/privacy-policy.md`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/pyproject.toml` & `cyclomonitor-2024.4.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/setup.py` & `cyclomonitor-2024.4.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import pathlib
 
-__version__ = "2024.4.15"
+__version__ = "2024.4.19"
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
```

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/__main__.py` & `cyclomonitor-2024.4.19/src/cyclomonitor/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,18 @@
 
 For those hosting a copy of this bot, you should have received a copy of the
 GNU Affero General Public License along with this program. If not, see
 <https://www.gnu.org/licenses/>.
 """
 logname = "bot.log"
 # PLEASE CHANGE THESE LINKS IF YOU ARE FORKING THIS PROJECT.
-INVITE = "https://discord.com/api/oauth2/authorize?client_id=1107462705004167230&permissions=67496000&scope=bot"
-GITHUB = "https://github.com/ntvmb/cyclomonitor"
+INVITE = "https://discord.com/api/oauth2/authorize?client_id={0}&permissions=67496000&scope=bot"
+GITHUB = "GITHUB_LINK"
 languages = ["C", "en_US"]
+emojis = {}
 
 # increase compatibility with python<3.11
 if not hasattr(datetime, "UTC"):
     datetime.UTC = datetime.timezone.utc
 
 try:
     from tendo import singleton
@@ -208,18 +209,17 @@
                     await asyncio.sleep(10 * (i + 2))
                     continue
             else:
                 break
         self.is_best_track_updating = False
 
 
-# this function needs to be a coroutine since other coroutines are called
 async def update_guild(guild: int, to_channel: int):
-    set_locale(server_vars.get("lang", guild))
     """Given a guild ID and channel ID, post ATCF data."""
+    set_locale(server_vars.get("lang", guild))
     logging.info(LOG_UPDATE_GUILD.format(guild))
     channel = bot.get_channel(to_channel)
     enabled_basins = server_vars.get("basins", guild)
     current_TC_record = global_vars.get("strongest_storm")  # record-keeping
     if enabled_basins is not None:
         sent_list = []
         for (
@@ -289,43 +289,43 @@
             All wind speed values shown are in knots rounded to the nearest 5 (except for ones after > operators)
             """
             if name == "INVEST" and (not (tc_class == "SD" or tc_class == "SS")):
                 tc_class = CLASS_AOI
             if tc_class == "EX":
                 if not name == "INVEST":
                     tc_class = CLASS_PTC
-                emoji = "<:ex:1109994645431259187>"
+                emoji = emojis.get("ex")
             elif tc_class == "LO" or tc_class == "INVEST":
                 if not name == "INVEST":
                     tc_class = CLASS_PTC
-                emoji = "<:low:1109997033227558923>"
+                emoji = emojis.get("low")
             elif tc_class == "DB" or tc_class == "WV":
                 if not name == "INVEST":
                     tc_class = CLASS_RL
-                emoji = "<:remnants:1109994646932836386>"
+                emoji = emojis.get("remnants")
             elif wind < 35:
                 if not (tc_class == "SD" or name == "INVEST"):
                     # ignored if invest in case of autoflagging
                     # ATCF will autoflag a system to be a TD once it has attained 1-minute sustained winds of between 23 and 33 kt
                     tc_class = CLASS_TD
-                    emoji = "<:td:1109994651169079297>"
+                    emoji = emojis.get("td")
                 elif name == "INVEST" and not tc_class == "SD":
-                    emoji = "<:low:1109997033227558923>"
+                    emoji = emojis.get("low")
                 else:
                     tc_class = CLASS_SD
-                    emoji = "<:sd:1109994648300163142>"
+                    emoji = emojis.get("sd")
             elif wind > 34 and wind < 65:
                 if not (tc_class == "SS" or name == "INVEST"):
                     tc_class = CLASS_TS
-                    emoji = "<:ts:1109994652368650310>"
+                    emoji = emojis.get("ts")
                 elif name == "INVEST" and not tc_class == "SS":
-                    emoji = "<:low:1109997033227558923>"
+                    emoji = emojis.get("low")
                 else:
                     tc_class = CLASS_SS
-                    emoji = "<:ss:1109994649654935563>"
+                    emoji = emojis.get("ss")
             else:
                 # determine the term to use based on the basin
                 # we assume at this point that the system is either a TC or extratropical
                 if basin == "ATL" or basin == "EPAC" or basin == "CPAC":
                     if wind < 100:
                         tc_class = CLASS_HU
                     else:
@@ -337,31 +337,33 @@
                         tc_class = CLASS_STY
                 else:
                     tc_class = CLASS_CY
 
                 # for custom emoji to work, the bot needs to be in the server it's from
                 # you also need the emoji's ID
                 if wind < 85:
-                    emoji = "<:cat1:1109994357257420902>"
+                    emoji = emojis.get("cat1")
                 elif wind > 84 and wind < 100:
-                    emoji = "<:cat2:1109994593895862364>"
+                    emoji = emojis.get("cat2")
                 elif wind > 99 and wind < 115:
-                    emoji = "<:cat3:1109994641094357024>"
+                    emoji = emojis.get("cat3")
                 elif wind > 114 and wind < 140:
-                    emoji = "<:cat4:1109994643057295401>"
+                    emoji = emojis.get("cat4")
                 elif wind > 139 and wind < 155:
-                    emoji = "<:cat5:1109994644386893864>"
+                    emoji = emojis.get("cat5")
                 elif wind > 154 and wind < 170:
-                    emoji = "<:cat5intense:1111376977664954470>"
+                    emoji = emojis.get("cat5intense")
                 else:
-                    emoji = "<:cat5veryintense:1111378049448026126>"
+                    emoji = emojis.get("cat5veryintense")
             if name == "INVEST":
                 name = display_name = cyc_id
             else:
                 display_name = f"{cyc_id} ({name})"
+            if emoji is None:
+                emoji = ":cyclone:"
             # update TC records
             if current_TC_record is not None:
                 if (wind > int(current_TC_record[5])) or (
                     wind == int(current_TC_record[5])
                     and pressure < int(current_TC_record[8])
                 ):
                     logging.info(LOG_NEW_RECORD)
@@ -976,14 +978,15 @@
                 await ctx.respond(file=discord.File(f))
 
 
 def main():
     import argparse
     import json
 
+    global GITHUB, INVITE
     locale_init()
     parser = argparse.ArgumentParser(
         prog="cyclomonitor",
         description=DESCRIPTION,
         epilog=HELP_EPILOG.format(GITHUB),
     )
     parser.add_argument("-b", "--bot", help=HELP_BOT, action="store_true")
@@ -1021,14 +1024,20 @@
         with open(args.config) as f:
             config = json.load(f)
         _token = config["token"]
         if config.get("log_file") is not None:
             log_params["filename"] = config["log_file"]
             log_params["filemode"] = "a"
             logging.captureWarnings(True)
+        if config.get("github") is not None:
+            GITHUB = config["github"]
+        if config.get("client_id") is not None:
+            INVITE = INVITE.format(config["client_id"])
+        if isinstance(config.get("emojis"), dict):
+            emojis.update(config["emojis"])
     if args.verbose:
         log_params["level"] = logging.DEBUG
     else:
         log_params["level"] = logging.INFO
     logging.basicConfig(
         format="%(asctime)s.%(msecs)d %(name)s %(levelname)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
```

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/atcf.py` & `cyclomonitor-2024.4.19/src/cyclomonitor/atcf.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/dir_calc.py` & `cyclomonitor-2024.4.19/src/cyclomonitor/dir_calc.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/global_vars.py` & `cyclomonitor-2024.4.19/src/cyclomonitor/global_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/__init__.py` & `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/ibtracs_ALL.sql` & `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/ibtracs_ALL.sql`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql` & `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/locales/C.json` & `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/C.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/locales/__init__.py` & `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/ibtracs/locales/en_US.json` & `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/locales/C.json` & `cyclomonitor-2024.4.19/src/cyclomonitor/locales/C.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/locales/__init__.py` & `cyclomonitor-2024.4.19/src/cyclomonitor/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/locales/en_US.json` & `cyclomonitor-2024.4.19/src/cyclomonitor/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/server_vars.py` & `cyclomonitor-2024.4.19/src/cyclomonitor/server_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor/uptime.py` & `cyclomonitor-2024.4.19/src/cyclomonitor/uptime.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.15/src/cyclomonitor.egg-info/SOURCES.txt` & `cyclomonitor-2024.4.19/src/cyclomonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

