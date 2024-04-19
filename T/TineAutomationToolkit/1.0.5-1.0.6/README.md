# Comparing `tmp/TineAutomationToolkit-1.0.5.tar.gz` & `tmp/TineAutomationToolkit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TineAutomationToolkit-1.0.5.tar", last modified: Wed Apr 17 15:56:42 2024, max compression
+gzip compressed data, was "dist\TineAutomationToolkit-1.0.6.tar", last modified: Fri Apr 19 09:33:36 2024, max compression
```

## Comparing `TineAutomationToolkit-1.0.5.tar` & `TineAutomationToolkit-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/
--rw-rw-rw-   0        0        0     2280 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/
--rw-rw-rw-   0        0        0      383 2024-04-17 15:32:05.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/detect/
--rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/detect/__init__.py
--rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/detect/detectelement.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/
--rw-rw-rw-   0        0        0      724 2024-04-17 15:54:04.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/__init__.py
--rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/capturescreenshot.py
--rw-rw-rw-   0        0        0     4726 2024-04-11 09:59:28.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/connectionmanagement.py
--rw-rw-rw-   0        0        0    18184 2024-04-17 15:53:05.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/controlelement.py
--rw-rw-rw-   0        0        0     2495 2024-04-17 15:53:57.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/keyevent.py
--rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/scroll.py
--rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/toolkitstest.py
--rw-rw-rw-   0        0        0     2444 2024-04-17 15:25:52.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/touch.py
--rw-rw-rw-   0        0        0     6663 2024-04-11 09:12:10.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/waitingelement.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/
--rw-rw-rw-   0        0        0     2280 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      782 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 15:56:42.000000 TineAutomationToolkit-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      739 2024-04-17 15:54:28.000000 TineAutomationToolkit-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/
+-rw-rw-rw-   0        0        0     2280 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/
+-rw-rw-rw-   0        0        0      383 2024-04-17 15:32:05.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/detect/
+-rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/detect/__init__.py
+-rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/detect/detectelement.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/
+-rw-rw-rw-   0        0        0      724 2024-04-17 15:54:04.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/capturescreenshot.py
+-rw-rw-rw-   0        0        0     4726 2024-04-11 09:59:28.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/connectionmanagement.py
+-rw-rw-rw-   0        0        0    18183 2024-04-19 08:45:03.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/controlelement.py
+-rw-rw-rw-   0        0        0     2495 2024-04-17 15:53:57.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/keyevent.py
+-rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/scroll.py
+-rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/toolkitstest.py
+-rw-rw-rw-   0        0        0     2444 2024-04-17 15:25:52.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/touch.py
+-rw-rw-rw-   0        0        0     8386 2024-04-19 09:32:00.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/waitingelement.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/
+-rw-rw-rw-   0        0        0     2280 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      782 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:33:36.000000 TineAutomationToolkit-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      739 2024-04-19 08:43:21.000000 TineAutomationToolkit-1.0.6/setup.py
```

### Comparing `TineAutomationToolkit-1.0.5/PKG-INFO` & `TineAutomationToolkit-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.5
+Version: 1.0.6
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.5/README.md` & `TineAutomationToolkit-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit/detect/detectelement.py` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit/detect/detectelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/__init__.py` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/capturescreenshot.py` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/capturescreenshot.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/connectionmanagement.py` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/connectionmanagement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/controlelement.py` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/controlelement.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         ตัวอย่างการใช้งาน:
 
         | ${text} | ดึงข้อความ | //*[contains(@text,'foo')] |
 
         ใหม่ใน AppiumLibrary 1.4.
         """
         text = self._get_text(locator)
-        self._info("Element '%s' text is '%s' " % (locator, text))
+        log._info("Element '%s' text is '%s' " % (locator, text))
         return text
     
       #Input
     
     def native_input_text(self, locator, text):
         """Types the given `text` into text field identified by `locator`.
```

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/keyevent.py` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/keyevent.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/scroll.py` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/scroll.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/touch.py` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/touch.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit/keywords/waitingelement.py` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit/keywords/waitingelement.py`

 * *Files 25% similar despite different names*

```diff
@@ -112,14 +112,49 @@
         `Wait Until Page Does Not Contain Element` and
         BuiltIn keyword `Wait Until Keyword Succeeds`.
         """
         if not error:
             error = "Text '%s' did not appear in <TIMEOUT>" % text
         self._wait_until(timeout, error, conelement._is_text_present, text)
 
+    def native_wait_until_page_does_not_contain(self, text, timeout=None, error=None):
+        """Waits until `text` disappears from current page.
+
+        Fails if `timeout` expires before the `text` disappears. See
+        `introduction` for more information about `timeout` and its
+        default value.
+
+        `error` can be used to override the default error message.
+
+        See also `Wait Until Page Contains`,
+        `Wait Until Page Contains Element`,
+        `Wait Until Page Does Not Contain Element` and
+        BuiltIn keyword `Wait Until Keyword Succeeds`.
+
+        ===================================================
+
+        จะล้มเหลวถ้า `timeout` หมดก่อนที่ `text` จะหายไป ดู
+        `introduction` เพื่อข้อมูลเพิ่มเติมเกี่ยวกับ `timeout` และค่าเริ่มต้นของมัน
+
+        `error` สามารถใช้เพื่อแทนที่ข้อความแสดงข้อผิดพลาดเริ่มต้น
+
+        ดูเพิ่มเติมที่ `Wait Until Page Contains`,
+        `Wait Until Page Contains Element`,
+        `Wait Until Page Does Not Contain Element` และคำสั่ง BuiltIn `Wait Until Keyword Succeeds`.
+        """
+
+        def check_present():
+            present = conelement._is_text_present(text)
+            if not present:
+                return
+            else:
+                return error or "Text '%s' did not disappear in %s" % (text, self._format_timeout(timeout))
+
+        self._wait_until_no_error(timeout, check_present)    
+
     
     #PRIVATE_FUNCTION
         
     def _format_timeout(self, timeout):
         timeout = robot.utils.timestr_to_secs(timeout) if timeout is not None else timeout_in_secs
         return robot.utils.secs_to_timestr(timeout)
```

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/PKG-INFO` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.5
+Version: 1.0.6
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.5/TineAutomationToolkit.egg-info/SOURCES.txt` & `TineAutomationToolkit-1.0.6/TineAutomationToolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.5/setup.py` & `TineAutomationToolkit-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="TineAutomationToolkit",
-    version="1.0.5",
+    version="1.0.6",
     author="Pornpawit Suttha",
     author_email="pornpawit14suttha@gmail.com",
     description="Test Library for TineAutomationToolkit",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/pornpawit08/TineAutomationToolkit.git",
     packages=find_packages(),
```

