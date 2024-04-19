# Comparing `tmp/sfmanager-0.0.8.tar.gz` & `tmp/sfmanager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfmanager-0.0.8.tar", last modified: Thu Apr 18 08:07:23 2024, max compression
+gzip compressed data, was "sfmanager-0.0.9.tar", last modified: Thu Apr 18 15:02:02 2024, max compression
```

## Comparing `sfmanager-0.0.8.tar` & `sfmanager-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 08:07:23.400433 sfmanager-0.0.8/
--rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 08:07:23.400433 sfmanager-0.0.8/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      365 2024-04-18 05:45:03.000000 sfmanager-0.0.8/README.md
--rw-rw-r--   0 grand     (1000) grand     (1000)       38 2024-04-18 08:07:23.400433 sfmanager-0.0.8/setup.cfg
--rw-rw-r--   0 grand     (1000) grand     (1000)      800 2024-04-18 08:07:19.000000 sfmanager-0.0.8/setup.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 08:07:23.396435 sfmanager-0.0.8/sfmanager/
--rw-rw-r--   0 grand     (1000) grand     (1000)       73 2024-04-18 06:32:48.000000 sfmanager-0.0.8/sfmanager/__init__.py
--rw-rw-r--   0 grand     (1000) grand     (1000)     1623 2024-04-18 08:06:12.000000 sfmanager-0.0.8/sfmanager/app.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 08:07:23.396435 sfmanager-0.0.8/sfmanager.egg-info/
--rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      231 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)        1 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       17 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/requires.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       10 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/top_level.txt
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 15:02:02.656167 sfmanager-0.0.9/
+-rw-rw-r--   0 grand     (1000) grand     (1000)      887 2024-04-18 15:02:02.656167 sfmanager-0.0.9/PKG-INFO
+-rw-rw-r--   0 grand     (1000) grand     (1000)      365 2024-04-18 05:45:03.000000 sfmanager-0.0.9/README.md
+-rw-rw-r--   0 grand     (1000) grand     (1000)       38 2024-04-18 15:02:02.660167 sfmanager-0.0.9/setup.cfg
+-rw-rw-r--   0 grand     (1000) grand     (1000)      822 2024-04-18 10:08:46.000000 sfmanager-0.0.9/setup.py
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 15:02:02.652167 sfmanager-0.0.9/sfmanager/
+-rw-rw-r--   0 grand     (1000) grand     (1000)       73 2024-04-18 06:32:48.000000 sfmanager-0.0.9/sfmanager/__init__.py
+-rw-rw-r--   0 grand     (1000) grand     (1000)     3392 2024-04-18 14:37:28.000000 sfmanager-0.0.9/sfmanager/app.py
+-rw-rw-r--   0 grand     (1000) grand     (1000)       75 2024-04-18 14:38:11.000000 sfmanager-0.0.9/sfmanager/test.py
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 15:02:02.656167 sfmanager-0.0.9/sfmanager.egg-info/
+-rw-rw-r--   0 grand     (1000) grand     (1000)      887 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 grand     (1000) grand     (1000)      249 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)        1 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)       31 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/requires.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)       10 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/top_level.txt
```

### Comparing `sfmanager-0.0.8/PKG-INFO` & `sfmanager-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: sfmanager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Super filemanager for python
 Home-page: https://t.me/grand_studios
 Author: GrandTheBest
 Author-email: grandinfo-cm@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/grandescobar/sfmanager
-Keywords: tensor
+Keywords: filemanager
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `sfmanager-0.0.8/setup.py` & `sfmanager-0.0.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='sfmanager',
-    version='0.0.8',
+    version='0.0.9',
     author='GrandTheBest',
     author_email='grandinfo-cm@gmail.com',
     description='Super filemanager for python',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/grand_studios',
     packages=find_packages(),
-    install_requires=['requests>=2.25.1'],
+    install_requires=['requests>=2.25.1', 'Pillow>=9.0.1'],
     classifiers=[
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
-    keywords='tensor',
+    keywords='filemanager',
     project_urls={
         'GitHub': 'https://github.com/grandescobar/sfmanager'
     },
     python_requires='>=3.6'
     )
```

### Comparing `sfmanager-0.0.8/sfmanager/app.py` & `sfmanager-0.0.9/sfmanager/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,145 @@
+from PIL import Image
+import os
+import shutil
+
 class FileManager:
 	filename = None
 	level = None
 
+	# Initialization func
+
 	def __init__(self, filename, level):
-		self.filename = str(filename)
-		self.level = int(level)
+		if level > 0 and level < 6:
+			self.filename = str(filename)
+			self.level = int(level)
+		else:
+			print("Invalid access level! Allowed only 1-6 access levels")
+
+	# Funcs for work with text files(.txt)
+
+	# Read line in text file
 
 	def readline(self):
 		if self.level >= 1:
 			try:
 				with open(f"{self.filename}", "r") as f:
 					raw = f.readline()
 				return raw
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 1")
 
+	# Read lines in text file (as array)
+
 	def readlines(self):
 		if self.level >= 1:
 			try:
 				with open(f"{self.filename}", "r") as f:
 					raw = f.readlines()
 				return raw
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 1")
+
+	# Set content in text file
+
 	def set(self, text):
 		if self.level >= 3:
 			try:
 				with open(f"{self.filename}", "w") as f:
 					f.write(text)
 					return 1
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 3")
-	def add(self, text):
+
+	# Add content in text file with separator(default separator is empty)
+
+	def add(self, text, sep=""):
 		if self.level >= 2:
 			try:
 				with open(f"{self.filename}", "r") as f:
 					old = f.read()
 				with open(f"{self.filename}", "w") as f:
-					f.write(old + " " + text)
+					f.write(old + sep + text)
 					return 1
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 2")
+
+	# Replace certain content in text file
+
 	def replace(self, target, text):
 		if self.level >= 3:
 			try:
 				with open(f"{self.filename}", "r") as f:
 					data = f.read().replace(target, text)
 				with open(f"{self.filename}", "w") as f:
 					f.write(data)
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
-			print(f"Low access level! {self.level}, but need 3")
+			print(f"Low access level! {self.level}, but need 3")
+
+	# Funcs for work with images(.png, .jpg, .jpeg, etc.)
+
+	# Open image
+
+	def openImage(self):
+		if self.level >= 1:
+			try:
+				Image.open(f"{self.filename}").show()
+			except FileNotFoundError:
+				print("Something went wrong...")
+		else:
+			print(f"Low access level! {self.level}, but need 1")
+
+	# Funcs for general work with files
+
+	# Rename file(from self.filename to name)
+
+	def rename(self, name):
+		if self.level >= 4:
+			try:
+				os.rename(f"{self.filename}", name)
+			except FileNotFoundError:
+				print("Something went wrong...")
+		else:
+			print(f"Low access level! {self.level}, but need 4")
+
+	# Delete file
+
+	def delete(self):
+		if self.level == 5:
+			try:
+				os.remove(f"{self.filename}")
+			except FileNotFoundError:
+				print("Something went wrong...")
+		else:
+			print(f"Low access level! {self.level}, but need 5")
+
+	# Copy file
+
+	def copy(self, directory):
+		if self.level >= 4:
+			try:
+				shutil.copy2(f"{self.filename}", f"{directory}")
+			except FileNotFoundError:
+				print("Something went wrong...")
+		else:
+			print(f"Low access level! {self.level}, but need 4")
+
+	# Move file
+
+	def move(self, dst):
+		if self.level >= 4:
+			try:
+				shutil.move(f"{self.filename}", f"{dst}")
+			except FileNotFoundError:
+				print("Something went wrong...")
+		else:
+			print(f"Low access level! {self.level}, but need 4")
```

### Comparing `sfmanager-0.0.8/sfmanager.egg-info/PKG-INFO` & `sfmanager-0.0.9/sfmanager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: sfmanager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Super filemanager for python
 Home-page: https://t.me/grand_studios
 Author: GrandTheBest
 Author-email: grandinfo-cm@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/grandescobar/sfmanager
-Keywords: tensor
+Keywords: filemanager
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

