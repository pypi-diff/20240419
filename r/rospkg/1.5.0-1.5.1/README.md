# Comparing `tmp/rospkg-1.5.0.tar.gz` & `tmp/rospkg-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rospkg-1.5.0.tar", last modified: Mon Mar 20 21:33:39 2023, max compression
+gzip compressed data, was "rospkg-1.5.1.tar", last modified: Fri Apr 19 18:57:21 2024, max compression
```

## Comparing `rospkg-1.5.0.tar` & `rospkg-1.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2023-03-20 21:33:39.880832 rospkg-1.5.0/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      603 2023-03-20 21:33:39.880832 rospkg-1.5.0/PKG-INFO
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      157 2023-03-20 21:17:46.000000 rospkg-1.5.0/README.md
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      111 2023-03-20 21:33:39.880832 rospkg-1.5.0/setup.cfg
--rwxrwxr-x   0 cottsay   (1000) cottsay   (1000)     1777 2023-03-20 21:17:46.000000 rospkg-1.5.0/setup.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2023-03-20 21:33:39.876832 rospkg-1.5.0/src/
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2023-03-20 21:33:39.880832 rospkg-1.5.0/src/rospkg/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2577 2023-03-20 21:17:46.000000 rospkg-1.5.0/src/rospkg/__init__.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2199 2023-03-20 21:17:46.000000 rospkg-1.5.0/src/rospkg/common.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    23442 2023-03-20 21:17:46.000000 rospkg-1.5.0/src/rospkg/distro.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7543 2023-03-20 21:17:46.000000 rospkg-1.5.0/src/rospkg/environment.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    17831 2023-03-20 21:17:46.000000 rospkg-1.5.0/src/rospkg/manifest.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    23784 2023-03-20 21:17:46.000000 rospkg-1.5.0/src/rospkg/os_detect.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    19447 2023-03-20 21:17:46.000000 rospkg-1.5.0/src/rospkg/rospack.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5174 2023-03-20 21:17:46.000000 rospkg-1.5.0/src/rospkg/rosversion.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8873 2023-03-20 21:17:46.000000 rospkg-1.5.0/src/rospkg/stack.py
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2023-03-20 21:33:39.880832 rospkg-1.5.0/src/rospkg.egg-info/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      603 2023-03-20 21:33:39.000000 rospkg-1.5.0/src/rospkg.egg-info/PKG-INFO
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      714 2023-03-20 21:33:39.000000 rospkg-1.5.0/src/rospkg.egg-info/SOURCES.txt
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        1 2023-03-20 21:33:39.000000 rospkg-1.5.0/src/rospkg.egg-info/dependency_links.txt
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       55 2023-03-20 21:33:39.000000 rospkg-1.5.0/src/rospkg.egg-info/entry_points.txt
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      111 2023-03-20 21:33:39.000000 rospkg-1.5.0/src/rospkg.egg-info/requires.txt
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        7 2023-03-20 21:33:39.000000 rospkg-1.5.0/src/rospkg.egg-info/top_level.txt
-drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2023-03-20 21:33:39.880832 rospkg-1.5.0/test/
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2970 2023-03-20 21:17:46.000000 rospkg-1.5.0/test/test_rospkg_catkin_packages.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2147 2023-03-20 21:17:46.000000 rospkg-1.5.0/test/test_rospkg_common.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    20635 2023-03-20 21:17:46.000000 rospkg-1.5.0/test/test_rospkg_distro.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    18270 2023-03-20 21:17:46.000000 rospkg-1.5.0/test/test_rospkg_distro_vcs_config.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6645 2023-03-20 21:17:46.000000 rospkg-1.5.0/test/test_rospkg_environment.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9169 2023-03-20 21:17:46.000000 rospkg-1.5.0/test/test_rospkg_manifest.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    18494 2023-03-20 21:17:46.000000 rospkg-1.5.0/test/test_rospkg_os_detect.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    13049 2023-03-20 21:17:46.000000 rospkg-1.5.0/test/test_rospkg_packages.py
--rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    10409 2023-03-20 21:17:46.000000 rospkg-1.5.0/test/test_rospkg_stacks.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-04-19 18:57:21.594638 rospkg-1.5.1/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      603 2024-04-19 18:57:21.594638 rospkg-1.5.1/PKG-INFO
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      157 2024-04-19 18:39:51.000000 rospkg-1.5.1/README.md
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      111 2024-04-19 18:57:21.594638 rospkg-1.5.1/setup.cfg
+-rwxrwxr-x   0 cottsay   (1000) cottsay   (1000)     1777 2024-04-19 18:39:51.000000 rospkg-1.5.1/setup.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-04-19 18:57:21.590638 rospkg-1.5.1/src/
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-04-19 18:57:21.594638 rospkg-1.5.1/src/rospkg/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2577 2024-04-19 18:39:51.000000 rospkg-1.5.1/src/rospkg/__init__.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2199 2024-04-19 18:39:51.000000 rospkg-1.5.1/src/rospkg/common.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    23442 2024-04-19 18:39:51.000000 rospkg-1.5.1/src/rospkg/distro.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     7543 2024-04-19 18:39:51.000000 rospkg-1.5.1/src/rospkg/environment.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    17831 2024-04-19 18:39:51.000000 rospkg-1.5.1/src/rospkg/manifest.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    23940 2024-04-19 18:39:51.000000 rospkg-1.5.1/src/rospkg/os_detect.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    19447 2024-04-19 18:39:51.000000 rospkg-1.5.1/src/rospkg/rospack.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     5174 2024-04-19 18:39:51.000000 rospkg-1.5.1/src/rospkg/rosversion.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     8873 2024-04-19 18:39:51.000000 rospkg-1.5.1/src/rospkg/stack.py
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-04-19 18:57:21.594638 rospkg-1.5.1/src/rospkg.egg-info/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      603 2024-04-19 18:57:21.000000 rospkg-1.5.1/src/rospkg.egg-info/PKG-INFO
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      714 2024-04-19 18:57:21.000000 rospkg-1.5.1/src/rospkg.egg-info/SOURCES.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        1 2024-04-19 18:57:21.000000 rospkg-1.5.1/src/rospkg.egg-info/dependency_links.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)       55 2024-04-19 18:57:21.000000 rospkg-1.5.1/src/rospkg.egg-info/entry_points.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)      111 2024-04-19 18:57:21.000000 rospkg-1.5.1/src/rospkg.egg-info/requires.txt
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)        7 2024-04-19 18:57:21.000000 rospkg-1.5.1/src/rospkg.egg-info/top_level.txt
+drwxrwxr-x   0 cottsay   (1000) cottsay   (1000)        0 2024-04-19 18:57:21.594638 rospkg-1.5.1/test/
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2970 2024-04-19 18:39:51.000000 rospkg-1.5.1/test/test_rospkg_catkin_packages.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     2147 2024-04-19 18:39:51.000000 rospkg-1.5.1/test/test_rospkg_common.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    20635 2024-04-19 18:39:51.000000 rospkg-1.5.1/test/test_rospkg_distro.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    18270 2024-04-19 18:39:51.000000 rospkg-1.5.1/test/test_rospkg_distro_vcs_config.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     6746 2024-04-19 18:39:51.000000 rospkg-1.5.1/test/test_rospkg_environment.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)     9286 2024-04-19 18:39:51.000000 rospkg-1.5.1/test/test_rospkg_manifest.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    18528 2024-04-19 18:39:51.000000 rospkg-1.5.1/test/test_rospkg_os_detect.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    13049 2024-04-19 18:39:51.000000 rospkg-1.5.1/test/test_rospkg_packages.py
+-rw-rw-r--   0 cottsay   (1000) cottsay   (1000)    10409 2024-04-19 18:39:51.000000 rospkg-1.5.1/test/test_rospkg_stacks.py
```

### Comparing `rospkg-1.5.0/PKG-INFO` & `rospkg-1.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rospkg
-Version: 1.5.0
+Version: 1.5.1
 Summary: ROS package library
 Home-page: http://wiki.ros.org/rospkg
 Author: Ken Conley
 Author-email: kwc@willowgarage.com
 Maintainer: ROS Infrastructure Team
 License: BSD
 Project-URL: Source code, https://github.com/ros-infrastructure/rospkg
```

### Comparing `rospkg-1.5.0/setup.py` & `rospkg-1.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     install_requires.append("distro >= 1.4.0; python_version >= '3.8'")
 
 kwargs = {
     'name': 'rospkg',
     # same version as in:
     # - src/rospkg/__init__.py
     # - stdeb.cfg
-    'version': '1.5.0',
+    'version': '1.5.1',
     'packages': ['rospkg'],
     'package_dir': {'': 'src'},
     'entry_points': {
         'console_scripts': ['rosversion=rospkg.rosversion:main'],
     },
     'install_requires': install_requires,
     'extras_require': {
```

### Comparing `rospkg-1.5.0/src/rospkg/__init__.py` & `rospkg-1.5.1/src/rospkg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from .manifest import InvalidManifest, Manifest, parse_manifest_file
 from .rospack import expand_to_packages, get_package_name, \
     get_stack_version_by_dir, list_by_path, RosPack, RosStack
 
 # same version as in:
 # - setup.py
 # - stdeb.cfg
-__version__ = '1.5.0'
+__version__ = '1.5.1'
 
 __all__ = (
     'MANIFEST_FILE', 'ResourceNotFound', 'STACK_FILE',
     'get_etc_ros_dir', 'get_log_dir', 'get_ros_home',
     'get_ros_package_path', 'get_ros_paths', 'get_ros_root',
     'get_test_results_dir', 'on_ros_path',
     'InvalidManifest', 'Manifest', 'parse_manifest_file',
```

### Comparing `rospkg-1.5.0/src/rospkg/common.py` & `rospkg-1.5.1/src/rospkg/common.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/src/rospkg/distro.py` & `rospkg-1.5.1/src/rospkg/distro.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/src/rospkg/environment.py` & `rospkg-1.5.1/src/rospkg/environment.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/src/rospkg/manifest.py` & `rospkg-1.5.1/src/rospkg/manifest.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/src/rospkg/os_detect.py` & `rospkg-1.5.1/src/rospkg/os_detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,16 +176,17 @@
                 '7': 'wheezy',
                 '8': 'jessie',
                 '9': 'stretch',
                 '10': 'buster',
                 '11': 'bullseye',
                 '12': 'bookworm',
                 '13': 'trixie',
+                '14': 'forky',
                 'unstable': 'sid',
-                'rodete': 'bookworm',
+                'rodete': 'trixie',
             }.get(v, '')
 
 
 class FdoDetect(OsDetector):
     """
     Generic detector for operating systems implementing /etc/os-release, as defined by the os-release spec hosted at Freedesktop.org (Fdo):
     http://www.freedesktop.org/software/systemd/man/os-release.html
@@ -314,15 +315,16 @@
  '10.11': 'el capitan',
  '10.12': 'sierra',
  '10.13': 'high sierra',
  '10.14': 'mojave',
  '10.15': 'catalina',
  '11': 'big sur',
  '12': 'monterey',
- '13': 'ventura'
+ '13': 'ventura',
+ '14': 'sonoma',
 }
 
 
 def _osx_codename(major, minor):
     if major == 10:
         key = '%s.%s' % (major, minor)
     else:
@@ -656,14 +658,15 @@
 OS_CENTOS = 'centos'
 OS_EULEROS = 'euleros'
 OS_CYGWIN = 'cygwin'
 OS_DEBIAN = 'debian'
 OS_ELEMENTARY = 'elementary'
 OS_ELEMENTARY_OLD = 'elementary'
 OS_FEDORA = 'fedora'
+OS_FEDORA_ASAHI = 'fedora-asahi'
 OS_FREEBSD = 'freebsd'
 OS_FUNTOO = 'funtoo'
 OS_GENTOO = 'gentoo'
 OS_LINARO = 'linaro'
 OS_MINT = 'mint'
 OS_MX = 'mx'
 OS_NEON = 'neon'
@@ -696,14 +699,15 @@
 OsDetect.register_default(OS_CENTOS, FdoDetect("centos"))
 OsDetect.register_default(OS_EULEROS, FdoDetect("euleros"))
 OsDetect.register_default(OS_CYGWIN, Cygwin())
 OsDetect.register_default(OS_DEBIAN, Debian())
 OsDetect.register_default(OS_ELEMENTARY, LsbDetect("elementary"))
 OsDetect.register_default(OS_ELEMENTARY_OLD, LsbDetect("elementary OS"))
 OsDetect.register_default(OS_FEDORA, FdoDetect("fedora"))
+OsDetect.register_default(OS_FEDORA_ASAHI, FdoDetect("fedora-asahi-remix"))
 OsDetect.register_default(OS_FREEBSD, FreeBSD())
 OsDetect.register_default(OS_FUNTOO, Funtoo())
 OsDetect.register_default(OS_GENTOO, Gentoo())
 OsDetect.register_default(OS_LINARO, LsbDetect("Linaro"))
 OsDetect.register_default(OS_MINT, LsbDetect("LinuxMint"))
 OsDetect.register_default(OS_MX, LsbDetect("MX"))
 OsDetect.register_default(OS_NEON, LsbDetect("neon"))
```

### Comparing `rospkg-1.5.0/src/rospkg/rospack.py` & `rospkg-1.5.1/src/rospkg/rospack.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/src/rospkg/rosversion.py` & `rospkg-1.5.1/src/rospkg/rosversion.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/src/rospkg/stack.py` & `rospkg-1.5.1/src/rospkg/stack.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/src/rospkg.egg-info/PKG-INFO` & `rospkg-1.5.1/src/rospkg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rospkg
-Version: 1.5.0
+Version: 1.5.1
 Summary: ROS package library
 Home-page: http://wiki.ros.org/rospkg
 Author: Ken Conley
 Author-email: kwc@willowgarage.com
 Maintainer: ROS Infrastructure Team
 License: BSD
 Project-URL: Source code, https://github.com/ros-infrastructure/rospkg
```

### Comparing `rospkg-1.5.0/src/rospkg.egg-info/SOURCES.txt` & `rospkg-1.5.1/src/rospkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/test/test_rospkg_catkin_packages.py` & `rospkg-1.5.1/test/test_rospkg_catkin_packages.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/test/test_rospkg_common.py` & `rospkg-1.5.1/test/test_rospkg_common.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/test/test_rospkg_distro.py` & `rospkg-1.5.1/test/test_rospkg_distro.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/test/test_rospkg_distro_vcs_config.py` & `rospkg-1.5.1/test/test_rospkg_distro_vcs_config.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/test/test_rospkg_environment.py` & `rospkg-1.5.1/test/test_rospkg_environment.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 import tempfile
 
 
 def test_get_ros_root():
     from rospkg import get_ros_root
     assert get_ros_root(env={}) is None
 
-    env = {'ROS_ROOT': '/fake/path'}
-    assert '/fake/path' == get_ros_root(env=env)
+    fake_path = os.path.normpath('/fake/path')
+    env = {'ROS_ROOT': fake_path}
+    assert fake_path == get_ros_root(env=env)
 
     real_ros_root = get_ros_root()
 
     if real_ros_root is not None:
         # make sure that ros root is a directory
         p = os.path.join(real_ros_root, 'Makefile')
         env = {'ROS_ROOT': p}
@@ -138,16 +139,16 @@
 def test_compute_package_paths():
     from rospkg.environment import _compute_package_paths as compute_package_paths
     assert compute_package_paths(None, None) == []
     assert compute_package_paths('foo', None) == ['foo']
     assert compute_package_paths(None, 'bar') == ['bar'], compute_package_paths(None, 'bar')
     assert compute_package_paths('foo', '') == ['foo']
     assert compute_package_paths('foo', 'bar') == ['foo', 'bar']
-    assert compute_package_paths('foo', 'bar:bz') == ['foo', 'bar', 'bz']
-    assert compute_package_paths('foo', 'bar:bz::blah') == ['foo', 'bar', 'bz', 'blah']
+    assert compute_package_paths('foo', os.path.pathsep.join(('bar', 'bz'))) == ['foo', 'bar', 'bz']
+    assert compute_package_paths('foo', os.path.pathsep.join(('bar', 'bz', '', 'blah'))) == ['foo', 'bar', 'bz', 'blah']
 
 
 def test_resolve_path():
     # mainly for coverage
     from rospkg.environment import _resolve_path
     assert os.path.expanduser('~') == _resolve_path('~')
```

### Comparing `rospkg-1.5.0/test/test_rospkg_manifest.py` & `rospkg-1.5.1/test/test_rospkg_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,17 @@
 
 
 def test_parse_manifest():
     # test_parse_manifest_file is more thorough; just want to make sure we have one call to lower-level API
     from rospkg.manifest import MANIFEST_FILE, parse_manifest
     d = get_test_dir()
     p = os.path.join(d, 'example1', MANIFEST_FILE)
-    with open(p, 'r') as f:
+    # Open in binary mode to match the parse_manifest_file function
+    # This is particularly important on Windows
+    with open(p, 'rb') as f:
         contents = f.read()
     _subtest_parse_example1(parse_manifest(MANIFEST_FILE, contents, p))
 
 
 def test__Manifest():
     from rospkg.manifest import Manifest
     m = Manifest()
```

### Comparing `rospkg-1.5.0/test/test_rospkg_os_detect.py` & `rospkg-1.5.1/test/test_rospkg_os_detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import absolute_import
 
 import os
+import sys
 
 try:
     from unittest.mock import Mock, patch
 except ImportError:
     from mock import Mock, patch
 
 
@@ -71,15 +72,15 @@
 
     def get_codename(self):
         return "os_codename"
 
 
 def test__read_stdout():
     from rospkg.os_detect import _read_stdout
-    assert 'hello' == _read_stdout(['echo', 'hello'])
+    assert 'hello' == _read_stdout([sys.executable, '-c', "print('hello')"])
     assert _read_stdout(['bad-command-input-for-rospkg-os-detect']) is None
 
 
 def test_tripwire_ubuntu():
     from rospkg.os_detect import OsDetect
     os_detect = OsDetect()
     os_detect.get_detector('ubuntu')
```

### Comparing `rospkg-1.5.0/test/test_rospkg_packages.py` & `rospkg-1.5.1/test/test_rospkg_packages.py`

 * *Files identical despite different names*

### Comparing `rospkg-1.5.0/test/test_rospkg_stacks.py` & `rospkg-1.5.1/test/test_rospkg_stacks.py`

 * *Files identical despite different names*

