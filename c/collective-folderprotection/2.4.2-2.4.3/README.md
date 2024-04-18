# Comparing `tmp/collective_folderprotection-2.4.2.tar.gz` & `tmp/collective_folderprotection-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective_folderprotection-2.4.2.tar", last modified: Wed Apr 17 16:10:19 2024, max compression
+gzip compressed data, was "collective_folderprotection-2.4.3.tar", last modified: Thu Apr 18 22:23:08 2024, max compression
```

## Comparing `collective_folderprotection-2.4.2.tar` & `collective_folderprotection-2.4.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.823803 collective_folderprotection-2.4.2/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      408 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/.gitignore
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1119 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/.travis.yml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2171 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/CHANGES.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      118 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/CONTRIBUTORS.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      284 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/MANIFEST.in
--rw-r--r--   0 frapell   (1000) frapell   (1000)     7413 2024-04-17 16:10:19.823803 collective_folderprotection-2.4.2/PKG-INFO
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3439 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/README.rst
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3439 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/README.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1130 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/base.cfg
--rwxrwxr-x   0 frapell   (1000) frapell   (1000)      224 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/bootstrap.sh
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      795 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/buildout.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1638 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/dev.cfg
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.811803 collective_folderprotection-2.4.2/docs/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)    18092 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/docs/LICENSE.GPL
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      740 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/docs/LICENSE.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      298 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/plone-5.0.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      104 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/plone-5.1.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      185 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/plone-5.2.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       19 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/requirements.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      261 2024-04-17 16:10:19.823803 collective_folderprotection-2.4.2/setup.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2269 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/setup.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.807803 collective_folderprotection-2.4.2/src/
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.815803 collective_folderprotection-2.4.2/src/collective_folderprotection/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      216 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/__init__.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.815803 collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/__init__.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1782 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/configure.zcml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      449 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/del_protected.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2614 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/interfaces.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2240 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/passwordprotected.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      449 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/rename_protected.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.815803 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/__init__.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      831 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/alert_viewlet.pt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2007 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/alert_viewlet.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3779 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/configure.zcml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     5018 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/delete_protected.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1271 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/passwordprotected.pt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)    10180 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/passwordprotected.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      238 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/reason_viewlet.pt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1359 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/reason_viewlet.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     4065 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/rename_protected.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.819803 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/widget/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/widget/__init__.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      372 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/widget/configure.zcml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      965 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/widget/password.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1875 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/browser/widget/password_input.pt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      343 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/config.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2526 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/configure.zcml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     5450 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/events.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1707 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/exceptions.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      105 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/interfaces.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      290 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/overrides.zcml
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.807803 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.819803 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/default/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      997 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/default/actions.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      150 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/default/browserlayer.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       68 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/default/metadata.xml
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.819803 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/test_fixture/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      241 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/test_fixture/metadata.xml
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.819803 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/test_fixture/types/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2156 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/test_fixture/types/folderish_not_protected.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2418 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/test_fixture/types/folderish_protected.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      313 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/test_fixture/types.xml
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.819803 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/uninstall/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      301 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/uninstall/actions.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       82 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1190 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/setuphandlers.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.819803 collective_folderprotection-2.4.2/src/collective_folderprotection/static/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1520 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/static/lock_locked_128.png
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      320 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/static/lock_locked_16.png
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1544 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/static/lock_unlocked_128.png
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      308 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/static/lock_unlocked_16.png
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1869 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/testing.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.819803 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        2 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/__init__.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.819803 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/robot/
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     4310 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/robot/keywords.robot
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     4021 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/robot/manager_functional.robot
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     6143 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/robot/member_functional.robot
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2922 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/robot/owner_functional.robot
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     2474 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_delprotect.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3602 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_passwordprotect.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3121 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_renameprotect.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      783 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_robot.py
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      544 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_setup.py
-drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-17 16:10:19.819803 collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/
--rw-r--r--   0 frapell   (1000) frapell   (1000)     7413 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/PKG-INFO
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     3734 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/SOURCES.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        1 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/dependency_links.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       40 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/entry_points.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)        1 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/not-zip-safe
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      229 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/requires.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       28 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/top_level.txt
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      331 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/tests-5.2.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)     1163 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/tests-6.0.x.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      629 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/tox.ini
--rw-rw-r--   0 frapell   (1000) frapell   (1000)      140 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/travis.cfg
--rw-rw-r--   0 frapell   (1000) frapell   (1000)       67 2024-04-17 16:10:19.000000 collective_folderprotection-2.4.2/versions.cfg
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.129128 collective_folderprotection-2.4.3/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      408 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/.gitignore
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1119 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/.travis.yml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2247 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/CHANGES.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      118 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/CONTRIBUTORS.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      284 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/MANIFEST.in
+-rw-r--r--   0 frapell   (1000) frapell   (1000)     7489 2024-04-18 22:23:08.129128 collective_folderprotection-2.4.3/PKG-INFO
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3439 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/README.rst
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3439 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/README.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1130 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/base.cfg
+-rwxrwxr-x   0 frapell   (1000) frapell   (1000)      224 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/bootstrap.sh
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      795 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/buildout.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1638 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/dev.cfg
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.117128 collective_folderprotection-2.4.3/docs/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)    18092 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/docs/LICENSE.GPL
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      740 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/docs/LICENSE.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      298 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/plone-5.0.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      104 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/plone-5.1.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      185 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/plone-5.2.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       19 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/requirements.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      261 2024-04-18 22:23:08.129128 collective_folderprotection-2.4.3/setup.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2269 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/setup.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.113127 collective_folderprotection-2.4.3/src/
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.121127 collective_folderprotection-2.4.3/src/collective_folderprotection/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      216 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/__init__.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.121127 collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/__init__.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1782 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/configure.zcml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      449 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/del_protected.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2614 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/interfaces.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2575 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/passwordprotected.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      449 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/rename_protected.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.121127 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/__init__.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      831 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/alert_viewlet.pt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2007 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/alert_viewlet.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3779 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/configure.zcml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     5018 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/delete_protected.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1271 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/passwordprotected.pt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)    10303 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/passwordprotected.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      238 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/reason_viewlet.pt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1359 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/reason_viewlet.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     4065 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/rename_protected.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.121127 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/widget/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/widget/__init__.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      372 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/widget/configure.zcml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      965 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/widget/password.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1875 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/browser/widget/password_input.pt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      343 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/config.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2526 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/configure.zcml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     5450 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/events.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1707 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/exceptions.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      105 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/interfaces.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      290 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/overrides.zcml
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.113127 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.121127 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/default/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      997 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/default/actions.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      150 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/default/browserlayer.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       68 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/default/metadata.xml
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.125127 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/test_fixture/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      241 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/test_fixture/metadata.xml
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.125127 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/test_fixture/types/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2156 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/test_fixture/types/folderish_not_protected.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2418 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/test_fixture/types/folderish_protected.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      313 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/test_fixture/types.xml
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.125127 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/uninstall/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      301 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/uninstall/actions.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       82 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1190 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/setuphandlers.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.125127 collective_folderprotection-2.4.3/src/collective_folderprotection/static/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1520 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/static/lock_locked_128.png
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      320 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/static/lock_locked_16.png
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1544 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/static/lock_unlocked_128.png
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      308 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/static/lock_unlocked_16.png
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1869 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/testing.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.125127 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        2 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/__init__.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.125127 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/robot/
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     4310 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/robot/keywords.robot
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     4021 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/robot/manager_functional.robot
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     6143 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/robot/member_functional.robot
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2922 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/robot/owner_functional.robot
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     2474 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_delprotect.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3602 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_passwordprotect.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3121 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_renameprotect.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      783 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_robot.py
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      544 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_setup.py
+drwxrwxr-x   0 frapell   (1000) frapell   (1000)        0 2024-04-18 22:23:08.125127 collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/
+-rw-r--r--   0 frapell   (1000) frapell   (1000)     7489 2024-04-18 22:23:08.000000 collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/PKG-INFO
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     3734 2024-04-18 22:23:08.000000 collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/SOURCES.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        1 2024-04-18 22:23:08.000000 collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/dependency_links.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       40 2024-04-18 22:23:08.000000 collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/entry_points.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)        1 2024-04-18 22:23:08.000000 collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/not-zip-safe
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      229 2024-04-18 22:23:08.000000 collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/requires.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       28 2024-04-18 22:23:08.000000 collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/top_level.txt
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      331 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/tests-5.2.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)     1163 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/tests-6.0.x.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      629 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/tox.ini
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)      140 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/travis.cfg
+-rw-rw-r--   0 frapell   (1000) frapell   (1000)       67 2024-04-18 22:23:07.000000 collective_folderprotection-2.4.3/versions.cfg
```

### Comparing `collective_folderprotection-2.4.2/.travis.yml` & `collective_folderprotection-2.4.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/CHANGES.txt` & `collective_folderprotection-2.4.3/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.4.3 (2024-04-18)
+++++++++++++++++++
+
+- Add a bit of logging
+  [frapell]
+
+
 2.4.2 (2024-04-17)
 ++++++++++++++++++
 
 - Only set a status message when there is a request
   [frapell]
```

### Comparing `collective_folderprotection-2.4.2/PKG-INFO` & `collective_folderprotection-2.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective_folderprotection
-Version: 2.4.2
+Version: 2.4.3
 Summary: Provide delete, rename and password protection for Plone items.
 Home-page: https://github.com/collective/collective_folderprotection
 Author: Enfold Systems, Inc.
 Author-email: info@enfoldsystems.com
 License: gpl
 Keywords: folder protection plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -118,14 +118,21 @@
 - Franco Pellegrini, Original Author
 
 Lock Icons provided by http://www.danilodemarco.com/
 
 Changelog
 =========
 
+2.4.3 (2024-04-18)
+++++++++++++++++++
+
+- Add a bit of logging
+  [frapell]
+
+
 2.4.2 (2024-04-17)
 ++++++++++++++++++
 
 - Only set a status message when there is a request
   [frapell]
```

### Comparing `collective_folderprotection-2.4.2/README.rst` & `collective_folderprotection-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/README.txt` & `collective_folderprotection-2.4.3/README.txt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/base.cfg` & `collective_folderprotection-2.4.3/base.cfg`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/buildout.cfg` & `collective_folderprotection-2.4.3/buildout.cfg`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/dev.cfg` & `collective_folderprotection-2.4.3/dev.cfg`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/docs/LICENSE.GPL` & `collective_folderprotection-2.4.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/docs/LICENSE.txt` & `collective_folderprotection-2.4.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/setup.py` & `collective_folderprotection-2.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = '2.4.2'
+version = '2.4.3'
 
 long_description = (
     open('README.txt').read()
     + '\n' +
     open('CONTRIBUTORS.txt').read()
     + '\n' +
     open('CHANGES.txt').read()
```

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/configure.zcml` & `collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/interfaces.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/behaviors/passwordprotected.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/behaviors/passwordprotected.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 # -*- coding: utf-8 -*-
+import logging
 import six
 from datetime import datetime
 from hashlib import md5
 
 from zope.annotation import IAnnotations
 
 from collective_folderprotection.config import HASHES_ANNOTATION_KEY
 from collective_folderprotection.config import HASH_COOKIE_KEY
 
+logger = logging.getLogger(__name__)
 
 class PasswordProtected(object):
     def __init__(self, context):
         self.context = context
 
     def is_password_protected(self):
         return getattr(self.context, "passw_hash", False)
 
     def allowed_to_access(self):
         allowed = False
         request = self.context.REQUEST
         ann = IAnnotations(self.context)
         hashes = ann.get(HASHES_ANNOTATION_KEY, {})
         user_hash = request.cookies.get(HASH_COOKIE_KEY, None)
+        logger.debug("Cookie hash: %s" % user_hash)
+        logger.debug("Stored hashes: %s" % hashes.keys())
 
         if user_hash and user_hash in hashes:
             now = datetime.now()
             valid_until = hashes[user_hash]
             allowed = valid_until > now
-
+        if allowed:
+            logger.debug("User allowed to access protected resource")
+        else:
+            logger.debug("User blocked access to protected resource")
         return allowed
 
     def _assign_password(self, passw=None):
         ann = IAnnotations(self.context)
 
         if passw:
             # If there's a password, assign it
```

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/alert_viewlet.pt` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/alert_viewlet.pt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/alert_viewlet.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/alert_viewlet.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/configure.zcml` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/delete_protected.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/delete_protected.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/passwordprotected.pt` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/passwordprotected.pt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/passwordprotected.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/passwordprotected.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import logging
 import six
 from hashlib import md5
 from datetime import datetime
 from random import random
 
 from z3c.form import button
 from z3c.form import field
@@ -26,14 +27,15 @@
 
 from collective_folderprotection.behaviors.interfaces import IPasswordProtected
 from collective_folderprotection.config import HASHES_ANNOTATION_KEY
 from collective_folderprotection.config import HASH_COOKIE_KEY
 from collective_folderprotection.config import TIME_TO_LIVE
 from collective_folderprotection import _
 
+logger = logging.getLogger(__name__)
 
 class RenderPasswordView(BrowserView):
     def __call__(self):
         self.came_from = self.request.get("URL")
 
         self.request.set("came_from", self.came_from)
         # Get the object for which we need to get access to
@@ -114,14 +116,15 @@
                         # Save the hash in a cookie
                         path = context.getPhysicalPath()
                         virtual_path = self.request.physicalPathToVirtualPath(path)
                         options = {
                             "path": "/".join(("",) + virtual_path),
                             "expires": (DateTime("GMT") + 5).rfc822(),
                         }
+                        logger.debug("Valid password, setting cookie")
                         self.request.response.setCookie(
                             HASH_COOKIE_KEY, random_hash, **options
                         )
                         # Now that we have our cookie set, go to
                         # the original url
                         self.request.response.redirect(came_from)
                         return
```

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/reason_viewlet.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/reason_viewlet.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/rename_protected.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/rename_protected.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/widget/password.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/widget/password.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/browser/widget/password_input.pt` & `collective_folderprotection-2.4.3/src/collective_folderprotection/browser/widget/password_input.pt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/configure.zcml` & `collective_folderprotection-2.4.3/src/collective_folderprotection/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/events.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/events.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/exceptions.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/exceptions.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/default/actions.xml` & `collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/test_fixture/types/folderish_not_protected.xml` & `collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/test_fixture/types/folderish_not_protected.xml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/profiles/test_fixture/types/folderish_protected.xml` & `collective_folderprotection-2.4.3/src/collective_folderprotection/profiles/test_fixture/types/folderish_protected.xml`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/setuphandlers.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/static/lock_locked_128.png` & `collective_folderprotection-2.4.3/src/collective_folderprotection/static/lock_locked_128.png`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/static/lock_unlocked_128.png` & `collective_folderprotection-2.4.3/src/collective_folderprotection/static/lock_unlocked_128.png`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/testing.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/testing.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/tests/robot/keywords.robot` & `collective_folderprotection-2.4.3/src/collective_folderprotection/tests/robot/keywords.robot`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/tests/robot/manager_functional.robot` & `collective_folderprotection-2.4.3/src/collective_folderprotection/tests/robot/manager_functional.robot`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/tests/robot/member_functional.robot` & `collective_folderprotection-2.4.3/src/collective_folderprotection/tests/robot/member_functional.robot`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/tests/robot/owner_functional.robot` & `collective_folderprotection-2.4.3/src/collective_folderprotection/tests/robot/owner_functional.robot`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_delprotect.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_delprotect.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_passwordprotect.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_passwordprotect.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_renameprotect.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_renameprotect.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_robot.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection/tests/test_setup.py` & `collective_folderprotection-2.4.3/src/collective_folderprotection/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/PKG-INFO` & `collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective_folderprotection
-Version: 2.4.2
+Version: 2.4.3
 Summary: Provide delete, rename and password protection for Plone items.
 Home-page: https://github.com/collective/collective_folderprotection
 Author: Enfold Systems, Inc.
 Author-email: info@enfoldsystems.com
 License: gpl
 Keywords: folder protection plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -118,14 +118,21 @@
 - Franco Pellegrini, Original Author
 
 Lock Icons provided by http://www.danilodemarco.com/
 
 Changelog
 =========
 
+2.4.3 (2024-04-18)
+++++++++++++++++++
+
+- Add a bit of logging
+  [frapell]
+
+
 2.4.2 (2024-04-17)
 ++++++++++++++++++
 
 - Only set a status message when there is a request
   [frapell]
```

### Comparing `collective_folderprotection-2.4.2/src/collective_folderprotection.egg-info/SOURCES.txt` & `collective_folderprotection-2.4.3/src/collective_folderprotection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/tests-6.0.x.cfg` & `collective_folderprotection-2.4.3/tests-6.0.x.cfg`

 * *Files identical despite different names*

### Comparing `collective_folderprotection-2.4.2/tox.ini` & `collective_folderprotection-2.4.3/tox.ini`

 * *Files identical despite different names*

