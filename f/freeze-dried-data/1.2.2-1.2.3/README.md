# Comparing `tmp/freeze_dried_data-1.2.2.tar.gz` & `tmp/freeze_dried_data-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-1.2.2.tar", last modified: Tue Apr 16 21:50:04 2024, max compression
+gzip compressed data, was "freeze_dried_data-1.2.3.tar", last modified: Fri Apr 19 18:02:04 2024, max compression
```

## Comparing `freeze_dried_data-1.2.2.tar` & `freeze_dried_data-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:04.170532 freeze_dried_data-1.2.2/
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7523 2024-04-16 21:50:04.170532 freeze_dried_data-1.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6657 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:04.166532 freeze_dried_data-1.2.2/freeze_dried_data/
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/freeze_dried_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10858 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/freeze_dried_data/freeze_dried_data.py
--rw-r--r--   0 root         (0) root         (0)     7889 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/freeze_dried_data/test_freeze_dried_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:04.166532 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7523 2024-04-16 21:50:04.000000 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      303 2024-04-16 21:50:04.000000 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 21:50:04.000000 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-16 21:50:04.000000 freeze_dried_data-1.2.2/freeze_dried_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 21:50:04.170532 freeze_dried_data-1.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-16 21:49:49.000000 freeze_dried_data-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:04.705601 freeze_dried_data-1.2.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1072 2024-04-19 17:43:53.000000 freeze_dried_data-1.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7523 2024-04-19 18:02:04.705601 freeze_dried_data-1.2.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6657 2024-04-19 17:43:53.000000 freeze_dried_data-1.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:04.705601 freeze_dried_data-1.2.3/freeze_dried_data/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-19 17:43:53.000000 freeze_dried_data-1.2.3/freeze_dried_data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11900 2024-04-19 17:54:08.000000 freeze_dried_data-1.2.3/freeze_dried_data/freeze_dried_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     7889 2024-04-19 17:43:53.000000 freeze_dried_data-1.2.3/freeze_dried_data/test_freeze_dried_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 18:02:04.705601 freeze_dried_data-1.2.3/freeze_dried_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7523 2024-04-19 18:02:04.000000 freeze_dried_data-1.2.3/freeze_dried_data.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      303 2024-04-19 18:02:04.000000 freeze_dried_data-1.2.3/freeze_dried_data.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-19 18:02:04.000000 freeze_dried_data-1.2.3/freeze_dried_data.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-19 18:02:04.000000 freeze_dried_data-1.2.3/freeze_dried_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 18:02:04.705601 freeze_dried_data-1.2.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1125 2024-04-19 18:02:02.000000 freeze_dried_data-1.2.3/setup.py
```

### Comparing `freeze_dried_data-1.2.2/LICENSE` & `freeze_dried_data-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-1.2.2/PKG-INFO` & `freeze_dried_data-1.2.3/freeze_dried_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: freeze_dried_data
-Version: 1.2.2
+Name: freeze-dried-data
+Version: 1.2.3
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-1.2.2/README.md` & `freeze_dried_data-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-1.2.2/freeze_dried_data/freeze_dried_data.py` & `freeze_dried_data-1.2.3/freeze_dried_data/freeze_dried_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,14 +209,44 @@
         :param key: The key of the item to retrieve.
         :return: The item.
         """
         start, data_len = self.index[key]
         self.file.seek(start)
         data = self.file.read(data_len)
         return pkl.loads(self.decompressor(data))
+    
+    def git_raw_bytes(self, key: Any) -> bytes:
+        """
+        Retrieve an item's bytes by key.
+
+        :param key: The key of the item to retrieve.
+        :return: The item in byte form.
+        """
+        start, data_len = self.index[key]
+        self.file.seek(start)
+        data = self.file.read(data_len)
+        return data
+    
+    def write_raw_bits(self, key: Any, data: bytes) -> None:
+        """
+        Add raw bits to the file with a specific key.
+
+        :param key: The key under which the item will be stored.
+        :param data: The item to store.
+
+        """
+        if key in self.index:
+            raise ValueError("trying to re-insert a record with key,", key, "FDD cannot re-assign items.")
+        if self.mode == 'read_mode':
+            raise ValueError("trying to insert into a read-mode FDD. This is not supported.", "key=", key)
+        
+        data_len = len(data)
+        self.file.write(data)
+        self.index[key] = (self.current_offset, data_len)
+        self.current_offset += data_len
 
     def _after_fork(self) -> None:
         """
         Reopen the file after a fork to prevent race conditions
         if the object is cloned to another process. For example when using PyTorch DataLoader.
         """
         # print("FDD: Reopening file after fork.")
```

### Comparing `freeze_dried_data-1.2.2/freeze_dried_data/test_freeze_dried_data.py` & `freeze_dried_data-1.2.3/freeze_dried_data/test_freeze_dried_data.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-1.2.2/freeze_dried_data.egg-info/PKG-INFO` & `freeze_dried_data-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: freeze-dried-data
-Version: 1.2.2
+Name: freeze_dried_data
+Version: 1.2.3
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-1.2.2/setup.py` & `freeze_dried_data-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='freeze_dried_data',
-    version='1.2.2',
+    version='1.2.3',
     description='A simple format for machine learning datasets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/tstandley/freeze_dried_data',
     author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
```

