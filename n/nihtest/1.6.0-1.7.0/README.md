# Comparing `tmp/nihtest-1.6.0.tar.gz` & `tmp/nihtest-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nihtest-1.6.0.tar", last modified: Wed Apr 10 09:27:50 2024, max compression
+gzip compressed data, was "nihtest-1.7.0.tar", last modified: Fri Apr 19 13:30:22 2024, max compression
```

## Comparing `nihtest-1.6.0.tar` & `nihtest-1.7.0.tar`

### file list

```diff
@@ -1,160 +1,164 @@
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.195079 nihtest-1.6.0/
--rw-r--r--   0 dillo      (501) staff       (20)      993 2024-04-10 09:25:50.000000 nihtest-1.6.0/CMakeLists.txt
--rw-r--r--   0 dillo      (501) staff       (20)     1406 2023-03-22 09:46:53.000000 nihtest-1.6.0/LICENSE
--rw-r--r--   0 dillo      (501) staff       (20)      168 2023-06-27 09:50:58.000000 nihtest-1.6.0/MANIFEST.in
--rw-r--r--   0 dillo      (501) staff       (20)      927 2024-04-10 09:25:07.000000 nihtest-1.6.0/NEWS.md
--rw-r--r--   0 dillo      (501) staff       (20)     1559 2024-04-10 09:27:50.195007 nihtest-1.6.0/PKG-INFO
--rw-r--r--   0 dillo      (501) staff       (20)      969 2023-07-01 07:17:52.000000 nihtest-1.6.0/README.md
--rw-r--r--   0 dillo      (501) staff       (20)      145 2024-01-03 16:10:59.000000 nihtest-1.6.0/TODO.md
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.172517 nihtest-1.6.0/manpages/
--rw-r--r--   0 dillo      (501) staff       (20)      576 2023-06-09 14:53:27.000000 nihtest-1.6.0/manpages/Makefile
--rw-r--r--   0 dillo      (501) staff       (20)    11543 2024-04-10 09:27:24.000000 nihtest-1.6.0/manpages/nihtest-case.html
--rw-r--r--   0 dillo      (501) staff       (20)     6783 2024-04-10 09:27:24.000000 nihtest-1.6.0/manpages/nihtest-case.man
--rw-r--r--   0 dillo      (501) staff       (20)     6638 2024-04-10 09:25:07.000000 nihtest-1.6.0/manpages/nihtest-case.mdoc
--rw-r--r--   0 dillo      (501) staff       (20)    13046 2024-04-10 09:23:20.000000 nihtest-1.6.0/manpages/nihtest.conf.html
--rw-r--r--   0 dillo      (501) staff       (20)     7613 2024-04-10 09:23:20.000000 nihtest-1.6.0/manpages/nihtest.conf.man
--rw-r--r--   0 dillo      (501) staff       (20)     7262 2024-01-03 16:08:10.000000 nihtest-1.6.0/manpages/nihtest.conf.mdoc
--rw-r--r--   0 dillo      (501) staff       (20)     7738 2024-04-10 09:23:20.000000 nihtest-1.6.0/manpages/nihtest.html
--rw-r--r--   0 dillo      (501) staff       (20)     4599 2024-04-10 09:23:20.000000 nihtest-1.6.0/manpages/nihtest.man
--rw-r--r--   0 dillo      (501) staff       (20)     4141 2023-06-09 14:24:21.000000 nihtest-1.6.0/manpages/nihtest.mdoc
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.174515 nihtest-1.6.0/nihtest/
--rw-r--r--   0 dillo      (501) staff       (20)     1361 2023-11-20 16:45:16.000000 nihtest-1.6.0/nihtest/Command.py
--rw-r--r--   0 dillo      (501) staff       (20)     4976 2023-04-17 17:35:22.000000 nihtest-1.6.0/nihtest/CompareArrays.py
--rw-r--r--   0 dillo      (501) staff       (20)     5831 2024-01-03 10:20:32.000000 nihtest-1.6.0/nihtest/Configuration.py
--rw-r--r--   0 dillo      (501) staff       (20)     1059 2023-06-28 11:07:23.000000 nihtest-1.6.0/nihtest/Environment.py
--rw-r--r--   0 dillo      (501) staff       (20)      667 2023-04-24 10:05:06.000000 nihtest-1.6.0/nihtest/Features.py
--rw-r--r--   0 dillo      (501) staff       (20)     5236 2024-04-10 09:02:06.000000 nihtest-1.6.0/nihtest/File.py
--rw-r--r--   0 dillo      (501) staff       (20)      359 2024-03-27 16:58:56.000000 nihtest-1.6.0/nihtest/Output.py
--rw-r--r--   0 dillo      (501) staff       (20)     1291 2023-12-27 15:18:23.000000 nihtest-1.6.0/nihtest/Sandbox.py
--rw-r--r--   0 dillo      (501) staff       (20)     6922 2024-04-10 09:17:51.000000 nihtest-1.6.0/nihtest/Test.py
--rw-r--r--   0 dillo      (501) staff       (20)    11504 2024-04-10 09:17:27.000000 nihtest-1.6.0/nihtest/TestCase.py
--rw-r--r--   0 dillo      (501) staff       (20)      690 2024-04-10 09:02:06.000000 nihtest-1.6.0/nihtest/Utility.py
--rw-r--r--   0 dillo      (501) staff       (20)        0 2023-03-22 10:19:23.000000 nihtest-1.6.0/nihtest/__init__.py
--rw-r--r--   0 dillo      (501) staff       (20)     1361 2024-04-10 09:25:50.000000 nihtest-1.6.0/nihtest/__main__.py
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.194741 nihtest-1.6.0/nihtest.egg-info/
--rw-r--r--   0 dillo      (501) staff       (20)     1559 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/PKG-INFO
--rw-r--r--   0 dillo      (501) staff       (20)     3767 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/SOURCES.txt
--rw-r--r--   0 dillo      (501) staff       (20)        1 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/dependency_links.txt
--rw-r--r--   0 dillo      (501) staff       (20)       50 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/entry_points.txt
--rw-r--r--   0 dillo      (501) staff       (20)       16 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/requires.txt
--rw-r--r--   0 dillo      (501) staff       (20)        8 2024-04-10 09:27:50.000000 nihtest-1.6.0/nihtest.egg-info/top_level.txt
--rw-r--r--   0 dillo      (501) staff       (20)     1018 2024-04-10 09:25:50.000000 nihtest-1.6.0/pyproject.toml
--rw-r--r--   0 dillo      (501) staff       (20)       76 2024-04-10 09:27:50.195308 nihtest-1.6.0/setup.cfg
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-10 09:27:50.194534 nihtest-1.6.0/tests/
--rw-r--r--   0 dillo      (501) staff       (20)     2216 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/CMakeLists.txt
--rw-r--r--   0 dillo      (501) staff       (20)      143 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/argument-escaped.input
--rw-r--r--   0 dillo      (501) staff       (20)      138 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/argument-escaped.test
--rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/binary-1
--rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/binary-2
--rw-r--r--   0 dillo      (501) staff       (20)     1808 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/can-preload.c
--rw-r--r--   0 dillo      (501) staff       (20)     2539 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/cat.c
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-05-19 12:10:40.000000 nihtest-1.6.0/tests/comparator-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      305 2023-05-19 12:16:34.000000 nihtest-1.6.0/tests/comparator-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       66 2023-05-19 12:12:53.000000 nihtest-1.6.0/tests/comparator-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      219 2023-05-19 12:10:40.000000 nihtest-1.6.0/tests/comparator-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-06-27 10:06:35.000000 nihtest-1.6.0/tests/comparator-preprocess.input
--rw-r--r--   0 dillo      (501) staff       (20)      290 2023-06-28 10:48:16.000000 nihtest-1.6.0/tests/comparator-preprocess.test
--rw-r--r--   0 dillo      (501) staff       (20)     1590 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/comparator.c
--rw-r--r--   0 dillo      (501) staff       (20)       65 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/compare-binary-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      279 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/compare-binary-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       56 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/compare-binary-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      140 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/compare-binary-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       64 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/config.h
--rw-r--r--   0 dillo      (501) staff       (20)      104 2024-01-03 10:11:30.000000 nihtest-1.6.0/tests/copier.input
--rw-r--r--   0 dillo      (501) staff       (20)      160 2024-01-03 10:12:56.000000 nihtest-1.6.0/tests/copier.test
--rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/default-stderr-replace.input
--rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-09 14:24:21.000000 nihtest-1.6.0/tests/default-stderr-replace.test
--rw-r--r--   0 dillo      (501) staff       (20)     1755 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/delete.c
--rw-r--r--   0 dillo      (501) staff       (20)     1651 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/delete.h
--rw-r--r--   0 dillo      (501) staff       (20)      103 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/description-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      136 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/diff-1.input
--rw-r--r--   0 dillo      (501) staff       (20)      250 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/diff-1.test
--rw-r--r--   0 dillo      (501) staff       (20)      106 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/diff-2.input
--rw-r--r--   0 dillo      (501) staff       (20)      220 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/diff-2.test
--rw-r--r--   0 dillo      (501) staff       (20)     1963 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/echo.c
--rw-r--r--   0 dillo      (501) staff       (20)       82 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/empty-lines.txt
--rw-r--r--   0 dillo      (501) staff       (20)      103 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-clear-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-clear-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       99 2023-06-28 11:05:36.000000 nihtest-1.6.0/tests/environment-not-passed-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      172 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-not-passed-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      155 2023-06-28 11:07:43.000000 nihtest-1.6.0/tests/environment-passthrough-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      173 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-passthrough-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      133 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-set-config-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-set-config-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      167 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-set-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      118 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-set-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      108 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-unset-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/environment-unset-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/failure.txt
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/false-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      237 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/false-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/false-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/false-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1664 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/false.c
--rw-r--r--   0 dillo      (501) staff       (20)       62 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/features-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      275 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/features-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/features-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      152 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/features-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/features-skip.input
--rw-r--r--   0 dillo      (501) staff       (20)      153 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/features-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/file-del-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      285 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/file-del-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      131 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/file-del-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      158 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/file-del-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       68 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/file-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      289 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/file-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      398 2023-04-15 14:27:28.000000 nihtest-1.6.0/tests/file-inline-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      362 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/file-inline-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      280 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/file-inline-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      142 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/file-inline-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/file-new-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      256 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/file-new-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      111 2023-04-12 10:55:14.000000 nihtest-1.6.0/tests/file-new-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/file-new-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:53:21.000000 nihtest-1.6.0/tests/file-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/file-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      165 2023-04-12 11:02:07.000000 nihtest-1.6.0/tests/file-subdirectory-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      156 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/file-subdirectory-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     3310 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/file.c
--rw-r--r--   0 dillo      (501) staff       (20)     2138 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/getenv.c
--rw-r--r--   0 dillo      (501) staff       (20)     1756 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/ineffective-delete.c
--rw-r--r--   0 dillo      (501) staff       (20)      508 2024-01-03 10:08:16.000000 nihtest-1.6.0/tests/nihtest-conf.in
--rw-r--r--   0 dillo      (501) staff       (20)      236 2023-06-27 09:50:58.000000 nihtest-1.6.0/tests/nihtest.conf.in
--rw-r--r--   0 dillo      (501) staff       (20)      415 2023-06-15 13:24:22.000000 nihtest-1.6.0/tests/parameter-tests-1.input
--rw-r--r--   0 dillo      (501) staff       (20)     1696 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/parameter-tests-1.test
--rw-r--r--   0 dillo      (501) staff       (20)       79 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/parameter-tests-2.input
--rw-r--r--   0 dillo      (501) staff       (20)      389 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/parameter-tests-2.test
--rw-r--r--   0 dillo      (501) staff       (20)       53 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/precheck-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      252 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/precheck-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       52 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/precheck-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/precheck-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       54 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/precheck-skip.input
--rw-r--r--   0 dillo      (501) staff       (20)      130 2023-04-12 12:29:19.000000 nihtest-1.6.0/tests/precheck-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)      174 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/preload-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      161 2023-04-12 13:00:35.000000 nihtest-1.6.0/tests/preload-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      163 2023-04-12 13:00:35.000000 nihtest-1.6.0/tests/preload-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)      127 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stderr-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      302 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/stderr-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stderr-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stderr-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      211 2023-04-12 11:16:36.000000 nihtest-1.6.0/tests/stderr-replace-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      147 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stderr-replace-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      112 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stdin-file-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      135 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stdin-file-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      146 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stdin-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stdin-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      124 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stdout-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      290 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/stdout-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/stdout-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/stdout-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      208 2024-04-10 09:19:57.000000 nihtest-1.6.0/tests/stdout-replace-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      117 2024-04-10 09:19:57.000000 nihtest-1.6.0/tests/stdout-replace-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       27 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/success.txt
--rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/true-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      232 2024-04-10 09:13:34.000000 nihtest-1.6.0/tests/true-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.6.0/tests/true-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.6.0/tests/true-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1785 2023-06-28 09:11:26.000000 nihtest-1.6.0/tests/true.c
--rw-r--r--   0 dillo      (501) staff       (20)     2546 2024-03-15 10:00:51.000000 nihtest-1.6.0/tests/uppercase.c
--rw-r--r--   0 dillo      (501) staff       (20)      251 2023-12-27 15:28:23.000000 nihtest-1.6.0/tests/working-directory.input
--rw-r--r--   0 dillo      (501) staff       (20)      115 2023-12-27 15:21:44.000000 nihtest-1.6.0/tests/working-directory.test
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-19 13:30:22.282809 nihtest-1.7.0/
+-rw-r--r--   0 dillo      (501) staff       (20)      993 2024-04-19 13:29:49.000000 nihtest-1.7.0/CMakeLists.txt
+-rw-r--r--   0 dillo      (501) staff       (20)     1406 2023-03-22 09:46:53.000000 nihtest-1.7.0/LICENSE
+-rw-r--r--   0 dillo      (501) staff       (20)      168 2023-06-27 09:50:58.000000 nihtest-1.7.0/MANIFEST.in
+-rw-r--r--   0 dillo      (501) staff       (20)     1036 2024-04-19 13:28:45.000000 nihtest-1.7.0/NEWS.md
+-rw-r--r--   0 dillo      (501) staff       (20)     1559 2024-04-19 13:30:22.282734 nihtest-1.7.0/PKG-INFO
+-rw-r--r--   0 dillo      (501) staff       (20)      969 2023-07-01 07:17:52.000000 nihtest-1.7.0/README.md
+-rw-r--r--   0 dillo      (501) staff       (20)      145 2024-01-03 16:10:59.000000 nihtest-1.7.0/TODO.md
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-19 13:30:22.260045 nihtest-1.7.0/manpages/
+-rw-r--r--   0 dillo      (501) staff       (20)      576 2023-06-09 14:53:27.000000 nihtest-1.7.0/manpages/Makefile
+-rw-r--r--   0 dillo      (501) staff       (20)    11543 2024-04-10 09:27:24.000000 nihtest-1.7.0/manpages/nihtest-case.html
+-rw-r--r--   0 dillo      (501) staff       (20)     6783 2024-04-10 09:27:24.000000 nihtest-1.7.0/manpages/nihtest-case.man
+-rw-r--r--   0 dillo      (501) staff       (20)     6788 2024-04-19 13:22:41.000000 nihtest-1.7.0/manpages/nihtest-case.mdoc
+-rw-r--r--   0 dillo      (501) staff       (20)    13046 2024-04-10 09:23:20.000000 nihtest-1.7.0/manpages/nihtest.conf.html
+-rw-r--r--   0 dillo      (501) staff       (20)     7613 2024-04-10 09:23:20.000000 nihtest-1.7.0/manpages/nihtest.conf.man
+-rw-r--r--   0 dillo      (501) staff       (20)     7262 2024-01-03 16:08:10.000000 nihtest-1.7.0/manpages/nihtest.conf.mdoc
+-rw-r--r--   0 dillo      (501) staff       (20)     7738 2024-04-10 09:23:20.000000 nihtest-1.7.0/manpages/nihtest.html
+-rw-r--r--   0 dillo      (501) staff       (20)     4599 2024-04-10 09:23:20.000000 nihtest-1.7.0/manpages/nihtest.man
+-rw-r--r--   0 dillo      (501) staff       (20)     4141 2023-06-09 14:24:21.000000 nihtest-1.7.0/manpages/nihtest.mdoc
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-19 13:30:22.262085 nihtest-1.7.0/nihtest/
+-rw-r--r--   0 dillo      (501) staff       (20)     1361 2023-11-20 16:45:16.000000 nihtest-1.7.0/nihtest/Command.py
+-rw-r--r--   0 dillo      (501) staff       (20)     4976 2023-04-17 17:35:22.000000 nihtest-1.7.0/nihtest/CompareArrays.py
+-rw-r--r--   0 dillo      (501) staff       (20)     5831 2024-01-03 10:20:32.000000 nihtest-1.7.0/nihtest/Configuration.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1059 2023-06-28 11:07:23.000000 nihtest-1.7.0/nihtest/Environment.py
+-rw-r--r--   0 dillo      (501) staff       (20)      667 2023-04-24 10:05:06.000000 nihtest-1.7.0/nihtest/Features.py
+-rw-r--r--   0 dillo      (501) staff       (20)     5236 2024-04-10 09:02:06.000000 nihtest-1.7.0/nihtest/File.py
+-rw-r--r--   0 dillo      (501) staff       (20)      359 2024-03-27 16:58:56.000000 nihtest-1.7.0/nihtest/Output.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1291 2023-12-27 15:18:23.000000 nihtest-1.7.0/nihtest/Sandbox.py
+-rw-r--r--   0 dillo      (501) staff       (20)     6925 2024-04-19 13:18:16.000000 nihtest-1.7.0/nihtest/Test.py
+-rw-r--r--   0 dillo      (501) staff       (20)    11889 2024-04-19 13:13:36.000000 nihtest-1.7.0/nihtest/TestCase.py
+-rw-r--r--   0 dillo      (501) staff       (20)      690 2024-04-10 09:02:06.000000 nihtest-1.7.0/nihtest/Utility.py
+-rw-r--r--   0 dillo      (501) staff       (20)        0 2023-03-22 10:19:23.000000 nihtest-1.7.0/nihtest/__init__.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1361 2024-04-19 13:29:49.000000 nihtest-1.7.0/nihtest/__main__.py
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-19 13:30:22.282488 nihtest-1.7.0/nihtest.egg-info/
+-rw-r--r--   0 dillo      (501) staff       (20)     1559 2024-04-19 13:30:22.000000 nihtest-1.7.0/nihtest.egg-info/PKG-INFO
+-rw-r--r--   0 dillo      (501) staff       (20)     3868 2024-04-19 13:30:22.000000 nihtest-1.7.0/nihtest.egg-info/SOURCES.txt
+-rw-r--r--   0 dillo      (501) staff       (20)        1 2024-04-19 13:30:22.000000 nihtest-1.7.0/nihtest.egg-info/dependency_links.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       50 2024-04-19 13:30:22.000000 nihtest-1.7.0/nihtest.egg-info/entry_points.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       16 2024-04-19 13:30:22.000000 nihtest-1.7.0/nihtest.egg-info/requires.txt
+-rw-r--r--   0 dillo      (501) staff       (20)        8 2024-04-19 13:30:22.000000 nihtest-1.7.0/nihtest.egg-info/top_level.txt
+-rw-r--r--   0 dillo      (501) staff       (20)     1018 2024-04-19 13:29:49.000000 nihtest-1.7.0/pyproject.toml
+-rw-r--r--   0 dillo      (501) staff       (20)       76 2024-04-19 13:30:22.283032 nihtest-1.7.0/setup.cfg
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2024-04-19 13:30:22.282319 nihtest-1.7.0/tests/
+-rw-r--r--   0 dillo      (501) staff       (20)     2216 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/CMakeLists.txt
+-rw-r--r--   0 dillo      (501) staff       (20)      143 2023-06-09 14:24:21.000000 nihtest-1.7.0/tests/argument-escaped.input
+-rw-r--r--   0 dillo      (501) staff       (20)      138 2023-06-09 14:24:21.000000 nihtest-1.7.0/tests/argument-escaped.test
+-rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.7.0/tests/binary-1
+-rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.7.0/tests/binary-2
+-rw-r--r--   0 dillo      (501) staff       (20)     1808 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/can-preload.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2539 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/cat.c
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-05-19 12:10:40.000000 nihtest-1.7.0/tests/comparator-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      305 2023-05-19 12:16:34.000000 nihtest-1.7.0/tests/comparator-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       66 2023-05-19 12:12:53.000000 nihtest-1.7.0/tests/comparator-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      219 2023-05-19 12:10:40.000000 nihtest-1.7.0/tests/comparator-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-06-27 10:06:35.000000 nihtest-1.7.0/tests/comparator-preprocess.input
+-rw-r--r--   0 dillo      (501) staff       (20)      290 2023-06-28 10:48:16.000000 nihtest-1.7.0/tests/comparator-preprocess.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1590 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/comparator.c
+-rw-r--r--   0 dillo      (501) staff       (20)       65 2023-06-09 14:24:21.000000 nihtest-1.7.0/tests/compare-binary-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      279 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/compare-binary-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       56 2023-06-09 14:24:21.000000 nihtest-1.7.0/tests/compare-binary-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      140 2023-06-09 14:24:21.000000 nihtest-1.7.0/tests/compare-binary-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       64 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/config.h
+-rw-r--r--   0 dillo      (501) staff       (20)      104 2024-01-03 10:11:30.000000 nihtest-1.7.0/tests/copier.input
+-rw-r--r--   0 dillo      (501) staff       (20)      160 2024-01-03 10:12:56.000000 nihtest-1.7.0/tests/copier.test
+-rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-09 14:24:21.000000 nihtest-1.7.0/tests/default-stderr-replace.input
+-rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-09 14:24:21.000000 nihtest-1.7.0/tests/default-stderr-replace.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1755 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/delete.c
+-rw-r--r--   0 dillo      (501) staff       (20)     1651 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/delete.h
+-rw-r--r--   0 dillo      (501) staff       (20)      103 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/description-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      136 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/diff-1.input
+-rw-r--r--   0 dillo      (501) staff       (20)      250 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/diff-1.test
+-rw-r--r--   0 dillo      (501) staff       (20)      106 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/diff-2.input
+-rw-r--r--   0 dillo      (501) staff       (20)      220 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/diff-2.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1963 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/echo.c
+-rw-r--r--   0 dillo      (501) staff       (20)       82 2023-06-28 09:11:26.000000 nihtest-1.7.0/tests/empty-lines.txt
+-rw-r--r--   0 dillo      (501) staff       (20)      103 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-clear-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-clear-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       99 2023-06-28 11:05:36.000000 nihtest-1.7.0/tests/environment-not-passed-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      172 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-not-passed-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      155 2023-06-28 11:07:43.000000 nihtest-1.7.0/tests/environment-passthrough-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      173 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-passthrough-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      133 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-set-config-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-set-config-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      167 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-set-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      118 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-set-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      108 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-unset-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/environment-unset-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/failure.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/false-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      237 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/false-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/false-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/false-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1664 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/false.c
+-rw-r--r--   0 dillo      (501) staff       (20)       62 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/features-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      275 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/features-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/features-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      152 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/features-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/features-skip.input
+-rw-r--r--   0 dillo      (501) staff       (20)      153 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/features-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/file-del-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      285 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/file-del-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      131 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/file-del-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      158 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/file-del-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       68 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/file-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      289 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/file-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      398 2023-04-15 14:27:28.000000 nihtest-1.7.0/tests/file-inline-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      362 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/file-inline-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      280 2023-06-28 09:11:26.000000 nihtest-1.7.0/tests/file-inline-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      142 2023-06-28 09:11:26.000000 nihtest-1.7.0/tests/file-inline-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/file-new-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      256 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/file-new-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      111 2023-04-12 10:55:14.000000 nihtest-1.7.0/tests/file-new-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/file-new-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:53:21.000000 nihtest-1.7.0/tests/file-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/file-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      165 2023-04-12 11:02:07.000000 nihtest-1.7.0/tests/file-subdirectory-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      156 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/file-subdirectory-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     3310 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/file.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2138 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/getenv.c
+-rw-r--r--   0 dillo      (501) staff       (20)     1756 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/ineffective-delete.c
+-rw-r--r--   0 dillo      (501) staff       (20)      508 2024-01-03 10:08:16.000000 nihtest-1.7.0/tests/nihtest-conf.in
+-rw-r--r--   0 dillo      (501) staff       (20)      236 2023-06-27 09:50:58.000000 nihtest-1.7.0/tests/nihtest.conf.in
+-rw-r--r--   0 dillo      (501) staff       (20)      415 2023-06-15 13:24:22.000000 nihtest-1.7.0/tests/parameter-tests-1.input
+-rw-r--r--   0 dillo      (501) staff       (20)     1696 2023-06-28 09:11:26.000000 nihtest-1.7.0/tests/parameter-tests-1.test
+-rw-r--r--   0 dillo      (501) staff       (20)       79 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/parameter-tests-2.input
+-rw-r--r--   0 dillo      (501) staff       (20)      389 2023-06-28 09:11:26.000000 nihtest-1.7.0/tests/parameter-tests-2.test
+-rw-r--r--   0 dillo      (501) staff       (20)       53 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/precheck-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      252 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/precheck-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       52 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/precheck-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/precheck-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       54 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/precheck-skip.input
+-rw-r--r--   0 dillo      (501) staff       (20)      130 2023-04-12 12:29:19.000000 nihtest-1.7.0/tests/precheck-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)      174 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/preload-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      161 2023-04-12 13:00:35.000000 nihtest-1.7.0/tests/preload-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      163 2023-04-12 13:00:35.000000 nihtest-1.7.0/tests/preload-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2024-04-19 10:37:32.000000 nihtest-1.7.0/tests/quiet-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2024-04-19 10:13:58.000000 nihtest-1.7.0/tests/quiet-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      127 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/stderr-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      302 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/stderr-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/stderr-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/stderr-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      211 2023-04-12 11:16:36.000000 nihtest-1.7.0/tests/stderr-replace-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      147 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/stderr-replace-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      112 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/stdin-file-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      135 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/stdin-file-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      146 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/stdin-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/stdin-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      124 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/stdout-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      290 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/stdout-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/stdout-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/stdout-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      208 2024-04-10 09:19:57.000000 nihtest-1.7.0/tests/stdout-replace-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2024-04-10 09:19:57.000000 nihtest-1.7.0/tests/stdout-replace-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       27 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/success.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       60 2024-04-19 13:22:41.000000 nihtest-1.7.0/tests/test-case-source.input
+-rw-r--r--   0 dillo      (501) staff       (20)      221 2024-04-19 13:27:11.000000 nihtest-1.7.0/tests/test-case-source.test
+-rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/true-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      232 2024-04-10 09:13:34.000000 nihtest-1.7.0/tests/true-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.7.0/tests/true-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.7.0/tests/true-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1785 2023-06-28 09:11:26.000000 nihtest-1.7.0/tests/true.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2546 2024-03-15 10:00:51.000000 nihtest-1.7.0/tests/uppercase.c
+-rw-r--r--   0 dillo      (501) staff       (20)      251 2023-12-27 15:28:23.000000 nihtest-1.7.0/tests/working-directory.input
+-rw-r--r--   0 dillo      (501) staff       (20)      115 2023-12-27 15:21:44.000000 nihtest-1.7.0/tests/working-directory.test
```

### Comparing `nihtest-1.6.0/CMakeLists.txt` & `nihtest-1.7.0/CMakeLists.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cmake_minimum_required(VERSION 3.12)
 
 # Also update version in nihtest/__main__.py and pyproject.toml
 project(nihtest
-        VERSION 1.6.0
+        VERSION 1.7.0
         DESCRIPTION "NiH testing framework"
         HOMEPAGE_URL "https://github.com/nih-at/nihtest"
         LANGUAGES C)
 
 enable_testing()
 
 find_package(Python3 REQUIRED COMPONENTS Interpreter)
```

### Comparing `nihtest-1.6.0/LICENSE` & `nihtest-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/PKG-INFO` & `nihtest-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nihtest
-Version: 1.6.0
+Version: 1.7.0
 Summary: A testing tool for command line utilities.
 Author-email: Dieter Baron <dillo@nih.at>, Thomas Klausner <wiz@gatalith.at>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/nih-at/nihtest
 Project-URL: Bug Tracker, https://github.com/nih-at/nihtest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nihtest-1.6.0/README.md` & `nihtest-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/manpages/Makefile` & `nihtest-1.7.0/manpages/Makefile`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/manpages/nihtest-case.html` & `nihtest-1.7.0/manpages/nihtest-case.html`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/manpages/nihtest-case.man` & `nihtest-1.7.0/manpages/nihtest-case.man`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/manpages/nihtest-case.mdoc` & `nihtest-1.7.0/manpages/nihtest-case.mdoc`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,19 @@
 Run regular expression replacement over the standard output
 and the expected output as provided by
 .Ic stdout
 before comparing them.
 See
 .Ic stderr-replace
 for details.
+.It Ic test-case-source Ar filename
+Use
+.Ar filename
+to refer to test case in error messages.
+This is useful if the test case is created by a script.
 .\" .It Ic ulimit Ar C VALUE
 .\" Set
 .\" .Xr ulimit 1
 .\" flag
 .\" .Fl Ar C
 .\" to
 .\" .Ar VALUE
```

### Comparing `nihtest-1.6.0/manpages/nihtest.conf.html` & `nihtest-1.7.0/manpages/nihtest.conf.html`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/manpages/nihtest.conf.man` & `nihtest-1.7.0/manpages/nihtest.conf.man`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/manpages/nihtest.conf.mdoc` & `nihtest-1.7.0/manpages/nihtest.conf.mdoc`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/manpages/nihtest.html` & `nihtest-1.7.0/manpages/nihtest.html`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/manpages/nihtest.man` & `nihtest-1.7.0/manpages/nihtest.man`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/manpages/nihtest.mdoc` & `nihtest-1.7.0/manpages/nihtest.mdoc`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/nihtest/Command.py` & `nihtest-1.7.0/nihtest/Command.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/nihtest/CompareArrays.py` & `nihtest-1.7.0/nihtest/CompareArrays.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/nihtest/Configuration.py` & `nihtest-1.7.0/nihtest/Configuration.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/nihtest/Environment.py` & `nihtest-1.7.0/nihtest/Environment.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/nihtest/Features.py` & `nihtest-1.7.0/nihtest/Features.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/nihtest/File.py` & `nihtest-1.7.0/nihtest/File.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/nihtest/Sandbox.py` & `nihtest-1.7.0/nihtest/Sandbox.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/nihtest/Test.py` & `nihtest-1.7.0/nihtest/Test.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
         for file in self.case.read_only:
             full_file = os.path.join(self.sandbox.directory, file)
             if os.path.exists(full_file):
                 st = os.stat(full_file)
                 os.chmod(full_file, st.st_mode | stat.S_IWRITE)
 
-        output = Output.Output(self.case.file_name + ":1: test case failed", self.case.configuration.verbose != Configuration.When.NEVER)
+        output = Output.Output(self.case.test_case_source + ":1: test case failed", self.case.configuration.verbose != Configuration.When.NEVER)
 
         self.compare(output, "exit code", [str(self.case.exit_code)], [str(command.exit_code)])
         self.compare(output,"output", self.case.stdout, self.process_output_replace(command.stdout, self.case.stdout_replace))
         self.compare(output, "error output", self.case.stderr, self.process_output_replace(command.stderr, self.case.stderr_replace))
 
         files_expected = []
         for file in self.case.files:
@@ -125,15 +125,15 @@
         if self.case.configuration.keep_sandbox == Configuration.When.NEVER or (
                 self.case.configuration.keep_sandbox == Configuration.When.FAILED and not self.failed):
             self.sandbox.cleanup()
 
         if self.failed:
             if self.case.configuration.verbose != Configuration.When.NEVER:
                 print(self.case.name + " -- FAIL: " + ", ".join(self.failed))
-                return TestResult.FAILED
+            return TestResult.FAILED
         else:
             return TestResult.OK
 
     def compare(self, output, description, expected, got):
         if not Utility.compare_lines(output, description, expected, got):
             self.failed.append(description)
```

### Comparing `nihtest-1.6.0/nihtest/TestCase.py` & `nihtest-1.7.0/nihtest/TestCase.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         self.environment_clear = configuration.environment_clear
         self.environment_passthrough = configuration.environment_passthrough.copy()
         self.environment_unset = configuration.environment_unset.copy()
         file_name = args.testcase
         if file_name[-5:] != ".test":
             file_name += ".test"
         self.file_name = self.configuration.find_input_file(file_name)
+        self.test_case_source = self.file_name
         self.file = open(self.file_name, mode="r", encoding='utf-8')
         self.line_number = 0
         self.directives_seen = {}
         self.arguments = []
         self.description = ""
         self.features = []
         self.files = []
@@ -203,14 +204,17 @@
 
     def directive_stdout(self, arguments):
         self.stdout = self.io_data(arguments)
 
     def directive_stdout_replace(self, arguments):
         self.stdout_replace.append((re.compile(arguments[0]), arguments[1]))
 
+    def directive_test_case_source(self, arguments):
+        self.test_case_source = arguments[0]
+
     def directive_working_directory(self, arguments):
         self.working_directory = arguments[0]
 
     directives = {
         "arguments": Directive(method=directive_arguments,
                                usage="[argument ...]",
                                minimum_arguments=0, maximum_arguments=-1),
@@ -273,14 +277,18 @@
         "stdout": Directive(method=directive_stdout,
                             usage="[file]",
                             minimum_arguments=0, maximum_arguments=1,
                             only_once=True),
         "stdout-replace": Directive(method=directive_stdout_replace,
                                     usage="pattern replacement",
                                     minimum_arguments=2),
+        "test-case-source": Directive(method=directive_test_case_source,
+                                      usage="file",
+                                      minimum_arguments=1,
+                                      only_once=True),
         "working-directory": Directive(method=directive_working_directory,
                                        usage="directory",
                                        minimum_arguments=1,
                                        only_once=True)
     }
 
     def get_program_directories(self):
```

### Comparing `nihtest-1.6.0/nihtest/Utility.py` & `nihtest-1.7.0/nihtest/Utility.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/nihtest/__main__.py` & `nihtest-1.7.0/nihtest/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import sys
 
 from nihtest import Test
 from nihtest import Configuration
 
-VERSION = "1.6.0"
+VERSION = "1.7.0"
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog='nihtest',
         description="nihtest " + VERSION + "\nCopyright (C) 2023 Dieter Baron and Thomas Klausner")
     parser.add_argument('testcase', help='Testcase to run')
```

### Comparing `nihtest-1.6.0/nihtest.egg-info/PKG-INFO` & `nihtest-1.7.0/nihtest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nihtest
-Version: 1.6.0
+Version: 1.7.0
 Summary: A testing tool for command line utilities.
 Author-email: Dieter Baron <dillo@nih.at>, Thomas Klausner <wiz@gatalith.at>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/nih-at/nihtest
 Project-URL: Bug Tracker, https://github.com/nih-at/nihtest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nihtest-1.6.0/nihtest.egg-info/SOURCES.txt` & `nihtest-1.7.0/nihtest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,16 @@
 tests/precheck-pass.input
 tests/precheck-pass.test
 tests/precheck-skip.input
 tests/precheck-skip.test
 tests/preload-pass.input
 tests/preload-pass.test
 tests/preload-skip.test
+tests/quiet-fail.test
+tests/quiet-pass.test
 tests/stderr-fail.input
 tests/stderr-fail.test
 tests/stderr-pass.input
 tests/stderr-pass.test
 tests/stderr-replace-pass.input
 tests/stderr-replace-pass.test
 tests/stdin-file-pass.input
@@ -140,14 +142,16 @@
 tests/stdout-fail.input
 tests/stdout-fail.test
 tests/stdout-pass.input
 tests/stdout-pass.test
 tests/stdout-replace-pass.input
 tests/stdout-replace-pass.test
 tests/success.txt
+tests/test-case-source.input
+tests/test-case-source.test
 tests/true-fail.input
 tests/true-fail.test
 tests/true-pass.input
 tests/true-pass.test
 tests/true.c
 tests/uppercase.c
 tests/working-directory.input
```

### Comparing `nihtest-1.6.0/pyproject.toml` & `nihtest-1.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nihtest"
-version = "1.6.0"
+version = "1.7.0"
 authors = [
     { name="Dieter Baron", email="dillo@nih.at" },
     { name="Thomas Klausner", email="wiz@gatalith.at"}
 ]
 description = "A testing tool for command line utilities."
 license = {text = "BSD-3-Clause"}
 readme = "README.md"
@@ -26,15 +26,15 @@
 "Homepage" = "https://github.com/nih-at/nihtest"
 "Bug Tracker" = "https://github.com/nih-at/nihtest/issues"
 
 [project.scripts]
 nihtest = "nihtest.__main__:main"
 
 [tool.bumpver]
-current_version = "1.6.0"
+current_version = "1.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 
 [tool.bumpver.file_patterns]
 "nihtest/__main__.py" = [
     'VERSION = "{version}"'
 ]
 "pyproject.toml" = [
```

### Comparing `nihtest-1.6.0/tests/CMakeLists.txt` & `nihtest-1.7.0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/can-preload.c` & `nihtest-1.7.0/tests/can-preload.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/cat.c` & `nihtest-1.7.0/tests/cat.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/comparator.c` & `nihtest-1.7.0/tests/comparator.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/delete.c` & `nihtest-1.7.0/tests/delete.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/delete.h` & `nihtest-1.7.0/tests/delete.h`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/echo.c` & `nihtest-1.7.0/tests/echo.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/false.c` & `nihtest-1.7.0/tests/false.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/file.c` & `nihtest-1.7.0/tests/file.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/getenv.c` & `nihtest-1.7.0/tests/getenv.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/ineffective-delete.c` & `nihtest-1.7.0/tests/ineffective-delete.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/parameter-tests-1.test` & `nihtest-1.7.0/tests/parameter-tests-1.test`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/true.c` & `nihtest-1.7.0/tests/true.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.6.0/tests/uppercase.c` & `nihtest-1.7.0/tests/uppercase.c`

 * *Files identical despite different names*

