# Comparing `tmp/ansar_connect-0.1.198.tar.gz` & `tmp/ansar_connect-0.1.199.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.198.tar", last modified: Thu Apr 18 01:22:16 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.199.tar", last modified: Fri Apr 19 03:57:52 2024, max compression
```

## Comparing `ansar_connect-0.1.198.tar` & `ansar_connect-0.1.199.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 01:22:16.987901 ansar_connect-0.1.198/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.198/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-18 01:22:16.987901 ansar_connect-0.1.198/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.198/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.198/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-18 01:22:16.987901 ansar_connect-0.1.198/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.198/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 01:22:16.987901 ansar_connect-0.1.198/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 01:22:16.987901 ansar_connect-0.1.198/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 01:22:16.987901 ansar_connect-0.1.198/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-17 22:39:03.000000 ansar_connect-0.1.198/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.198/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.198/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.198/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 01:22:16.987901 ansar_connect-0.1.198/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-18 01:22:13.000000 ansar_connect-0.1.198/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.198/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77775 2024-04-18 00:04:05.000000 ansar_connect-0.1.198/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.198/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.198/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.198/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.198/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.198/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.198/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.198/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.198/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.198/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32848 2024-04-17 22:39:03.000000 ansar_connect-0.1.198/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.198/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    40928 2024-04-18 01:20:43.000000 ansar_connect-0.1.198/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.198/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.198/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.198/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6600 2024-04-18 00:04:05.000000 ansar_connect-0.1.198/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-18 01:22:16.987901 ansar_connect-0.1.198/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-18 01:22:16.000000 ansar_connect-0.1.198/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-18 01:22:16.000000 ansar_connect-0.1.198/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-18 01:22:16.000000 ansar_connect-0.1.198/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-18 01:22:16.000000 ansar_connect-0.1.198/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-18 01:22:16.000000 ansar_connect-0.1.198/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-18 01:22:16.000000 ansar_connect-0.1.198/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 03:57:52.274644 ansar_connect-0.1.199/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.199/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-19 03:57:52.274644 ansar_connect-0.1.199/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.199/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.199/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-19 03:57:52.274644 ansar_connect-0.1.199/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.199/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 03:57:52.270644 ansar_connect-0.1.199/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 03:57:52.270644 ansar_connect-0.1.199/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 03:57:52.270644 ansar_connect-0.1.199/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.199/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.199/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.199/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.199/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 03:57:52.274644 ansar_connect-0.1.199/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-04-19 03:57:49.000000 ansar_connect-0.1.199/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.199/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77775 2024-04-18 00:04:05.000000 ansar_connect-0.1.199/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.199/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.199/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.199/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.199/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.199/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.199/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.199/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.199/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.199/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.199/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.199/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    40928 2024-04-18 01:20:43.000000 ansar_connect-0.1.199/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.199/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2101 2024-04-17 21:48:32.000000 ansar_connect-0.1.199/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.199/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6600 2024-04-18 00:04:05.000000 ansar_connect-0.1.199/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-19 03:57:52.274644 ansar_connect-0.1.199/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-19 03:57:52.000000 ansar_connect-0.1.199/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-19 03:57:52.000000 ansar_connect-0.1.199/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-19 03:57:52.000000 ansar_connect-0.1.199/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-19 03:57:52.000000 ansar_connect-0.1.199/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-19 03:57:52.000000 ansar_connect-0.1.199/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-19 03:57:52.000000 ansar_connect-0.1.199/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.198/LICENSE` & `ansar_connect-0.1.199/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/PKG-INFO` & `ansar_connect-0.1.199/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.198
+Version: 0.1.199
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.198/README.md` & `ansar_connect-0.1.199/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/pyproject.toml` & `ansar_connect-0.1.199/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/setup.py` & `ansar_connect-0.1.199/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.199/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.199/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.199/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.199/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/__init__.py` & `ansar_connect-0.1.199/src/ansar/connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 868855a0d5eea6c062a008e92a7f23db9c2a9053
-Version: 0.1.197 (2024-04-18@13:22:13+NZST)
+Commit: 09daa9618fcec6a7e8a845fa69e625c5afe0aafb
+Version: 0.1.198 (2024-04-19@15:57:49+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.198/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.199/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/directory.py` & `ansar_connect-0.1.199/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.199/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.199/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/group_if.py` & `ansar_connect-0.1.199/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/grouping.py` & `ansar_connect-0.1.199/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/moving.py` & `ansar_connect-0.1.199/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/networking.py` & `ansar_connect-0.1.199/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.199/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/node.py` & `ansar_connect-0.1.199/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.199/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/procedure.py` & `ansar_connect-0.1.199/src/ansar/connect/procedure.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,15 +532,15 @@
 		self.send(ar.Close(), session)
 		self.select(ar.Closed, ar.Stop)
 
 # Refresh the session with an account.
 def procedure_login(self, account):
 	settings = ar.object_custom_settings()
 	cloud_ip = settings.cloud_ip
-	login_token = settings.login_token
+	login_token = settings.login_token or uuid.uuid4()
 
 	f = crud_address_and_token(1, cloud_ip, login_token)
 	if f:
 		return f
 
 	encrypted = settings.encrypted
 	ar.connect(self, ar.HostPort(cloud_ip, FOH_PORT), encrypted=encrypted)
```

### Comparing `ansar_connect-0.1.198/src/ansar/connect/product.py` & `ansar_connect-0.1.199/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/socketry.py` & `ansar_connect-0.1.199/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/standard.py` & `ansar_connect-0.1.199/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/transporting.py` & `ansar_connect-0.1.199/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.199/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar/connect/wan.py` & `ansar_connect-0.1.199/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.198/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.199/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.198
+Version: 0.1.199
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.198/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.199/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

