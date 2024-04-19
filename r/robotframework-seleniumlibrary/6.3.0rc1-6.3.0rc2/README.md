# Comparing `tmp/robotframework-seleniumlibrary-6.3.0rc1.tar.gz` & `tmp/robotframework-seleniumlibrary-6.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-seleniumlibrary-6.3.0rc1.tar", last modified: Sat Mar 30 17:21:48 2024, max compression
+gzip compressed data, was "robotframework-seleniumlibrary-6.3.0rc2.tar", last modified: Tue Apr 16 12:21:29 2024, max compression
```

## Comparing `robotframework-seleniumlibrary-6.3.0rc1.tar` & `robotframework-seleniumlibrary-6.3.0rc2.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.413687 robotframework-seleniumlibrary-6.3.0rc1/
--rw-rw-rw-   0        0        0      667 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/COPYRIGHT.txt
--rw-rw-rw-   0        0        0    11358 2023-12-18 00:23:36.000000 robotframework-seleniumlibrary-6.3.0rc1/LICENSE.txt
--rw-rw-rw-   0        0        0      101 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/MANIFEST.in
--rw-rw-rw-   0        0        0    15039 2024-03-30 17:21:48.412688 robotframework-seleniumlibrary-6.3.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0    13554 2024-01-05 01:33:26.000000 robotframework-seleniumlibrary-6.3.0rc1/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.336331 robotframework-seleniumlibrary-6.3.0rc1/docs/
--rw-rw-rw-   0        0        0   483578 2024-01-05 01:33:26.000000 robotframework-seleniumlibrary-6.3.0rc1/docs/SeleniumLibrary.html
--rw-rw-rw-   0        0        0      251 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/pyproject.toml
--rw-rw-rw-   0        0        0       80 2023-12-19 23:24:33.000000 robotframework-seleniumlibrary-6.3.0rc1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 17:21:48.413687 robotframework-seleniumlibrary-6.3.0rc1/setup.cfg
--rw-rw-rw-   0        0        0     1789 2024-03-10 16:51:18.000000 robotframework-seleniumlibrary-6.3.0rc1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.163568 robotframework-seleniumlibrary-6.3.0rc1/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.346170 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/
--rw-rw-rw-   0        0        0    34687 2024-03-30 17:16:44.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/__init__.py
--rw-rw-rw-   0        0        0    16694 2024-03-30 17:17:25.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/__init__.pyi
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.350170 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/base/
--rw-rw-rw-   0        0        0      834 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/base/__init__.py
--rw-rw-rw-   0        0        0     4506 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/base/context.py
--rw-rw-rw-   0        0        0     3189 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/base/librarycomponent.py
--rw-rw-rw-   0        0        0     1061 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/errors.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.367940 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/
--rw-rw-rw-   0        0        0     1444 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/__init__.py
--rw-rw-rw-   0        0        0     6139 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/alert.py
--rw-rw-rw-   0        0        0    36141 2024-01-05 01:33:26.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/browsermanagement.py
--rw-rw-rw-   0        0        0     7383 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/cookie.py
--rw-rw-rw-   0        0        0    49684 2024-03-07 01:25:27.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/element.py
--rw-rw-rw-   0        0        0    19701 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/formelement.py
--rw-rw-rw-   0        0        0     4195 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/frames.py
--rw-rw-rw-   0        0        0     7769 2024-01-05 01:33:26.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/javascript.py
--rw-rw-rw-   0        0        0     3109 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/runonfailure.py
--rw-rw-rw-   0        0        0    10287 2024-01-05 01:33:26.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/screenshot.py
--rw-rw-rw-   0        0        0    14608 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/selectelement.py
--rw-rw-rw-   0        0        0    10396 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/tableelement.py
--rw-rw-rw-   0        0        0    15488 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/waiting.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.371941 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/webdrivertools/
--rw-rw-rw-   0        0        0      912 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/webdrivertools/__init__.py
--rw-rw-rw-   0        0        0     1593 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/webdrivertools/sl_file_detector.py
--rw-rw-rw-   0        0        0    21207 2024-03-07 01:27:08.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/webdrivertools/webdrivertools.py
--rw-rw-rw-   0        0        0    12754 2024-01-23 18:54:44.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/window.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.376941 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/locators/
--rw-rw-rw-   0        0        0      841 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/locators/__init__.py
--rw-rw-rw-   0        0        0     1674 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/locators/customlocator.py
--rw-rw-rw-   0        0        0    14458 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/locators/elementfinder.py
--rw-rw-rw-   0        0        0     7786 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/locators/windowmanager.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.382472 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/
--rw-rw-rw-   0        0        0     1275 2023-12-19 23:24:33.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.386472 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/events/
--rw-rw-rw-   0        0        0     1467 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/events/__init__.py
--rw-rw-rw-   0        0        0     1086 2023-12-19 23:24:33.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/events/event.py
--rw-rw-rw-   0        0        0     1456 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/events/scope_event.py
--rw-rw-rw-   0        0        0     1141 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/librarylistener.py
--rw-rw-rw-   0        0        0      882 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/path_formatter.py
--rw-rw-rw-   0        0        0     1532 2023-12-19 23:24:33.000000 robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/types.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:21:48.410690 robotframework-seleniumlibrary-6.3.0rc1/src/robotframework_seleniumlibrary.egg-info/
--rw-rw-rw-   0        0        0    15039 2024-03-30 17:21:48.000000 robotframework-seleniumlibrary-6.3.0rc1/src/robotframework_seleniumlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2024-03-30 17:21:48.000000 robotframework-seleniumlibrary-6.3.0rc1/src/robotframework_seleniumlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 17:21:48.000000 robotframework-seleniumlibrary-6.3.0rc1/src/robotframework_seleniumlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-03-30 17:21:48.000000 robotframework-seleniumlibrary-6.3.0rc1/src/robotframework_seleniumlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-30 17:21:48.000000 robotframework-seleniumlibrary-6.3.0rc1/src/robotframework_seleniumlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.214051 robotframework-seleniumlibrary-6.3.0rc2/
+-rw-rw-rw-   0        0        0      667 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/COPYRIGHT.txt
+-rw-rw-rw-   0        0        0    11358 2023-12-18 00:23:36.000000 robotframework-seleniumlibrary-6.3.0rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0      101 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/MANIFEST.in
+-rw-rw-rw-   0        0        0    15039 2024-04-16 12:21:29.213052 robotframework-seleniumlibrary-6.3.0rc2/PKG-INFO
+-rw-rw-rw-   0        0        0    13554 2024-04-02 10:51:36.000000 robotframework-seleniumlibrary-6.3.0rc2/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.127284 robotframework-seleniumlibrary-6.3.0rc2/docs/
+-rw-rw-rw-   0        0        0   483578 2024-04-02 10:51:36.000000 robotframework-seleniumlibrary-6.3.0rc2/docs/SeleniumLibrary.html
+-rw-rw-rw-   0        0        0      251 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/pyproject.toml
+-rw-rw-rw-   0        0        0       80 2023-12-19 23:24:33.000000 robotframework-seleniumlibrary-6.3.0rc2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 12:21:29.214051 robotframework-seleniumlibrary-6.3.0rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1789 2024-04-02 10:51:36.000000 robotframework-seleniumlibrary-6.3.0rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:28.948210 robotframework-seleniumlibrary-6.3.0rc2/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.140153 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/
+-rw-rw-rw-   0        0        0    34765 2024-04-16 12:18:22.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/__init__.py
+-rw-rw-rw-   0        0        0    16792 2024-04-16 12:18:54.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/__init__.pyi
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.145170 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/base/
+-rw-rw-rw-   0        0        0      834 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/base/__init__.py
+-rw-rw-rw-   0        0        0     4506 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/base/context.py
+-rw-rw-rw-   0        0        0     3189 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/base/librarycomponent.py
+-rw-rw-rw-   0        0        0     1128 2024-04-16 11:28:53.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.164378 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/
+-rw-rw-rw-   0        0        0     1510 2024-04-16 11:28:53.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/__init__.py
+-rw-rw-rw-   0        0        0     6139 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/alert.py
+-rw-rw-rw-   0        0        0    36141 2024-04-02 10:51:36.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/browsermanagement.py
+-rw-rw-rw-   0        0        0     7383 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/cookie.py
+-rw-rw-rw-   0        0        0    50819 2024-04-16 11:28:53.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/element.py
+-rw-rw-rw-   0        0        0     2991 2024-04-16 11:28:53.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/expectedconditions.py
+-rw-rw-rw-   0        0        0    19701 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/formelement.py
+-rw-rw-rw-   0        0        0     4195 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/frames.py
+-rw-rw-rw-   0        0        0     7769 2024-04-02 10:51:36.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/javascript.py
+-rw-rw-rw-   0        0        0     3109 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/runonfailure.py
+-rw-rw-rw-   0        0        0    10287 2024-01-05 01:33:26.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/screenshot.py
+-rw-rw-rw-   0        0        0    14608 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/selectelement.py
+-rw-rw-rw-   0        0        0    10396 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/tableelement.py
+-rw-rw-rw-   0        0        0    15488 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/waiting.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.168377 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/webdrivertools/
+-rw-rw-rw-   0        0        0      912 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/webdrivertools/__init__.py
+-rw-rw-rw-   0        0        0     1593 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/webdrivertools/sl_file_detector.py
+-rw-rw-rw-   0        0        0    21207 2024-04-02 10:51:36.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/webdrivertools/webdrivertools.py
+-rw-rw-rw-   0        0        0    12754 2024-04-02 10:51:36.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/window.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.175052 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/locators/
+-rw-rw-rw-   0        0        0      841 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/locators/__init__.py
+-rw-rw-rw-   0        0        0     1674 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/locators/customlocator.py
+-rw-rw-rw-   0        0        0    14458 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/locators/elementfinder.py
+-rw-rw-rw-   0        0        0     7786 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/locators/windowmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.180052 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/
+-rw-rw-rw-   0        0        0     1275 2023-12-19 23:24:33.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.184052 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/events/
+-rw-rw-rw-   0        0        0     1467 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/events/__init__.py
+-rw-rw-rw-   0        0        0     1086 2023-12-19 23:24:33.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/events/event.py
+-rw-rw-rw-   0        0        0     1456 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/events/scope_event.py
+-rw-rw-rw-   0        0        0     1141 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/librarylistener.py
+-rw-rw-rw-   0        0        0      882 2023-12-19 23:23:16.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/path_formatter.py
+-rw-rw-rw-   0        0        0     1532 2023-12-19 23:24:33.000000 robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/types.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:21:29.212052 robotframework-seleniumlibrary-6.3.0rc2/src/robotframework_seleniumlibrary.egg-info/
+-rw-rw-rw-   0        0        0    15039 2024-04-16 12:21:28.000000 robotframework-seleniumlibrary-6.3.0rc2/src/robotframework_seleniumlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1918 2024-04-16 12:21:28.000000 robotframework-seleniumlibrary-6.3.0rc2/src/robotframework_seleniumlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 12:21:28.000000 robotframework-seleniumlibrary-6.3.0rc2/src/robotframework_seleniumlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-16 12:21:28.000000 robotframework-seleniumlibrary-6.3.0rc2/src/robotframework_seleniumlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-16 12:21:28.000000 robotframework-seleniumlibrary-6.3.0rc2/src/robotframework_seleniumlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/COPYRIGHT.txt` & `robotframework-seleniumlibrary-6.3.0rc2/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/LICENSE.txt` & `robotframework-seleniumlibrary-6.3.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/PKG-INFO` & `robotframework-seleniumlibrary-6.3.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-seleniumlibrary
-Version: 6.3.0rc1
+Version: 6.3.0rc2
 Summary: Web testing library for Robot Framework
 Home-page: https://github.com/robotframework/SeleniumLibrary
 Author: Ed Manlove, Yuri Verweij, Lisa Crispin
 Author-email: emanlove@verizon.net
 License: Apache License 2.0
 Keywords: robotframework testing testautomation selenium webdriver web
 Platform: any
```

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/README.rst` & `robotframework-seleniumlibrary-6.3.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/docs/SeleniumLibrary.html` & `robotframework-seleniumlibrary-6.3.0rc2/docs/SeleniumLibrary.html`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/setup.py` & `robotframework-seleniumlibrary-6.3.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/__init__.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from SeleniumLibrary.base import LibraryComponent
 from SeleniumLibrary.errors import NoOpenBrowser, PluginError
 from SeleniumLibrary.keywords import (
     AlertKeywords,
     BrowserManagementKeywords,
     CookieKeywords,
     ElementKeywords,
+    ExpectedConditionKeywords,
     FormElementKeywords,
     FrameKeywords,
     JavaScriptKeywords,
     RunOnFailureKeywords,
     ScreenshotKeywords,
     SelectElementKeywords,
     TableElementKeywords,
@@ -47,15 +48,15 @@
     WindowKeywords,
 )
 from SeleniumLibrary.keywords.screenshot import EMBED
 from SeleniumLibrary.locators import ElementFinder
 from SeleniumLibrary.utils import LibraryListener, is_truthy, _convert_timeout, _convert_delay
 
 
-__version__ = "6.3.0rc1"
+__version__ = "6.3.0rc2"
 
 
 class SeleniumLibrary(DynamicCore):
     """SeleniumLibrary is a web testing library for Robot Framework.
 
     This document explains how to use keywords provided by SeleniumLibrary.
     For information about installation, support, and more, please visit the
@@ -486,14 +487,15 @@
         self._element_finder = ElementFinder(self)
         self._plugin_keywords = []
         libraries = [
             AlertKeywords(self),
             BrowserManagementKeywords(self),
             CookieKeywords(self),
             ElementKeywords(self),
+            ExpectedConditionKeywords(self),
             FormElementKeywords(self),
             FrameKeywords(self),
             JavaScriptKeywords(self),
             RunOnFailureKeywords(self),
             ScreenshotKeywords(self),
             SelectElementKeywords(self),
             TableElementKeywords(self),
```

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/__init__.pyi` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
     def unselect_all_from_list(self, locator: Union): ...
     def unselect_checkbox(self, locator: Union): ...
     def unselect_frame(self): ...
     def unselect_from_list_by_index(self, locator: Union, *indexes: str): ...
     def unselect_from_list_by_label(self, locator: Union, *labels: str): ...
     def unselect_from_list_by_value(self, locator: Union, *values: str): ...
     def wait_for_condition(self, condition: str, timeout: Optional[Optional] = None, error: Optional[Optional] = None): ...
+    def wait_for_expected_condition(self, condition: string, *args, timeout: Optional = 10): ...
     def wait_until_element_contains(self, locator: Union, text: str, timeout: Optional[Optional] = None, error: Optional[Optional] = None): ...
     def wait_until_element_does_not_contain(self, locator: Union, text: str, timeout: Optional[Optional] = None, error: Optional[Optional] = None): ...
     def wait_until_element_is_enabled(self, locator: Union, timeout: Optional[Optional] = None, error: Optional[Optional] = None): ...
     def wait_until_element_is_not_visible(self, locator: Union, timeout: Optional[Optional] = None, error: Optional[Optional] = None): ...
     def wait_until_element_is_visible(self, locator: Union, timeout: Optional[Optional] = None, error: Optional[Optional] = None): ...
     def wait_until_location_contains(self, expected: str, timeout: Optional[Optional] = None, message: Optional[Optional] = None): ...
     def wait_until_location_does_not_contain(self, location: str, timeout: Optional[Optional] = None, message: Optional[Optional] = None): ...
```

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/base/__init__.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/base/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/base/context.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/base/context.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/base/librarycomponent.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/base/librarycomponent.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/errors.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,7 +33,11 @@
 
 class NoOpenBrowser(SeleniumLibraryException):
     pass
 
 
 class PluginError(SeleniumLibraryException):
     pass
+
+
+class UnkownExpectedCondition(SeleniumLibraryException):
+    pass
```

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/__init__.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .alert import AlertKeywords  # noqa
 from .browsermanagement import BrowserManagementKeywords  # noqa
 from .cookie import CookieKeywords  # noqa
 from .element import ElementKeywords  # noqa
+from .expectedconditions import ExpectedConditionKeywords  # noqa
 from .formelement import FormElementKeywords  # noqa
 from .frames import FrameKeywords  # noqa
 from .javascript import JavaScriptKeywords  # noqa
 from .runonfailure import RunOnFailureKeywords  # noqa
 from .screenshot import ScreenshotKeywords  # noqa
 from .selectelement import SelectElementKeywords  # noqa
 from .tableelement import TableElementKeywords  # noqa
```

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/alert.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/alert.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/browsermanagement.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/browsermanagement.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/cookie.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/cookie.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/element.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -895,15 +895,34 @@
 evt.initEvent(eventName, true, true);
 return !element.dispatchEvent(evt);
         """
         self.driver.execute_script(script, element, event)
 
     @keyword
     def press_key(self, locator: Union[WebElement, str], key: str):
-        """*DEPRECATED in SeleniumLibrary 4.0.* use `Press Keys` instead."""
+        """Simulates user pressing key on element identified by ``locator``.
+
+        See the `Locating elements` section for details about the locator
+        syntax.
+
+        ``key`` is either a single character, a string, or a numerical ASCII
+        code of the key lead by '\\'.
+
+        Examples:
+        | `Press Key` | text_field   | q     |
+        | `Press Key` | text_field   | abcde |
+        | `Press Key` | login_button | \\13  | # ASCII code for enter key |
+
+        `Press Key` and `Press Keys` differ in the methods to simulate key
+        presses. `Press Key` uses the WebDriver `SEND_KEYS_TO_ELEMENT` command
+        using the selenium send_keys method. Although one is not recommended
+        over the other if `Press Key` does not work we recommend trying
+        `Press Keys`.
+        send_
+        """
         if key.startswith("\\") and len(key) > 1:
             key = self._map_ascii_key_code_to_key(int(key[1:]))
         element = self.find_element(locator)
         element.send_keys(key)
 
     @keyword
     def press_keys(self, locator: Union[WebElement, None, str] = None, *keys: str):
@@ -948,14 +967,21 @@
         | `Press Keys` | text_field | E+N+D          |            | # Sends string "END" to element.                                                  |
         | `Press Keys` | text_field | XXX            | YY         | # Sends strings "XXX" and "YY" to element.                                        |
         | `Press Keys` | text_field | XXX+YY         |            | # Same as above.                                                                  |
         | `Press Keys` | text_field | ALT+ARROW_DOWN |            | # Pressing "ALT" key down, then pressing ARROW_DOWN and then releasing both keys. |
         | `Press Keys` | text_field | ALT            | ARROW_DOWN | # Pressing "ALT" key and then pressing ARROW_DOWN.                                |
         | `Press Keys` | text_field | CTRL+c         |            | # Pressing CTRL key down, sends string "c" and then releases CTRL key.            |
         | `Press Keys` | button     | RETURN         |            | # Pressing "ENTER" key to element.                                                |
+
+        `Press Key` and `Press Keys` differ in the methods to simulate key
+        presses. `Press Keys` uses the Selenium/WebDriver Actions.
+        `Press Keys` also has a more extensive syntax for describing keys,
+        key combinations, and key actions. Although one is not recommended
+        over the other if `Press Keys` does not work we recommend trying
+        `Press Key`.
         """
         parsed_keys = self._parse_keys(*keys)
         if not is_noney(locator):
             self.info(f"Sending key(s) {keys} to {locator} element.")
             element = self.find_element(locator)
             ActionChains(self.driver, duration=self.ctx.action_chain_delay).click(element).perform()
         else:
```

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/formelement.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/formelement.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/frames.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/frames.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/javascript.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/javascript.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/runonfailure.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/runonfailure.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/screenshot.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/screenshot.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/selectelement.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/selectelement.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/tableelement.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/tableelement.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/waiting.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/waiting.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/webdrivertools/__init__.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/webdrivertools/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/webdrivertools/sl_file_detector.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/webdrivertools/sl_file_detector.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/webdrivertools/webdrivertools.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/webdrivertools/webdrivertools.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/keywords/window.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/keywords/window.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/locators/__init__.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/locators/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/locators/customlocator.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/locators/customlocator.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/locators/elementfinder.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/locators/elementfinder.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/locators/windowmanager.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/locators/windowmanager.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/__init__.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/events/__init__.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/events/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/events/event.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/events/event.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/events/scope_event.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/events/scope_event.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/librarylistener.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/librarylistener.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/path_formatter.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/path_formatter.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/SeleniumLibrary/utils/types.py` & `robotframework-seleniumlibrary-6.3.0rc2/src/SeleniumLibrary/utils/types.py`

 * *Files identical despite different names*

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/robotframework_seleniumlibrary.egg-info/PKG-INFO` & `robotframework-seleniumlibrary-6.3.0rc2/src/robotframework_seleniumlibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-seleniumlibrary
-Version: 6.3.0rc1
+Version: 6.3.0rc2
 Summary: Web testing library for Robot Framework
 Home-page: https://github.com/robotframework/SeleniumLibrary
 Author: Ed Manlove, Yuri Verweij, Lisa Crispin
 Author-email: emanlove@verizon.net
 License: Apache License 2.0
 Keywords: robotframework testing testautomation selenium webdriver web
 Platform: any
```

### Comparing `robotframework-seleniumlibrary-6.3.0rc1/src/robotframework_seleniumlibrary.egg-info/SOURCES.txt` & `robotframework-seleniumlibrary-6.3.0rc2/src/robotframework_seleniumlibrary.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/SeleniumLibrary/base/context.py
 src/SeleniumLibrary/base/librarycomponent.py
 src/SeleniumLibrary/keywords/__init__.py
 src/SeleniumLibrary/keywords/alert.py
 src/SeleniumLibrary/keywords/browsermanagement.py
 src/SeleniumLibrary/keywords/cookie.py
 src/SeleniumLibrary/keywords/element.py
+src/SeleniumLibrary/keywords/expectedconditions.py
 src/SeleniumLibrary/keywords/formelement.py
 src/SeleniumLibrary/keywords/frames.py
 src/SeleniumLibrary/keywords/javascript.py
 src/SeleniumLibrary/keywords/runonfailure.py
 src/SeleniumLibrary/keywords/screenshot.py
 src/SeleniumLibrary/keywords/selectelement.py
 src/SeleniumLibrary/keywords/tableelement.py
```

