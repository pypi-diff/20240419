# Comparing `tmp/sa818-0.2.2.tar.gz` & `tmp/sa818-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sa818-0.2.2.tar", last modified: Thu Jan  5 21:01:39 2023, max compression
+gzip compressed data, was "sa818-0.2.3.tar", last modified: Fri Apr 19 15:22:47 2024, max compression
```

## Comparing `sa818-0.2.2.tar` & `sa818-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-01-05 21:01:39.111873 sa818-0.2.2/
--rw-r--r--   0 fred       (501) staff       (20)       56 2020-12-28 23:07:23.000000 sa818-0.2.2/.gitignore
--rw-r--r--   0 fred       (501) staff       (20)     1321 2020-12-25 18:38:33.000000 sa818-0.2.2/LICENSE
--rw-r--r--   0 fred       (501) staff       (20)     1062 2023-01-05 21:01:39.111341 sa818-0.2.2/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)     4964 2023-01-05 21:00:46.000000 sa818-0.2.2/README.md
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-01-05 21:01:39.105281 sa818-0.2.2/docs/
--rw-r--r--   0 fred       (501) staff       (20)   316331 2020-12-25 22:25:10.000000 sa818-0.2.2/docs/IMG_0716.JPG
--rw-r--r--   0 fred       (501) staff       (20)   816814 2023-01-05 21:00:46.000000 sa818-0.2.2/docs/SA818_moduleV3.4.pdf
--rw-r--r--   0 fred       (501) staff       (20)   232499 2020-12-25 17:28:59.000000 sa818-0.2.2/docs/SA818_programming_manual.pdf
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2023-01-05 21:01:39.110623 sa818-0.2.2/sa818.egg-info/
--rw-r--r--   0 fred       (501) staff       (20)     1062 2023-01-05 21:01:38.000000 sa818-0.2.2/sa818.egg-info/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      300 2023-01-05 21:01:38.000000 sa818-0.2.2/sa818.egg-info/SOURCES.txt
--rw-r--r--   0 fred       (501) staff       (20)        1 2023-01-05 21:01:38.000000 sa818-0.2.2/sa818.egg-info/dependency_links.txt
--rw-r--r--   0 fred       (501) staff       (20)       37 2023-01-05 21:01:38.000000 sa818-0.2.2/sa818.egg-info/entry_points.txt
--rw-r--r--   0 fred       (501) staff       (20)        9 2023-01-05 21:01:38.000000 sa818-0.2.2/sa818.egg-info/requires.txt
--rw-r--r--   0 fred       (501) staff       (20)        6 2023-01-05 21:01:38.000000 sa818-0.2.2/sa818.egg-info/top_level.txt
--rwxr-xr-x   0 fred       (501) staff       (20)    12970 2023-01-05 21:00:46.000000 sa818-0.2.2/sa818.py
--rw-r--r--   0 fred       (501) staff       (20)       38 2023-01-05 21:01:39.112028 sa818-0.2.2/setup.cfg
--rw-r--r--   0 fred       (501) staff       (20)     1478 2023-01-05 21:01:13.000000 sa818-0.2.2/setup.py
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-19 15:22:47.175787 sa818-0.2.3/
+-rw-r--r--   0 fred       (501) staff       (20)       70 2024-04-19 14:31:50.000000 sa818-0.2.3/.gitignore
+-rw-r--r--   0 fred       (501) staff       (20)     1321 2020-12-25 18:38:33.000000 sa818-0.2.3/LICENSE
+-rw-r--r--   0 fred       (501) staff       (20)     1062 2024-04-19 15:22:47.175694 sa818-0.2.3/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)     4982 2024-03-15 15:47:46.000000 sa818-0.2.3/README.md
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-19 15:22:47.174323 sa818-0.2.3/docs/
+-rw-r--r--   0 fred       (501) staff       (20)   316331 2020-12-25 22:25:10.000000 sa818-0.2.3/docs/IMG_0716.JPG
+-rw-r--r--   0 fred       (501) staff       (20)   816814 2023-01-05 21:00:46.000000 sa818-0.2.3/docs/SA818_moduleV3.4.pdf
+-rw-r--r--   0 fred       (501) staff       (20)   232499 2020-12-25 17:28:59.000000 sa818-0.2.3/docs/SA818_programming_manual.pdf
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-19 15:22:47.175550 sa818-0.2.3/sa818.egg-info/
+-rw-r--r--   0 fred       (501) staff       (20)     1062 2024-04-19 15:22:47.000000 sa818-0.2.3/sa818.egg-info/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      300 2024-04-19 15:22:47.000000 sa818-0.2.3/sa818.egg-info/SOURCES.txt
+-rw-r--r--   0 fred       (501) staff       (20)        1 2024-04-19 15:22:47.000000 sa818-0.2.3/sa818.egg-info/dependency_links.txt
+-rw-r--r--   0 fred       (501) staff       (20)       37 2024-04-19 15:22:47.000000 sa818-0.2.3/sa818.egg-info/entry_points.txt
+-rw-r--r--   0 fred       (501) staff       (20)        9 2024-04-19 15:22:47.000000 sa818-0.2.3/sa818.egg-info/requires.txt
+-rw-r--r--   0 fred       (501) staff       (20)        6 2024-04-19 15:22:47.000000 sa818-0.2.3/sa818.egg-info/top_level.txt
+-rwxr-xr-x   0 fred       (501) staff       (20)    12871 2024-04-19 14:50:18.000000 sa818-0.2.3/sa818.py
+-rw-r--r--   0 fred       (501) staff       (20)       38 2024-04-19 15:22:47.175817 sa818-0.2.3/setup.cfg
+-rw-r--r--   0 fred       (501) staff       (20)     1564 2024-04-19 15:17:38.000000 sa818-0.2.3/setup.py
```

### Comparing `sa818-0.2.2/LICENSE` & `sa818-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sa818-0.2.2/PKG-INFO` & `sa818-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sa818
-Version: 0.2.2
+Version: 0.2.3
 Summary: SA818 Programming Software
 Home-page: https://github.com/0x9900/SA818/
 Author: Fred C. (W6BSD)
 Author-email: w6bsd@bsdworld.org
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -30,13 +30,14 @@
 $ pip install sa818
 ```
 
 ### Example
 
 ```
 $ sa818 radio --frequency 145.230 --offset -.6 --ctcss 100
-SA818: INFO: +DMOSETGROUP:0, RX frequency: 145.2300, TX frequency: 144.6300, ctcss: 100.0, squelch: 4, OK
+SA818: INFO: +DMOSETGROUP:0, RX frequency: 145.2300, TX frequency: 144.6300, ctcss: 100.0,
+squelch: 4, OK
 
 $ sa818 volume --level 5
 SA818: INFO: +DMOSETVOLUME:0 Volume level: 5
 ```
```

### Comparing `sa818-0.2.2/README.md` & `sa818-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 can be used for Allstar, Echolink, APRS, or any digital modes.
 
 We use the program in this GitHub repository to program the radio
 module SA818 used for the Pi-Hat.
 
 <img src="docs/IMG_0716.JPG" width="250" height="250" />
 
-We have some PCB left. We are selling them for [$25 on tindie][1].
-You can also visit the this blog post [about this program][2]
+> Out of stock: ~We have some PCB left. We are selling them for [$25 on tindie][1].
+You can also visit the this blog post [about this program][2]~
 
 **Before programming the SA818 module, make sure you consult the band
 plan for your country and transmit on a frequency you are allowed to
 use.**
 
 ## Intallation
```

### Comparing `sa818-0.2.2/docs/IMG_0716.JPG` & `sa818-0.2.3/docs/IMG_0716.JPG`

 * *Files identical despite different names*

### Comparing `sa818-0.2.2/docs/SA818_moduleV3.4.pdf` & `sa818-0.2.3/docs/SA818_moduleV3.4.pdf`

 * *Files identical despite different names*

### Comparing `sa818-0.2.2/docs/SA818_programming_manual.pdf` & `sa818-0.2.3/docs/SA818_programming_manual.pdf`

 * *Files identical despite different names*

### Comparing `sa818-0.2.2/sa818.egg-info/PKG-INFO` & `sa818-0.2.3/sa818.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sa818
-Version: 0.2.2
+Version: 0.2.3
 Summary: SA818 Programming Software
 Home-page: https://github.com/0x9900/SA818/
 Author: Fred C. (W6BSD)
 Author-email: w6bsd@bsdworld.org
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -30,13 +30,14 @@
 $ pip install sa818
 ```
 
 ### Example
 
 ```
 $ sa818 radio --frequency 145.230 --offset -.6 --ctcss 100
-SA818: INFO: +DMOSETGROUP:0, RX frequency: 145.2300, TX frequency: 144.6300, ctcss: 100.0, squelch: 4, OK
+SA818: INFO: +DMOSETGROUP:0, RX frequency: 145.2300, TX frequency: 144.6300, ctcss: 100.0,
+squelch: 4, OK
 
 $ sa818 volume --level 5
 SA818: INFO: +DMOSETVOLUME:0 Volume level: 5
 ```
```

### Comparing `sa818-0.2.2/sa818.py` & `sa818-0.2.3/sa818.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/env python3
-# Fred (W6BSD)
+#
+# BSD 2-Clause License
+#
+# Copyright (c) 2022-2023 Fred W6BSD
+# All rights reserved.
 #
 
 __doc__ = """sa818"""
 
 import argparse
 import logging
 import os
@@ -37,14 +41,15 @@
   "703", "712", "723", "731", "732", "734", "743", "754"
 ]
 
 BAUD_RATES = [300, 1200, 2400, 4800, 9600, 19200, 38400, 57600, 115200]
 
 DEFAULT_BAUDRATE = 9600
 
+
 class SA818:
   EOL = "\r\n"
   INIT = "AT+DMOCONNECT"
   SETGRP = "AT+DMOSETGROUP"
   FILTER = "AT+SETFILTER"
   VOLUME = "AT+DMOSETVOLUME"
   TAIL = "AT+SETTAIL"
@@ -119,21 +124,20 @@
     tone = opts.ctcss if opts.ctcss else opts.dcs
     if tone:                # 0000 = No ctcss or dcs tone
       tx_tone, rx_tone = tone
     else:
       tx_tone, rx_tone = ['0000', '0000']
 
     if opts.offset == 0.0:
-      tx_freq = rx_freq = "{:.4f}".format(opts.frequency)
+      tx_freq = rx_freq = "{opts.frequency:.4f}"
     else:
-      rx_freq = "{:.4f}".format(opts.frequency)
-      tx_freq = "{:.4f}".format(opts.frequency + opts.offset)
+      rx_freq = "{opts.frequency:.4f}"
+      tx_freq = "{opts.frequency + opts.offset:.4f}"
 
-    cmd = "{}={},{},{},{},{},{}".format(self.SETGRP, opts.bw, tx_freq, rx_freq,
-                                        tx_tone, opts.squelch, rx_tone)
+    cmd = "{self.SETGRP}={opts.bw},{tx_freq},{rx_freq},{tx_tone},{opts.squelch},{rx_tone}"
     self.send(cmd)
     time.sleep(1)
     response = self.readline()
     if response != '+DMOSETGROUP:0':
       logger.error('SA818 programming error')
     else:
       bw_label = ['Narrow', 'Wide'][opts.bw]
@@ -153,38 +157,37 @@
       self.close_tail(opts)
     elif opts.close_tail is not None:
       logger.warning('Ignoring "--close-tail" specified without ctcss')
 
   def set_filter(self, opts):
     _yn = {True: "Yes", False: "No"}
     # filters are pre-emphasis, high-pass, low-pass
-    cmd = "{}={},{},{}".format(self.FILTER, int(not opts.emphasis),
-                               int(opts.highpass), int(opts.lowpass))
+    cmd = "{self.FILTER}={nt(not opts.emphasis)},{int(opts.highpass)},{int(opts.lowpass)}"
     self.send(cmd)
     time.sleep(1)
     response = self.readline()
     if response != "+DMOSETFILTER:0":
       logger.error('SA818 set filter error')
     else:
       logger.info("%s filters [Pre/De]emphasis: %s, high-pass: %s, low-pass: %s",
                   response, _yn[opts.emphasis], _yn[opts.highpass], _yn[opts.lowpass])
 
   def set_volume(self, opts):
-    cmd = "{}={:d}".format(self.VOLUME, opts.level)
+    cmd = "{self.VOLUME}={opts.level:d}"
     self.send(cmd)
     time.sleep(1)
     response = self.readline()
     if response != "+DMOSETVOLUME:0":
       logger.error('SA818 set volume error')
     else:
       logger.info("%s Volume level: %d, OK", response, opts.level)
 
   def close_tail(self, opts):
     _yn = {True: "Yes", False: "No"}
-    cmd = "{}={}".format(self.TAIL, int(opts.close_tail))
+    cmd = "{self.TAIL}={int(opts.close_tail)}"
     self.send(cmd)
     time.sleep(1)
     response = self.readline()
     if response != "+DMOSETTAIL:0":
       logger.error('SA818 set filter error')
     else:
       logger.info("%s close tail: %s", response, _yn[opts.close_tail])
@@ -197,14 +200,15 @@
     raise argparse.ArgumentTypeError from None
 
   if not 144 < frequency < 148 and not 420 < frequency < 450:
     logger.error('Frequency outside the amateur bands')
     raise argparse.ArgumentError
   return frequency
 
+
 def type_ctcss(parg):
   err_msg = 'Invalid CTCSS use the --help argument for the list of CTCSS'
   tone_codes = []
   codes = parg.split(',')
   if len(codes) == 1:
     codes.append(codes[0])
   elif len(codes) > 2:
@@ -220,14 +224,15 @@
       tone_codes.append(f"{ctcss:04d}")
     except ValueError:
       logger.error(err_msg)
       raise argparse.ArgumentTypeError from None
 
   return tone_codes
 
+
 def type_dcs(parg):
   err_msg = 'Invalid DCS use the --help argument for the list of DCS'
   dcs_codes = []
   codes = parg.split(',')
   if len(codes) == 1:
     codes.append(codes[0])
   elif len(codes) > 2:
@@ -237,85 +242,91 @@
   for code in codes:
     if code[-1] not in ('N', 'I'):
       logger.error(err_msg)
       raise argparse.ArgumentError from None
 
     code, direction = code[:-1], code[-1]
     try:
-      dcs = "{:03d}".format(int(code))
+      dcs = "{int(code):03d}"
       if dcs not in DCS_CODES:
         logger.error(err_msg)
         raise argparse.ArgumentError
     except ValueError:
       raise argparse.ArgumentTypeError from None
     dcs_codes.append(dcs + direction)
 
   return dcs_codes
 
+
 def type_squelch(parg):
   try:
     value = int(parg)
   except ValueError:
     raise argparse.ArgumentTypeError from None
 
   if value not in range(0, 9):
     logger.error('The value must must be between 0 and 8 (inclusive)')
     raise argparse.ArgumentError
   return value
 
+
 def type_level(parg):
   try:
     value = int(parg)
   except ValueError:
     raise argparse.ArgumentTypeError from None
 
   if value not in range(1, 9):
     logger.error('The value must must be between 1 and 8 (inclusive)')
     raise argparse.ArgumentError
   return value
 
+
 def yesno(parg):
   yes_strings = ["y", "yes", "true", "1", "on"]
   no_strings = ["n", "no", "false", "0", "off"]
   if parg.lower() in yes_strings:
     return True
   if parg.lower() in no_strings:
     return False
   raise argparse.ArgumentError
 
+
 def noneyesno(parg):
   if parg is not None:
     return yesno(parg)
   return None
 
+
 def set_loglevel():
   loglevel = os.getenv('LOGLEVEL', 'INFO')
   loglevel = loglevel.upper()
   try:
     logger.root.setLevel(loglevel)
   except ValueError:
     logger.warning('Loglevel error: %s', loglevel)
 
+
 def format_codes():
   ctcss = textwrap.wrap(', '.join(CTCSS[1:]))
   dcs = textwrap.wrap(', '.join(DCS_CODES))
 
   codes = (
     "You can specify a different code for transmit and receive by separating "
     "them by a comma.\n",
     "> Example: --ctcss 94.8,127.3 or --dcs 043N,047N\n\n",
-    "CTCSS codes (PL Tones):\n{}".format('\n'.join(ctcss)),
+    f"CTCSS codes (PL Tones)\n{chr(10).join(ctcss)}",
     "\n\n",
     "DCS Codes:\n"
     "DCS codes must be followed by N or I for Normal or Inverse:\n",
-    "> Example: 047I\n"
-    "{}".format('\n'.join(dcs))
+    f"> Example: 047I\n{chr(10).join(dcs)}"
   )
   return ''.join(codes)
 
+
 def main():
   set_loglevel()
   parser = argparse.ArgumentParser(
     description="generate configuration for switch port",
     epilog=format_codes(),
     formatter_class=argparse.RawDescriptionHelpFormatter,
   )
@@ -344,15 +355,15 @@
                                 "[I inverse]  [default: %(default)s]"))
   p_radio.add_argument("--close-tail", default=None, type=noneyesno,
                        help="Close CTCSS Tail Tone (yes/no)")
 
   p_volume = subparsers.add_parser("volume", help="Set the volume level")
   p_volume.set_defaults(func="volume")
   p_volume.add_argument("--level", type=type_level, default=4,
-                      help="Volume value (1 to 8) [default: %(default)s]")
+                        help="Volume value (1 to 8) [default: %(default)s]")
 
   p_filter = subparsers.add_parser("filters", help="Set/Unset filters")
   p_filter.set_defaults(func="filters")
   p_filter.add_argument("--emphasis", type=yesno, required=True,
                         help="Disable [Pr/De]-emphasis (yes/no)")
   p_filter.add_argument("--highpass", type=yesno, required=True,
                         help="Disable high pass filter (yes/no)")
@@ -385,9 +396,10 @@
   elif opts.func == 'radio':
     radio.set_radio(opts)
   elif opts.func == 'filters':
     radio.set_filter(opts)
   elif opts.func == 'volume':
     radio.set_volume(opts)
 
+
 if __name__ == "__main__":
   main()
```

### Comparing `sa818-0.2.2/setup.py` & `sa818-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 #!/usr/bin/env python3
 #
+# BSD 2-Clause License
+#
+# Copyright (c) 2022-2023 Fred W6BSD
+# All rights reserved.
+#
+
 import sys
 
 from setuptools import setup
 
 __doc__ = """
 
 ## SA818 Programming
@@ -17,24 +23,25 @@
 $ pip install sa818
 ```
 
 ### Example
 
 ```
 $ sa818 radio --frequency 145.230 --offset -.6 --ctcss 100
-SA818: INFO: +DMOSETGROUP:0, RX frequency: 145.2300, TX frequency: 144.6300, ctcss: 100.0, squelch: 4, OK
+SA818: INFO: +DMOSETGROUP:0, RX frequency: 145.2300, TX frequency: 144.6300, ctcss: 100.0,
+squelch: 4, OK
 
 $ sa818 volume --level 5
 SA818: INFO: +DMOSETVOLUME:0 Volume level: 5
 ```
 
 """
 
 __author__ = "Fred C. (W6BSD)"
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 __license__ = 'BSD'
 
 py_version = sys.version_info[:2]
 if py_version < (3, 8):
   raise RuntimeError('SA818 requires Python 3.8 or later')
 
 setup(
@@ -45,15 +52,15 @@
   long_description_content_type='text/markdown',
   url='https://github.com/0x9900/SA818/',
   license=__license__,
   author=__author__,
   author_email='w6bsd@bsdworld.org',
   py_modules=['sa818'],
   install_requires=['pyserial'],
-  entry_points = {
+  entry_points={
     'console_scripts': ['sa818 = sa818:main'],
   },
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
```

