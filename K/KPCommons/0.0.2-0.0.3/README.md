# Comparing `tmp/KPCommons-0.0.2.tar.gz` & `tmp/kpcommons-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KPCommons-0.0.2.tar", last modified: Tue Apr  9 09:07:26 2024, max compression
+gzip compressed data, was "kpcommons-0.0.3.tar", last modified: Fri Apr 19 15:27:05 2024, max compression
```

## Comparing `KPCommons-0.0.2.tar` & `kpcommons-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:07:26.008922 KPCommons-0.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:07:26.008922 KPCommons-0.0.2/KPCommons.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14020 2024-04-09 09:07:26.000000 KPCommons-0.0.2/KPCommons.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2024-04-09 09:07:26.000000 KPCommons-0.0.2/KPCommons.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 09:07:26.000000 KPCommons-0.0.2/KPCommons.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-09 09:07:26.000000 KPCommons-0.0.2/KPCommons.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-09 06:42:51.000000 KPCommons-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14020 2024-04-09 09:07:26.008922 KPCommons-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-09 09:06:35.000000 KPCommons-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:07:26.008922 KPCommons-0.0.2/kpcommons/
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-04-09 06:42:51.000000 KPCommons-0.0.2/kpcommons/Footnote.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2024-04-09 09:06:35.000000 KPCommons-0.0.2/kpcommons/Util.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 09:07:11.000000 KPCommons-0.0.2/kpcommons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-04-09 09:06:35.000000 KPCommons-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 09:07:26.008922 KPCommons-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:27:05.769439 kpcommons-0.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:27:05.769439 kpcommons-0.0.3/KPCommons.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15163 2024-04-19 15:27:05.000000 kpcommons-0.0.3/KPCommons.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2024-04-19 15:27:05.000000 kpcommons-0.0.3/KPCommons.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 15:27:05.000000 kpcommons-0.0.3/KPCommons.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-19 15:27:05.000000 kpcommons-0.0.3/KPCommons.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-19 09:06:15.000000 kpcommons-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15163 2024-04-19 15:27:05.769439 kpcommons-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-19 09:06:15.000000 kpcommons-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 15:27:05.769439 kpcommons-0.0.3/kpcommons/
+-rw-rw-rw-   0 root         (0) root         (0)     4165 2024-04-19 09:06:15.000000 kpcommons-0.0.3/kpcommons/Footnote.py
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2024-04-19 09:06:15.000000 kpcommons-0.0.3/kpcommons/Util.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 15:26:52.000000 kpcommons-0.0.3/kpcommons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-04-19 09:06:15.000000 kpcommons-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 15:27:05.769439 kpcommons-0.0.3/setup.cfg
```

### Comparing `KPCommons-0.0.2/KPCommons.egg-info/PKG-INFO` & `kpcommons-0.0.3/KPCommons.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KPCommons
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of reusable methods.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,22 +214,35 @@
 License-File: LICENSE
 
 # Readme
 
 KPCommons is a collection of methods which are regularly needed.
 
 ## Util
+Util.py contains the following methods:
 
-Util.py contains a method to calculate the overlap between two ranges. For example,
-
-~~~
-Util.calculate_overlap(0, 10, 5, 10)
-~~~
-
-would return a result of 5. The first two arguments are the start and end position of the first range, and the last two
-arguments are the positions of the second range.
-
-**Note**: In case of no overlap, the distance between the two ranges is returned as a negative result.
+- `calculate_overlap` is a method to calculate the overlap between two ranges.
+  ~~~
+  overlap = Util.calculate_overlap(0, 10, 5, 10)
+  ~~~
+  would return a result of 5. The first two arguments are the start and end position of the first range, and the last
+  two arguments are the positions of the second range.
+  
+  **Note**: In case of no overlap, the distance between the two ranges is returned as a negative result.
+- `calculate_overlap_ratios` is a method to calculate the overlap ratios of two ranges.
+  ~~~
+  ratio_1, ratio_2 = Util.calculate_overlap_ratio(0, 10, 5, 10)
+  ~~~
 
 ## Footnote
-
 Footnote.py contains a collection of methods for working with footnotes.
+
+- `get_footnotes_ranges` takes a text and returns two list of tuples of start and end character positions of footnote
+  ranges, that is, text surrounded by '[[[' and ']]]'. The first list is without an offset, that is, the actual
+  positions, and the second list is with an offset, that is, as if the footnotes were removed.
+- `get_footnote_ranges_without_offset` and `get_footnote_ranges_with_offset` are variants of `get_footnotes_ranges`
+  which only return one of the lists.
+- `is_position_in_ranges` checks if a position is in one of the ranges.
+- `is_range_in_ranges` checks if a range given by a start and end position overlaps with one of the given ranges.
+- `remove_footnotes` removes footnotes from a text. Footnotes are marked by '[[[' and ']]]'.
+- `map_to_real_pos` maps start and end character positions of a text with footnotes removed to real positions, that is,
+  positions before footnotes where removed.
```

### Comparing `KPCommons-0.0.2/LICENSE` & `kpcommons-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `KPCommons-0.0.2/PKG-INFO` & `kpcommons-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KPCommons
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of reusable methods.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,22 +214,35 @@
 License-File: LICENSE
 
 # Readme
 
 KPCommons is a collection of methods which are regularly needed.
 
 ## Util
+Util.py contains the following methods:
 
-Util.py contains a method to calculate the overlap between two ranges. For example,
-
-~~~
-Util.calculate_overlap(0, 10, 5, 10)
-~~~
-
-would return a result of 5. The first two arguments are the start and end position of the first range, and the last two
-arguments are the positions of the second range.
-
-**Note**: In case of no overlap, the distance between the two ranges is returned as a negative result.
+- `calculate_overlap` is a method to calculate the overlap between two ranges.
+  ~~~
+  overlap = Util.calculate_overlap(0, 10, 5, 10)
+  ~~~
+  would return a result of 5. The first two arguments are the start and end position of the first range, and the last
+  two arguments are the positions of the second range.
+  
+  **Note**: In case of no overlap, the distance between the two ranges is returned as a negative result.
+- `calculate_overlap_ratios` is a method to calculate the overlap ratios of two ranges.
+  ~~~
+  ratio_1, ratio_2 = Util.calculate_overlap_ratio(0, 10, 5, 10)
+  ~~~
 
 ## Footnote
-
 Footnote.py contains a collection of methods for working with footnotes.
+
+- `get_footnotes_ranges` takes a text and returns two list of tuples of start and end character positions of footnote
+  ranges, that is, text surrounded by '[[[' and ']]]'. The first list is without an offset, that is, the actual
+  positions, and the second list is with an offset, that is, as if the footnotes were removed.
+- `get_footnote_ranges_without_offset` and `get_footnote_ranges_with_offset` are variants of `get_footnotes_ranges`
+  which only return one of the lists.
+- `is_position_in_ranges` checks if a position is in one of the ranges.
+- `is_range_in_ranges` checks if a range given by a start and end position overlaps with one of the given ranges.
+- `remove_footnotes` removes footnotes from a text. Footnotes are marked by '[[[' and ']]]'.
+- `map_to_real_pos` maps start and end character positions of a text with footnotes removed to real positions, that is,
+  positions before footnotes where removed.
```

### Comparing `KPCommons-0.0.2/pyproject.toml` & `kpcommons-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "KPCommons"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Frederik Arnold", email = "frederik.arnold@hu-berlin.de"}
 ]
 description = "A collection of reusable methods."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

