# Comparing `tmp/pyspartn-0.2.1.tar.gz` & `tmp/pyspartn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspartn-0.2.1.tar", last modified: Sun Mar 17 17:05:40 2024, max compression
+gzip compressed data, was "pyspartn-0.3.0.tar", last modified: Fri Apr 19 06:31:55 2024, max compression
```

## Comparing `pyspartn-0.2.1.tar` & `pyspartn-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-17 17:05:40.580819 pyspartn-0.2.1/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2023-03-28 07:19:43.000000 pyspartn-0.2.1/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2023-08-07 08:57:54.000000 pyspartn-0.2.1/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    18704 2024-03-17 17:05:40.580345 pyspartn-0.2.1/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    15102 2023-12-05 07:22:17.000000 pyspartn-0.2.1/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2455 2024-03-17 17:02:57.000000 pyspartn-0.2.1/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-03-17 17:05:40.580894 pyspartn-0.2.1/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-17 17:05:40.571558 pyspartn-0.2.1/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-17 17:05:40.578241 pyspartn-0.2.1/src/pyspartn/
--rw-r--r--   0 steve      (501) staff       (20)      598 2023-06-06 06:30:11.000000 pyspartn-0.2.1/src/pyspartn/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2024-03-17 17:02:57.000000 pyspartn-0.2.1/src/pyspartn/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      671 2023-03-28 07:19:43.000000 pyspartn-0.2.1/src/pyspartn/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     2441 2023-06-12 06:49:18.000000 pyspartn-0.2.1/src/pyspartn/socket_stream.py
--rw-r--r--   0 steve      (501) staff       (20)     7808 2024-03-07 14:54:08.000000 pyspartn-0.2.1/src/pyspartn/spartnhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    18785 2024-03-17 17:02:57.000000 pyspartn-0.2.1/src/pyspartn/spartnmessage.py
--rw-r--r--   0 steve      (501) staff       (20)    10066 2024-03-07 14:54:08.000000 pyspartn-0.2.1/src/pyspartn/spartnreader.py
--rw-r--r--   0 steve      (501) staff       (20)      222 2023-03-28 07:19:43.000000 pyspartn-0.2.1/src/pyspartn/spartntables.py
--rw-r--r--   0 steve      (501) staff       (20)     8855 2024-03-07 14:54:08.000000 pyspartn-0.2.1/src/pyspartn/spartntypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    22382 2024-03-07 14:54:08.000000 pyspartn-0.2.1/src/pyspartn/spartntypes_get.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-17 17:05:40.579506 pyspartn-0.2.1/src/pyspartn.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    18704 2024-03-17 17:05:40.000000 pyspartn-0.2.1/src/pyspartn.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      576 2024-03-17 17:05:40.000000 pyspartn-0.2.1/src/pyspartn.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-03-17 17:05:40.000000 pyspartn-0.2.1/src/pyspartn.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      134 2024-03-17 17:05:40.000000 pyspartn-0.2.1/src/pyspartn.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        9 2024-03-17 17:05:40.000000 pyspartn-0.2.1/src/pyspartn.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-03-17 17:05:40.579285 pyspartn-0.2.1/tests/
--rw-r--r--   0 steve      (501) staff       (20)     4043 2023-03-28 07:19:43.000000 pyspartn-0.2.1/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)     6172 2024-01-29 08:03:46.000000 pyspartn-0.2.1/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)    36197 2023-11-20 10:51:30.000000 pyspartn-0.2.1/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-19 06:31:55.616942 pyspartn-0.3.0/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2023-03-28 07:19:43.000000 pyspartn-0.3.0/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2023-08-07 08:57:53.000000 pyspartn-0.3.0/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    19291 2024-04-19 06:31:55.616666 pyspartn-0.3.0/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    15697 2024-04-19 06:26:54.000000 pyspartn-0.3.0/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2446 2024-04-19 06:26:54.000000 pyspartn-0.3.0/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-04-19 06:31:55.616987 pyspartn-0.3.0/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-19 06:31:55.612523 pyspartn-0.3.0/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-19 06:31:55.614604 pyspartn-0.3.0/src/pyspartn/
+-rw-r--r--   0 steve      (501) staff       (20)      598 2023-06-06 06:30:11.000000 pyspartn-0.3.0/src/pyspartn/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2024-04-19 06:26:54.000000 pyspartn-0.3.0/src/pyspartn/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      671 2023-03-28 07:19:43.000000 pyspartn-0.3.0/src/pyspartn/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     2441 2023-06-12 06:49:18.000000 pyspartn-0.3.0/src/pyspartn/socket_stream.py
+-rw-r--r--   0 steve      (501) staff       (20)     7808 2024-03-07 14:54:08.000000 pyspartn-0.3.0/src/pyspartn/spartnhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    18484 2024-04-19 06:26:54.000000 pyspartn-0.3.0/src/pyspartn/spartnmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)    10066 2024-03-07 14:54:08.000000 pyspartn-0.3.0/src/pyspartn/spartnreader.py
+-rw-r--r--   0 steve      (501) staff       (20)      222 2023-03-28 07:19:43.000000 pyspartn-0.3.0/src/pyspartn/spartntables.py
+-rw-r--r--   0 steve      (501) staff       (20)     8453 2024-04-19 06:26:54.000000 pyspartn-0.3.0/src/pyspartn/spartntypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    25738 2024-04-19 06:26:54.000000 pyspartn-0.3.0/src/pyspartn/spartntypes_get.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-19 06:31:55.615919 pyspartn-0.3.0/src/pyspartn.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    19291 2024-04-19 06:31:55.000000 pyspartn-0.3.0/src/pyspartn.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      576 2024-04-19 06:31:55.000000 pyspartn-0.3.0/src/pyspartn.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-04-19 06:31:55.000000 pyspartn-0.3.0/src/pyspartn.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      134 2024-04-19 06:31:55.000000 pyspartn-0.3.0/src/pyspartn.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        9 2024-04-19 06:31:55.000000 pyspartn-0.3.0/src/pyspartn.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-19 06:31:55.615683 pyspartn-0.3.0/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     4043 2023-03-28 07:19:43.000000 pyspartn-0.3.0/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)     6172 2024-01-29 08:03:46.000000 pyspartn-0.3.0/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)    95165 2024-04-19 06:26:54.000000 pyspartn-0.3.0/tests/test_stream.py
```

### Comparing `pyspartn-0.2.1/LICENSE` & `pyspartn-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspartn-0.2.1/PKG-INFO` & `pyspartn-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.2.1
+Version: 0.3.0
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -32,15 +32,15 @@
         SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/semuconsulting/pyspartn
 Project-URL: documentation, https://www.semuconsulting.com/pyspartn/
 Project-URL: repository, https://github.com/semuconsulting/pyspartn
 Project-URL: changelog, https://github.com/semuconsulting/pyspartn/blob/master/RELEASE_NOTES.md
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
@@ -80,50 +80,54 @@
 [Parsing](#parsing) |
 [Generating](#generating) |
 [Serializing](#serializing) |
 [Examples](#examples) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
-`pyspartn` is an original Python 3 parser for the SPARTN &copy; GPS/GNSS protocol. SPARTN is an open-source GPS/GNSS [differential correction or DGPS](https://en.wikipedia.org/wiki/Differential_GPS) protocol published by u-blox.
+`pyspartn` is an original Python 3 parser for the SPARTN &copy; GPS/GNSS protocol. SPARTN is an open-source GPS/GNSS [differential correction or DGPS](https://en.wikipedia.org/wiki/Differential_GPS) protocol published by u-blox:
 
-[SPARTN Protocol 2.01](https://www.spartnformat.org/download/) (available in the public domain).
+[SPARTN Protocol](https://www.spartnformat.org/download/) (available in the public domain).
 © 2021 u-blox AG. All rights reserved.
 
 The `pyspartn` homepage is located at [https://github.com/semuconsulting/pyspartn](https://github.com/semuconsulting/pyspartn).
 
 This is an independent project and we have no affiliation whatsoever with u-blox.
 
 **FYI** There are companion libraries which handle standard NMEA 0183 &copy;, UBX &copy; (u-blox) and RTCM3 &copy; GNSS/GPS messages:
-- [pyubx2](http://github.com/semuconsulting/pyubx2) (**FYI** installing `pyubx2` via pip also installs `pynmeagps` and `pyrtcm`)
+- [pyubx2](http://github.com/semuconsulting/pyubx2)
 - [pynmeagps](http://github.com/semuconsulting/pynmeagps)
 - [pyrtcm](http://github.com/semuconsulting/pyrtcm)
 
 ## <a name="currentstatus">Current Status</a>
 
-**WORK IN PROGRESS - CURRENTLY IN ALPHA.**
+**CURRENTLY IN BETA**
 
 <!--![Status](https://img.shields.io/pypi/status/pyspartn)-->
 ![Release](https://img.shields.io/github/v/release/semuconsulting/pyspartn?include_prereleases)
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
 The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class implements a provisional decrypt and decode for OCB, HPAC and GAD message types but it has not yet been fully tested (*appears to be working OK for GAD, HPAC and most OCB payloads, but some small OCB payloads (nData < 35) are still failing. For the time being, a temporary override has been implemented in `spartnmessage.py` to suppress the `decode` flag for those payload types that cannot yet be successfully decoded*).
+The `SPARTNMessage` class implements decrypt and decode algorithms for OCB, HPAC and GAD message types:
+ - GAD payload decryption and decode is fully tested and functional, which confirms that the global decryption mechanism and parsing algorithms are essentially correct.
+ - HPAC and OCB payload decodes appear to be working OK, but results have not yet been fully validated and some individual attributes may be incorrect.
+
+*For the time being, a temporary override has been implemented in `spartnmessage.py` to suppress the `decode` flag for those payload types that cannot yet be successfully decoded. Testing contributions welcome*.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
-[Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
+[Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, please use the [Discussion](https://github.com/semuconsulting/pyspartn/discussions) Forum.
 
 ---
 ## <a name="installation">Installation</a>
 
 `pyspartn` is compatible with Python >=3.8 and is dependent on the `cryptography` library.
 
 **NB:** If you're installing `pyspartn` on a 32-bit Linux platform, some additional installation steps may be required - see note *¹* below.
@@ -299,16 +303,19 @@
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
+1. `spartn_mqtt_client.py` - implements a simple SPARTN MQTT client using the pygnssutils.GNSSMQTTClient class. **NB**: requires a valid ClientID for a
+SPARTN MQTT service e.g. u-blox Thingstream PointPerfect.
+1. `spartn_decrypt.py` - illustrates how to read, decrypt and decode a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` example above).
 1. `rxmpmp_extract_spartn.py` - ilustrates how to extract individual SPARTN messages from the accumulated UBX-RXM-PMP data output by an NEO-D9S L-band correction receiver.
-1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the example above.
+1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the `rxmpmp_extract_spartn.py` above.
 1. `gad_plot.py` - illustrates how to extract geographic area definitions from a series of SPARTN-GAD-1X messages - the output file from the example above can be used as an input. This example also serves to illustrate how to decrypt SPARTN messages.
 
 ---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3 and SPARTN protocols is available at:
```

### Comparing `pyspartn-0.2.1/README.md` & `pyspartn-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,50 +6,54 @@
 [Parsing](#parsing) |
 [Generating](#generating) |
 [Serializing](#serializing) |
 [Examples](#examples) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
-`pyspartn` is an original Python 3 parser for the SPARTN &copy; GPS/GNSS protocol. SPARTN is an open-source GPS/GNSS [differential correction or DGPS](https://en.wikipedia.org/wiki/Differential_GPS) protocol published by u-blox.
+`pyspartn` is an original Python 3 parser for the SPARTN &copy; GPS/GNSS protocol. SPARTN is an open-source GPS/GNSS [differential correction or DGPS](https://en.wikipedia.org/wiki/Differential_GPS) protocol published by u-blox:
 
-[SPARTN Protocol 2.01](https://www.spartnformat.org/download/) (available in the public domain).
+[SPARTN Protocol](https://www.spartnformat.org/download/) (available in the public domain).
 © 2021 u-blox AG. All rights reserved.
 
 The `pyspartn` homepage is located at [https://github.com/semuconsulting/pyspartn](https://github.com/semuconsulting/pyspartn).
 
 This is an independent project and we have no affiliation whatsoever with u-blox.
 
 **FYI** There are companion libraries which handle standard NMEA 0183 &copy;, UBX &copy; (u-blox) and RTCM3 &copy; GNSS/GPS messages:
-- [pyubx2](http://github.com/semuconsulting/pyubx2) (**FYI** installing `pyubx2` via pip also installs `pynmeagps` and `pyrtcm`)
+- [pyubx2](http://github.com/semuconsulting/pyubx2)
 - [pynmeagps](http://github.com/semuconsulting/pynmeagps)
 - [pyrtcm](http://github.com/semuconsulting/pyrtcm)
 
 ## <a name="currentstatus">Current Status</a>
 
-**WORK IN PROGRESS - CURRENTLY IN ALPHA.**
+**CURRENTLY IN BETA**
 
 <!--![Status](https://img.shields.io/pypi/status/pyspartn)-->
 ![Release](https://img.shields.io/github/v/release/semuconsulting/pyspartn?include_prereleases)
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
 The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class implements a provisional decrypt and decode for OCB, HPAC and GAD message types but it has not yet been fully tested (*appears to be working OK for GAD, HPAC and most OCB payloads, but some small OCB payloads (nData < 35) are still failing. For the time being, a temporary override has been implemented in `spartnmessage.py` to suppress the `decode` flag for those payload types that cannot yet be successfully decoded*).
+The `SPARTNMessage` class implements decrypt and decode algorithms for OCB, HPAC and GAD message types:
+ - GAD payload decryption and decode is fully tested and functional, which confirms that the global decryption mechanism and parsing algorithms are essentially correct.
+ - HPAC and OCB payload decodes appear to be working OK, but results have not yet been fully validated and some individual attributes may be incorrect.
+
+*For the time being, a temporary override has been implemented in `spartnmessage.py` to suppress the `decode` flag for those payload types that cannot yet be successfully decoded. Testing contributions welcome*.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
-[Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
+[Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, please use the [Discussion](https://github.com/semuconsulting/pyspartn/discussions) Forum.
 
 ---
 ## <a name="installation">Installation</a>
 
 `pyspartn` is compatible with Python >=3.8 and is dependent on the `cryptography` library.
 
 **NB:** If you're installing `pyspartn` on a 32-bit Linux platform, some additional installation steps may be required - see note *¹* below.
@@ -225,16 +229,19 @@
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
+1. `spartn_mqtt_client.py` - implements a simple SPARTN MQTT client using the pygnssutils.GNSSMQTTClient class. **NB**: requires a valid ClientID for a
+SPARTN MQTT service e.g. u-blox Thingstream PointPerfect.
+1. `spartn_decrypt.py` - illustrates how to read, decrypt and decode a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` example above).
 1. `rxmpmp_extract_spartn.py` - ilustrates how to extract individual SPARTN messages from the accumulated UBX-RXM-PMP data output by an NEO-D9S L-band correction receiver.
-1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the example above.
+1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the `rxmpmp_extract_spartn.py` above.
 1. `gad_plot.py` - illustrates how to extract geographic area definitions from a series of SPARTN-GAD-1X messages - the output file from the example above can be used as an input. This example also serves to illustrate how to decrypt SPARTN messages.
 
 ---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3 and SPARTN protocols is available at:
```

### Comparing `pyspartn-0.2.1/pyproject.toml` & `pyspartn-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pyspartn"
 authors = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 maintainers = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 description = "SPARTN protocol parser"
-version = "0.2.1"
+version = "0.3.0"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Operating System :: OS Independent",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: MacOS X",
     "Environment :: Win32 (MS Windows)",
     "Environment :: X11 Applications",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: End Users/Desktop",
@@ -65,15 +65,15 @@
 skips = []
 
 [tool.pylint]
 jobs = 0
 reports = "y"
 recursive = "y"
 py-version = "3.8"
-fail-under = "9.6"
+fail-under = "9.8"
 fail-on = "E,F"
 clear-cache-post-run = "y"
 disable = """
     raw-checker-failed,
     bad-inline-option,
     locally-disabled,
     file-ignored,
@@ -81,12 +81,12 @@
     useless-suppression,
     deprecated-pragma,
     use-symbolic-message-instead,
 """
 
 [tool.pytest.ini_options]
 minversion = "7.0"
-addopts = "--cov --cov-report term-missing --cov-fail-under 80"
+addopts = "--cov --cov-report html --cov-fail-under 85"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 source = ["src"]
```

### Comparing `pyspartn-0.2.1/src/pyspartn/__init__.py` & `pyspartn-0.3.0/src/pyspartn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.2.1/src/pyspartn/exceptions.py` & `pyspartn-0.3.0/src/pyspartn/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.2.1/src/pyspartn/socket_stream.py` & `pyspartn-0.3.0/src/pyspartn/socket_stream.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.2.1/src/pyspartn/spartnhelpers.py` & `pyspartn-0.3.0/src/pyspartn/spartnhelpers.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.2.1/src/pyspartn/spartnmessage.py` & `pyspartn-0.3.0/src/pyspartn/spartnmessage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
-Skeleton SPARTNMessage class.
-
-TODO work in progress
+SPARTNMessage class.
 
 The MQTT key, required for payload decryption, can be passed as a keyword
 or set up as environment variable MQTTKEY.
 
 Created on 10 Feb 2023
 
 :author: semuadmin
@@ -31,15 +29,14 @@
     escapeall,
     timetag2date,
     valid_crc,
 )
 from pyspartn.spartntypes_core import (
     CBBMLEN,
     NB,
-    NESTED_DEPTH,
     PBBMLEN,
     SPARTN_DATA_FIELDS,
     SPARTN_MSGIDS,
     SPARTN_PRE,
     STBMLEN,
     VALCRC,
 )
@@ -167,16 +164,16 @@
             if not valid_crc(core, self.crc, self.crcType):
                 raise SPARTNMessageError(f"Invalid CRC {self.crc}")
 
         offset = 0  # payload offset in bits
         index = []  # array of (nested) group indices
 
         # ***********************************************************************************
-        # TODO temporary override of decode flag for message types that cannot yet be decoded
-        if self.msgType not in (0, 1, 2) or self.msgType == 0 and self.nData < 35:
+        # override of decode flag for message types that cannot yet be decoded
+        if self.msgType not in (0, 1, 2):
             self._decode = False
         # ***********************************************************************************
 
         # decrypt payload if encrypted
         if self.eaf and self._decode:
             iv = self._get_iv()
             self._payload = decrypt(payload, self._key, iv)
@@ -225,31 +222,14 @@
             + (self.solutionProcId << 64)  # TF011 4 bits
             + (self.encryptionId << 60)  # TF012 4 bits
             + (self.encryptionSeq << 54)  # TF012 6 bits
             + 1  # padding to 128 bits
         )
         return iv.to_bytes(16, "big")
 
-    def _get_attr_sfx(self, key: str, index: list) -> str:
-        """
-        Append nested group attribute name with appropriate indices.
-
-        :param str key: attribute keyword e.g. SF054
-        :param list index: repeating group index array e.g. [3,4]
-        :return: keyname with suffix e.g. SF054_03_04
-        :rtype: str
-        """
-
-        keyr = key
-        keyl = NESTED_DEPTH[key]
-        for i in range(keyl + 1):
-            n = index[i]
-            keyr += f"_{n:02d}"
-        return keyr
-
     def _set_attribute(self, offset: int, pdict: dict, key: str, index: list) -> tuple:
         """
         Recursive routine to set individual, optional or grouped payload attributes.
 
         :param int offset: payload offset in bits
         :param dict pdict: dict representing payload definition
         :param str key: attribute keyword
@@ -280,20 +260,25 @@
         :param int offset: payload offset in bits
         :param list index: repeating group index array
         :return: (offset, index[])
         :rtype: tuple
         """
 
         pres = False
-        (key, con), gdict = attg  # (attribute, condition), group dictionary
-        keyr = self._get_attr_sfx(key, index)
+        (numr, con), gdict = attg  # (attribute, condition), group dictionary
+        # "+n" suffix signifies that one or more nested group indices
+        # must be appended to name e.g. "DF379_01", "IDF023_03"
+        if "+" in numr:
+            numr, nestlevel = numr.split("+")
+            for i in range(int(nestlevel)):
+                numr += f"_{index[i]:02d}"
         if isinstance(con, int):  # present if attribute == value
-            pres = getattr(self, keyr) == con
+            pres = getattr(self, numr) == con
         elif isinstance(con, list):  # present if attribute in range of values
-            pres = getattr(self, keyr) in con
+            pres = getattr(self, numr) in con
 
         # recursively process each group attribute,
         # incrementing the payload offset as we go
         if pres:
             for key1 in gdict:
                 (offset, index) = self._set_attribute(offset, gdict, key1, index)
 
@@ -311,30 +296,30 @@
         :param int offset: payload offset in bits
         :param list index: repeating group index array
         :return: (offset, index[])
         :rtype: tuple
         """
 
         index.append(0)
-        key, gdict = attg  # size, group dictionary
-
-        # if attribute is part of a (nested) repeating group, suffix name with index
-        keyr = key
-        for i in index:  # one index for each nested level
-            if i > 0:
-                keyr += f"_{i:02d}"
+        numr, gdict = attg  # size, group dictionary
 
         # derive or retrieve number of items in group
-        if isinstance(keyr, int):  # repeats = fixed integer
-            rng = keyr
-        elif isinstance(keyr, str):  # repeats defined in named attribute
-            if keyr[0:3] == NB:  # repeats = num bits set
-                rng = bin(getattr(self, keyr[3:])).count("1")
+        if isinstance(numr, int):  # repeats = fixed integer
+            rng = numr
+        elif isinstance(numr, str):  # repeats defined in named attribute
+            # "+n" suffix signifies that one or more nested group indices
+            # must be appended to name e.g. "DF379_01", "IDF023_03"
+            if "+" in numr:
+                numr, nestlevel = numr.split("+")
+                for i in range(int(nestlevel)):
+                    numr += f"_{index[i]:02d}"
+            if numr[0:3] == NB:  # repeats = num bits set
+                rng = bin(getattr(self, numr[3:])).count("1")
             else:
-                rng = getattr(self, keyr)  # repeats = attribute value
+                rng = getattr(self, numr)  # repeats = attribute value
 
         # recursively process each group attribute,
         # incrementing the payload offset and index as we go
         for i in range(rng):
             index[-1] = i + 1
             for key1 in gdict:
                 (offset, index) = self._set_attribute(offset, gdict, key1, index)
@@ -371,19 +356,19 @@
         # get value of required number of bits at current payload offset
         # (attribute length, resolution, description)
         attlen, res, _ = SPARTN_DATA_FIELDS[key]
         if isinstance(attlen, str):  # variable length attribute
             attlen = self._getvarlen(key, index)
         if not self._scaling:
             res = 0
-        try:  # TODO temporary DEBUG of payload failure
+        try:
             val = bitsval(self._payload, offset, attlen)
         except SPARTNMessageError as err:
             # print(self)
-            raise (err)
+            raise err
 
         setattr(self, keyr, val)
 
         offset += attlen
 
         return offset
 
@@ -455,15 +440,15 @@
             elif key == "SF105":  # Galileo code bias mask
                 attl = [8, 15][sflen]
             elif key == "SF106":  # BDS code bias mask
                 attl = [8, 15][sflen]
             elif key == "SF107":  # QZSS code bias mask
                 attl = [6, 11][sflen]
         elif key == "SF079":  # Grid node present mask
-            pass  # TODO used by BPAC
+            pass  # TODO used by BPAC, not yet implemented
         elif key == "SF088":  # Cryptographic Key,
             attl = self.SF087
         elif key == "SF092":  # Computed Authentication Data (CAD),
             attl = self.SF091
 
         return attl
```

### Comparing `pyspartn-0.2.1/src/pyspartn/spartnreader.py` & `pyspartn-0.3.0/src/pyspartn/spartnreader.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.2.1/src/pyspartn/spartntypes_core.py` & `pyspartn-0.3.0/src/pyspartn/spartntypes_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,35 +50,14 @@
 
 # Transient attribute names used to store variable bitmask length flags
 NB = "NB_"
 STBMLEN = "SatBitmaskLen"
 PBBMLEN = "PhaseBiasBitmaskLen"
 CBBMLEN = "CodeBiasBitmaskLen"
 
-# Nested group depth for conditional attributes
-# (so we know how many group indices to add e.g. SF011_02, SF056_02_04)
-NESTED_DEPTH = {
-    "SF008": -1,
-    "SF011": 0,
-    "SF012": 0,
-    "SF013": 0,
-    "SF014O": 0,
-    "SF014C": 0,
-    "SF014B": 0,
-    "SF093": 0,
-    "SF094": 0,
-    "SF095": 0,
-    "SF040T": 0,
-    "SF040I": 0,
-    "SF041": 0,
-    "SF044": 0,
-    "SF054": 0,
-    "SF056": 1,
-}
-
 # datafields used in message definitions
 # key: (length in bits, resolution, description)
 SPARTN_DATA_FIELDS = {
     "SF005": (9, "1", "Solution issue of update (SIOU)"),
     "SF008": (1, "n/a", "Yaw present flag"),
     "SF009": (1, "1", "Satellite reference datum"),
     "SF010": (1, "n/a", "End of OCB set (EOS)"),
```

### Comparing `pyspartn-0.2.1/src/pyspartn/spartntypes_get.py` & `pyspartn-0.3.0/src/pyspartn/spartntypes_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,31 +31,17 @@
 OCB_SAT_FLAGS = {  # table 6.4
     "SF014O": "Orbit data present flag",
     "SF014C": "Clock data present flag",
     "SF014B": "Bias data present flag",
     "SF015": "Continuity indicator",
 }
 
-ORBCLK_BLOCK = {  # tables 6.5 & 6.6 Orbit and Clock Blocks
-    "optOrbit": (
-        ("SF014O", 1),  # if SF014O = 1
-        {
-            "SF020R": "Orbit radial correction",
-            "SF020A": "Orbit along-track correction",
-            "SF020C": "Orbit cross-track correction",
-            "optSF008-1": (
-                ("SF008", 1),  # if SF008 = 1
-                {
-                    "SF021": "Satellite yaw",
-                },
-            ),
-        },
-    ),
+OCB_CLOCK_BLOCK = {  # table 6.6 Clock Block
     "optClock": (
-        ("SF014C", 1),  # if SF014C = 1
+        ("SF014C+1", 1),  # if SF014C = 1
         {
             "SF022": "IODE continuity",
             "SF020CK": "Clock correction",
             "SF024": "User range error",
         },
     ),
 }
@@ -71,62 +57,62 @@
     "SF039": "Number of grid points present",
     "SF040T": "Tropo blocks indicator",
     "SF040I": "Iono blocks indicator",
 }
 
 TROP_DATA_BLOCK = {  # table 6.16 Troposphere Data Block
     "optSF040T-12": (
-        ("SF040T", [1, 2]),  # if SF040T in 1,2
+        ("SF040T+1", [1, 2]),  # if SF040T in 1,2
         {
             "SF041": "Troposhere equation type",
             "SF042": "Troposphere quality",
             "SF043": "Area average vertical hydrostatic delay",
             "SF044": "Troposphere polynomial coefficient size indicator",
             "optSF044-0": (
-                ("SF044", 0),  # if SF044 = 0 table 6.17
+                ("SF044+1", 0),  # if SF044 = 0 table 6.17
                 {
                     "SF045": "Troposphere coefficient T00",
                     "optSF041-12": (
-                        ("SF041", [1, 2]),  # if SF041 in 1,2
+                        ("SF041+1", [1, 2]),  # if SF041 in 1,2
                         {
                             "SF046a": "Troposphere coefficient T01",
                             "SF046b": "Troposphere coefficient T10",
                         },
                     ),
                     "optSF041-2": (
-                        ("SF041", 2),  # if SF041 = 2
+                        ("SF041+1", 2),  # if SF041 = 2
                         {
                             "SF047": "Troposphere coefficient T11",
                         },
                     ),
                 },
             ),
             "optSF044-1": (
-                ("SF044", 1),  # if SF044 = 1 table 6.18
+                ("SF044+1", 1),  # if SF044 = 1 table 6.18
                 {
                     "SF048": "Troposphere coefficient T00",
                     "optSF041-12": (
-                        ("SF041", [1, 2]),  # if SF041 in 1,2
+                        ("SF041+1", [1, 2]),  # if SF041 in 1,2
                         {
                             "SF049a": "Troposphere coefficient T01",
                             "SF049b": "Troposphere coefficient T10",
                         },
                     ),
                     "optSF041-2": (
-                        ("SF041", 2),  # if SF041 = 2
+                        ("SF041+1", 2),  # if SF041 = 2
                         {
                             "SF050": "Troposphere coefficient T11",
                         },
                     ),
                 },
             ),
         },
     ),
     "optSF040T-2": (  # if SF040T = 2
-        ("SF040T", 2),  # if SF040T = 2
+        ("SF040T+1", 2),  # if SF040T = 2
         {
             "SF051": "Troposphere residual field size",
             "optSF051-0": (
                 ("SF051", 0),  # if SF051 = 0
                 {"SF052": "Troposphere grid residuals"},
             ),
             "optSF051-1": (  # if SF051 = 1
@@ -135,60 +121,60 @@
             ),
         },
     ),
 }
 
 ION_SAT_BLOCK = {  # table 6.20 Ionosphere Satellite Block
     "optSF041-12": (
-        ("SF041", [1, 2]),  # if SF041I in 1,2
+        ("SF041+1", [1, 2]),  # if SF041I in 1,2
         {
             "SF055": "Ionosphere quality",
             "SF056": "Ionosphere polynomial coefficient size indicator",
             "optSF064-0": (
-                ("SF056", 0),  # if SF056 = 0 table 6.21
+                ("SF056+2", 0),  # if SF056 = 0 table 6.21
                 {
                     "SF057": "Ionosphere coefficient C00",
                     "optSF054-12": (
-                        ("SF054", [1, 2]),  # if SF054 in 1,2
+                        ("SF054+1", [1, 2]),  # if SF054 in 1,2
                         {
                             "SF058a": "Ionosphere coefficient C01",
                             "SF058b": "Ionosphere coefficient C10",
                         },
                     ),
                     "optSF054-2": (
-                        ("SF054", 2),  # if SF054 = 2
+                        ("SF054+1", 2),  # if SF054 = 2
                         {
                             "SF059": "Ionosphere coefficient C11",
                         },
                     ),
                 },
             ),
             "optSF056-1": (
-                ("SF056", 1),  # if SF056 = 1 table 6.22
+                ("SF056+2", 1),  # if SF056 = 1 table 6.22
                 {
                     "SF060": "Ionosphere coefficient C00",
                     "optSF054-12": (
-                        ("SF054", [1, 2]),  # if SF054 in 1,2
+                        ("SF054+1", [1, 2]),  # if SF054 in 1,2
                         {
                             "SF061a": "Ionosphere coefficient C01",
                             "SF061b": "Ionosphere coefficient C10",
                         },
                     ),
                     "optSF054-2": (
-                        ("SF054", 2),  # if SF054 = 2
+                        ("SF054+1", 2),  # if SF054 = 2
                         {
                             "SF062": "Ionosphere coefficient C11",
                         },
                     ),
                 },
             ),
         },
     ),
     "optSF041-2": (
-        ("SF041", 2),  # if SF041I = 2
+        ("SF041+1", 2),  # if SF041I = 2
         {
             "SF063": "Ionosphere residual field size",
             "optSF063-0": (
                 ("SF063", 0),  # if SF063 = 0
                 {"SF064": "Ionosphere grid residuals"},
             ),
             "optSF063-1": (
@@ -221,36 +207,50 @@
         STBMLEN: "GPS Satellite mask length",
         "SF011": "GPS Satellite mask",
         "groupSat": (  # Satellite Block table 6.4
             NB + "SF011",  # repeating group * num bits set in SF011
             {
                 "SF013": "Do not use (DNU)",
                 "optSat": (
-                    ("SF013", 0),  # if SF013 = 0
+                    ("SF013+1", 0),  # if SF013 = 0
                     {
                         **OCB_SAT_FLAGS,
-                        "SF018": "GPS IODE",
-                        **ORBCLK_BLOCK,
+                        "optOrbit": (  # # table 6.5 Orbit Block
+                            ("SF014O+1", 1),  # if SF014O = 1
+                            {
+                                "SF018": "GPS IODE",
+                                "SF020R": "Orbit radial correction",
+                                "SF020A": "Orbit along-track correction",
+                                "SF020C": "Orbit cross-track correction",
+                                "optSF008-1": (
+                                    ("SF008", 1),  # if SF008 = 1
+                                    {
+                                        "SF021": "Satellite yaw",
+                                    },
+                                ),
+                            },
+                        ),
+                        **OCB_CLOCK_BLOCK,
                         "optBias": (
-                            ("SF014B", 1),  # if SF014B = 1
+                            ("SF014B+1", 1),  # if SF014B = 1
                             {
                                 PBBMLEN: "Phase bias mask length",
                                 "SF025": "GPS phase bias mask",
                                 "groupSF025-BITS": (
                                     NB
-                                    + "SF025",  # repeating group * num bits set in SF025
+                                    + "SF025+1",  # repeating group * num bits set in SF025
                                     {
                                         **PHAS_BIAS_BLOCK,
                                     },
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF027": "GPS code bias mask",
                                 "groupSF027-BITS": (
                                     NB
-                                    + "SF027",  # repeating group * num bits set in SF027
+                                    + "SF027+1",  # repeating group * num bits set in SF027
                                     {
                                         "SF029": "Code bias correction",
                                     },
                                 ),
                             },
                         ),
                     },
@@ -264,36 +264,50 @@
         STBMLEN: "GPS Satellite mask length",
         "SF012": "GLO Satellite mask",
         "groupSat": (  # Satellite Block table 6.4
             NB + "SF012",  # repeating group * num bits set in SF012
             {
                 "SF013": "Do not use (DNU)",
                 "optSat": (
-                    ("SF013", 0),  # if SF013 = 0
+                    ("SF013+1", 0),  # if SF013 = 0
                     {
                         **OCB_SAT_FLAGS,
-                        "SF019": "GLONASS IODE",
-                        **ORBCLK_BLOCK,
+                        "optOrbit": (  # table 6.5 Orbit Block
+                            ("SF014O+1", 1),  # if SF014O = 1
+                            {
+                                "SF019": "GLONASS IODE",
+                                "SF020R": "Orbit radial correction",
+                                "SF020A": "Orbit along-track correction",
+                                "SF020C": "Orbit cross-track correction",
+                                "optSF008-1": (
+                                    ("SF008", 1),  # if SF008 = 1
+                                    {
+                                        "SF021": "Satellite yaw",
+                                    },
+                                ),
+                            },
+                        ),
+                        **OCB_CLOCK_BLOCK,
                         "optBias": (
-                            ("SF014B", 1),  # if SF014B = 1
+                            ("SF014B+1", 1),  # if SF014B = 1
                             {
                                 PBBMLEN: "Phase bias mask length",
                                 "SF026": "GLONASS phase bias mask",
                                 "groupSF026-BITS": (
                                     NB
-                                    + "SF026",  # repeating group * num bits set in SF026
+                                    + "SF026+1",  # repeating group * num bits set in SF026
                                     {
                                         **PHAS_BIAS_BLOCK,
                                     },
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF028": "GLONASScode bias mask",
                                 "groupSF028-BITS": (
                                     NB
-                                    + "SF028",  # repeating group * num bits set in SF028
+                                    + "SF028+1",  # repeating group * num bits set in SF028
                                     {
                                         "SF029": "Code bias correction",
                                     },
                                 ),
                             },
                         ),
                     },
@@ -307,36 +321,50 @@
         STBMLEN: "GPS Satellite mask length",
         "SF093": "GALILEO Satellite mask",
         "groupSat": (  # Satellite Block table 6.4
             NB + "SF093",  # repeating group * num bits set in SF093
             {
                 "SF013": "Do not use (DNU)",
                 "optSat": (
-                    ("SF013", 0),  # if SF013 = 0
+                    ("SF013+1", 0),  # if SF013 = 0
                     {
                         **OCB_SAT_FLAGS,
-                        "SF099": "GALILEO IODE",
-                        **ORBCLK_BLOCK,
+                        "optOrbit": (  # table 6.5 Orbit Block
+                            ("SF014O+1", 1),  # if SF014O = 1
+                            {
+                                "SF099": "GALILEO IODE",
+                                "SF020R": "Orbit radial correction",
+                                "SF020A": "Orbit along-track correction",
+                                "SF020C": "Orbit cross-track correction",
+                                "optSF008-1": (
+                                    ("SF008", 1),  # if SF008 = 1
+                                    {
+                                        "SF021": "Satellite yaw",
+                                    },
+                                ),
+                            },
+                        ),
+                        **OCB_CLOCK_BLOCK,
                         "optBias": (
-                            ("SF014B", 1),  # if SF014B = 1
+                            ("SF014B+1", 1),  # if SF014B = 1
                             {
                                 PBBMLEN: "Phase bias mask length",
                                 "SF102": "GALILEO phase bias mask",
                                 "groupSF102-BITS": (
                                     NB
-                                    + "SF102",  # repeating group * num bits set in SF0102
+                                    + "SF102+1",  # repeating group * num bits set in SF0102
                                     {
                                         **PHAS_BIAS_BLOCK,
                                     },
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF105": "GALILEO code bias mask",
                                 "groupSF105-BITS": (
                                     NB
-                                    + "SF105",  # repeating group * num bits set in SF0105
+                                    + "SF105+1",  # repeating group * num bits set in SF0105
                                     {
                                         "SF029": "Code bias correction",
                                     },
                                 ),
                             },
                         ),
                     },
@@ -350,36 +378,50 @@
         STBMLEN: "GPS Satellite mask length",
         "SF094": "BEIDOU Satellite mask",
         "groupSat": (  # Satellite Block table 6.4
             NB + "SF094",  # repeating group * num bits set in SF094
             {
                 "SF013": "Do not use (DNU)",
                 "optSat": (
-                    ("SF013", 0),  # if SF013 = 0
+                    ("SF013+1", 0),  # if SF013 = 0
                     {
                         **OCB_SAT_FLAGS,
-                        "SF100": "BEIDOU IODE",
-                        **ORBCLK_BLOCK,
+                        "optOrbit": (  # table 6.5 Orbit Block
+                            ("SF014O+1", 1),  # if SF014O = 1
+                            {
+                                "SF100": "BEIDOU IODE",
+                                "SF020R": "Orbit radial correction",
+                                "SF020A": "Orbit along-track correction",
+                                "SF020C": "Orbit cross-track correction",
+                                "optSF008-1": (
+                                    ("SF008", 1),  # if SF008 = 1
+                                    {
+                                        "SF021": "Satellite yaw",
+                                    },
+                                ),
+                            },
+                        ),
+                        **OCB_CLOCK_BLOCK,
                         "optBias": (
-                            ("SF014B", 1),  # if SF014B = 1
+                            ("SF014B+1", 1),  # if SF014B = 1
                             {
                                 PBBMLEN: "Phase bias mask length",
                                 "SF103": "BEIDOU phase bias mask",
                                 "groupSF103-BITS": (
                                     NB
-                                    + "SF103",  # repeating group * num bits set in SF0103
+                                    + "SF103+1",  # repeating group * num bits set in SF0103
                                     {
                                         **PHAS_BIAS_BLOCK,
                                     },
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF106": "BEIDOU code bias mask",
                                 "groupSF106-BITS": (
                                     NB
-                                    + "SF106",  # repeating group * num bits set in SF0106
+                                    + "SF106+1",  # repeating group * num bits set in SF0106
                                     {
                                         "SF029": "Code bias correction",
                                     },
                                 ),
                             },
                         ),
                     },
@@ -393,36 +435,50 @@
         STBMLEN: "GPS Satellite mask length",
         "SF095": "QZSS Satellite mask",
         "groupSat": (  # Satellite Block table 6.4
             NB + "SF095",  # repeating group * num bits set in SF095
             {
                 "SF013": "Do not use (DNU)",
                 "optSat": (
-                    ("SF013", 0),  # if SF013 = 0
+                    ("SF013+1", 0),  # if SF013 = 0
                     {
                         **OCB_SAT_FLAGS,
-                        "SF101": "QZSS IODE",
-                        **ORBCLK_BLOCK,
+                        "optOrbit": (  # table 6.5 Orbit Block
+                            ("SF014O+1", 1),  # if SF014O = 1
+                            {
+                                "SF101": "QZSS IODE",
+                                "SF020R": "Orbit radial correction",
+                                "SF020A": "Orbit along-track correction",
+                                "SF020C": "Orbit cross-track correction",
+                                "optSF008-1": (
+                                    ("SF008", 1),  # if SF008 = 1
+                                    {
+                                        "SF021": "Satellite yaw",
+                                    },
+                                ),
+                            },
+                        ),
+                        **OCB_CLOCK_BLOCK,
                         "optBias": (
-                            ("SF014B", 1),  # if SF014B = 1
+                            ("SF014B+1", 1),  # if SF014B = 1
                             {
                                 PBBMLEN: "Phase bias mask length",
                                 "SF104": "QZSS phase bias mask",
                                 "groupSF104-BITS": (
                                     NB
-                                    + "SF104",  # repeating group * num bits set in SF0104
+                                    + "SF104+1",  # repeating group * num bits set in SF0104
                                     {
                                         **PHAS_BIAS_BLOCK,
                                     },
                                 ),
                                 CBBMLEN: "Code bias mask length",
                                 "SF107": "QZSS code bias mask",
                                 "groupSF107-BITS": (
                                     NB
-                                    + "SF107",  # repeating group * num bits set in SF0107
+                                    + "SF107+1",  # repeating group * num bits set in SF0107
                                     {
                                         "SF029": "Code bias correction",
                                     },
                                 ),
                             },
                         ),
                     },
@@ -437,21 +493,21 @@
         **HPAC_HDR,
         "groupAtm": (  # Atmosphere Data Block repeating group * SF030
             "SF030",
             {
                 **AREA_DATA_BLOCK,
                 **TROP_DATA_BLOCK,
                 "optSF040I-12": (  # table 6.19 Ionosphere Data Block
-                    ("SF040I", [1, 2]),  # if SF040I in 1,2
+                    ("SF040I+1", [1, 2]),  # if SF040I in 1,2
                     {
                         "SF054": "Ionosphere equation type",
                         STBMLEN: "GPS Satellite mask length",
                         "SF011": "GPS Satellite mask",
                         "groupSF011": (  # repeating group * num bits set in SF011
-                            NB + "SF011",
+                            NB + "SF011+1",
                             {
                                 **ION_SAT_BLOCK,
                             },
                         ),
                     },
                 ),
             },
@@ -461,21 +517,21 @@
         **HPAC_HDR,
         "groupAtm": (  # Atmosphere Data Block repeating group * SF030
             "SF030",
             {
                 **AREA_DATA_BLOCK,
                 **TROP_DATA_BLOCK,
                 "optSF040I-12": (  # table 6.19 Ionosphere Data Block
-                    ("SF040I", [1, 2]),  # if SF040I in 1,2
+                    ("SF040I+1", [1, 2]),  # if SF040I in 1,2
                     {
                         "SF054": "Ionosphere equation type",
                         STBMLEN: "GPS Satellite mask length",
                         "SF012": "GLONASS Satellite mask",
                         "groupSF012": (  # repeating group * num bits set in SF012
-                            NB + "SF012",
+                            NB + "SF012+1",
                             {
                                 **ION_SAT_BLOCK,
                             },
                         ),
                     },
                 ),
             },
@@ -485,21 +541,21 @@
         **HPAC_HDR,
         "groupAtm": (  # Atmosphere Data Block repeating group * SF030
             "SF030",
             {
                 **AREA_DATA_BLOCK,
                 **TROP_DATA_BLOCK,
                 "optSF040I-12": (  # table 6.19 Ionosphere Data Block
-                    ("SF040I", [1, 2]),  # if SF040I in 1,2
+                    ("SF040I+1", [1, 2]),  # if SF040I in 1,2
                     {
                         "SF054": "Ionosphere equation type",
                         STBMLEN: "GPS Satellite mask length",
                         "SF093": "GALILEO Satellite mask",
                         "groupSF093": (  # repeating group * num bits set in SF093
-                            NB + "SF093",
+                            NB + "SF093+1",
                             {
                                 **ION_SAT_BLOCK,
                             },
                         ),
                     },
                 ),
             },
@@ -509,21 +565,21 @@
         **HPAC_HDR,
         "groupAtm": (  # Atmosphere Data Block repeating group * SF030
             "SF030",
             {
                 **AREA_DATA_BLOCK,
                 **TROP_DATA_BLOCK,
                 "optSF040I-12": (  # table 6.19 Ionosphere Data Block
-                    ("SF040I", [1, 2]),  # if SF040I in 1,2
+                    ("SF040I+1", [1, 2]),  # if SF040I in 1,2
                     {
                         "SF054": "Ionosphere equation type",
                         STBMLEN: "GPS Satellite mask length",
                         "SF094": "BEIDOU Satellite mask",
                         "groupSF094": (  # repeating group * num bits set in SF094
-                            NB + "SF094",
+                            NB + "SF094+1",
                             {
                                 **ION_SAT_BLOCK,
                             },
                         ),
                     },
                 ),
             },
@@ -533,21 +589,21 @@
         **HPAC_HDR,
         "groupAtm": (  # Atmosphere Data Block repeating group * SF030
             "SF030",
             {
                 **AREA_DATA_BLOCK,
                 **TROP_DATA_BLOCK,
                 "optSF040I-12": (  # table 6.19 Ionosphere Data Block
-                    ("SF040I", [1, 2]),  # if SF040I in 1,2
+                    ("SF040I+1", [1, 2]),  # if SF040I in 1,2
                     {
                         "SF054": "Ionosphere equation type",
                         STBMLEN: "GPS Satellite mask length",
                         "SF095": "QZSS Satellite mask",
                         "groupSF095": (  # repeating group * num bits set in SF095
-                            NB + "SF095",
+                            NB + "SF095+1",
                             {
                                 **ION_SAT_BLOCK,
                             },
                         ),
                     },
                 ),
             },
@@ -581,9 +637,9 @@
     # ********************************************************************
     # EAS-DYN
     # ********************************************************************
     "SPARTN-1X-EAS-DYN": {},  # TODO
     # ********************************************************************
     # EAS-GRP deprecated
     # ********************************************************************
-    "SPARTN-1X-EAS-GRP": {},  # TODO
+    "SPARTN-1X-EAS-GRP": {},  # no current plans to implement
 }
```

### Comparing `pyspartn-0.2.1/src/pyspartn.egg-info/PKG-INFO` & `pyspartn-0.3.0/src/pyspartn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.2.1
+Version: 0.3.0
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -32,15 +32,15 @@
         SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/semuconsulting/pyspartn
 Project-URL: documentation, https://www.semuconsulting.com/pyspartn/
 Project-URL: repository, https://github.com/semuconsulting/pyspartn
 Project-URL: changelog, https://github.com/semuconsulting/pyspartn/blob/master/RELEASE_NOTES.md
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
@@ -80,50 +80,54 @@
 [Parsing](#parsing) |
 [Generating](#generating) |
 [Serializing](#serializing) |
 [Examples](#examples) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
-`pyspartn` is an original Python 3 parser for the SPARTN &copy; GPS/GNSS protocol. SPARTN is an open-source GPS/GNSS [differential correction or DGPS](https://en.wikipedia.org/wiki/Differential_GPS) protocol published by u-blox.
+`pyspartn` is an original Python 3 parser for the SPARTN &copy; GPS/GNSS protocol. SPARTN is an open-source GPS/GNSS [differential correction or DGPS](https://en.wikipedia.org/wiki/Differential_GPS) protocol published by u-blox:
 
-[SPARTN Protocol 2.01](https://www.spartnformat.org/download/) (available in the public domain).
+[SPARTN Protocol](https://www.spartnformat.org/download/) (available in the public domain).
 © 2021 u-blox AG. All rights reserved.
 
 The `pyspartn` homepage is located at [https://github.com/semuconsulting/pyspartn](https://github.com/semuconsulting/pyspartn).
 
 This is an independent project and we have no affiliation whatsoever with u-blox.
 
 **FYI** There are companion libraries which handle standard NMEA 0183 &copy;, UBX &copy; (u-blox) and RTCM3 &copy; GNSS/GPS messages:
-- [pyubx2](http://github.com/semuconsulting/pyubx2) (**FYI** installing `pyubx2` via pip also installs `pynmeagps` and `pyrtcm`)
+- [pyubx2](http://github.com/semuconsulting/pyubx2)
 - [pynmeagps](http://github.com/semuconsulting/pynmeagps)
 - [pyrtcm](http://github.com/semuconsulting/pyrtcm)
 
 ## <a name="currentstatus">Current Status</a>
 
-**WORK IN PROGRESS - CURRENTLY IN ALPHA.**
+**CURRENTLY IN BETA**
 
 <!--![Status](https://img.shields.io/pypi/status/pyspartn)-->
 ![Release](https://img.shields.io/github/v/release/semuconsulting/pyspartn?include_prereleases)
 ![Build](https://img.shields.io/github/actions/workflow/status/semuconsulting/pyspartn/main.yml?branch=main)
 ![Codecov](https://img.shields.io/codecov/c/github/semuconsulting/pyspartn)
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
 The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class implements a provisional decrypt and decode for OCB, HPAC and GAD message types but it has not yet been fully tested (*appears to be working OK for GAD, HPAC and most OCB payloads, but some small OCB payloads (nData < 35) are still failing. For the time being, a temporary override has been implemented in `spartnmessage.py` to suppress the `decode` flag for those payload types that cannot yet be successfully decoded*).
+The `SPARTNMessage` class implements decrypt and decode algorithms for OCB, HPAC and GAD message types:
+ - GAD payload decryption and decode is fully tested and functional, which confirms that the global decryption mechanism and parsing algorithms are essentially correct.
+ - HPAC and OCB payload decodes appear to be working OK, but results have not yet been fully validated and some individual attributes may be incorrect.
+
+*For the time being, a temporary override has been implemented in `spartnmessage.py` to suppress the `decode` flag for those payload types that cannot yet be successfully decoded. Testing contributions welcome*.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
-[Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided.
+[Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, please use the [Discussion](https://github.com/semuconsulting/pyspartn/discussions) Forum.
 
 ---
 ## <a name="installation">Installation</a>
 
 `pyspartn` is compatible with Python >=3.8 and is dependent on the `cryptography` library.
 
 **NB:** If you're installing `pyspartn` on a 32-bit Linux platform, some additional installation steps may be required - see note *¹* below.
@@ -299,16 +303,19 @@
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
 
+1. `spartn_mqtt_client.py` - implements a simple SPARTN MQTT client using the pygnssutils.GNSSMQTTClient class. **NB**: requires a valid ClientID for a
+SPARTN MQTT service e.g. u-blox Thingstream PointPerfect.
+1. `spartn_decrypt.py` - illustrates how to read, decrypt and decode a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` example above).
 1. `rxmpmp_extract_spartn.py` - ilustrates how to extract individual SPARTN messages from the accumulated UBX-RXM-PMP data output by an NEO-D9S L-band correction receiver.
-1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the example above.
+1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the `rxmpmp_extract_spartn.py` above.
 1. `gad_plot.py` - illustrates how to extract geographic area definitions from a series of SPARTN-GAD-1X messages - the output file from the example above can be used as an input. This example also serves to illustrate how to decrypt SPARTN messages.
 
 ---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3 and SPARTN protocols is available at:
```

### Comparing `pyspartn-0.2.1/src/pyspartn.egg-info/SOURCES.txt` & `pyspartn-0.3.0/src/pyspartn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspartn-0.2.1/tests/test_socket.py` & `pyspartn-0.3.0/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.2.1/tests/test_static.py` & `pyspartn-0.3.0/tests/test_static.py`

 * *Files identical despite different names*

