# Comparing `tmp/sponge-0.0.5.tar.gz` & `tmp/sponge-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sponge-0.0.5.tar", last modified: Thu Jun  7 03:15:32 2018, max compression
+gzip compressed data, was "sponge-0.0.6.tar", last modified: Fri Apr 19 05:12:46 2024, max compression
```

## Comparing `sponge-0.0.5.tar` & `sponge-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,27 @@
-drwxr-xr-x   0 william    (501) staff       (20)        0 2018-06-07 03:15:32.000000 sponge-0.0.5/
--rw-r--r--   0 william    (501) staff       (20)     2706 2018-06-07 03:15:32.000000 sponge-0.0.5/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)     1375 2018-05-30 07:17:54.000000 sponge-0.0.5/README.md
--rw-r--r--   0 william    (501) staff       (20)     1275 2018-05-30 07:18:03.000000 sponge-0.0.5/README.rst
--rw-r--r--   0 william    (501) staff       (20)       38 2018-06-07 03:15:32.000000 sponge-0.0.5/setup.cfg
--rw-r--r--   0 william    (501) staff       (20)     1348 2018-05-27 07:07:55.000000 sponge-0.0.5/setup.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2018-06-07 03:15:32.000000 sponge-0.0.5/sponge/
--rw-r--r--   0 william    (501) staff       (20)      543 2018-06-07 03:15:30.000000 sponge-0.0.5/sponge/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2018-06-07 03:15:32.000000 sponge-0.0.5/sponge/drivers/
--rw-r--r--   0 william    (501) staff       (20)      172 2018-05-22 08:07:07.000000 sponge-0.0.5/sponge/drivers/__init__.py
--rw-r--r--   0 william    (501) staff       (20)     1146 2018-05-26 09:29:34.000000 sponge-0.0.5/sponge/drivers/driver.py
--rw-r--r--   0 william    (501) staff       (20)     1393 2018-05-23 04:34:25.000000 sponge-0.0.5/sponge/drivers/memory.py
--rw-r--r--   0 william    (501) staff       (20)     1252 2018-05-25 01:55:27.000000 sponge-0.0.5/sponge/drivers/redis.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2018-06-07 03:15:32.000000 sponge-0.0.5/sponge/events/
--rw-r--r--   0 william    (501) staff       (20)      172 2018-05-24 15:17:17.000000 sponge-0.0.5/sponge/events/__init__.py
--rw-r--r--   0 william    (501) staff       (20)      373 2018-05-24 15:07:36.000000 sponge-0.0.5/sponge/events/event.py
--rw-r--r--   0 william    (501) staff       (20)      300 2018-05-24 15:18:02.000000 sponge-0.0.5/sponge/events/forgotten.py
--rw-r--r--   0 william    (501) staff       (20)      386 2018-05-24 15:14:47.000000 sponge-0.0.5/sponge/events/hit.py
--rw-r--r--   0 william    (501) staff       (20)      295 2018-05-24 15:15:01.000000 sponge-0.0.5/sponge/events/missed.py
--rw-r--r--   0 william    (501) staff       (20)     1539 2018-06-07 03:14:25.000000 sponge-0.0.5/sponge/manager.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2018-06-07 03:15:32.000000 sponge-0.0.5/sponge.egg-info/
--rw-r--r--   0 william    (501) staff       (20)        1 2018-06-07 03:15:32.000000 sponge-0.0.5/sponge.egg-info/dependency_links.txt
--rw-r--r--   0 william    (501) staff       (20)     2706 2018-06-07 03:15:32.000000 sponge-0.0.5/sponge.egg-info/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)       14 2018-06-07 03:15:32.000000 sponge-0.0.5/sponge.egg-info/requires.txt
--rw-r--r--   0 william    (501) staff       (20)      512 2018-06-07 03:15:32.000000 sponge-0.0.5/sponge.egg-info/SOURCES.txt
--rw-r--r--   0 william    (501) staff       (20)       13 2018-06-07 03:15:32.000000 sponge-0.0.5/sponge.egg-info/top_level.txt
-drwxr-xr-x   0 william    (501) staff       (20)        0 2018-06-07 03:15:32.000000 sponge-0.0.5/tests/
--rw-r--r--   0 william    (501) staff       (20)      172 2018-05-22 10:42:05.000000 sponge-0.0.5/tests/__init__.py
--rw-r--r--   0 william    (501) staff       (20)     2137 2018-05-23 04:36:00.000000 sponge-0.0.5/tests/driver.py
--rw-r--r--   0 william    (501) staff       (20)      380 2018-05-23 02:38:21.000000 sponge-0.0.5/tests/test_memory.py
--rw-r--r--   0 william    (501) staff       (20)      379 2018-05-23 02:28:45.000000 sponge-0.0.5/tests/test_redis.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.086076 sponge-0.0.6/
+-rw-r--r--   0 william    (502) staff       (20)    35147 2024-04-19 04:29:01.000000 sponge-0.0.6/LICENSE
+-rw-r--r--   0 william    (502) staff       (20)     2189 2024-04-19 05:12:46.085789 sponge-0.0.6/PKG-INFO
+-rw-r--r--   0 william    (502) staff       (20)     1275 2024-04-19 04:29:01.000000 sponge-0.0.6/README.rst
+-rw-r--r--   0 william    (502) staff       (20)       38 2024-04-19 05:12:46.086189 sponge-0.0.6/setup.cfg
+-rw-r--r--   0 william    (502) staff       (20)     1348 2024-04-19 04:29:01.000000 sponge-0.0.6/setup.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.076770 sponge-0.0.6/sponge/
+-rw-r--r--   0 william    (502) staff       (20)      324 2024-04-19 05:12:38.000000 sponge-0.0.6/sponge/__init__.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.083453 sponge-0.0.6/sponge/drivers/
+-rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/drivers/__init__.py
+-rw-r--r--   0 william    (502) staff       (20)      624 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/drivers/driver.py
+-rw-r--r--   0 william    (502) staff       (20)     1393 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/drivers/memory.py
+-rw-r--r--   0 william    (502) staff       (20)     1252 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/drivers/redis.py
+-rw-r--r--   0 william    (502) staff       (20)     1842 2024-04-19 04:49:21.000000 sponge-0.0.6/sponge/drivers/sqlite.py
+-rw-r--r--   0 william    (502) staff       (20)     1539 2024-04-19 04:29:01.000000 sponge-0.0.6/sponge/manager.py
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.081742 sponge-0.0.6/sponge.egg-info/
+-rw-r--r--   0 william    (502) staff       (20)     2189 2024-04-19 05:12:45.000000 sponge-0.0.6/sponge.egg-info/PKG-INFO
+-rw-r--r--   0 william    (502) staff       (20)      435 2024-04-19 05:12:46.000000 sponge-0.0.6/sponge.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (502) staff       (20)        1 2024-04-19 05:12:45.000000 sponge-0.0.6/sponge.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (502) staff       (20)       14 2024-04-19 05:12:45.000000 sponge-0.0.6/sponge.egg-info/requires.txt
+-rw-r--r--   0 william    (502) staff       (20)       13 2024-04-19 05:12:45.000000 sponge-0.0.6/sponge.egg-info/top_level.txt
+drwxr-xr-x   0 william    (502) staff       (20)        0 2024-04-19 05:12:46.085182 sponge-0.0.6/tests/
+-rw-r--r--   0 william    (502) staff       (20)      172 2024-04-19 04:29:01.000000 sponge-0.0.6/tests/__init__.py
+-rw-r--r--   0 william    (502) staff       (20)     2137 2024-04-19 04:29:01.000000 sponge-0.0.6/tests/driver.py
+-rw-r--r--   0 william    (502) staff       (20)      380 2024-04-19 04:29:01.000000 sponge-0.0.6/tests/test_memory.py
+-rw-r--r--   0 william    (502) staff       (20)      379 2024-04-19 04:29:01.000000 sponge-0.0.6/tests/test_redis.py
+-rw-r--r--   0 william    (502) staff       (20)     2291 2024-04-19 04:51:57.000000 sponge-0.0.6/tests/test_sqlite.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sponge-0.0.5/PKG-INFO` & `sponge-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,93 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sponge
-Version: 0.0.5
+Version: 0.0.6
 Summary: An elegant cache library for python
 Home-page: https://github.com/IamBusy/sponge
 Author: William Wei
 Author-email: 1342247033@qq.com
+Maintainer: William Wei
+Maintainer-email: 1342247033@qq.com
 License: GNU Lesser General Public License v3 (LGPLv3)
-Description-Content-Type: UNKNOWN
-Description: `Build Status <https://travis-ci.org/IamBusy/sponge>`__ `PyPI - Python
-        Version <https://pypi.org/project/sponge/#description>`__ `PyPI -
-        License <https://pypi.org/project/sponge/#description>`__ `Codecov
-        branch <https://codecov.io/gh/IamBusy/sponge>`__
-        
-        sponge
-        ======
-        
-        An elegant cache library for python
-        
-        How to use
-        ==========
-        
-        Install
-        ~~~~~~~
-        
-        .. code:: bash
-        
-           pip install sponge
-        
-        Usage
-        ~~~~~
-        
-        .. code:: python
-        
-           from sponge import CacheManager
-        
-           # config cache manager
-           manager = CacheManager({
-               'default': 'redis',
-               'redis': {
-                   'host': 'localhost',
-                   'port': 3306,
-                   'db': 0
-               },
-               'memory': {}
-           })
-        
-           # get cache instance
-           cache = manager.store('redis')
-        
-           # set cache
-           cache.put('mykey', 'myvalue', 30) # 30 seconds
-           cache.get('mykey')                # myvalue
-        
-           # remove cache
-           cache.forget('mykey')
-        
-           # cache fover
-           cache.fover('mykey', 1)
-        
-           # increase
-           cache.increase('mykey')     # the value will be 2
-        
-           # decrease
-           cache.decrease('mykey', 2)  # the value will be -1
-        
-        
-           # clear all
-           cache.flush()
-        
-        TODO
-        ====
-        
-        -  [ ] Support cache events
-        -  [ ] Support file driver
-        -  [ ] Support database driver
-        -  [ ] Added into
-           `awesome-python <https://github.com/vinta/awesome-python>`__
-        
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+`Build Status <https://travis-ci.org/IamBusy/sponge>`__ `PyPI - Python
+Version <https://pypi.org/project/sponge/#description>`__ `PyPI -
+License <https://pypi.org/project/sponge/#description>`__ `Codecov
+branch <https://codecov.io/gh/IamBusy/sponge>`__
+
+sponge
+======
+
+An elegant cache library for python
+
+How to use
+==========
+
+Install
+~~~~~~~
+
+.. code:: bash
+
+   pip install sponge
+
+Usage
+~~~~~
+
+.. code:: python
+
+   from sponge import CacheManager
+
+   # config cache manager
+   manager = CacheManager({
+       'default': 'redis',
+       'redis': {
+           'host': 'localhost',
+           'port': 3306,
+           'db': 0
+       },
+       'memory': {}
+   })
+
+   # get cache instance
+   cache = manager.store('redis')
+
+   # set cache
+   cache.put('mykey', 'myvalue', 30) # 30 seconds
+   cache.get('mykey')                # myvalue
+
+   # remove cache
+   cache.forget('mykey')
+
+   # cache fover
+   cache.fover('mykey', 1)
+
+   # increase
+   cache.increase('mykey')     # the value will be 2
+
+   # decrease
+   cache.decrease('mykey', 2)  # the value will be -1
+
+
+   # clear all
+   cache.flush()
+
+TODO
+====
+
+-  [ ] Support cache events
+-  [ ] Support file driver
+-  [ ] Support database driver
+-  [ ] Added into
+   `awesome-python <https://github.com/vinta/awesome-python>`__
```

### Comparing `sponge-0.0.5/README.rst` & `sponge-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `sponge-0.0.5/setup.py` & `sponge-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.5/sponge/drivers/memory.py` & `sponge-0.0.6/sponge/drivers/memory.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.5/sponge/drivers/redis.py` & `sponge-0.0.6/sponge/drivers/redis.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.5/sponge/manager.py` & `sponge-0.0.6/sponge/manager.py`

 * *Files identical despite different names*

### Comparing `sponge-0.0.5/sponge.egg-info/PKG-INFO` & `sponge-0.0.6/sponge.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,93 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: sponge
-Version: 0.0.5
+Version: 0.0.6
 Summary: An elegant cache library for python
 Home-page: https://github.com/IamBusy/sponge
 Author: William Wei
 Author-email: 1342247033@qq.com
+Maintainer: William Wei
+Maintainer-email: 1342247033@qq.com
 License: GNU Lesser General Public License v3 (LGPLv3)
-Description-Content-Type: UNKNOWN
-Description: `Build Status <https://travis-ci.org/IamBusy/sponge>`__ `PyPI - Python
-        Version <https://pypi.org/project/sponge/#description>`__ `PyPI -
-        License <https://pypi.org/project/sponge/#description>`__ `Codecov
-        branch <https://codecov.io/gh/IamBusy/sponge>`__
-        
-        sponge
-        ======
-        
-        An elegant cache library for python
-        
-        How to use
-        ==========
-        
-        Install
-        ~~~~~~~
-        
-        .. code:: bash
-        
-           pip install sponge
-        
-        Usage
-        ~~~~~
-        
-        .. code:: python
-        
-           from sponge import CacheManager
-        
-           # config cache manager
-           manager = CacheManager({
-               'default': 'redis',
-               'redis': {
-                   'host': 'localhost',
-                   'port': 3306,
-                   'db': 0
-               },
-               'memory': {}
-           })
-        
-           # get cache instance
-           cache = manager.store('redis')
-        
-           # set cache
-           cache.put('mykey', 'myvalue', 30) # 30 seconds
-           cache.get('mykey')                # myvalue
-        
-           # remove cache
-           cache.forget('mykey')
-        
-           # cache fover
-           cache.fover('mykey', 1)
-        
-           # increase
-           cache.increase('mykey')     # the value will be 2
-        
-           # decrease
-           cache.decrease('mykey', 2)  # the value will be -1
-        
-        
-           # clear all
-           cache.flush()
-        
-        TODO
-        ====
-        
-        -  [ ] Support cache events
-        -  [ ] Support file driver
-        -  [ ] Support database driver
-        -  [ ] Added into
-           `awesome-python <https://github.com/vinta/awesome-python>`__
-        
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
+
+`Build Status <https://travis-ci.org/IamBusy/sponge>`__ `PyPI - Python
+Version <https://pypi.org/project/sponge/#description>`__ `PyPI -
+License <https://pypi.org/project/sponge/#description>`__ `Codecov
+branch <https://codecov.io/gh/IamBusy/sponge>`__
+
+sponge
+======
+
+An elegant cache library for python
+
+How to use
+==========
+
+Install
+~~~~~~~
+
+.. code:: bash
+
+   pip install sponge
+
+Usage
+~~~~~
+
+.. code:: python
+
+   from sponge import CacheManager
+
+   # config cache manager
+   manager = CacheManager({
+       'default': 'redis',
+       'redis': {
+           'host': 'localhost',
+           'port': 3306,
+           'db': 0
+       },
+       'memory': {}
+   })
+
+   # get cache instance
+   cache = manager.store('redis')
+
+   # set cache
+   cache.put('mykey', 'myvalue', 30) # 30 seconds
+   cache.get('mykey')                # myvalue
+
+   # remove cache
+   cache.forget('mykey')
+
+   # cache fover
+   cache.fover('mykey', 1)
+
+   # increase
+   cache.increase('mykey')     # the value will be 2
+
+   # decrease
+   cache.decrease('mykey', 2)  # the value will be -1
+
+
+   # clear all
+   cache.flush()
+
+TODO
+====
+
+-  [ ] Support cache events
+-  [ ] Support file driver
+-  [ ] Support database driver
+-  [ ] Added into
+   `awesome-python <https://github.com/vinta/awesome-python>`__
```

### Comparing `sponge-0.0.5/tests/driver.py` & `sponge-0.0.6/tests/driver.py`

 * *Files identical despite different names*

