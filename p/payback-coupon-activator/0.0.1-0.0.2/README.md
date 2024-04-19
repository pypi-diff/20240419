# Comparing `tmp/payback-coupon-activator-0.0.1.tar.gz` & `tmp/payback_coupon_activator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payback-coupon-activator-0.0.1.tar", last modified: Sat Jul 22 13:06:58 2023, max compression
+gzip compressed data, was "payback_coupon_activator-0.0.2.tar", last modified: Fri Apr 19 10:31:02 2024, max compression
```

## Comparing `payback-coupon-activator-0.0.1.tar` & `payback_coupon_activator-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 13:06:58.787127 payback-coupon-activator-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-22 12:33:59.000000 payback-coupon-activator-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2380 2023-07-22 13:06:58.786127 payback-coupon-activator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      731 2023-07-22 11:49:23.000000 payback-coupon-activator-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 13:06:58.784125 payback-coupon-activator-0.0.1/payback_coupon_activator.egg-info/
--rw-rw-rw-   0        0        0     2380 2023-07-22 13:06:58.000000 payback-coupon-activator-0.0.1/payback_coupon_activator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-07-22 13:06:58.000000 payback-coupon-activator-0.0.1/payback_coupon_activator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 13:06:58.000000 payback-coupon-activator-0.0.1/payback_coupon_activator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-07-22 13:06:58.000000 payback-coupon-activator-0.0.1/payback_coupon_activator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-22 13:06:58.000000 payback-coupon-activator-0.0.1/payback_coupon_activator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-22 13:06:58.000000 payback-coupon-activator-0.0.1/payback_coupon_activator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1494 2023-07-22 12:12:16.000000 payback-coupon-activator-0.0.1/payback_coupon_activator.py
--rw-rw-rw-   0        0        0      570 2023-07-22 12:18:08.000000 payback-coupon-activator-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 13:06:58.787127 payback-coupon-activator-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 10:31:02.653519 payback_coupon_activator-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-22 12:33:59.000000 payback_coupon_activator-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2405 2024-04-19 10:31:02.650520 payback_coupon_activator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      731 2023-07-22 11:49:23.000000 payback_coupon_activator-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 10:31:02.648521 payback_coupon_activator-0.0.2/payback_coupon_activator.egg-info/
+-rw-rw-rw-   0        0        0     2405 2024-04-19 10:31:02.000000 payback_coupon_activator-0.0.2/payback_coupon_activator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-04-19 10:31:02.000000 payback_coupon_activator-0.0.2/payback_coupon_activator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 10:31:02.000000 payback_coupon_activator-0.0.2/payback_coupon_activator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-19 10:31:02.000000 payback_coupon_activator-0.0.2/payback_coupon_activator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 10:31:02.000000 payback_coupon_activator-0.0.2/payback_coupon_activator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-19 10:31:02.000000 payback_coupon_activator-0.0.2/payback_coupon_activator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2008 2024-04-17 11:21:25.000000 payback_coupon_activator-0.0.2/payback_coupon_activator.py
+-rw-rw-rw-   0        0        0      587 2024-04-19 10:12:13.000000 payback_coupon_activator-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 10:31:02.653519 payback_coupon_activator-0.0.2/setup.cfg
```

### Comparing `payback-coupon-activator-0.0.1/LICENSE.txt` & `payback_coupon_activator-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `payback-coupon-activator-0.0.1/PKG-INFO` & `payback_coupon_activator-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payback-coupon-activator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Activates all Payback coupons with Selenium WebDriver in Chrome logged into your Payback account.
 Author-email: Robert Kampf <Robert.Kampf@gmx.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Kampf
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,14 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/BobbyCephy/payback-coupon-activator
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: selenium
 
 # Payback Coupon Activator
 Activates all Payback coupons with Selenium WebDriver in Chrome logged into your Payback account.
 
 ## Installation
 * Install [Chrome](https://www.google.com/chrome)
 * Log in to your [Payback](https://www.payback.de/login) account permanently
```

### Comparing `payback-coupon-activator-0.0.1/README.md` & `payback_coupon_activator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `payback-coupon-activator-0.0.1/payback_coupon_activator.egg-info/PKG-INFO` & `payback_coupon_activator-0.0.2/payback_coupon_activator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payback-coupon-activator
-Version: 0.0.1
+Version: 0.0.2
 Summary: Activates all Payback coupons with Selenium WebDriver in Chrome logged into your Payback account.
 Author-email: Robert Kampf <Robert.Kampf@gmx.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Kampf
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,14 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/BobbyCephy/payback-coupon-activator
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: selenium
 
 # Payback Coupon Activator
 Activates all Payback coupons with Selenium WebDriver in Chrome logged into your Payback account.
 
 ## Installation
 * Install [Chrome](https://www.google.com/chrome)
 * Log in to your [Payback](https://www.payback.de/login) account permanently
```

### Comparing `payback-coupon-activator-0.0.1/payback_coupon_activator.py` & `payback_coupon_activator-0.0.2/payback_coupon_activator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,51 @@
 from selenium.webdriver import Chrome
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions
 import os
+import platform
 
 
 def element(by, value, parent, timeout=10):
     return WebDriverWait(parent, timeout).until(
         expected_conditions.presence_of_element_located((by, value))
     )
 
 
 def main():
-    options = Options()
-    options.add_argument(
-        "user-data-dir="
-        + os.path.join(
-            os.getenv("LOCALAPPDATA"), "Google", "Chrome", "User Data"
+    if platform.system() == "Windows":
+        user_data_dir = (
+            os.getenv("LOCALAPPDATA"),
+            "Google",
+            "Chrome",
+            "User Data",
         )
-    )
+
+    elif platform.system() == "Linux":
+        user_data_dir = (
+            os.path.expanduser("~"),
+            ".config",
+            "google-chrome",
+        )
+
+    elif platform.system() == "Darwin":
+        user_data_dir = (
+            os.path.expanduser("~"),
+            "Library",
+            "Application Support",
+            "Google",
+            "Chrome",
+        )
+
+    options = Options()
+    options.add_argument("user-data-dir=" + os.path.join(user_data_dir))
+
     service = Service()
     driver = Chrome(options, service)
     driver.get("https://www.payback.de/coupons")
     center = element(By.ID, "coupon-center", driver).shadow_root
     headline = element(
         By.CLASS_NAME, "coupon-center__header-published-headline", center
     )
```

### Comparing `payback-coupon-activator-0.0.1/pyproject.toml` & `payback_coupon_activator-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-[project]
-name = "payback-coupon-activator"
-version = "0.0.1"
-description = "Activates all Payback coupons with Selenium WebDriver in Chrome logged into your Payback account."
-readme = "README.md"
-license = {file = "LICENSE.txt"}
-authors = [{name = "Robert Kampf", email = "Robert.Kampf@gmx.de"}]
-dependencies = ["selenium"]
-
-[project.urls]
-"Homepage" = "https://github.com/BobbyCephy/payback-coupon-activator"
-
-[project.scripts]
-payback-coupon-activator = "payback_coupon_activator:main"
-
-[build-system]
-requires = ["setuptools"]
+[project]
+name = "payback-coupon-activator"
+version = "0.0.2"
+description = "Activates all Payback coupons with Selenium WebDriver in Chrome logged into your Payback account."
+readme = "README.md"
+license = {file = "LICENSE.txt"}
+authors = [{name = "Robert Kampf", email = "Robert.Kampf@gmx.de"}]
+dependencies = ["selenium"]
+
+[project.urls]
+"Homepage" = "https://github.com/BobbyCephy/payback-coupon-activator"
+
+[project.scripts]
+payback-coupon-activator = "payback_coupon_activator:main"
+
+[build-system]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

