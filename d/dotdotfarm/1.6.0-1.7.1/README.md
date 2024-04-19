# Comparing `tmp/dotdotfarm-1.6.0.tar.gz` & `tmp/dotdotfarm-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotdotfarm-1.6.0.tar", last modified: Sun Oct  8 19:41:35 2023, max compression
+gzip compressed data, was "dotdotfarm-1.7.1.tar", last modified: Fri Apr 19 14:54:40 2024, max compression
```

## Comparing `dotdotfarm-1.6.0.tar` & `dotdotfarm-1.7.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-10-08 19:41:35.627315 dotdotfarm-1.6.0/
--rw-rw-rw-   0        0        0    35810 2023-01-16 18:50:58.000000 dotdotfarm-1.6.0/LICENSE
--rw-rw-rw-   0        0        0      470 2023-10-08 19:41:35.627315 dotdotfarm-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     6936 2023-09-24 14:29:57.000000 dotdotfarm-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-08 19:41:35.627315 dotdotfarm-1.6.0/dotdotfarm/
--rw-rw-rw-   0        0        0        0 2023-01-22 10:12:14.000000 dotdotfarm-1.6.0/dotdotfarm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-08 19:41:35.627315 dotdotfarm-1.6.0/dotdotfarm/callbacks/
--rw-rw-rw-   0        0        0      139 2023-03-09 19:14:53.000000 dotdotfarm-1.6.0/dotdotfarm/callbacks/__init__.py
--rw-rw-rw-   0        0        0     3286 2023-09-25 08:58:56.000000 dotdotfarm-1.6.0/dotdotfarm/callbacks/callbacks.py
--rw-rw-rw-   0        0        0      364 2023-09-25 08:56:13.000000 dotdotfarm-1.6.0/dotdotfarm/callbacks/cobject.py
--rw-rw-rw-   0        0        0     6501 2023-10-08 19:41:35.000000 dotdotfarm-1.6.0/dotdotfarm/dotdotweb.py
-drwxrwxrwx   0        0        0        0 2023-10-08 19:41:35.627315 dotdotfarm-1.6.0/dotdotfarm/engines/
--rw-rw-rw-   0        0        0        0 2023-01-17 19:46:18.000000 dotdotfarm-1.6.0/dotdotfarm/engines/__init__.py
--rw-rw-rw-   0        0        0     4918 2023-10-08 19:26:45.000000 dotdotfarm-1.6.0/dotdotfarm/engines/http_engine.py
--rw-rw-rw-   0        0        0        0 2023-05-01 19:28:12.000000 dotdotfarm-1.6.0/dotdotfarm/engines/websock_engine.py
-drwxrwxrwx   0        0        0        0 2023-10-08 19:41:35.627315 dotdotfarm-1.6.0/dotdotfarm/generators/
--rw-rw-rw-   0        0        0       81 2023-01-17 19:46:18.000000 dotdotfarm-1.6.0/dotdotfarm/generators/__init__.py
--rw-rw-rw-   0        0        0     2634 2023-09-25 09:04:13.000000 dotdotfarm-1.6.0/dotdotfarm/generators/words_generator.py
-drwxrwxrwx   0        0        0        0 2023-10-08 19:41:35.627315 dotdotfarm-1.6.0/dotdotfarm.egg-info/
--rw-rw-rw-   0        0        0      470 2023-10-08 19:41:35.000000 dotdotfarm-1.6.0/dotdotfarm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-10-08 19:41:35.000000 dotdotfarm-1.6.0/dotdotfarm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-08 19:41:35.000000 dotdotfarm-1.6.0/dotdotfarm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-10-08 19:41:35.000000 dotdotfarm-1.6.0/dotdotfarm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2023-10-08 19:41:35.000000 dotdotfarm-1.6.0/dotdotfarm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-10-08 19:41:35.000000 dotdotfarm-1.6.0/dotdotfarm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-08 19:41:35.627315 dotdotfarm-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1590 2023-10-08 19:40:31.000000 dotdotfarm-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:54:40.898567 dotdotfarm-1.7.1/
+-rw-rw-rw-   0        0        0    35810 2023-01-16 18:50:58.000000 dotdotfarm-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0     8245 2024-04-19 14:54:40.897593 dotdotfarm-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7525 2024-04-19 14:13:32.000000 dotdotfarm-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 14:54:40.890780 dotdotfarm-1.7.1/dotdotfarm/
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:12:14.000000 dotdotfarm-1.7.1/dotdotfarm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:54:40.894673 dotdotfarm-1.7.1/dotdotfarm/callbacks/
+-rw-rw-rw-   0        0        0      139 2023-03-09 19:14:53.000000 dotdotfarm-1.7.1/dotdotfarm/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     3544 2024-04-18 22:57:04.000000 dotdotfarm-1.7.1/dotdotfarm/callbacks/callbacks.py
+-rw-rw-rw-   0        0        0      364 2023-09-25 08:56:13.000000 dotdotfarm-1.7.1/dotdotfarm/callbacks/cobject.py
+-rw-rw-rw-   0        0        0     7372 2024-04-19 14:54:40.000000 dotdotfarm-1.7.1/dotdotfarm/dotdotweb.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:54:40.895646 dotdotfarm-1.7.1/dotdotfarm/engines/
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:46:18.000000 dotdotfarm-1.7.1/dotdotfarm/engines/__init__.py
+-rw-rw-rw-   0        0        0     9861 2024-04-19 14:38:07.000000 dotdotfarm-1.7.1/dotdotfarm/engines/http_engine.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 19:28:12.000000 dotdotfarm-1.7.1/dotdotfarm/engines/websock_engine.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:54:40.896620 dotdotfarm-1.7.1/dotdotfarm/generators/
+-rw-rw-rw-   0        0        0       81 2023-01-17 19:46:18.000000 dotdotfarm-1.7.1/dotdotfarm/generators/__init__.py
+-rw-rw-rw-   0        0        0     2634 2023-09-25 09:04:13.000000 dotdotfarm-1.7.1/dotdotfarm/generators/words_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:54:40.897593 dotdotfarm-1.7.1/dotdotfarm.egg-info/
+-rw-rw-rw-   0        0        0     8245 2024-04-19 14:54:40.000000 dotdotfarm-1.7.1/dotdotfarm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2024-04-19 14:54:40.000000 dotdotfarm-1.7.1/dotdotfarm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 14:54:40.000000 dotdotfarm-1.7.1/dotdotfarm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-19 14:54:40.000000 dotdotfarm-1.7.1/dotdotfarm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-19 14:54:40.000000 dotdotfarm-1.7.1/dotdotfarm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 14:54:40.000000 dotdotfarm-1.7.1/dotdotfarm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 14:54:40.898567 dotdotfarm-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2024-04-19 14:11:25.000000 dotdotfarm-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:54:40.896620 dotdotfarm-1.7.1/tests/
+-rw-rw-rw-   0        0        0      256 2023-10-13 18:53:51.000000 dotdotfarm-1.7.1/tests/test-http_engine.py
```

### Comparing `dotdotfarm-1.6.0/LICENSE` & `dotdotfarm-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dotdotfarm-1.6.0/README.md` & `dotdotfarm-1.7.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 dotdotfarm
 ==========
 
-![Version](https://img.shields.io/badge/version-1.6.0-blue?style=for-the-badge)
+![Version](https://img.shields.io/badge/version-1.7.1-blue?style=for-the-badge)
 
 Utility for detection & exploitation of Path Traversal vulnerabilities in various network services
 
 dotdotweb - PT tool for HTTP services
 
 
 Tools are written in Python with using asyncio requests (aiohttp) with some acceleration techniques, which allows you to make up to ~3K requests per second
 
 Features
-========
-- async client for parallel requesting of target (speedup)
+--------
+- using asynchronous requests for increasing scan of target
 - ability to fetch files' content after succeeding a payload
-- specifying payload in any part of query (url, headers or POST data)
-- using callbacks for future handling of results
+- specifying payload in any part of query (URL, headers or POST data)
+- using callbacks for handling of results
 
 Installation
 ============
 Install from PyPi
 ```bash
 pip install dotdotfarm
 ```
 You can also install it directly from GitHub repository
 ```bash
 git clone https://github.com/treddis/dotdotfarm.git
 cd dotdotfarm
-pip install -r requirements.txt
 pip3 install .
 ```
+To upgrade tool run
+```bash
+pip install --upgrade dotdotfarm
+```
 
 Usage
 =====
 ```text
 
     .___      __      .___      __    _____                      
   __| _/_____/  |_  __| _/_____/  |__/ ____\____ _______  _____  
@@ -70,38 +73,48 @@
                         timeout of connections (default 60)
   -fs FS                filter output by size
   -fc FC                filter output by response code
   --header HEADERS      custom header for requests
   --data DATA           specify POST data
 ```
 
-Passing in GET parameters
-----------------------
+### Passing payload in GET parameters
 Passing brute parameters via `?par=val` pairs:
 ```text
 dotdotweb -o windows -fc 500 \ 
           http://someserver.com:1280/newpath?testparameter=FUZZ&secondparameter=somevalue
 ```
 
-Passing via headers
--------------------
+### Passing payload in headers
 Passing brute parameters via `Origin: master=FUZZ` pairs:
 ```text
 dotdotweb -o linux -fc 500,404 -H "Referer: https://www.google.com/path?q=FUZZ" \
           http://someserver.com:1280/newpath?testparameter=firstvalue&secondparameter=somevalue
 ```
 
-Passing via POST data
----------------------
+### Passing payload in POST data
 Passing brute parameters via POST data parameters
 ```text
 dotdotweb -o linux -fc 500 -fs 111 -d "key0=val0&key1=val1" \
           http://someserver.com:1280/newpath?testparameter=firstvalue&secondparameter=somevalue
 ```
 
+### Using regexp to filter responses
+Pass -fs (filter by size) or -fc (filter by status code) to filter out not related responses
+```text
+dotdotweb -fc 50*,4* -fs 18??,1834* http://someserver.com:1234/testpath/FUZZ
+```
+
+### Launch callbacks on responses
+You can launch callbacks on your responses to perform some check or make other actions.
+In the box implemented callbacks:
+- validate response content using regexp and print then (-V). You can pass your regexp too!
+- try all payloads even entry point is found (-A)
+- read traversed files content and print them on screen (-P)
+
 Example output
 ==============
 ```text
 dotdotweb -o windows "http://localhost:8080/pathtrav?query=FUZZ" 
 
     .___      __      .___      __    _____
   __| _/_____/  |_  __| _/_____/  |__/ ____\____ _______  _____
```

### Comparing `dotdotfarm-1.6.0/dotdotfarm/callbacks/callbacks.py` & `dotdotfarm-1.7.1/dotdotfarm/callbacks/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
                                                    f' [Status: {Fore.GREEN}{cobject.response.status}{Style.RESET_ALL}, Size: {len(cobject.response.data)}]'))
             elif cobject.response.status // 100 == 5:
                 tqdm.write(' {:<100}{:>20}'.format(cobject.response.payload,
                                                    f' [Status: {Fore.RED}{cobject.response.status}{Style.RESET_ALL}, Size: {len(cobject.response.data)}]'))
             elif cobject.response.status // 100 == 4:
                 tqdm.write(' {:<100}{:>20}'.format(cobject.response.payload,
                                                    f' [Status: {Fore.YELLOW}{cobject.response.status}{Style.RESET_ALL}, Size: {len(cobject.response.data)}]'))
+    except KeyboardInterrupt:
+        raise asyncio.CancelledError
     except:
         pass
 
 
 def validate_file(stop_on_success):
     """ Callback used for checking files' content. """
 
@@ -64,14 +66,18 @@
             elif stop_on_success:
                 for task in asyncio.all_tasks(asyncio.get_event_loop()):
                     task.cancel()
             else:
                 pass
         except AttributeError:
             pass
+        except KeyboardInterrupt:
+            raise asyncio.CancelledError
+        except:
+            pass
 
     return validate
 
 
 def add_file(files_dict):
     """ Callback used for saving data from response. """
 # @container(files_dict)
@@ -82,14 +88,16 @@
                 return
             if cobject.state == Failed:
                 return
             if type(cobject.response) == dotdotfarm.engines.http_engine.HttpResponse:
                 data = cobject.response.data.decode()
             if data not in files_dict.values():
                 files_dict[cobject.response.url] = data
+        except KeyboardInterrupt:
+            raise asyncio.CancelledError
         except:
             pass
 
     return add
 
 
 def exec():
```

### Comparing `dotdotfarm-1.6.0/dotdotfarm/dotdotweb.py` & `dotdotfarm-1.7.1/dotdotfarm/dotdotweb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,90 +1,103 @@
 #!/usr/bin/env python3
 #! -*- coding: utf-8 -*-
 
 import argparse
-import logging
+# import logging
 import asyncio
+import re
+
 import yarl
 import time
 from functools import partial
 from colorama import init, Fore, Style
 init()
 
 from dotdotfarm.generators.words_generator import Generator
 from dotdotfarm.engines.http_engine import HTTPEngine
 from dotdotfarm.callbacks.callbacks import print_http_result, add_file, validate_file
 
-__version__ = '1.6.0'
+__version__ = '1.7.1'
 
 argparse_list = partial(str.split, sep=',')
 
 async def factory(engine):
     try:
-        task = asyncio.create_task(engine.run())
+        task = asyncio.get_running_loop().create_task(engine.run())
         await task
     except asyncio.CancelledError:
         task.cancel()
     except ConnectionResetError:
         pass
-    except BaseException:
-        pass
+    except BaseException as e:
+        print(e)
 
 def main():
     print(f"""{Fore.CYAN}
     .___      __      .___      __    {Fore.RED}_____                      
   {Fore.CYAN}__| _/{Fore.YELLOW}____{Fore.CYAN}_/  |_  __| _/{Fore.YELLOW}____{Fore.CYAN}_/  |__{Fore.RED}/ ____\\____ _______  _____  
  {Fore.CYAN}/ __ |{Fore.YELLOW}/  _ \\{Fore.CYAN}   __\\/ __ |{Fore.YELLOW}/  _ \\{Fore.CYAN}   __{Fore.RED}\\   __\\\\__  \\\\_  __ \\/     \\ 
 {Fore.CYAN}/ /_/ {Fore.YELLOW}(  <_> ){Fore.CYAN}  | / /_/ {Fore.YELLOW}(  <_> ){Fore.CYAN}  |  {Fore.RED}|  |   / __ \\|  | \\/  Y Y  \\
 {Fore.CYAN}\\____ |{Fore.YELLOW}\\____/{Fore.CYAN}|__| \\____ |{Fore.YELLOW}\\____/{Fore.CYAN}|__|  {Fore.RED}|__|  (____  /__|  |__|_|  /
      {Fore.CYAN}\\/                \\/                       {Fore.RED}\\/            \\/ 
      {Style.RESET_ALL}""")
 
     parser = argparse.ArgumentParser(description='fast path traversal identificator & exploit')
     parser.add_argument('--version', action='version', version=f'dotdotweb {__version__}', help='print version of the tool')
+    parser.add_argument('--proxy', default='', help='specify proxy to test selected url')
 
     # Callbacks
-    callbacks = parser.add_argument_group('Callbacks', '')
+    callbacks = parser.add_argument_group('Callbacks')
     callbacks.add_argument('-V', '--validate', action='store_true', help='validate files\' content after successfull exploitation (default false)')
     # parser.add_argument('-v', '--verbose', action='store_true', help='verbose output of responses')
     # parser.add_argument('--debug', action='store_true', help='debug output')
     callbacks.add_argument('-A', '--all', action='store_true', help='try all files after successfull exploitation (default false)')
     callbacks.add_argument('-P', '--print-files', action='store_true', help='read traversed files (default false)')
     # parser.add_argument('-M', '--module-detect', action='store_true', default=False, help='intelligent service detection')
 
     # Parameters for payload generator
-    generator = parser.add_argument_group('Payload parameters')
+    generator = parser.add_argument_group('Payload generator parameters')
     generator.add_argument('-o', '--os-type', choices=['windows', 'linux'], default='', help='target OS type (default all)')
     generator.add_argument('-d', '--depth', type=int, default=5, help='depth of PT searching (default 5)')
     generator.add_argument('-f', '--file', help='specific file for PT detection')
 
     # Timings
     parser.add_argument('--rate', type=int, default=0, help='limit requests per second (default 0)')
     parser.add_argument('-t', '--timeout', type=int, default=60, help='timeout of connections (default 60)')
 
     # Filters
     filters = parser.add_argument_group('Filters')
-    filters.add_argument('-fs', type=argparse_list, default=[], help='filter output by size')
-    filters.add_argument('-fc', type=argparse_list, default=[], help='filter output by response code')
+    filters.add_argument('-fs', type=argparse_list, default=[], help='filter output by size (with quantifiers)')
+    filters.add_argument('-fc', type=argparse_list, default=[], help='filter output by response code (with quantifiers)')
 
     # Payload specificators
     locations = parser.add_argument_group('Payload locations')
     locations.add_argument('--method', help='custom method for requests')
     locations.add_argument('--header', dest='headers', default=[], action='append', help='custom header for requests')
     locations.add_argument('--data', default='', help='specify POST data')
     locations.add_argument('url', help='target URL')
 
     opts = parser.parse_args()
     # if opts.debug:
     #     logging.getLogger("asyncio").setLevel(logging.WARNING)
 
     if opts.fs:
-        opts.fs = list(map(int, opts.fs))
+        if not all(map(lambda x: re.match(r'[0-9\*\?]+', x), opts.fs)):
+            parser.error('Invalid -fs parameter')
+        else:
+            opts.fs = list(map(lambda x: x.replace("*", "\\d*").replace("?", "\\d?"), opts.fs))
     if opts.fc:
-        opts.fc = list(map(int, opts.fc))
+        if not all(map(lambda x: re.match(r'[0-9\*\?]+', x), opts.fc)):
+            parser.error('Invalid -fc parameter')
+        else:
+            opts.fc = list(map(lambda x: x.replace("*", "\\d*").replace("?", "\\d?"), opts.fc))
+    if opts.proxy:
+        if not re.match(r'^(socks(5|4)|https?)://(\S+:\S+@)?(([0-9]\.){3}[0-9]{1,3}|[a-zA-Z0-9-.]{1,255})(:\d+)?\/?$', opts.proxy):
+            parser.error('Invalid --proxy parameter')
+        # opts.fc = list(map(int, opts.fc))
 
     if 'FUZZ' not in opts.url and 'FUZZ' not in opts.data and not any(map(lambda x: 'FUZZ' in x, opts.headers)):
         parser.error('You must specify FUZZ parameter in URL/Header/Data by example Referer: https://google.com/path?param=FUZZ')
     inputs = {}
     if 'FUZZ' in opts.url:
         inputs['url'] = [opts.url]
     if 'FUZZ' in opts.data:
@@ -113,19 +126,20 @@
         engine = HTTPEngine(
             opts.url,
             opts.method, headers, opts.data,
             payloads,
             callbacks=callbacks,
             filters=(opts.fc, opts.fs),
             timeout=opts.timeout,
-            rate=opts.rate)
+            rate=opts.rate,
+            proxy=opts.proxy)
 
         task = loop.create_task(factory(engine))
     else:
-        parser.error('Not implemented')
+        parser.error('This URL scheme is not implemented yet')
 
     try:
         start = time.time()
         print(f'[{Fore.CYAN}*{Style.RESET_ALL}] Started at {time.ctime(start)}')
         loop.run_until_complete(task)
     except KeyboardInterrupt:
         print(f'\n[{Fore.CYAN}*{Style.RESET_ALL}] Got keyboard interrupt')
```

### Comparing `dotdotfarm-1.6.0/dotdotfarm/generators/words_generator.py` & `dotdotfarm-1.7.1/dotdotfarm/generators/words_generator.py`

 * *Files identical despite different names*

### Comparing `dotdotfarm-1.6.0/dotdotfarm.egg-info/SOURCES.txt` & `dotdotfarm-1.7.1/dotdotfarm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 dotdotfarm/callbacks/__init__.py
 dotdotfarm/callbacks/callbacks.py
 dotdotfarm/callbacks/cobject.py
 dotdotfarm/engines/__init__.py
 dotdotfarm/engines/http_engine.py
 dotdotfarm/engines/websock_engine.py
 dotdotfarm/generators/__init__.py
-dotdotfarm/generators/words_generator.py
+dotdotfarm/generators/words_generator.py
+tests/test-http_engine.py
```

### Comparing `dotdotfarm-1.6.0/setup.py` & `dotdotfarm-1.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,35 +5,38 @@
 import shutil
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-__version__ = '1.6.0'
+__version__ = '1.7.1'
 install_requires = [
-    "aiohttp==3.8.4",
-    "colorama==0.4.6",
-    "setuptools==66.1.1",
-    "tqdm==4.64.1",
-    "yarl==1.8.2",
-    "multidict==6.0.4",
-    "attrs==22.2.0",
-    "yarl==1.8.2",
-    "async-timeout==4.0.2",
-    "aiosignal==1.3.1"
+    "aiohttp~=3.9.3",
+    'tqdm>=4.64.1',
+    "colorama~=0.4.6",
+    "setuptools",
+    "tqdm",
+    "yarl",
+    "multidict",
+    "attrs",
+    "yarl",
+    "async-timeout",
+    "aiosignal"
 ]
 
 install_dir = os.path.abspath('.')
 try:
     shutil.copy(os.path.join(install_dir, 'dotdotweb.py'), os.path.join(install_dir, 'dotdotfarm', 'dotdotweb.py'))
     setup(
         name='dotdotfarm',
         version=__version__,
-        description='Path Traversal exploitation tool',
+        description='Fast Path Traversal exploitation tool',
+        long_description_content_type='text/markdown',
+        long_description=long_description,
         license='GPL',
         author='treddis',
         packages=find_packages(),
         install_requires=install_requires,
         entry_points={
             'console_scripts':
                 ['dotdotweb = dotdotfarm.dotdotweb:main']
```

