# Comparing `tmp/google-cloud-storage-control-0.1.2.tar.gz` & `tmp/google-cloud-storage-control-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-storage-control-0.1.2.tar", last modified: Thu Apr  4 18:15:48 2024, max compression
+gzip compressed data, was "google-cloud-storage-control-0.1.3.tar", last modified: Fri Apr 19 00:24:45 2024, max compression
```

## Comparing `google-cloud-storage-control-0.1.2.tar` & `google-cloud-storage-control-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5526 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4138 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.522830 google-cloud-storage-control-0.1.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.522830 google-cloud-storage-control-0.1.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.526831 google-cloud-storage-control-0.1.2/google/cloud/storage_control/
--rw-rw-r--   0 root         (0)     1003     2064 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.526831 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/
--rw-rw-r--   0 root         (0)     1003     1899 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     3061 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.526831 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.530833 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/
--rw-rw-r--   0 root         (0)     1003      769 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/__init__.py
--rw-rw-r--   0 root         (0)     1003    58574 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/async_client.py
--rw-rw-r--   0 root         (0)     1003    78950 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/client.py
--rw-rw-r--   0 root         (0)     1003    11060 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.530833 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14186 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22977 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23517 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.530833 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/
--rw-rw-r--   0 root         (0)     1003     1624 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    27732 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/storage_control.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.530833 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/
--rw-r--r--   0 root         (0)     1003     5526 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1590 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3201 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   194411 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/test_storage_control.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5526 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4138 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.141650 google-cloud-storage-control-0.1.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.141650 google-cloud-storage-control-0.1.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.141650 google-cloud-storage-control-0.1.3/google/cloud/storage_control/
+-rw-rw-r--   0 root         (0)     1003     2064 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/
+-rw-rw-r--   0 root         (0)     1003     1899 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3061 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/
+-rw-rw-r--   0 root         (0)     1003      769 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61018 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/async_client.py
+-rw-rw-r--   0 root         (0)     1003    81394 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/client.py
+-rw-rw-r--   0 root         (0)     1003    11060 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14186 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    23737 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    24277 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.145651 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1624 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28587 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/storage_control.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/
+-rw-r--r--   0 root         (0)     1003     5526 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1590 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-19 00:24:45.000000 google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3201 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-19 00:24:45.149651 google-cloud-storage-control-0.1.3/tests/unit/gapic/storage_control_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/unit/gapic/storage_control_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   194411 2024-04-19 00:21:34.000000 google-cloud-storage-control-0.1.3/tests/unit/gapic/storage_control_v2/test_storage_control.py
```

### Comparing `google-cloud-storage-control-0.1.2/LICENSE` & `google-cloud-storage-control-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/MANIFEST.in` & `google-cloud-storage-control-0.1.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/PKG-INFO` & `google-cloud-storage-control-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-control
-Version: 0.1.2
+Version: 0.1.3
 Summary: Google Cloud Storage Control API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-storage-control-0.1.2/README.rst` & `google-cloud-storage-control-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control/__init__.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control/gapic_version.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.2"  # {x-release-please-version}
+__version__ = "0.1.3"  # {x-release-please-version}
```

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/__init__.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/gapic_metadata.json` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/gapic_version.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.2"  # {x-release-please-version}
+__version__ = "0.1.3"  # {x-release-please-version}
```

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/__init__.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/__init__.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/async_client.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -275,15 +275,17 @@
         parent: Optional[str] = None,
         folder: Optional[storage_control.Folder] = None,
         folder_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> storage_control.Folder:
-        r"""Creates a new folder.
+        r"""Creates a new folder. This operation is only
+        applicable to a hierarchical namespace enabled bucket.
+        Hierarchical namespace buckets are in allowlist preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -307,17 +309,23 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.storage_control_v2.types.CreateFolderRequest, dict]]):
                 The request object. Request message for CreateFolder.
+                This operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             parent (:class:`str`):
                 Required. Name of the bucket in which
-                the folder will reside.
+                the folder will reside. The bucket must
+                be a hierarchical namespace enabled
+                bucket.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             folder (:class:`google.cloud.storage_control_v2.types.Folder`):
                 Required. Properties of the new folder being created.
                 The bucket and name of the folder are specified in the
@@ -342,15 +350,19 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.storage_control_v2.types.Folder:
-                A folder.
+                A folder resource. This resource can
+                only exist in a hierarchical namespace
+                enabled bucket. Hierarchical namespace
+                buckets are in allowlist preview.
+
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, folder, folder_id])
         if request is not None and has_flattened_params:
             raise ValueError(
@@ -399,15 +411,18 @@
         request: Optional[Union[storage_control.DeleteFolderRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
-        r"""Permanently deletes an empty folder.
+        r"""Permanently deletes an empty folder. This operation
+        is only applicable to a hierarchical namespace enabled
+        bucket. Hierarchical namespace buckets are in allowlist
+        preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -427,14 +442,18 @@
 
                 # Make the request
                 await client.delete_folder(request=request)
 
         Args:
             request (Optional[Union[google.cloud.storage_control_v2.types.DeleteFolderRequest, dict]]):
                 The request object. Request message for DeleteFolder.
+                This operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             name (:class:`str`):
                 Required. Name of the folder. Format:
                 ``projects/{project}/buckets/{bucket}/folders/{folder}``
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -488,15 +507,18 @@
         request: Optional[Union[storage_control.GetFolderRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> storage_control.Folder:
-        r"""Returns metadata for the specified folder.
+        r"""Returns metadata for the specified folder. This
+        operation is only applicable to a hierarchical namespace
+        enabled bucket. Hierarchical namespace buckets are in
+        allowlist preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -518,15 +540,19 @@
                 response = await client.get_folder(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.storage_control_v2.types.GetFolderRequest, dict]]):
-                The request object. Request message for GetFolder.
+                The request object. Request message for GetFolder. This
+                operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             name (:class:`str`):
                 Required. Name of the folder. Format:
                 ``projects/{project}/buckets/{bucket}/folders/{folder}``
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -534,15 +560,19 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.storage_control_v2.types.Folder:
-                A folder.
+                A folder resource. This resource can
+                only exist in a hierarchical namespace
+                enabled bucket. Hierarchical namespace
+                buckets are in allowlist preview.
+
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
@@ -600,15 +630,17 @@
         request: Optional[Union[storage_control.ListFoldersRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListFoldersAsyncPager:
-        r"""Retrieves a list of folders for a given bucket.
+        r"""Retrieves a list of folders. This operation is only
+        applicable to a hierarchical namespace enabled bucket.
+        Hierarchical namespace buckets are in allowlist preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -631,18 +663,23 @@
 
                 # Handle the response
                 async for response in page_result:
                     print(response)
 
         Args:
             request (Optional[Union[google.cloud.storage_control_v2.types.ListFoldersRequest, dict]]):
-                The request object. Request message for ListFolders.
+                The request object. Request message for ListFolders. This
+                operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             parent (:class:`str`):
                 Required. Name of the bucket in which
-                to look for folders.
+                to look for folders. The bucket must be
+                a hierarchical namespace enabled bucket.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -725,17 +762,20 @@
         *,
         name: Optional[str] = None,
         destination_folder_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation_async.AsyncOperation:
-        r"""Renames a source folder to a destination folder.
-        During a rename, the source and destination folders are
-        locked until the long running operation completes.
+        r"""Renames a source folder to a destination folder. This
+        operation is only applicable to a hierarchical namespace
+        enabled bucket. During a rename, the source and
+        destination folders are locked until the long running
+        operation completes.
+        Hierarchical namespace buckets are in allowlist preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -763,14 +803,18 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.storage_control_v2.types.RenameFolderRequest, dict]]):
                 The request object. Request message for RenameFolder.
+                This operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             name (:class:`str`):
                 Required. Name of the source folder being renamed.
                 Format:
                 ``projects/{project}/buckets/{bucket}/folders/{folder}``
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -786,17 +830,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation_async.AsyncOperation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be
-                :class:`google.cloud.storage_control_v2.types.Folder` A
-                folder.
+                The result type for the operation will be :class:`google.cloud.storage_control_v2.types.Folder` A folder resource. This resource can only exist in a hierarchical namespace
+                   enabled bucket. Hierarchical namespace buckets are in
+                   allowlist preview.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, destination_folder_id])
         if request is not None and has_flattened_params:
```

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/client.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -721,15 +721,17 @@
         parent: Optional[str] = None,
         folder: Optional[storage_control.Folder] = None,
         folder_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> storage_control.Folder:
-        r"""Creates a new folder.
+        r"""Creates a new folder. This operation is only
+        applicable to a hierarchical namespace enabled bucket.
+        Hierarchical namespace buckets are in allowlist preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -753,17 +755,23 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.storage_control_v2.types.CreateFolderRequest, dict]):
                 The request object. Request message for CreateFolder.
+                This operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             parent (str):
                 Required. Name of the bucket in which
-                the folder will reside.
+                the folder will reside. The bucket must
+                be a hierarchical namespace enabled
+                bucket.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             folder (google.cloud.storage_control_v2.types.Folder):
                 Required. Properties of the new folder being created.
                 The bucket and name of the folder are specified in the
@@ -788,15 +796,19 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.storage_control_v2.types.Folder:
-                A folder.
+                A folder resource. This resource can
+                only exist in a hierarchical namespace
+                enabled bucket. Hierarchical namespace
+                buckets are in allowlist preview.
+
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, folder, folder_id])
         if request is not None and has_flattened_params:
             raise ValueError(
@@ -857,15 +869,18 @@
         request: Optional[Union[storage_control.DeleteFolderRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
-        r"""Permanently deletes an empty folder.
+        r"""Permanently deletes an empty folder. This operation
+        is only applicable to a hierarchical namespace enabled
+        bucket. Hierarchical namespace buckets are in allowlist
+        preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -885,14 +900,18 @@
 
                 # Make the request
                 client.delete_folder(request=request)
 
         Args:
             request (Union[google.cloud.storage_control_v2.types.DeleteFolderRequest, dict]):
                 The request object. Request message for DeleteFolder.
+                This operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             name (str):
                 Required. Name of the folder. Format:
                 ``projects/{project}/buckets/{bucket}/folders/{folder}``
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -960,15 +979,18 @@
         request: Optional[Union[storage_control.GetFolderRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> storage_control.Folder:
-        r"""Returns metadata for the specified folder.
+        r"""Returns metadata for the specified folder. This
+        operation is only applicable to a hierarchical namespace
+        enabled bucket. Hierarchical namespace buckets are in
+        allowlist preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -990,15 +1012,19 @@
                 response = client.get_folder(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.storage_control_v2.types.GetFolderRequest, dict]):
-                The request object. Request message for GetFolder.
+                The request object. Request message for GetFolder. This
+                operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             name (str):
                 Required. Name of the folder. Format:
                 ``projects/{project}/buckets/{bucket}/folders/{folder}``
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
@@ -1006,15 +1032,19 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.cloud.storage_control_v2.types.Folder:
-                A folder.
+                A folder resource. This resource can
+                only exist in a hierarchical namespace
+                enabled bucket. Hierarchical namespace
+                buckets are in allowlist preview.
+
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
@@ -1073,15 +1103,17 @@
         request: Optional[Union[storage_control.ListFoldersRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListFoldersPager:
-        r"""Retrieves a list of folders for a given bucket.
+        r"""Retrieves a list of folders. This operation is only
+        applicable to a hierarchical namespace enabled bucket.
+        Hierarchical namespace buckets are in allowlist preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1104,18 +1136,23 @@
 
                 # Handle the response
                 for response in page_result:
                     print(response)
 
         Args:
             request (Union[google.cloud.storage_control_v2.types.ListFoldersRequest, dict]):
-                The request object. Request message for ListFolders.
+                The request object. Request message for ListFolders. This
+                operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             parent (str):
                 Required. Name of the bucket in which
-                to look for folders.
+                to look for folders. The bucket must be
+                a hierarchical namespace enabled bucket.
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1197,17 +1234,20 @@
         *,
         name: Optional[str] = None,
         destination_folder_id: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""Renames a source folder to a destination folder.
-        During a rename, the source and destination folders are
-        locked until the long running operation completes.
+        r"""Renames a source folder to a destination folder. This
+        operation is only applicable to a hierarchical namespace
+        enabled bucket. During a rename, the source and
+        destination folders are locked until the long running
+        operation completes.
+        Hierarchical namespace buckets are in allowlist preview.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1235,14 +1275,18 @@
 
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.cloud.storage_control_v2.types.RenameFolderRequest, dict]):
                 The request object. Request message for RenameFolder.
+                This operation is only applicable to a
+                hierarchical namespace enabled bucket.
+                Hierarchical namespace buckets are in
+                allowlist preview.
             name (str):
                 Required. Name of the source folder being renamed.
                 Format:
                 ``projects/{project}/buckets/{bucket}/folders/{folder}``
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
@@ -1258,17 +1302,17 @@
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
-                The result type for the operation will be
-                :class:`google.cloud.storage_control_v2.types.Folder` A
-                folder.
+                The result type for the operation will be :class:`google.cloud.storage_control_v2.types.Folder` A folder resource. This resource can only exist in a hierarchical namespace
+                   enabled bucket. Hierarchical namespace buckets are in
+                   allowlist preview.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([name, destination_folder_id])
         if request is not None and has_flattened_params:
```

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/pagers.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/base.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,15 +248,17 @@
 
     @property
     def create_folder(
         self,
     ) -> Callable[[storage_control.CreateFolderRequest], storage_control.Folder]:
         r"""Return a callable for the create folder method over gRPC.
 
-        Creates a new folder.
+        Creates a new folder. This operation is only
+        applicable to a hierarchical namespace enabled bucket.
+        Hierarchical namespace buckets are in allowlist preview.
 
         Returns:
             Callable[[~.CreateFolderRequest],
                     ~.Folder]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -274,15 +276,18 @@
 
     @property
     def delete_folder(
         self,
     ) -> Callable[[storage_control.DeleteFolderRequest], empty_pb2.Empty]:
         r"""Return a callable for the delete folder method over gRPC.
 
-        Permanently deletes an empty folder.
+        Permanently deletes an empty folder. This operation
+        is only applicable to a hierarchical namespace enabled
+        bucket. Hierarchical namespace buckets are in allowlist
+        preview.
 
         Returns:
             Callable[[~.DeleteFolderRequest],
                     ~.Empty]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -300,15 +305,18 @@
 
     @property
     def get_folder(
         self,
     ) -> Callable[[storage_control.GetFolderRequest], storage_control.Folder]:
         r"""Return a callable for the get folder method over gRPC.
 
-        Returns metadata for the specified folder.
+        Returns metadata for the specified folder. This
+        operation is only applicable to a hierarchical namespace
+        enabled bucket. Hierarchical namespace buckets are in
+        allowlist preview.
 
         Returns:
             Callable[[~.GetFolderRequest],
                     ~.Folder]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -328,15 +336,17 @@
     def list_folders(
         self,
     ) -> Callable[
         [storage_control.ListFoldersRequest], storage_control.ListFoldersResponse
     ]:
         r"""Return a callable for the list folders method over gRPC.
 
-        Retrieves a list of folders for a given bucket.
+        Retrieves a list of folders. This operation is only
+        applicable to a hierarchical namespace enabled bucket.
+        Hierarchical namespace buckets are in allowlist preview.
 
         Returns:
             Callable[[~.ListFoldersRequest],
                     ~.ListFoldersResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -354,17 +364,20 @@
 
     @property
     def rename_folder(
         self,
     ) -> Callable[[storage_control.RenameFolderRequest], operations_pb2.Operation]:
         r"""Return a callable for the rename folder method over gRPC.
 
-        Renames a source folder to a destination folder.
-        During a rename, the source and destination folders are
-        locked until the long running operation completes.
+        Renames a source folder to a destination folder. This
+        operation is only applicable to a hierarchical namespace
+        enabled bucket. During a rename, the source and
+        destination folders are locked until the long running
+        operation completes.
+        Hierarchical namespace buckets are in allowlist preview.
 
         Returns:
             Callable[[~.RenameFolderRequest],
                     ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -255,15 +255,17 @@
     def create_folder(
         self,
     ) -> Callable[
         [storage_control.CreateFolderRequest], Awaitable[storage_control.Folder]
     ]:
         r"""Return a callable for the create folder method over gRPC.
 
-        Creates a new folder.
+        Creates a new folder. This operation is only
+        applicable to a hierarchical namespace enabled bucket.
+        Hierarchical namespace buckets are in allowlist preview.
 
         Returns:
             Callable[[~.CreateFolderRequest],
                     Awaitable[~.Folder]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -281,15 +283,18 @@
 
     @property
     def delete_folder(
         self,
     ) -> Callable[[storage_control.DeleteFolderRequest], Awaitable[empty_pb2.Empty]]:
         r"""Return a callable for the delete folder method over gRPC.
 
-        Permanently deletes an empty folder.
+        Permanently deletes an empty folder. This operation
+        is only applicable to a hierarchical namespace enabled
+        bucket. Hierarchical namespace buckets are in allowlist
+        preview.
 
         Returns:
             Callable[[~.DeleteFolderRequest],
                     Awaitable[~.Empty]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -309,15 +314,18 @@
     def get_folder(
         self,
     ) -> Callable[
         [storage_control.GetFolderRequest], Awaitable[storage_control.Folder]
     ]:
         r"""Return a callable for the get folder method over gRPC.
 
-        Returns metadata for the specified folder.
+        Returns metadata for the specified folder. This
+        operation is only applicable to a hierarchical namespace
+        enabled bucket. Hierarchical namespace buckets are in
+        allowlist preview.
 
         Returns:
             Callable[[~.GetFolderRequest],
                     Awaitable[~.Folder]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -338,15 +346,17 @@
         self,
     ) -> Callable[
         [storage_control.ListFoldersRequest],
         Awaitable[storage_control.ListFoldersResponse],
     ]:
         r"""Return a callable for the list folders method over gRPC.
 
-        Retrieves a list of folders for a given bucket.
+        Retrieves a list of folders. This operation is only
+        applicable to a hierarchical namespace enabled bucket.
+        Hierarchical namespace buckets are in allowlist preview.
 
         Returns:
             Callable[[~.ListFoldersRequest],
                     Awaitable[~.ListFoldersResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -366,17 +376,20 @@
     def rename_folder(
         self,
     ) -> Callable[
         [storage_control.RenameFolderRequest], Awaitable[operations_pb2.Operation]
     ]:
         r"""Return a callable for the rename folder method over gRPC.
 
-        Renames a source folder to a destination folder.
-        During a rename, the source and destination folders are
-        locked until the long running operation completes.
+        Renames a source folder to a destination folder. This
+        operation is only applicable to a hierarchical namespace
+        enabled bucket. During a rename, the source and
+        destination folders are locked until the long running
+        operation completes.
+        Hierarchical namespace buckets are in allowlist preview.
 
         Returns:
             Callable[[~.RenameFolderRequest],
                     Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/__init__.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/storage_control.py` & `google-cloud-storage-control-0.1.3/google/cloud/storage_control_v2/types/storage_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,17 @@
     operation: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class Folder(proto.Message):
-    r"""A folder.
+    r"""A folder resource. This resource can only exist in a
+    hierarchical namespace enabled bucket.
+    Hierarchical namespace buckets are in allowlist preview.
 
     Attributes:
         name (str):
             Identifier. The name of this folder. Format:
             ``projects/{project}/buckets/{bucket}/folders/{folder}``
         metageneration (int):
             Output only. The version of the metadata for
@@ -108,15 +110,18 @@
         proto.MESSAGE,
         number=7,
         message="PendingRenameInfo",
     )
 
 
 class GetFolderRequest(proto.Message):
-    r"""Request message for GetFolder.
+    r"""Request message for GetFolder. This operation is only
+    applicable to a hierarchical namespace enabled bucket.
+    Hierarchical namespace buckets are in allowlist preview.
+
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             Required. Name of the folder. Format:
             ``projects/{project}/buckets/{bucket}/folders/{folder}``
@@ -155,20 +160,23 @@
     request_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class CreateFolderRequest(proto.Message):
-    r"""Request message for CreateFolder.
+    r"""Request message for CreateFolder. This operation is only
+    applicable to a hierarchical namespace enabled bucket.
+    Hierarchical namespace buckets are in allowlist preview.
 
     Attributes:
         parent (str):
             Required. Name of the bucket in which the
-            folder will reside.
+            folder will reside. The bucket must be a
+            hierarchical namespace enabled bucket.
         folder (google.cloud.storage_control_v2.types.Folder):
             Required. Properties of the new folder being created. The
             bucket and name of the folder are specified in the parent
             and folder_id fields, respectively. Populating those fields
             in ``folder`` will result in an error.
         folder_id (str):
             Required. The full name of a folder, including all its
@@ -177,18 +185,17 @@
             the folder_id of "books/biographies/" would create a new
             "biographies/" folder under the "books/" folder.
         recursive (bool):
             Optional. If true, parent folder doesn't have
             to be present and all missing ancestor folders
             will be created atomically.
         request_id (str):
-            Optional. A unique identifier for this request. UUID is the
-            recommended format, but other formats are still accepted.
-            This request is only idempotent if a ``request_id`` is
-            provided.
+            Optional. A unique identifier for this
+            request. UUID is the recommended format, but
+            other formats are still accepted.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     folder: "Folder" = proto.Field(
@@ -207,15 +214,18 @@
     request_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class DeleteFolderRequest(proto.Message):
-    r"""Request message for DeleteFolder.
+    r"""Request message for DeleteFolder. This operation is only
+    applicable to a hierarchical namespace enabled bucket.
+    Hierarchical namespace buckets are in allowlist preview.
+
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             Required. Name of the folder. Format:
             ``projects/{project}/buckets/{bucket}/folders/{folder}``
@@ -228,18 +238,17 @@
         if_metageneration_not_match (int):
             Makes the operation only succeed conditional
             on whether the folder's current metageneration
             does not match the given value.
 
             This field is a member of `oneof`_ ``_if_metageneration_not_match``.
         request_id (str):
-            Optional. A unique identifier for this request. UUID is the
-            recommended format, but other formats are still accepted.
-            This request is only idempotent if a ``request_id`` is
-            provided.
+            Optional. A unique identifier for this
+            request. UUID is the recommended format, but
+            other formats are still accepted.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=6,
     )
     if_metageneration_match: int = proto.Field(
@@ -255,20 +264,23 @@
     request_id: str = proto.Field(
         proto.STRING,
         number=5,
     )
 
 
 class ListFoldersRequest(proto.Message):
-    r"""Request message for ListFolders.
+    r"""Request message for ListFolders. This operation is only
+    applicable to a hierarchical namespace enabled bucket.
+    Hierarchical namespace buckets are in allowlist preview.
 
     Attributes:
         parent (str):
             Required. Name of the bucket in which to look
-            for folders.
+            for folders. The bucket must be a hierarchical
+            namespace enabled bucket.
         page_size (int):
             Optional. Maximum number of folders to return
             in a single response. The service will use this
             parameter or 1,000 items, whichever is smaller.
         page_token (str):
             Optional. A previously-returned page token
             representing part of the larger set of results
@@ -361,15 +373,18 @@
     next_page_token: str = proto.Field(
         proto.STRING,
         number=2,
     )
 
 
 class RenameFolderRequest(proto.Message):
-    r"""Request message for RenameFolder.
+    r"""Request message for RenameFolder. This operation is only
+    applicable to a hierarchical namespace enabled bucket.
+    Hierarchical namespace buckets are in allowlist preview.
+
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
             Required. Name of the source folder being renamed. Format:
             ``projects/{project}/buckets/{bucket}/folders/{folder}``
```

### Comparing `google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/PKG-INFO` & `google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-control
-Version: 0.1.2
+Version: 0.1.3
 Summary: Google Cloud Storage Control API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/SOURCES.txt` & `google-cloud-storage-control-0.1.3/google_cloud_storage_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/setup.py` & `google-cloud-storage-control-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/tests/__init__.py` & `google-cloud-storage-control-0.1.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/tests/unit/__init__.py` & `google-cloud-storage-control-0.1.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/tests/unit/gapic/__init__.py` & `google-cloud-storage-control-0.1.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/__init__.py` & `google-cloud-storage-control-0.1.3/tests/unit/gapic/storage_control_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/test_storage_control.py` & `google-cloud-storage-control-0.1.3/tests/unit/gapic/storage_control_v2/test_storage_control.py`

 * *Files identical despite different names*

