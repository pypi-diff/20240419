# Comparing `tmp/mpd_what-1.0.9.tar.gz` & `tmp/mpd_what-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mpd_what-1.0.9.tar", last modified: Tue Dec  6 17:20:48 2022, max compression
+gzip compressed data, was "mpd_what-1.1.0.tar", last modified: Thu Apr 18 22:38:37 2024, max compression
```

## Comparing `mpd_what-1.0.9.tar` & `mpd_what-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-12-06 17:20:48.000000 mpd_what-1.0.9/
--rw-rw-r--   0 rob       (1000) rob       (1000)    35149 2021-04-17 23:51:16.000000 mpd_what-1.0.9/LICENSE.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)     1198 2022-12-06 17:20:48.000000 mpd_what-1.0.9/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)       30 2021-04-17 23:50:19.000000 mpd_what-1.0.9/MANIFEST.in
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2022-12-06 17:20:48.000000 mpd_what-1.0.9/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)      775 2022-04-10 19:10:54.000000 mpd_what-1.0.9/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-12-06 17:20:48.000000 mpd_what-1.0.9/mpd_what.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1198 2022-12-06 17:20:48.000000 mpd_what-1.0.9/mpd_what.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      214 2022-12-06 17:20:48.000000 mpd_what-1.0.9/mpd_what.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-12-06 17:20:48.000000 mpd_what-1.0.9/mpd_what.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-12-06 17:20:48.000000 mpd_what-1.0.9/mpd_what.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       88 2022-12-06 17:20:48.000000 mpd_what-1.0.9/mpd_what.egg-info/requires.txt
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2022-12-06 17:20:48.000000 mpd_what-1.0.9/bin/
--rwxrwxr-x   0 rob       (1000) rob       (1000)    24378 2022-12-06 17:20:41.000000 mpd_what-1.0.9/bin/mpd_what
--rw-rw-r--   0 rob       (1000) rob       (1000)      644 2022-12-06 17:18:52.000000 mpd_what-1.0.9/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2024-04-18 22:38:37.853092 mpd_what-1.1.0/
+-rw-rw-r--   0 rob       (1000) rob       (1000)    35149 2021-04-17 23:51:16.000000 mpd_what-1.1.0/LICENSE.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       30 2021-04-17 23:50:19.000000 mpd_what-1.1.0/MANIFEST.in
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1099 2024-04-18 22:38:37.853092 mpd_what-1.1.0/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      775 2022-04-10 19:10:54.000000 mpd_what-1.1.0/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2024-04-18 22:38:37.849092 mpd_what-1.1.0/bin/
+-rwxrwxr-x   0 rob       (1000) rob       (1000)    25755 2024-04-18 22:32:45.000000 mpd_what-1.1.0/bin/mpd_what
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2024-04-18 22:38:37.853092 mpd_what-1.1.0/mpd_what.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1099 2024-04-18 22:38:36.000000 mpd_what-1.1.0/mpd_what.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      214 2024-04-18 22:38:36.000000 mpd_what-1.1.0/mpd_what.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2024-04-18 22:38:36.000000 mpd_what-1.1.0/mpd_what.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       95 2024-04-18 22:38:36.000000 mpd_what-1.1.0/mpd_what.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2024-04-18 22:38:36.000000 mpd_what-1.1.0/mpd_what.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2024-04-18 22:38:37.853092 mpd_what-1.1.0/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)      662 2024-04-18 22:34:43.000000 mpd_what-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mpd_what-1.0.9/LICENSE.txt` & `mpd_what-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpd_what-1.0.9/PKG-INFO` & `mpd_what-1.1.0/mpd_what.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 1.1
-Name: mpd_what
-Version: 1.0.9
+Metadata-Version: 2.1
+Name: mpd-what
+Version: 1.1.0
 Summary: A python album art and music info getter
 Home-page: https://github.com/charmparticle/mpd_what
 Author: github.com/charmparticle
-Author-email: UNKNOWN
 License: GPL3
-Description: mpd_what is a python script to grab album art and find out what is playing on your mpd server. In addition to finding art and info for what you're playing locally, it also will try to find art and info for internet radio stations you might be playing. I'm not aware of any other mpd album art getters that do this. Since every internet radio station is unique in its configuration, this script doesn't work with all of them, and probably it never will, but it tries to do the best it can.
-        
-        Since this script relies on pycurl, you need to install pycurl first.
-        
-        Since pycurl has complex dependencies on libpython, it's best to install it using your distro's package manager, ie:
-        
-            sudo apt install python3-pycurl
-        
-        find out more at https://github.com/charmparticle/mpd_what
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+License-File: LICENSE.txt
+
+mpd_what is a python script to grab album art and find out what is playing on your mpd server. In addition to finding art and info for what you're playing locally, it also will try to find art and info for internet radio stations you might be playing. I'm not aware of any other mpd album art getters that do this. Since every internet radio station is unique in its configuration, this script doesn't work with all of them, and probably it never will, but it tries to do the best it can.
+
+Since this script relies on pycurl, you need to install pycurl first.
+
+Since pycurl has complex dependencies on libpython, it's best to install it using your distro's package manager, ie:
+
+    sudo apt install python3-pycurl
+
+find out more at https://github.com/charmparticle/mpd_what
```

### Comparing `mpd_what-1.0.9/README.md` & `mpd_what-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mpd_what-1.0.9/mpd_what.egg-info/PKG-INFO` & `mpd_what-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 1.1
-Name: mpd-what
-Version: 1.0.9
+Metadata-Version: 2.1
+Name: mpd_what
+Version: 1.1.0
 Summary: A python album art and music info getter
 Home-page: https://github.com/charmparticle/mpd_what
 Author: github.com/charmparticle
-Author-email: UNKNOWN
 License: GPL3
-Description: mpd_what is a python script to grab album art and find out what is playing on your mpd server. In addition to finding art and info for what you're playing locally, it also will try to find art and info for internet radio stations you might be playing. I'm not aware of any other mpd album art getters that do this. Since every internet radio station is unique in its configuration, this script doesn't work with all of them, and probably it never will, but it tries to do the best it can.
-        
-        Since this script relies on pycurl, you need to install pycurl first.
-        
-        Since pycurl has complex dependencies on libpython, it's best to install it using your distro's package manager, ie:
-        
-            sudo apt install python3-pycurl
-        
-        find out more at https://github.com/charmparticle/mpd_what
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+License-File: LICENSE.txt
+
+mpd_what is a python script to grab album art and find out what is playing on your mpd server. In addition to finding art and info for what you're playing locally, it also will try to find art and info for internet radio stations you might be playing. I'm not aware of any other mpd album art getters that do this. Since every internet radio station is unique in its configuration, this script doesn't work with all of them, and probably it never will, but it tries to do the best it can.
+
+Since this script relies on pycurl, you need to install pycurl first.
+
+Since pycurl has complex dependencies on libpython, it's best to install it using your distro's package manager, ie:
+
+    sudo apt install python3-pycurl
+
+find out more at https://github.com/charmparticle/mpd_what
```

### Comparing `mpd_what-1.0.9/bin/mpd_what` & `mpd_what-1.1.0/bin/mpd_what`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python3
 import os
+#import logging
 import yaml
 import difflib
 import random
 from time import time, ctime, sleep, mktime, localtime
 from sys import argv, stderr
 #from requests.utils import requote_uri
+from urllib.parse import urlparse
 from latest_user_agents import get_random_user_agent
 import json
 from mpd import MPDClient
 import pycurl
 import magic
 import unicodedata
 import discogs_client
@@ -36,14 +38,15 @@
     mpd_port="6600"
     discogs_token = ""
     lastfm_user = ""
     lastfm_pass = ""
     lastfm_api_key = ""
     lastfm_api_secret = ""
     showinfo=True
+    fdl=False
     dl=False
     scrobble=False
 ################################################################################
 # This part is necessary for python to understand what '~' means.
     config_dir = os.path.expanduser(config_dir)
     coverart_dir = os.path.expanduser(coverart_dir)
     lastplayed = os.path.expanduser(lastplayed)
@@ -76,14 +79,16 @@
     else:
         os.makedirs(config_dir, exist_ok=True)
         config_dict={'coverart_dir':coverart_dir, 'mpd_host':mpd_host,
                 'mpd_port':mpd_port, 'discogs_token':'please_sign_up_at_discogs_and_generate_a_token'}
         with open(config, 'w+') as config_file:
             config_file.write(yaml.dump(config_dict, default_flow_style=False))
 
+    #logging.basicConfig(filename=errlog, encoding='utf-8', level=logging.DEBUG)
+
     global useragent
     useragent = get_random_user_agent()
     global coverart
     
     def help_msg(me):
         print("usage:\n" +
               "\n{} -sc  or --scrobble to try to scrobble music to last.fm or libre.fm".format(me) +
@@ -213,15 +218,15 @@
                         epoch = time()
                         when = ctime(epoch)
                         with open (errlog, 'a') as logfile:
                             logfile.write(str(when) + ': ' + ' in get_coverart() ' + str(e) + '\n')
                         #print("error getting file " + str(e))
                         return False
             #fi
-        except OSError as e:
+        except Exception as e:
             epoch = time()
             when = ctime(epoch)
             with open (errlog, 'a') as logfile:
                 logfile.write(str(when) + ': ' + ' in get_coverart() ' + str(e) + '\n')
             #print("error in get_coverart: " + str(e))
             return False
     
@@ -244,15 +249,15 @@
                     artist = "KEXP"
                     song = "Air Break"
                 else:
                     artist = str(json.loads(onair)["results"][0]["artist"]["name"])
                     album = str(json.loads(onair)["results"][0]["release"]["name"])
                     song = str(json.loads(onair)["results"][0]["track"]["name"])
                 #fi
-            elif 'kusf' in station:
+            elif 'kusf' in station or 'no name' in station:
                 url = "http://www.kusf.org/api/broadcasting"
                 onair = get_url(url, "utf-8")
                 artist = str(json.loads(onair)["Track"]["artist"]).replace('"', '')
                 album = str(json.loads(onair)["Track"]["album"]).replace('"', '')
                 song = str(json.loads(onair)["Track"]["title"]).replace('"', '')
                 if album == " ":
                     album = song
@@ -383,15 +388,15 @@
                 #station I haven't gotten the stream for.
                 mpdinfo = init()
                 if 'title' in mpdinfo:
                     info = mpdinfo['title'].split(' - ')
                     if len(info) == 1:
                         (artist)=info[0]
                     elif len(info) == 2:
-                        (artist,song) = info
+                        (artist,album) = info
                     elif len(info) == 3:
                         (artist,album,song) = info
             #fi
         except KeyError:
             pass
         return([artist, album, song])
     
@@ -409,17 +414,16 @@
                     results = dc.search(data[1], artist=data[0], type='release')
                     url = results.page(1)[0].images[0]['uri']
                     #with open (errlog, 'a') as logfile:
                     #    logfile.write(str(url) + ': ' + ' in get_coverart_info() ' + str(e) + '\n')
                 elif len(data) == 1:
                     results = dc.search(data[0], type='release')
                     url = results.page(1)[0].images[0]['uri']
-                    #with open (errlog, 'a') as logfile:
-                    #    logfile.write(str(url) + ': ' + ' in get_coverart_info() ' + str(e) + '\n')
-                print(fname)
+                #with open (errlog, 'a') as logfile:
+                #    logfile.write("url: " + url + ' in get_coverart_info() ' + '\n')
                 get_coverart(fname, url)
             except:
                 try:
                     get_coverart("generic_lp_icon.jpg", "https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/LP_Vinyl_Symbol_Icon.png/240px-LP_Vinyl_Symbol_Icon.png")
                     exit()
                     #print('prepare query failed')
                 except OSError as e:
@@ -433,28 +437,34 @@
     def get_mpd_info():
         global showinfo
         global dl
         global scrobble
         global lastfm
         mpdinfo = init()
     
-        #I prefer albumartist
-        if 'albumartist' in mpdinfo:
-            artist = mpdinfo['albumartist']
-        elif 'artist' in mpdinfo:
+        if 'artist' in mpdinfo:
             artist = mpdinfo['artist']
         elif 'name' in mpdinfo:
             station = mpdinfo['name']
             whatsplaying = get_station_info(station,dl)
             artist = whatsplaying[0]
         elif 'file' in mpdinfo:
-            whatsplaying = mpdinfo['file'].split('/')
-            artist = whatsplaying[0]
-            album = whatsplaying[1]
-            song = whatsplaying[2]
+            #if a station doesn't embed a name in the stream, we get get a url as a file
+            if (mpdinfo['file'].startswith("http://") or mpdinfo['file'].startswith("https://")):
+                fqdn = urlparse(mpdinfo['file']).netloc
+                dn = ('.'.join(fqdn.split('.')[-2:]))
+                #sometimes (perhaps, often), the url includes a port number. We don't want that.
+                dn = (dn.split(':')[0:])[0]
+                whatsplaying = get_station_info(dn,dl)
+                artist = whatsplaying[0]
+            else:
+                whatsplaying = mpdinfo['file'].split('/')
+                artist = whatsplaying[0]
+                album = whatsplaying[1]
+                song = whatsplaying[2]
         #fi
         #The , '' means, if album isn't there, use null instead of erroring out.
         if 'whatsplaying' in vars():
             pass
         else:
             album = mpdinfo.get('album', '')
             song = mpdinfo.get('title', '')
@@ -471,88 +481,100 @@
         last = ""
 
         if os.path.exists(lastplayed):
             with open(lastplayed, 'r') as lastfile:
                 last = lastfile.readlines()
                 last = ''.join(last).strip()
 
-        if (infostr != last):
-            if dl:
-                get_coverart_info(whatsplaying)
-            if (len(whatsplaying) >= 2):
-                if (len(whatsplaying) == 3):
-                    artist = whatsplaying[0]
-                    album = whatsplaying[1]
-                    title = whatsplaying[2]
-                    #print(whatsplaying)
-                elif (len(whatsplaying) == 2):
-                    artist = whatsplaying[0]
-                    album = ""
-                    title = whatsplaying[1]
-
-                if not ("http" in artist):
-                    with open(lastplayed, 'w+') as lastfile:
-                        lastfile.write(infostr)
-
-                    oneline_infostr = infostr.replace('\n', ';')
-
-                    with open(playlist, 'a') as p:
-                        epoch = time()
-                        today_date = ctime(epoch)
-                        p.write(today_date + ': ' + oneline_infostr + '\n')
-
-                    if ((lastfm_user, lastfm_pass, lastfm_api_key, lastfm_api_secret) != ("", "", "", "")) and scrobble and lastfm:
-
-                        epoch = time()
-                        when = ctime(epoch)
-                        try:
-                            lastfm = pylast.LastFMNetwork(api_key=lastfm_api_key,
-                                                          api_secret=lastfm_api_secret,
-                                                          username=lastfm_user,
-                                                          password_hash=pylast.md5(lastfm_pass))
-                            librefm = pylast.LibreFMNetwork(api_key=lastfm_api_key,
-                                                          api_secret=lastfm_api_secret,
-                                                          username=librefm_user,
-                                                          password_hash=pylast.md5(librefm_pass))
-                            if album == "":
-                                lastfm.scrobble(artist=artist, title=title, timestamp=epoch) 
-                                librefm.scrobble(artist=artist, title=title, timestamp=epoch) 
-                            else:
-                                lastfm.scrobble(artist=artist, album=album, title=title, timestamp=epoch) 
-                                librefm.scrobble(artist=artist, album=album, title=title, timestamp=epoch) 
-
-                        except Exception as e:
-                            with open (errlog, 'a') as logfile:
-                                logfile.write(str(when) + ': ' + str(e) + '\n')
-                        
+        if fdl:
+            get_coverart_info(whatsplaying)
+        else:
+            if (infostr != last):
+                if dl:
+                    get_coverart_info(whatsplaying)
+                if (len(whatsplaying) >= 2):
+                    if (len(whatsplaying) == 3):
+                        artist = whatsplaying[0]
+                        album = whatsplaying[1]
+                        title = whatsplaying[2]
+                        #print(whatsplaying)
+                    elif (len(whatsplaying) == 2):
+                        artist = whatsplaying[0]
+                        album = ""
+                        title = whatsplaying[1]
+                    artist = str(artist)
+                    album = str(album)
+                    title = str(title)
+
+                    if not ("http" in artist):
+                        with open(lastplayed, 'w+') as lastfile:
+                            lastfile.write(infostr)
+
+                        oneline_infostr = infostr.replace('\n', ';')
+
+                        with open(playlist, 'a') as p:
+                            epoch = time()
+                            today_date = ctime(epoch)
+                            p.write(today_date + ': ' + oneline_infostr + '\n')
+
+                        if ((lastfm_user, lastfm_pass, lastfm_api_key, lastfm_api_secret) != ("", "", "", "")) and scrobble and lastfm:
+
+                            epoch = time()
+                            when = ctime(epoch)
+                            try:
+                                with open (errlog, 'a') as logfile:
+                                    lastfm = pylast.LastFMNetwork(api_key=lastfm_api_key,
+                                                                  api_secret=lastfm_api_secret,
+                                                                  username=lastfm_user,
+                                                                  password_hash=pylast.md5(lastfm_pass))
+                                    librefm = pylast.LibreFMNetwork(api_key=lastfm_api_key,
+                                                                  api_secret=lastfm_api_secret,
+                                                                  username=librefm_user,
+                                                                  password_hash=pylast.md5(librefm_pass))
+                                    if album == "":
+                                        lastfm.scrobble(artist=artist, title=title, timestamp=epoch)
+                                        librefm.scrobble(artist=artist, title=title, timestamp=epoch)
+                                    else:
+                                        lastfm.scrobble(artist=artist, album=album, title=title, timestamp=epoch)
+                                        librefm.scrobble(artist=artist, album=album, title=title, timestamp=epoch)
+
+                            except Exception as e:
+                                with open (errlog, 'a') as logfile:
+                                    logfile.write("problem scrobbling: " + str(when) + ': ' + str(e) + '\n')
+                                    logfile.write(artist + '\n')
+                                    logfile.write(album + '\n')
+                                    logfile.write(title + '\n')
+                            
 
-        if showinfo: 
-            print(infostr)
-        #fi
+            if showinfo: 
+                print(infostr)
+            #fi
 
     def verify_args(a, gs):
         a = [s.lower() for s in a]
         #now we see if the user entered invalid args
         if len(a) > 1:
             for arg in a[1:]:
                 if arg in gs:
                     pass
                 else:
                     help_msg(a[0])
                     exit(0)
     
     def parse_args(a):
-        valid_singles = ['-g', '--get',  '-sc', '--scrobble', '-h', '--help', '-q', '--quiet']
+        valid_singles = ['-g', '--get',  '-sc', '--scrobble', '-h', '--help', '-q', '--quiet', '--force-download']
         verify_args(a, valid_singles)
         global dl, scrobble, showinfo
         if '-h' in a[1:] or '--help' in a[1:]:
             help_msg(a[0])
             exit(0)
         if '-g' in a[1:] or '--get' in a[1:] :
             dl=True
+        if '--force-download' in a[1:] :
+            fdl=True
         if '-q' in a[1:] or '--quiet' in a[1:]:
             showinfo=False
         if '-sc' in a[1:] or '--scrobble' in a[1:]:
             scrobble=True
     
 parse_args(argv)
 get_mpd_info()
```

### Comparing `mpd_what-1.0.9/setup.py` & `mpd_what-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup
 
 setup(
     name='mpd_what',
-    version='1.0.9',
+    version='1.1.0',
     author='github.com/charmparticle',
     scripts=['bin/mpd_what'],
     url='https://github.com/charmparticle/mpd_what',
     license='GPL3',
     description='A python album art and music info getter',
     long_description=open('README.md').read(),
     install_requires=[
         "python-mpd2",
         "pyyaml",
         "pycurl",
         "latest-user-agents",
         "python-magic",
         "python3-discogs-client",
         "pylast",
+        "urllib",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```

