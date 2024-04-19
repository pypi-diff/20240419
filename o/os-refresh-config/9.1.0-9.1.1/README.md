# Comparing `tmp/os-refresh-config-9.1.0.tar.gz` & `tmp/os-refresh-config-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/os-refresh-config-9.1.0.tar", last modified: Fri Aug 24 14:52:03 2018, max compression
+gzip compressed data, was "dist/os-refresh-config-9.1.1.tar", last modified: Thu Mar 14 10:46:43 2019, max compression
```

## Comparing `os-refresh-config-9.1.0.tar` & `os-refresh-config-9.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      747 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/setup.cfg
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1616 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/os_refresh_config.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2018-08-24 14:52:02.000000 os-refresh-config-9.1.0/os_refresh_config.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2624 2018-08-24 14:52:02.000000 os-refresh-config-9.1.0/os_refresh_config.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2018-08-24 14:52:02.000000 os-refresh-config-9.1.0/os_refresh_config.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2018-08-24 14:52:02.000000 os-refresh-config-9.1.0/os_refresh_config.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/os_refresh_config.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2018-08-24 14:52:02.000000 os-refresh-config-9.1.0/os_refresh_config.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2018-08-24 14:52:02.000000 os-refresh-config-9.1.0/os_refresh_config.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2018-08-24 14:51:53.000000 os-refresh-config-9.1.0/os_refresh_config.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2018-08-24 14:52:02.000000 os-refresh-config-9.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2624 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/PKG-INFO
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/tests/pre-configure.d/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)       27 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/tests/pre-configure.d/01-test
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/tests/configure.d/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)       60 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/tests/configure.d/40-error
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      500 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/test-requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      292 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/setup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      792 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/zuul.d/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      115 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/zuul.d/layout.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11358 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/LICENSE
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/os_refresh_config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:52:03.000000 os-refresh-config-9.1.0/os_refresh_config/tests/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/os_refresh_config/tests/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1534 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/os_refresh_config/tests/test_os_refresh_config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5925 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/os_refresh_config/tests/test_cmd.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1536 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/os_refresh_config/tests/test_main.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/os_refresh_config/__init__.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     5783 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/os_refresh_config/os_refresh_config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      111 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2018-08-24 14:52:02.000000 os-refresh-config-9.1.0/ChangeLog
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       58 2018-08-24 14:48:38.000000 os-refresh-config-9.1.0/.stestr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/tests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/tests/pre-configure.d/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)       27 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/tests/pre-configure.d/01-test
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/tests/configure.d/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)       60 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/tests/configure.d/40-error
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      292 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/requirements.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1616 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/README.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      747 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/setup.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config/tests/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1536 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/os_refresh_config/tests/test_main.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/os_refresh_config/tests/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1534 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/os_refresh_config/tests/test_os_refresh_config.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5925 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/os_refresh_config/tests/test_cmd.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     5783 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/os_refresh_config/os_refresh_config.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/os_refresh_config/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/AUTHORS
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/setup.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      500 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/test-requirements.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      807 2019-03-14 10:44:48.000000 os-refresh-config-9.1.1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3505 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/ChangeLog
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11358 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/LICENSE
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/zuul.d/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      284 2019-03-14 10:44:48.000000 os-refresh-config-9.1.1/zuul.d/layout.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       58 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/.stestr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2624 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/os_refresh_config.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2624 2019-03-14 10:46:43.000000 os-refresh-config-9.1.1/PKG-INFO
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      111 2019-03-14 10:44:45.000000 os-refresh-config-9.1.1/.coveragerc
```

### Comparing `os-refresh-config-9.1.0/setup.cfg` & `os-refresh-config-9.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `os-refresh-config-9.1.0/README.rst` & `os-refresh-config-9.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `os-refresh-config-9.1.0/os_refresh_config.egg-info/PKG-INFO` & `os-refresh-config-9.1.1/os_refresh_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: os-refresh-config
-Version: 9.1.0
+Version: 9.1.1
 Summary: Refresh system configuration
 Home-page: http://github.com/openstack/os-refresh-config
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `os-refresh-config-9.1.0/os_refresh_config.egg-info/SOURCES.txt` & `os-refresh-config-9.1.1/os_refresh_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `os-refresh-config-9.1.0/AUTHORS` & `os-refresh-config-9.1.1/AUTHORS`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Andreas Jaeger <aj@suse.com>
 Ben Nemec <bnemec@redhat.com>
 Christian Berendt <berendt@b1-systems.de>
 Clint Byrum <clint@fewbar.com>
 Dirk Mueller <dirk@dmllr.de>
+Doug Hellmann <doug@doughellmann.com>
 Emilien Macchi <emilien@redhat.com>
 Flavio Percoco <flaper87@gmail.com>
 JUN JIE NAN <nanjj@cn.ibm.com>
 James E. Blair <jeblair@openstack.org>
 James E. Blair <jeblair@redhat.com>
 James Slagle <jslagle@redhat.com>
 Jeremy Stanley <fungi@yuggoth.org>
 Lucas Alvares Gomes <lucasagomes@gmail.com>
 Monty Taylor <mordred@inaugust.com>
 Motohiro OTSUKA <ootsuka@mxs.nes.nec.co.jp>
 Ondřej Nový <ondrej.novy@firma.seznam.cz>
+OpenStack Release Bot <infra-root@openstack.org>
 Sagi Shnaidman <sshnaidm@redhat.com>
 Sascha Peilicke <speilicke@suse.com>
 Steve Baker <sbaker@redhat.com>
 Steve Kowalik <steven@wedontsleep.org>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Tim Miller <tim.miller.0@gmail.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
-Zuul <zuul@review.openstack.org>
 gecong1973 <ge.cong@zte.com.cn>
 melissaml <ma.lei@99cloud.net>
 ricolin <rico.lin@easystack.cn>
```

### Comparing `os-refresh-config-9.1.0/PKG-INFO` & `os-refresh-config-9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: os-refresh-config
-Version: 9.1.0
+Version: 9.1.1
 Summary: Refresh system configuration
 Home-page: http://github.com/openstack/os-refresh-config
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `os-refresh-config-9.1.0/setup.py` & `os-refresh-config-9.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `os-refresh-config-9.1.0/tox.ini` & `os-refresh-config-9.1.1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 minversion = 2.0
 skipsdist = True
 envlist = py27,pep8
 
 [testenv]
 usedevelop = True
 deps =
-       -c{env:UPPER_CONSTRAINTS_FILE:https://git.openstack.org/cgit/openstack/requirements/plain/upper-constraints.txt}
+       -c{env:UPPER_CONSTRAINTS_FILE:https://git.openstack.org/cgit/openstack/requirements/plain/upper-constraints.txt?h=stable/rocky}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 install_command = pip install {opts} {packages}
 commands =
   stestr run --slowest {posargs}
 
 [tox:jenkins]
```

### Comparing `os-refresh-config-9.1.0/LICENSE` & `os-refresh-config-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `os-refresh-config-9.1.0/os_refresh_config/tests/test_os_refresh_config.py` & `os-refresh-config-9.1.1/os_refresh_config/tests/test_os_refresh_config.py`

 * *Files identical despite different names*

### Comparing `os-refresh-config-9.1.0/os_refresh_config/tests/test_cmd.py` & `os-refresh-config-9.1.1/os_refresh_config/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `os-refresh-config-9.1.0/os_refresh_config/tests/test_main.py` & `os-refresh-config-9.1.1/os_refresh_config/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `os-refresh-config-9.1.0/os_refresh_config/os_refresh_config.py` & `os-refresh-config-9.1.1/os_refresh_config/os_refresh_config.py`

 * *Files identical despite different names*

### Comparing `os-refresh-config-9.1.0/ChangeLog` & `os-refresh-config-9.1.1/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+9.1.1
+-----
+
+* import zuul job settings from project-config
+* Update UPPER\_CONSTRAINTS\_FILE for stable/rocky
+* Update .gitreview for stable/rocky
+
 9.1.0
 -----
 
 * Switch to stestr
 
 9.0.0
 -----
```

