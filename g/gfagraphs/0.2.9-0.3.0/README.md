# Comparing `tmp/gfagraphs-0.2.9.tar.gz` & `tmp/gfagraphs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfagraphs-0.2.9.tar", last modified: Fri Dec  8 14:59:10 2023, max compression
+gzip compressed data, was "gfagraphs-0.3.0.tar", last modified: Fri Apr 19 08:42:21 2024, max compression
```

## Comparing `gfagraphs-0.2.9.tar` & `gfagraphs-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.784022 gfagraphs-0.2.9/
--rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.2.9/LICENSE.md
--rw-r--r--   0 sidubois (669136) genscale (35005)     1994 2023-12-08 14:59:10.784022 gfagraphs-0.2.9/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)     1368 2023-11-29 09:43:15.000000 gfagraphs-0.2.9/README.md
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.783022 gfagraphs-0.2.9/gfagraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      192 2023-09-22 08:36:37.000000 gfagraphs-0.2.9/gfagraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    39437 2023-11-29 14:54:03.000000 gfagraphs-0.2.9/gfagraphs/gfagraphs.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.784022 gfagraphs-0.2.9/gfagraphs.egg-info/
--rw-r--r--   0 sidubois (669136) genscale (35005)     1994 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/gfagraphs.egg-info/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      374 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/gfagraphs.egg-info/SOURCES.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/gfagraphs.egg-info/dependency_links.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2023-09-22 09:02:54.000000 gfagraphs-0.2.9/gfagraphs.egg-info/not-zip-safe
--rw-r--r--   0 sidubois (669136) genscale (35005)       19 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/gfagraphs.egg-info/top_level.txt
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.783022 gfagraphs-0.2.9/pgGraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      184 2023-11-29 08:56:43.000000 gfagraphs-0.2.9/pgGraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      533 2023-11-29 08:50:19.000000 gfagraphs-0.2.9/pgGraphs/abstractions.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    12000 2023-12-08 14:51:41.000000 gfagraphs-0.2.9/pgGraphs/gfaparser.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    15532 2023-12-08 14:58:48.000000 gfagraphs-0.2.9/pgGraphs/graph.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     5228 2023-11-29 09:41:37.000000 gfagraphs-0.2.9/pgGraphs/networkx.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      695 2023-12-08 14:59:10.000000 gfagraphs-0.2.9/pyproject.toml
--rw-r--r--   0 sidubois (669136) genscale (35005)       38 2023-12-08 14:59:10.784022 gfagraphs-0.2.9/setup.cfg
--rw-r--r--   0 sidubois (669136) genscale (35005)     2436 2023-12-08 14:59:07.000000 gfagraphs-0.2.9/setup.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2023-12-08 14:59:10.783022 gfagraphs-0.2.9/tests/
--rw-r--r--   0 sidubois (669136) genscale (35005)     1302 2023-09-18 13:15:00.000000 gfagraphs-0.2.9/tests/test.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/
+-rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.0/LICENSE
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2038 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1415 2024-04-19 08:32:43.000000 gfagraphs-0.3.0/README.md
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-19 08:42:21.745107 gfagraphs-0.3.0/gfagraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.0/gfagraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.0/gfagraphs/gfagraphs.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/gfagraphs.egg-info/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2038 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/gfagraphs.egg-info/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      357 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/gfagraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/gfagraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.0/gfagraphs.egg-info/not-zip-safe
+-rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/gfagraphs.egg-info/top_level.txt
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/pgGraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      184 2024-01-25 14:21:38.000000 gfagraphs-0.3.0/pgGraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      548 2024-02-19 09:05:35.000000 gfagraphs-0.3.0/pgGraphs/abstractions.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    15566 2024-04-16 12:23:19.000000 gfagraphs-0.3.0/pgGraphs/gfaparser.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    29827 2024-04-18 09:35:46.000000 gfagraphs-0.3.0/pgGraphs/graph.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     5261 2024-04-08 10:15:17.000000 gfagraphs-0.3.0/pgGraphs/networkx.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/pyproject.toml
+-rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/setup.cfg
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2489 2024-04-19 08:32:52.000000 gfagraphs-0.3.0/setup.py
```

### Comparing `gfagraphs-0.2.9/LICENSE.md` & `gfagraphs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.2.9/PKG-INFO` & `gfagraphs-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.2.9
+Version: 0.3.0
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
+License-File: LICENSE
 
 [![](https://img.shields.io/badge/Python-3.10-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.11-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.12-blue.svg)]()
 [![](https://img.shields.io/badge/documentation-unfinished-orange.svg)]()
 
 # GFAGraphs - A Python GFA library
 
+> [!WARNING]\
+> A paper is in preparation about this work. If you consider to use this tool, please contact the author for attribution.
+
 This Python library aims to be an abstraction layer for GFA file format.
-Two implementations are proposed:
-+ a legacy one, which will remain until deprecated, in `gfagraphs/`
-+ a new, cleaner and faster implementation, in `pgGraphs/`
 
 > [!WARNING]\
-> Moving forward, features will only be added to `pgGraphs`, while `gfagraphs` will remain as it, until full migration is done in [pancat](https://github.com/Tharos-ux/pancat) tool.
+> The old version of `gfagraphs` has been deprecated (since v0.3.0), in favour of `pgGraphs`. Using `gfagraphs` or `pgGraphs` to import resolves now in using the same library. In a near future, `pgGraphs` namespace will be deprecated.
 
-## Package pgGraphs
+## Package `pgGraphs`/`gfagraphs`
 
 ![](https://media.discordapp.net/attachments/874430800802754623/1179353568105467964/library.png)
 
 The package is organized in 4 modules:
-+ `pgGraphs.abstractions` contains abstractions over GFA formats
-+ `pgGraphs.gfaparser` contains an abstract class for parsing and saving GFA file format
-+ `pgGraphs.graph` contains the main `Graph` class that represents a GFA graph in memory, and edit functions
-+ `pgGraphs.networkx` conains an abstract class for visualization and modelization of GFA in a NetworkX object
++ `gfagraphs.abstractions` contains abstractions over GFA formats
++ `gfagraphs.gfaparser` contains an abstract class for parsing and saving GFA file format
++ `gfagraphs.graph` contains the main `Graph` class that represents a GFA graph in memory, and edit functions
++ `gfagraphs.networkx` conains an abstract class for visualization and modelization of GFA in a NetworkX object
 
 > [!NOTE]\
 > Want to contribute? Feel free to open a PR on an issue about a missing, buggy or incomplete feature!
```

### Comparing `gfagraphs-0.2.9/README.md` & `gfagraphs-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [![](https://img.shields.io/badge/Python-3.10-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.11-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.12-blue.svg)]()
 [![](https://img.shields.io/badge/documentation-unfinished-orange.svg)]()
 
 # GFAGraphs - A Python GFA library
 
+> [!WARNING]\
+> A paper is in preparation about this work. If you consider to use this tool, please contact the author for attribution.
+
 This Python library aims to be an abstraction layer for GFA file format.
-Two implementations are proposed:
-+ a legacy one, which will remain until deprecated, in `gfagraphs/`
-+ a new, cleaner and faster implementation, in `pgGraphs/`
 
 > [!WARNING]\
-> Moving forward, features will only be added to `pgGraphs`, while `gfagraphs` will remain as it, until full migration is done in [pancat](https://github.com/Tharos-ux/pancat) tool.
+> The old version of `gfagraphs` has been deprecated (since v0.3.0), in favour of `pgGraphs`. Using `gfagraphs` or `pgGraphs` to import resolves now in using the same library. In a near future, `pgGraphs` namespace will be deprecated.
 
-## Package pgGraphs
+## Package `pgGraphs`/`gfagraphs`
 
 ![](https://media.discordapp.net/attachments/874430800802754623/1179353568105467964/library.png)
 
 The package is organized in 4 modules:
-+ `pgGraphs.abstractions` contains abstractions over GFA formats
-+ `pgGraphs.gfaparser` contains an abstract class for parsing and saving GFA file format
-+ `pgGraphs.graph` contains the main `Graph` class that represents a GFA graph in memory, and edit functions
-+ `pgGraphs.networkx` conains an abstract class for visualization and modelization of GFA in a NetworkX object
++ `gfagraphs.abstractions` contains abstractions over GFA formats
++ `gfagraphs.gfaparser` contains an abstract class for parsing and saving GFA file format
++ `gfagraphs.graph` contains the main `Graph` class that represents a GFA graph in memory, and edit functions
++ `gfagraphs.networkx` conains an abstract class for visualization and modelization of GFA in a NetworkX object
 
 > [!NOTE]\
 > Want to contribute? Feel free to open a PR on an issue about a missing, buggy or incomplete feature!
```

### Comparing `gfagraphs-0.2.9/gfagraphs/gfagraphs.py` & `gfagraphs-0.3.0/gfagraphs/gfagraphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from re import sub, match
 from typing import Callable
 from copy import deepcopy
 from json import loads, dumps
 from itertools import chain
 from networkx import MultiDiGraph, DiGraph
 from tharospytools.matplotlib_tools import get_palette
+from warnings import warn
+
+warn("The lib gfagraphs is now deprecated. Please move your program to use pgGraphs (also included in the lib) as delepoppement efforts goes into it.")
 
 
 def get_gfa_subtype(gfa_file_path: str | list[str]) -> str | list[str]:
     """Given a file, or more, returns the gfa subtypes, and raises error if file is invalid or does not exists
 
     Args:
         gfa_file_path (str | list[str]): one or more file paths
```

### Comparing `gfagraphs-0.2.9/gfagraphs.egg-info/PKG-INFO` & `gfagraphs-0.3.0/gfagraphs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.2.9
+Version: 0.3.0
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
+License-File: LICENSE
 
 [![](https://img.shields.io/badge/Python-3.10-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.11-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.12-blue.svg)]()
 [![](https://img.shields.io/badge/documentation-unfinished-orange.svg)]()
 
 # GFAGraphs - A Python GFA library
 
+> [!WARNING]\
+> A paper is in preparation about this work. If you consider to use this tool, please contact the author for attribution.
+
 This Python library aims to be an abstraction layer for GFA file format.
-Two implementations are proposed:
-+ a legacy one, which will remain until deprecated, in `gfagraphs/`
-+ a new, cleaner and faster implementation, in `pgGraphs/`
 
 > [!WARNING]\
-> Moving forward, features will only be added to `pgGraphs`, while `gfagraphs` will remain as it, until full migration is done in [pancat](https://github.com/Tharos-ux/pancat) tool.
+> The old version of `gfagraphs` has been deprecated (since v0.3.0), in favour of `pgGraphs`. Using `gfagraphs` or `pgGraphs` to import resolves now in using the same library. In a near future, `pgGraphs` namespace will be deprecated.
 
-## Package pgGraphs
+## Package `pgGraphs`/`gfagraphs`
 
 ![](https://media.discordapp.net/attachments/874430800802754623/1179353568105467964/library.png)
 
 The package is organized in 4 modules:
-+ `pgGraphs.abstractions` contains abstractions over GFA formats
-+ `pgGraphs.gfaparser` contains an abstract class for parsing and saving GFA file format
-+ `pgGraphs.graph` contains the main `Graph` class that represents a GFA graph in memory, and edit functions
-+ `pgGraphs.networkx` conains an abstract class for visualization and modelization of GFA in a NetworkX object
++ `gfagraphs.abstractions` contains abstractions over GFA formats
++ `gfagraphs.gfaparser` contains an abstract class for parsing and saving GFA file format
++ `gfagraphs.graph` contains the main `Graph` class that represents a GFA graph in memory, and edit functions
++ `gfagraphs.networkx` conains an abstract class for visualization and modelization of GFA in a NetworkX object
 
 > [!NOTE]\
 > Want to contribute? Feel free to open a PR on an issue about a missing, buggy or incomplete feature!
```

### Comparing `gfagraphs-0.2.9/pgGraphs/abstractions.py` & `gfagraphs-0.3.0/pgGraphs/abstractions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 
 class Orientation(Enum):
     "Describes the way a node is read"
     FORWARD = '+'
     REVERSE = '-'
     ANY = '?'
+    BOTH = '='
 
 
 class GFAFormat(Enum):
     "Describes the different possible gfa-like formats"
     RGFA = 'rGFA'
     GFA1 = 'GFA1'
     GFA1_1 = 'GFA1.1'
```

### Comparing `gfagraphs-0.2.9/pgGraphs/gfaparser.py` & `gfagraphs-0.3.0/pgGraphs/gfaparser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 "Abstract class for parsing and saving GFA file format"
-from re import match, sub
+from re import match
 from typing import Callable
 from json import loads, dumps
 from os import path, stat
 from tharospytools.path_tools import path_allocator
 from pgGraphs.abstractions import Orientation, GFALine, GFAFormat
+from gzip import open as gz_open
+from re import search
 
 
 class GFAParser:
     """This class implements static methods to get informations about the contents of a GFA file, and to parse them.
 
     Raises:
         OSError: _description_
@@ -41,24 +43,25 @@
         for gfa_file in gfa_file_path:
             # Checking if path exists
             if not path.exists(gfa_file):
                 raise OSError(
                     "Specified file does not exists. Please check provided path."
                 )
             # Checking if file descriptor is valid
-            if not gfa_file.endswith('.gfa'):
+            if not gfa_file.endswith('.gfa') and not gfa_file.endswith('.gfa.gz'):
                 raise IOError(
                     "File descriptor is invalid. Please check format, this lib is designed to work with Graphical Fragment Assembly (GFA) files."
                 )
             # Checking if file is not empty
             if stat(gfa_file).st_size == 0:
                 raise IOError(
                     "File is empty."
                 )
-            with open(gfa_file, 'r', encoding='utf-8') as gfa_reader:
+
+            with open(gfa_file, 'r', encoding='utf-8') if gfa_file.endswith('.gfa') else gz_open(gfa_file, 'rt') as gfa_reader:
                 header: str = gfa_reader.readline()
                 if header[0] != 'H':
                     styles.append('rGFA')
                 else:
                     try:
                         version_number: str = GFAParser.supplementary_datas(
                             header.strip('\n').split('\t'), 1
@@ -147,15 +150,15 @@
             return 'Z'
         else:
             try:
                 _: str = dumps(data, indent=0, separators=(',', ':'))
                 return 'J'
             except (TypeError, OverflowError) as exc:
                 raise ValueError(
-                    f"Type {type(data)} is not in the GFA standard") from exc
+                    f"Data {data} of type {type(data)} is not in the GFA standard") from exc
 
     @staticmethod
     def supplementary_datas(datas: list, length_condition: int) -> dict:
         """Computes the optional tags of a gfa line and returns them as a dict
 
         Args:
             datas (list): parsed data line
@@ -173,96 +176,154 @@
                         additional_tag[3])(additional_tag[5:])
                 else:
                     mapping[f"ARG{nargs}"] = additional_tag
                     nargs += 1
         return mapping
 
     @staticmethod
-    def read_gfa_line(datas: list[str], load_sequence_in_memory: bool = True) -> tuple[str, GFALine, dict]:
+    def read_gfa_line(datas: list[str], load_sequence_in_memory: bool = True, regexp_pattern: str = ".*", memory_mode: bool = True) -> tuple[str, GFALine, dict]:
         """Calls methods to parse a GFA line,
         accordingly to it's fields described in the GFAspec github.
 
         Args:
             datas (list): a list of the fileds in the line
             load_sequence_in_memory (bool): if the line is a segment, ask to load its sequence
+            memory_mode (bool): if the strict minimum in information should be inserted
 
         Returns:
             tuple[str, GFALine, dict]: datas of the line in Python-compatible formats.
         """
         line_datas: dict = dict()
+        if not (datas[0].isupper() or len(datas) == 0):
+            return (None, None, None)
+
         match (line_type := GFALine(datas[0])):
             case GFALine.SEGMENT:
                 line_datas["length"] = len(datas[2])
                 if load_sequence_in_memory:
                     line_datas["seq"] = datas[2]
-                return (sub('\D', '', datas[1]), line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 3)})
+                if memory_mode:
+                    return (datas[1], line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 3)})
+                else:
+                    return (datas[1], line_type, line_datas)
             case GFALine.LINE:
-                line_datas["start"] = sub('\D', '', datas[1])
-                line_datas["end"] = sub('\D', '', datas[3])
-                line_datas["orientation"] = f"{datas[2]}/{datas[4]}"
-                return ((line_datas['start'], line_datas['end']), line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 5)})
+                if memory_mode:
+                    line_datas["start"] = datas[1]
+                    line_datas["end"] = datas[3]
+                    line_datas["orientation"] = f"{datas[2]}/{datas[4]}"
+                    return ((line_datas['start'], line_datas['end']), line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 5)})
+                else:
+                    return (None, None, None)
             case GFALine.WALK:
+                line_datas["name"] = datas[1]
                 line_datas["id"] = datas[3]
-                line_datas["origin"] = int(datas[2])
+                line_datas["origin"] = datas[2]
                 line_datas["start_offset"] = datas[4]
                 line_datas["stop_offset"] = datas[5]
                 line_datas["path"] = [
                     (
                         node[1:],
                         Orientation(node[0])
                     )
                     for node in datas[6].replace('>', ',+').replace('<', ',-')[1:].split(',')
                 ]
-                return (datas[1], line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 7)})
+                try:
+                    label: str = search(
+                        regexp_pattern, datas[3]).group(1).upper()
+                except:
+                    label: str = datas[3].upper()
+                return (label, line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 7)})
             case GFALine.PATH:
+                line_datas["name"] = datas[1]
                 line_datas["id"] = datas[1]
                 line_datas["origin"] = None
                 line_datas["start_offset"] = None
                 line_datas["stop_offset"] = None
                 line_datas["path"] = [
                     (
                         node[:-1],
                         Orientation(node[-1])
                     )
                     for node in datas[2].split(',')
                 ]
-                return (datas[1], line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 7)})
+                try:
+                    label: str = search(
+                        regexp_pattern, datas[1]).group(1).upper()
+                except:
+                    label: str = datas[1].upper()
+                return (label, line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 7)})
             case GFALine.HEADER | GFALine.ANY:
                 return (None, line_type, GFAParser.supplementary_datas(datas, 1))
 
     @staticmethod
-    def save_graph(graph, output_path: str) -> None:
+    def save_graph(graph, output_path: str, force_format: GFAFormat | bool = False, minimal_graph: bool = False) -> None:
         """Given a gfa Graph object, saves to a valid gfa file the Graph.
 
         Args:
             output_path (str): a path on disk where to save
-            output_format (GfaStyle): a format to choose for output.
-                if None, default graph format will be used.
+            force_format (GfaFormat|bool): a format to choose for output.
+                if False, default graph format will be used.
+            minimal_graph (bool) if only necessary info should be kept in output gfa
         """
-        line_number: int = 0
+        # Haplotype number serves when we convert GFA1 to GFA1.1 for W-lines
+        haplotype_number: int = 0
+        gfa_format: GFAFormat = graph.metadata['version'] if not force_format else force_format
+
         with open(path_allocator(output_path), 'w', encoding='utf-8') as gfa_writer:
-            if graph.headers:
+            if graph.headers and gfa_format != GFAFormat.RGFA:
+                # Writing hearder to output file if file is not rgfa
                 for header in graph.headers:
+                    supplementary_text: str = '' if minimal_graph else '\t' + \
+                        '\t'.join(
+                            [str(value) for key, value in header.items() if key.startswith('ARG')])
                     gfa_writer.write(
-                        "H\t"+'\t'.join([f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in header.items()])+"\n")
+                        "H\t"
+                        +
+                        '\t'.join(
+                            [
+                                f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" for key, value in header.items() if not key.startswith('ARG')
+                            ]
+                        )
+                        +
+                        supplementary_text
+                        +
+                        "\n"
+                    )
             if graph.segments:
+                # Whichever the format, those should be written
                 for segment_name, segment_datas in graph.segments.items():
-                    gfa_writer.write("S\t"+f"{segment_name}\t{segment_datas['seq'] if 'seq' in segment_datas else 'N'*segment_datas['length']}\t" + '\t'.join(
-                        [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in segment_datas.items() if key not in ['length', 'seq']])+"\n")
+                    supplementary_text: str = '' if minimal_graph else "\t" + '\t'.join(
+                        [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in segment_datas.items() if key not in ['length', 'seq']])
+                    gfa_writer.write(
+                        "S\t"+f"{segment_name}\t{segment_datas['seq'] if 'seq' in segment_datas else 'N'*segment_datas['length']}{supplementary_text}\n")
             if graph.lines:
                 for line in graph.lines.values():
-                    ori1, ori2 = line['orientation'].split('/')
-                    gfa_writer.write(f"L\t"+f"{line['start']}\t{ori1}\t{line['end']}\t{ori2}\t" + '\t'.join(
-                        [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in line.items() if key not in ['orientation', 'start', 'end']])+"\n")
+                    supplementary_text: str = '' if minimal_graph else "\t" + '\t'.join(
+                        [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in line.items() if key not in ['orientation', 'start', 'end']])
+                    # We accomodate for all alternatives orientation versions that are described in the input graph file to be written back
+                    all_alternates = line.pop(
+                        'alternates', []) + [line['orientation']]
+                    for alt in all_alternates:
+                        ori1, ori2 = alt.split('/')
+                        gfa_writer.write(
+                            f"L\t"+f"{line['start']}\t{ori1}\t{line['end']}\t{ori2}\t0M{supplementary_text}\n")
             if graph.paths:
                 for path_name, path_datas in graph.paths.items():
-                    if graph.metadata['version'] == GFAFormat.GFA1:  # P-line
+                    supplementary_text: str = '' if minimal_graph else "\t" + '\t'.join(
+                        [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in path_datas.items() if key not in ['path', 'start_offset', 'stop_offset', 'origin', 'name', 'id']])
+                    if gfa_format == GFAFormat.GFA1:  # P-line
+                        strpath: str = ','.join(
+                            [node_name+'+' if orient == Orientation.FORWARD else node_name+'-' for node_name, orient in path_datas['path']])
                         gfa_writer.write(
-                            f"P\t{path_name}\t{','.join([node_name+'+' if orient == Orientation.FORWARD else node_name+'-' for node_name, orient in path_datas['path']])}\t*")
-                    else:
+                            f"P\t{path_name}\t{strpath}{supplementary_text}\n")
+                    elif gfa_format == GFAFormat.GFA1_1 or gfa_format == GFAFormat.GFA1_2 or gfa_format == GFAFormat.GFA2:
                         # W-line
-                        offset_start: int | str = path_datas['start_offset'] if 'start_offset' in path_datas else '?'
-                        offset_stop: int | str = path_datas['stop_offset'] if 'stop_offset' in path_datas else '?'
+                        offset_start: int | str = path_datas[
+                            'start_offset'] if 'start_offset' in path_datas and path_datas['start_offset'] else 0
+                        offset_stop: int | str = path_datas['stop_offset'] if 'stop_offset' in path_datas and path_datas['stop_offset'] else sum(
+                            [graph.segments[x]['length'] for (x, _) in path_datas['path']])
                         strpath: str = ''.join(
-                            [f"{'>' if orient == Orientation.FORWARD else '<'}{node_name}" for node_name, orient in path_datas['path']])
-                        return f"W\t{path_name}\t{path_datas['origin'] if 'origin' in path_datas else line_number}\t{path_name}\t{offset_start}\t{offset_stop}\t{strpath}\t*\n"
-                    line_number += 1
+                            [f"{'>' if orient == Orientation.FORWARD or orient == '+' else '<'}{node_name}" for node_name, orient in path_datas['path']])
+                        gfa_writer.write(
+                            f"W\t{path_name}\t{path_datas['origin'] if 'origin' in path_datas and path_datas['origin'] else haplotype_number}\t{path_name}\t{offset_start}\t{offset_stop}\t{strpath}{supplementary_text}\n")
+                    # In the case graph format is rgfa, we don't write any paths to output file
+                    haplotype_number += 1
```

### Comparing `gfagraphs-0.2.9/pgGraphs/networkx.py` & `gfagraphs-0.3.0/pgGraphs/networkx.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,35 +26,38 @@
         for edge_datas in graph.lines.values():
 
             backbone.add_edge(
                 edge_datas['start'],
                 edge_datas['end'],
                 label=edge_datas["orientation"],
             )
-        graph.metadata['backbone']
         return backbone
 
     @staticmethod
     def compute_networkx(
         graph: Graph,
         node_prefix: str | None = None,
         node_size_classes: tuple[list] = (
             [0, 1], [2, 10], [11, 50], [51, 200], [201, 500], [
                 501, 1000], [1001, 10000], [10001, float('inf')]
-        )
+        ),
+        start_stop_ref: tuple | bool = False,
     ) -> MultiDiGraph:
         """Computes the networkx representation of the GFA.
         This function is intended to be used for graphical representation purposes, and not for computing metrics on the graph.
 
         Args:
             node_prefix (str): a prefix used when displaying multiple graphs to prevent node name collisions
 
         Returns:
             MultiDiGraph: a networkx graph featuring the maximum of information
         """
+        if start_stop_ref:
+            graph.sequence_offsets(recalculate=True)
+            start, stop, ref = start_stop_ref
         # Define empty graph
         nx_graph: MultiDiGraph = MultiDiGraph()
         # Creating the palette for node class colors
         node_palette: list = get_palette(
             len(node_size_classes),
             cmap_name='cool',
             as_hex=True
@@ -110,17 +113,15 @@
                 nx_graph.add_edge(
                     f"{node_prefix}{edge_datas['start']}",
                     f"{node_prefix}{edge_datas['end']}",
                     color='darkred',
                     label=edge_datas["orientation"],
                     weight=3
                 )
-        # Adding NX representation to metadata
-        graph.metadata['graph'] = nx_graph
-        return graph.metadata['graph']
+        return nx_graph
 
     def get_most_external_nodes(self) -> list[str]:
         """Get nodes that are on the edges of the graph (starting and ending nodes)
         Those are characterized by their in/out degree : one of those has to be 0.
 
         Returns:
             list[str]: nodes names matching the condition.
```

### Comparing `gfagraphs-0.2.9/pyproject.toml` & `gfagraphs-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0"]
     build-backend = "setuptools.build_meta"
 
     [project]
     name = "gfagraphs"
-    version = "0.2.9"
+    version = "0.3.0"
     authors = [
     { name="Siegfried Dubois", email="siegfried.dubois@inria.fr" },
     ]
     description = "Library to parse, edit and handle in memory GFA graphs"
     readme = "README.md"
     requires-python = ">=3.10"
     classifiers = [
```

### Comparing `gfagraphs-0.2.9/setup.py` & `gfagraphs-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,23 @@
 NAME: str = "gfagraphs"
 AUTHOR: str = "Siegfried Dubois",
 AUTHOR_EMAIL: str = "siegfried.dubois@inria.fr",
 LICENCE: str = "LICENCE"
 DESCRIPTION: str = "Library to parse, edit and handle in memory GFA graphs"
 REQUIRED_PYTHON: tuple = (3, 10)
 OVERRIDE_VN: bool = True
-VN: str = "0.2.9"
+VN: str = "0.3.0"
 URL: str = "https://github.com/Tharos-ux/gfagraphs"
-REQUIREMENTS: list[str] = ['networkx', 'tharos-pytools']
+REQUIREMENTS: list[str] = [
+    'networkx',
+    'tharos-pytools',
+    'matplotlib',
+    'mycolorpy',
+    ''
+]
 
 
 if argv[1] in ('install', 'sdist', 'bdist_wheel'):
     # Checking if Python version is correct
     if version_info[:2] < REQUIRED_PYTHON:
         stderr.write(
             f"{NAME} requires Python {'.'.join(REQUIRED_PYTHON)} or higher and your current version is {version_info[:2]}.")
```

