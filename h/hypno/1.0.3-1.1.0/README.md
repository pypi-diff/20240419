# Comparing `tmp/hypno-1.0.3.tar.gz` & `tmp/hypno-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypno-1.0.3.tar", last modified: Tue Jul 11 22:45:38 2023, max compression
+gzip compressed data, was "hypno-1.1.0.tar", last modified: Fri Apr 19 11:25:52 2024, max compression
```

## Comparing `hypno-1.0.3.tar` & `hypno-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 22:45:38.686725 hypno-1.0.3/
--rw-rw-rw-   0        0        0     1092 2023-07-11 22:44:13.000000 hypno-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       29 2023-07-11 22:44:13.000000 hypno-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2711 2023-07-11 22:45:38.686725 hypno-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1798 2023-07-11 22:44:13.000000 hypno-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 22:45:38.678343 hypno-1.0.3/hypno/
--rw-rw-rw-   0        0        0       50 2023-07-11 22:44:13.000000 hypno-1.0.3/hypno/__init__.py
--rw-rw-rw-   0        0        0      675 2023-07-11 22:44:13.000000 hypno-1.0.3/hypno/__main__.py
--rw-rw-rw-   0        0        0     2636 2023-07-11 22:44:13.000000 hypno-1.0.3/hypno/api.py
--rw-rw-rw-   0        0        0     1063 2023-07-11 22:44:13.000000 hypno-1.0.3/hypno/injection.c
-drwxrwxrwx   0        0        0        0 2023-07-11 22:45:38.684628 hypno-1.0.3/hypno.egg-info/
--rw-rw-rw-   0        0        0     2711 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-11 22:44:58.000000 hypno-1.0.3/hypno.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      989 2023-07-11 22:45:38.687766 hypno-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-07-11 22:44:13.000000 hypno-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 22:45:38.685665 hypno-1.0.3/tests/
--rw-rw-rw-   0        0        0     1114 2023-07-11 22:44:13.000000 hypno-1.0.3/tests/test_hypno.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:25:52.178293 hypno-1.1.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-19 11:24:46.000000 hypno-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       29 2024-04-19 11:24:46.000000 hypno-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2752 2024-04-19 11:25:52.178293 hypno-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1856 2024-04-19 11:24:46.000000 hypno-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 11:25:52.173515 hypno-1.1.0/hypno/
+-rw-rw-rw-   0        0        0       50 2024-04-19 11:24:46.000000 hypno-1.1.0/hypno/__init__.py
+-rw-rw-rw-   0        0        0      675 2024-04-19 11:24:46.000000 hypno-1.1.0/hypno/__main__.py
+-rw-rw-rw-   0        0        0     2250 2024-04-19 11:24:46.000000 hypno-1.1.0/hypno/api.py
+-rw-rw-rw-   0        0        0      987 2024-04-19 11:24:46.000000 hypno-1.1.0/hypno/injection.c
+drwxrwxrwx   0        0        0        0 2024-04-19 11:25:52.178293 hypno-1.1.0/hypno.egg-info/
+-rw-rw-rw-   0        0        0     2752 2024-04-19 11:25:52.000000 hypno-1.1.0/hypno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-19 11:25:52.000000 hypno-1.1.0/hypno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:25:52.000000 hypno-1.1.0/hypno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-19 11:25:52.000000 hypno-1.1.0/hypno.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 11:25:25.000000 hypno-1.1.0/hypno.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2024-04-19 11:25:52.000000 hypno-1.1.0/hypno.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-19 11:25:52.000000 hypno-1.1.0/hypno.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      949 2024-04-19 11:25:52.179374 hypno-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      203 2024-04-19 11:24:46.000000 hypno-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:25:52.177194 hypno-1.1.0/tests/
+-rw-rw-rw-   0        0        0     2490 2024-04-19 11:24:46.000000 hypno-1.1.0/tests/test_hypno.py
```

### Comparing `hypno-1.0.3/LICENSE.txt` & `hypno-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hypno-1.0.3/PKG-INFO` & `hypno-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: hypno
-Version: 1.0.3
+Version: 1.1.0
 Summary: A tool/library allowing to inject python code into a running python process.
 Home-page: https://github.com/kmaork/hypno
 Author: Maor Kleinberger
 Author-email: kmaork@gmail.com
 Keywords: injection library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
+Requires-Dist: pyinjector>=0.1.2
 
 # Hypno
 
 [![PyPI version](https://badge.fury.io/py/hypno.svg)](https://badge.fury.io/py/hypno)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/hypno.svg)](https://pypi.python.org/pypi/hypno/)
 [![GitHub license](https://img.shields.io/github/license/kmaork/hypno)](https://github.com/kmaork/hypno/blob/master/LICENSE.txt)
 [![Tests (GitHub Actions)](https://github.com/kmaork/hypno/workflows/Tests/badge.svg)](https://github.com/kmaork/hypno)
@@ -50,15 +50,15 @@
 from hypno import inject_py
 
 inject_py(pid, python_code)
 ```
 
 #### Example
 This example runs a python program that prints its pid, and then attaches to the newly created process and
-injects it with another print statement using hypno.
+injects it with another print statement using hypno. Mac users will need to use `sudo` for the second command.
 ```shell script
 python -c "import os, time; print('Hello from', os.getpid()); time.sleep(0.5)" &\
 hypno $! "import os; print('Hello again from', os.getpid())"
 ```
 
 ### Security
 Hypno briefly generates a temporary file containing the requested python code.
```

### Comparing `hypno-1.0.3/README.md` & `hypno-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from hypno import inject_py
 
 inject_py(pid, python_code)
 ```
 
 #### Example
 This example runs a python program that prints its pid, and then attaches to the newly created process and
-injects it with another print statement using hypno.
+injects it with another print statement using hypno. Mac users will need to use `sudo` for the second command.
 ```shell script
 python -c "import os, time; print('Hello from', os.getpid()); time.sleep(0.5)" &\
 hypno $! "import os; print('Hello again from', os.getpid())"
 ```
 
 ### Security
 Hypno briefly generates a temporary file containing the requested python code.
```

### Comparing `hypno-1.0.3/hypno/__main__.py` & `hypno-1.1.0/hypno/__main__.py`

 * *Files identical despite different names*

### Comparing `hypno-1.0.3/hypno/api.py` & `hypno-1.1.0/hypno/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,18 +41,11 @@
         with NamedTemporaryFile(prefix='hypno', suffix=INJECTION_LIB_PATH.suffix, delete=False) as temp:
             path = Path(temp.name)
             temp.write(lib[:code_addr])
             temp.write(python_code)
             temp.write(b'\0')
             temp.write(lib[code_addr + len(python_code) + 1:])
         path.chmod(permissions)
-        try:
-            inject(pid, str(temp.name))
-        except InjectorError as e:
-            # On Windows we are failing the load on purpose so the library will be immediately unloaded
-            if not WINDOWS or e.ret_val != -5 or e.error_str != \
-                    "LoadLibrary in the target process failed: " \
-                    "A dynamic link library (DLL) initialization routine failed.":
-                raise
+        inject(pid, str(temp.name), uninject=True)
     finally:
         if path is not None and path.exists():
             path.unlink()
```

### Comparing `hypno-1.0.3/hypno/injection.c` & `hypno-1.1.0/hypno/injection.c`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 #ifdef _WIN32
     #include <windows.h>
 
     BOOL WINAPI DllMain(HINSTANCE hinstDLL, DWORD fdwReason, LPVOID lpReserved) {
         switch( fdwReason ) {
             case DLL_PROCESS_ATTACH:
                 run_python_code();
-                // "Failing" so the library is immediately unloaded
-                return FALSE;
+                break;
         }
         return TRUE;
     }
 #else
     __attribute__((constructor))
     static void init(void) {
         run_python_code();
```

### Comparing `hypno-1.0.3/hypno.egg-info/PKG-INFO` & `hypno-1.1.0/hypno.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: hypno
-Version: 1.0.3
+Version: 1.1.0
 Summary: A tool/library allowing to inject python code into a running python process.
 Home-page: https://github.com/kmaork/hypno
 Author: Maor Kleinberger
 Author-email: kmaork@gmail.com
 Keywords: injection library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
+Requires-Dist: pyinjector>=0.1.2
 
 # Hypno
 
 [![PyPI version](https://badge.fury.io/py/hypno.svg)](https://badge.fury.io/py/hypno)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/hypno.svg)](https://pypi.python.org/pypi/hypno/)
 [![GitHub license](https://img.shields.io/github/license/kmaork/hypno)](https://github.com/kmaork/hypno/blob/master/LICENSE.txt)
 [![Tests (GitHub Actions)](https://github.com/kmaork/hypno/workflows/Tests/badge.svg)](https://github.com/kmaork/hypno)
@@ -50,15 +50,15 @@
 from hypno import inject_py
 
 inject_py(pid, python_code)
 ```
 
 #### Example
 This example runs a python program that prints its pid, and then attaches to the newly created process and
-injects it with another print statement using hypno.
+injects it with another print statement using hypno. Mac users will need to use `sudo` for the second command.
 ```shell script
 python -c "import os, time; print('Hello from', os.getpid()); time.sleep(0.5)" &\
 hypno $! "import os; print('Hello again from', os.getpid())"
 ```
 
 ### Security
 Hypno briefly generates a temporary file containing the requested python code.
```

### Comparing `hypno-1.0.3/setup.cfg` & `hypno-1.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 python_requires = >=3.7
 packages = hypno
 install_requires = 
 	pyinjector>=0.1.2
 
 [metadata]
 name = hypno
-version = 1.0.3
+version = 1.1.0
 description = A tool/library allowing to inject python code into a running python process.
 author = Maor Kleinberger
 author_email = kmaork@gmail.com
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 license_file = LICENSE.txt
 keywords = injection library
 url = https://github.com/kmaork/hypno
 classifiers = 
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [egg_info]
```

