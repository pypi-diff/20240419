# Comparing `tmp/csoundengine-2.8.2.tar.gz` & `tmp/csoundengine-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csoundengine-2.8.2.tar", last modified: Wed Apr 17 09:31:32 2024, max compression
+gzip compressed data, was "csoundengine-2.8.3.tar", last modified: Fri Apr 19 13:24:18 2024, max compression
```

## Comparing `csoundengine-2.8.2.tar` & `csoundengine-2.8.3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.742738 csoundengine-2.8.2/
--rw-rw-r--   0 em        (1000) em        (1000)    35128 2021-11-13 21:37:59.000000 csoundengine-2.8.2/LICENSE.txt
--rw-rw-r--   0 em        (1000) em        (1000)       24 2021-11-13 21:37:59.000000 csoundengine-2.8.2/MANIFEST.in
--rw-rw-r--   0 em        (1000) em        (1000)     6142 2024-04-17 09:31:32.742738 csoundengine-2.8.2/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     5728 2024-01-10 12:24:51.000000 csoundengine-2.8.2/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.699737 csoundengine-2.8.2/csoundengine/
--rw-r--r--   0 em        (1000) em        (1000)     4116 2023-11-15 12:26:35.000000 csoundengine-2.8.2/csoundengine/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     1055 2023-03-14 09:38:54.000000 csoundengine-2.8.2/csoundengine/__sessionbase.py
--rw-r--r--   0 em        (1000) em        (1000)      177 2023-11-24 08:20:24.000000 csoundengine-2.8.2/csoundengine/_common.py
--rw-r--r--   0 em        (1000) em        (1000)     5978 2023-11-14 20:14:02.000000 csoundengine-2.8.2/csoundengine/abstractrenderer.py
--rw-r--r--   0 em        (1000) em        (1000)    11621 2024-02-21 14:58:04.000000 csoundengine-2.8.2/csoundengine/baseschedevent.py
--rw-rw-r--   0 em        (1000) em        (1000)     5848 2024-04-17 08:24:25.000000 csoundengine-2.8.2/csoundengine/busproxy.py
--rw-r--r--   0 em        (1000) em        (1000)     8213 2024-04-03 07:08:12.000000 csoundengine-2.8.2/csoundengine/config.py
--rw-rw-r--   0 em        (1000) em        (1000)        0 2023-10-17 11:02:49.000000 csoundengine-2.8.2/csoundengine/contants.py
--rwxr-xr-x   0 em        (1000) em        (1000)   126529 2024-04-10 06:06:37.000000 csoundengine-2.8.2/csoundengine/csoundlib.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.688737 csoundengine-2.8.2/csoundengine/data/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.688737 csoundengine-2.8.2/csoundengine/data/plugins6/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.704737 csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:27.000000 csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libbeosc.so
--rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:27.000000 csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libelse.so
--rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:27.000000 csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libjsfx.so
--rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:27.000000 csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libklib.so
--rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:27.000000 csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libpathtools.so
--rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:27.000000 csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libpoly.so
--rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:27.000000 csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/librisset.so
--rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:27.000000 csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.706737 csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/
--rw-rw-r--   0 em        (1000) em        (1000)    67147 2024-04-03 07:40:28.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   122938 2024-04-03 07:40:28.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   104074 2024-04-03 07:40:28.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    51231 2024-04-03 07:40:28.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    67578 2024-04-03 07:40:28.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50588 2024-04-03 07:40:28.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/librisset.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.714738 csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/librisset.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.716737 csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/beosc.dll
--rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/else.dll
--rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/klib.dll
--rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/pathtools.dll
--rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:29.000000 csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/poly.dll
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.688737 csoundengine-2.8.2/csoundengine/data/plugins7/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.730738 csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:30.000000 csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libbeosc.so
--rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:30.000000 csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libelse.so
--rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:30.000000 csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libjsfx.so
--rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:30.000000 csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libklib.so
--rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:30.000000 csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libpathtools.so
--rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:30.000000 csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libpoly.so
--rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:30.000000 csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/librisset.so
--rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:30.000000 csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.738738 csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:31.000000 csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:31.000000 csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:31.000000 csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:31.000000 csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:31.000000 csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:31.000000 csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:31.000000 csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/librisset.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:31.000000 csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.741738 csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:32.000000 csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/beosc.dll
--rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:32.000000 csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/else.dll
--rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:32.000000 csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/klib.dll
--rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:32.000000 csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/pathtools.dll
--rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:32.000000 csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/poly.dll
--rw-rw-r--   0 em        (1000) em        (1000)    13483 2024-02-05 17:19:21.000000 csoundengine-2.8.2/csoundengine/dependencies.py
--rwxr-xr-x   0 em        (1000) em        (1000)   153752 2024-04-17 08:22:46.000000 csoundengine-2.8.2/csoundengine/engine.py
--rw-r--r--   0 em        (1000) em        (1000)    24396 2024-04-17 08:14:41.000000 csoundengine-2.8.2/csoundengine/engineorc.py
--rw-rw-r--   0 em        (1000) em        (1000)      145 2023-10-11 21:51:48.000000 csoundengine-2.8.2/csoundengine/errors.py
--rw-r--r--   0 em        (1000) em        (1000)     2741 2024-02-22 09:52:16.000000 csoundengine-2.8.2/csoundengine/event.py
--rw-r--r--   0 em        (1000) em        (1000)    41732 2024-04-03 10:37:27.000000 csoundengine-2.8.2/csoundengine/instr.py
--rw-r--r--   0 em        (1000) em        (1000)    12223 2024-04-03 10:31:58.000000 csoundengine-2.8.2/csoundengine/instrtools.py
--rw-r--r--   0 em        (1000) em        (1000)    10720 2023-11-14 20:14:02.000000 csoundengine-2.8.2/csoundengine/interact.py
--rw-r--r--   0 em        (1000) em        (1000)    21429 2024-04-10 06:06:37.000000 csoundengine-2.8.2/csoundengine/internal.py
--rw-r--r--   0 em        (1000) em        (1000)     4997 2023-11-14 20:14:02.000000 csoundengine-2.8.2/csoundengine/jacktools.py
--rw-rw-r--   0 em        (1000) em        (1000)     3121 2023-10-26 22:00:07.000000 csoundengine-2.8.2/csoundengine/jupytertools.py
--rw-r--r--   0 em        (1000) em        (1000)     4517 2024-04-17 08:24:52.000000 csoundengine-2.8.2/csoundengine/linuxaudio.py
--rw-r--r--   0 em        (1000) em        (1000)     5815 2023-11-14 20:14:02.000000 csoundengine-2.8.2/csoundengine/magic.py
--rw-r--r--   0 em        (1000) em        (1000)    69596 2024-04-17 08:24:02.000000 csoundengine-2.8.2/csoundengine/offline.py
--rw-rw-r--   0 em        (1000) em        (1000)     5690 2023-11-01 14:45:02.000000 csoundengine-2.8.2/csoundengine/offlineorc.py
--rw-rw-r--   0 em        (1000) em        (1000)     6007 2023-10-11 21:51:48.000000 csoundengine-2.8.2/csoundengine/paramtable.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7787 2024-04-17 07:56:12.000000 csoundengine-2.8.2/csoundengine/plotting.py
--rw-rw-r--   0 em        (1000) em        (1000)        0 2021-11-13 21:37:59.000000 csoundengine-2.8.2/csoundengine/py.typed
--rw-r--r--   0 em        (1000) em        (1000)    14940 2024-02-25 13:29:47.000000 csoundengine-2.8.2/csoundengine/schedevent.py
--rw-r--r--   0 em        (1000) em        (1000)    87324 2024-04-10 06:06:37.000000 csoundengine-2.8.2/csoundengine/session.py
--rw-rw-r--   0 em        (1000) em        (1000)      779 2024-03-28 17:26:41.000000 csoundengine-2.8.2/csoundengine/sessionhandler.py
--rw-r--r--   0 em        (1000) em        (1000)     6917 2024-02-29 10:28:35.000000 csoundengine-2.8.2/csoundengine/sessioninstrs.py
--rw-rw-r--   0 em        (1000) em        (1000)     1996 2023-05-10 15:18:41.000000 csoundengine-2.8.2/csoundengine/state.py
--rw-r--r--   0 em        (1000) em        (1000)    35007 2024-04-17 08:23:35.000000 csoundengine-2.8.2/csoundengine/synth.py
--rw-r--r--   0 em        (1000) em        (1000)     5965 2023-11-14 20:14:02.000000 csoundengine-2.8.2/csoundengine/tableproxy.py
--rw-rw-r--   0 em        (1000) em        (1000)      600 2022-09-25 13:10:18.000000 csoundengine-2.8.2/csoundengine/termui.py
--rw-rw-r--   0 em        (1000) em        (1000)     3101 2024-04-16 11:20:08.000000 csoundengine-2.8.2/csoundengine/tools.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.701737 csoundengine-2.8.2/csoundengine.egg-info/
--rw-r--r--   0 em        (1000) em        (1000)     6142 2024-04-17 09:31:32.000000 csoundengine-2.8.2/csoundengine.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     3778 2024-04-17 09:31:32.000000 csoundengine-2.8.2/csoundengine.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2024-04-17 09:31:32.000000 csoundengine-2.8.2/csoundengine.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-17 19:50:17.000000 csoundengine-2.8.2/csoundengine.egg-info/not-zip-safe
--rw-rw-r--   0 em        (1000) em        (1000)      258 2024-04-17 09:31:32.000000 csoundengine-2.8.2/csoundengine.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       13 2024-04-17 09:31:32.000000 csoundengine-2.8.2/csoundengine.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)       38 2024-04-17 09:31:32.742738 csoundengine-2.8.2/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)     1724 2024-04-17 09:31:20.000000 csoundengine-2.8.2/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-17 09:31:32.741738 csoundengine-2.8.2/test/
--rw-rw-r--   0 em        (1000) em        (1000)      548 2023-09-17 06:41:11.000000 csoundengine-2.8.2/test/test1.py
--rw-rw-r--   0 em        (1000) em        (1000)      642 2024-02-23 13:40:16.000000 csoundengine-2.8.2/test/test2.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.604920 csoundengine-2.8.3/
+-rw-rw-r--   0 em        (1000) em        (1000)    35128 2021-11-13 21:37:59.000000 csoundengine-2.8.3/LICENSE.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       24 2021-11-13 21:37:59.000000 csoundengine-2.8.3/MANIFEST.in
+-rw-r--r--   0 em        (1000) em        (1000)     6716 2024-04-19 13:24:18.604920 csoundengine-2.8.3/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     5728 2024-01-10 12:24:51.000000 csoundengine-2.8.3/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.586920 csoundengine-2.8.3/csoundengine/
+-rw-r--r--   0 em        (1000) em        (1000)     4112 2024-04-19 12:36:50.000000 csoundengine-2.8.3/csoundengine/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1055 2023-03-14 09:38:54.000000 csoundengine-2.8.3/csoundengine/__sessionbase.py
+-rw-r--r--   0 em        (1000) em        (1000)      177 2023-11-24 08:20:24.000000 csoundengine-2.8.3/csoundengine/_common.py
+-rw-r--r--   0 em        (1000) em        (1000)     5978 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/abstractrenderer.py
+-rw-r--r--   0 em        (1000) em        (1000)    11621 2024-02-21 14:58:04.000000 csoundengine-2.8.3/csoundengine/baseschedevent.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5848 2024-04-17 08:24:25.000000 csoundengine-2.8.3/csoundengine/busproxy.py
+-rw-r--r--   0 em        (1000) em        (1000)     8213 2024-04-03 07:08:12.000000 csoundengine-2.8.3/csoundengine/config.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2023-10-17 11:02:49.000000 csoundengine-2.8.3/csoundengine/contants.py
+-rwxr-xr-x   0 em        (1000) em        (1000)   126875 2024-04-19 12:01:57.000000 csoundengine-2.8.3/csoundengine/csoundlib.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.579920 csoundengine-2.8.3/csoundengine/data/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.579920 csoundengine-2.8.3/csoundengine/data/plugins6/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.589920 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libbeosc.so
+-rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libelse.so
+-rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libjsfx.so
+-rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libklib.so
+-rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libpathtools.so
+-rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libpoly.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/librisset.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.592920 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/
+-rw-rw-r--   0 em        (1000) em        (1000)    67147 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   122938 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   104074 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    51231 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    67578 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50588 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/librisset.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.595920 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/librisset.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.596920 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/beosc.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/else.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/klib.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/pathtools.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/poly.dll
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.579920 csoundengine-2.8.3/csoundengine/data/plugins7/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.598920 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libbeosc.so
+-rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libelse.so
+-rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libjsfx.so
+-rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libklib.so
+-rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libpathtools.so
+-rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libpoly.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/librisset.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.601920 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/librisset.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.602920 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/beosc.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/else.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/klib.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/pathtools.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/poly.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    13367 2024-04-19 12:39:25.000000 csoundengine-2.8.3/csoundengine/dependencies.py
+-rwxr-xr-x   0 em        (1000) em        (1000)   154239 2024-04-18 20:01:10.000000 csoundengine-2.8.3/csoundengine/engine.py
+-rw-r--r--   0 em        (1000) em        (1000)    24396 2024-04-17 08:14:41.000000 csoundengine-2.8.3/csoundengine/engineorc.py
+-rw-rw-r--   0 em        (1000) em        (1000)      145 2023-10-11 21:51:48.000000 csoundengine-2.8.3/csoundengine/errors.py
+-rw-r--r--   0 em        (1000) em        (1000)     2686 2024-04-18 10:55:30.000000 csoundengine-2.8.3/csoundengine/event.py
+-rw-r--r--   0 em        (1000) em        (1000)    41738 2024-04-18 11:00:12.000000 csoundengine-2.8.3/csoundengine/instr.py
+-rw-r--r--   0 em        (1000) em        (1000)    12223 2024-04-03 10:31:58.000000 csoundengine-2.8.3/csoundengine/instrtools.py
+-rw-r--r--   0 em        (1000) em        (1000)    10720 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/interact.py
+-rw-r--r--   0 em        (1000) em        (1000)    21429 2024-04-10 06:06:37.000000 csoundengine-2.8.3/csoundengine/internal.py
+-rw-r--r--   0 em        (1000) em        (1000)     4997 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/jacktools.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3121 2023-10-26 22:00:07.000000 csoundengine-2.8.3/csoundengine/jupytertools.py
+-rw-r--r--   0 em        (1000) em        (1000)     4517 2024-04-17 08:24:52.000000 csoundengine-2.8.3/csoundengine/linuxaudio.py
+-rw-r--r--   0 em        (1000) em        (1000)     5815 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/magic.py
+-rw-r--r--   0 em        (1000) em        (1000)    69729 2024-04-18 20:08:09.000000 csoundengine-2.8.3/csoundengine/offline.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5690 2023-11-01 14:45:02.000000 csoundengine-2.8.3/csoundengine/offlineorc.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6007 2023-10-11 21:51:48.000000 csoundengine-2.8.3/csoundengine/paramtable.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7787 2024-04-17 07:56:12.000000 csoundengine-2.8.3/csoundengine/plotting.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2021-11-13 21:37:59.000000 csoundengine-2.8.3/csoundengine/py.typed
+-rw-r--r--   0 em        (1000) em        (1000)    14940 2024-02-25 13:29:47.000000 csoundengine-2.8.3/csoundengine/schedevent.py
+-rw-r--r--   0 em        (1000) em        (1000)    87296 2024-04-18 19:40:51.000000 csoundengine-2.8.3/csoundengine/session.py
+-rw-rw-r--   0 em        (1000) em        (1000)      779 2024-03-28 17:26:41.000000 csoundengine-2.8.3/csoundengine/sessionhandler.py
+-rw-r--r--   0 em        (1000) em        (1000)     6917 2024-02-29 10:28:35.000000 csoundengine-2.8.3/csoundengine/sessioninstrs.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1996 2024-04-19 11:09:00.000000 csoundengine-2.8.3/csoundengine/state.py
+-rw-r--r--   0 em        (1000) em        (1000)    35051 2024-04-18 20:04:42.000000 csoundengine-2.8.3/csoundengine/synth.py
+-rw-r--r--   0 em        (1000) em        (1000)     5965 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/tableproxy.py
+-rw-rw-r--   0 em        (1000) em        (1000)      600 2022-09-25 13:10:18.000000 csoundengine-2.8.3/csoundengine/termui.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3101 2024-04-16 11:20:08.000000 csoundengine-2.8.3/csoundengine/tools.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.604920 csoundengine-2.8.3/csoundengine.egg-info/
+-rw-r--r--   0 em        (1000) em        (1000)     6716 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     3778 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-17 19:50:17.000000 csoundengine-2.8.3/csoundengine.egg-info/not-zip-safe
+-rw-rw-r--   0 em        (1000) em        (1000)      259 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       13 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2024-04-19 13:24:18.604920 csoundengine-2.8.3/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)     1725 2024-04-19 13:21:08.000000 csoundengine-2.8.3/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.603920 csoundengine-2.8.3/test/
+-rw-rw-r--   0 em        (1000) em        (1000)      548 2023-09-17 06:41:11.000000 csoundengine-2.8.3/test/test1.py
+-rw-rw-r--   0 em        (1000) em        (1000)      642 2024-02-23 13:40:16.000000 csoundengine-2.8.3/test/test2.py
```

### Comparing `csoundengine-2.8.2/LICENSE.txt` & `csoundengine-2.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/PKG-INFO` & `csoundengine-2.8.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: csoundengine
-Version: 2.8.2
-Summary: A synthesis framework using csound
-Home-page: https://github.com/gesellkammer/csoundengine
-Author: Eduardo Moguillansky
-Author-email: eduardo.moguillansky@gmail.com
-License: BSD
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
-License-File: LICENSE.txt
-
 csoundengine
 ============
 
 |sh-month|
 
 .. |sh-month| image:: https://static.pepy.tech/badge/csoundengine/month
```

### Comparing `csoundengine-2.8.2/README.rst` & `csoundengine-2.8.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: csoundengine
+Version: 2.8.3
+Summary: A synthesis framework using csound
+Home-page: https://github.com/gesellkammer/csoundengine
+Author: Eduardo Moguillansky
+Author-email: eduardo.moguillansky@gmail.com
+License: BSD
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: cachetools
+Requires-Dist: JACK-client
+Requires-Dist: appdirs
+Requires-Dist: pygments
+Requires-Dist: sf2utils
+Requires-Dist: ipywidgets
+Requires-Dist: progressbar2
+Requires-Dist: xxhash
+Requires-Dist: docstring-parser
+Requires-Dist: ctcsound7>=0.4.6
+Requires-Dist: sndfileio>=1.9.4
+Requires-Dist: emlib>=1.14.1
+Requires-Dist: configdict>=2.10.0
+Requires-Dist: bpf4>=1.10.1
+Requires-Dist: numpyx>=1.3.3
+Requires-Dist: pitchtools>=1.14.0
+Requires-Dist: risset>=2.9.1
+Requires-Dist: sounddevice
+
 csoundengine
 ============
 
 |sh-month|
 
 .. |sh-month| image:: https://static.pepy.tech/badge/csoundengine/month
```

### Comparing `csoundengine-2.8.2/csoundengine/__init__.py` & `csoundengine-2.8.3/csoundengine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,25 +95,25 @@
         # synth, so that it is evaluated later in the chain
         filt = session.sched("filter", delay=start, dur=5, priority=synth.priority+1,
                              kcutoff=2000, kresonance=0.92, ibus=bus)
 
         # Automate the cutoff freq. of the filter
         filt.automate('kcutoff', [0, 2000, dur*0.8, 500, dur, 6000], delay=start)
 """
-# sndfileio sets numpy's denormal behaviour. If it happens later numpy spits
-# multiple warnings about it
-import sndfileio
+# This disables warning about denormals
+import numpy as np
+np.finfo(np.dtype("float32"))
+np.finfo(np.dtype("float64"))
 
 from .config import config, setLoggingLevel
 from .dependencies import checkDependencies, installDependencies
-ok = checkDependencies(force=False, fix=True)
-if not ok:
+_ok = checkDependencies(force=True, fix=True)
+if not _ok:
     raise RuntimeError("csoundengine: Depencencies not fullfilled")
 
-
 from .engine import *
 from .config import config, setLoggingLevel
 from .session import Session
 from .instr import Instr
 from .offline import Renderer
 from .synth import SynthGroup
 from . import csoundlib
```

### Comparing `csoundengine-2.8.2/csoundengine/__sessionbase.py` & `csoundengine-2.8.3/csoundengine/__sessionbase.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/abstractrenderer.py` & `csoundengine-2.8.3/csoundengine/abstractrenderer.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/baseschedevent.py` & `csoundengine-2.8.3/csoundengine/baseschedevent.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/busproxy.py` & `csoundengine-2.8.3/csoundengine/busproxy.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/config.py` & `csoundengine-2.8.3/csoundengine/config.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/csoundlib.py` & `csoundengine-2.8.3/csoundengine/csoundlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from csoundengine.config import config
 from csoundengine.internal import normalizePlatform
 import functools as _functools
 import emlib.misc
 import emlib.textlib
 import emlib.dialogs
 import emlib.mathlib
+from emlib.common import runonce
 import numpy as np
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import Callable, Sequence, Iterator, Any, Set
     Curve = Callable[[float], float]
 
@@ -404,14 +405,15 @@
                          alwaysAvailable=True,
                          longname=longname,
                          hasSystemSr=hasSystemSr)
 
     def getSystemSr(self) -> int | None:
         if sys.platform == 'linux' and linuxaudio.isPipewireRunning():
             info = linuxaudio.pipewireInfo()
+            assert info is not None
             return info.sr
         return super().getSystemSr()
 
     @_functools.cache
     def defaultAudioDevices(self) -> tuple[AudioDevice | None, AudioDevice | None]:
         logger.debug("Querying default device via portaudio/sounddevice")
         try:
@@ -503,15 +505,15 @@
 
 
 def nextpow2(n:int) -> int:
     """ Returns the power of 2 higher or equal than n"""
     return int(2 ** _math.ceil(_math.log(n, 2)))
     
 
-@emlib.misc.runonce
+@runonce
 def findCsound() -> str | None:
     """
     Find the csound binary or None if not found
     """
     csound = _shutil.which("csound")
     if not csound:
         logger.error("csound is not in the path!")
@@ -731,22 +733,22 @@
     if sys.platform not in folders:
         raise RuntimeError(f"Platform {sys.platform} not known")
     folder = folders[sys.platform]
     return _os.path.abspath(_os.path.expandvars(folder))
 
 
 def runCsd(csdfile:str,
-           outdev="",
-           indev="",
-           backend="",
+           outdev='',
+           indev='',
+           backend='',
            nodisplay=False,
            nomessages=False,
            comment='',
            piped=False,
-           extra: list[str] = None
+           extra: list[str] | None = None
            ) -> _subprocess.Popen:
     """
     Run the given .csd as a csound subprocess
 
     Args:
         csdfile: the path to a .csd file
         outdev: "dac" to output to the default device, the label of the
@@ -787,22 +789,23 @@
     if indev:
         args.append(f"-i {indev}")
     if nodisplay:
         args.append('-d')
     if nomessages:
         args.append('-m16')
     if comment and offline:
-        args.append(f'-+id_comment="{comment}"')
+        args.append(f'-+id_comment="{comment}"'
+                    )
     if extra:
         args.extend(extra)
     args.append(csdfile)
     return csoundSubproc(args, piped=piped)
     
 
-def joinCsd(orc: str, sco="", options: list[str] | None = None) -> str:
+def joinCsd(orc: str, sco='', options: list[str] | None = None) -> str:
     """
     Joins an orc and a score (both as str), returns a csd as string
 
     Args:
         orc: the text of the orchestra
         sco: the text of the score
         options: any command line options to be included
@@ -1035,30 +1038,40 @@
         cached = False
     if cached and _cache.get('opcodes') is not None:
         return _cache['opcodes']
     return _csoundGetInfoViaAPI(opcodedir=opcodedir)['opcodes']
 
 
 def _csoundGetInfoViaAPI(opcodedir='') -> dict:
+    global _cache
+
     cs = ctcsound.Csound()
-    cs.setOption("-d")  # supress displays
+    cs.setOption("-d")
+    cs.setOption("--nosound")
+    cs.setOption("--messagelevel=0")
+    cs.setOption("--m-amps=0")
+    cs.setOption("--m-range=0")
+
     if opcodedir:
         cs.setOption(f'--opcode-dir={opcodedir}')
-    opcodes, n = cs.newOpcodeList()
-    opcodeNames = [opc.opname.decode('utf-8') for opc in opcodes]
-    cs.disposeOpcodeList(opcodes)
     version = cs.version()
     vs = str(version)
     patch = int(vs[-1])
     minor = int(vs[-3:-1])
     major = int(vs[:-3])
-    opcodes = list(set(opcodeNames))
     versionTriplet = (major, minor, patch)
-    _cache['opcodes'] = opcodes
     _cache['versionTriplet'] = versionTriplet
+
+    opcodes, n = cs.newOpcodeList()
+    assert opcodes is not None
+    opcodeNames = [opc.opname.decode('utf-8') for opc in opcodes]
+    cs.disposeOpcodeList(opcodes)
+    opcodes = list(set(opcodeNames))
+    _cache['opcodes'] = opcodes
+    cs.stop()
     return {'opcodes': opcodes,
             'versionTriplet': versionTriplet}
 
 
 def _opcodesList(opcodedir='') -> list[str]:
     options = ["-z"]
     if opcodedir:
@@ -1075,15 +1088,15 @@
             allopcodes.extend(opcodes)
     return allopcodes
 
    
 def saveAsGen23(data: Sequence[float] | np.ndarray,
                 outfile: str,
                 fmt="%.12f",
-                header=""
+                header=''
                 ) -> None:
     """
     Saves the data to a gen23 table
 
     .. note::
         gen23 is a 1D list of numbers in text format, sepparated by a space
 
@@ -2424,21 +2437,22 @@
         self._writeScore(stream, datadir=datadir)
         
         write("\n</CsScore>\n")
         write("</CsoundSynthesizer>")
 
     def run(self,
             output: str,
-            csdfile: str = None,
-            inputdev: str = None,
-            backend: str = None,
+            csdfile='',
+            inputdev='',
+            backend='',
             suppressdisplay=True,
             nomessages=False,
             piped=False,
-            extraOptions: list[str] = None) -> _subprocess.Popen:
+            extraOptions: list[str] | None = None
+            ) -> _subprocess.Popen:
         """
         Run this csd. 
         
         Args:
             output: the output of the csd. This will be passed
                 as the -o argument to csound. If an empty string or None is given,
                 no sound is produced (adds the '--nosound' flag).
@@ -2548,17 +2562,17 @@
     else:
         raise TypeError("timecurve should be either a scalar or a bpf")
     
     assert isinstance(pitchcurve, (int, float, bpf.core.BpfInterface))
     ts = np.arange(t0, t1+dt, dt)
     fmt = "%.12f"
     _, time_gen23 = _tempfile.mkstemp(prefix='time-', suffix='.gen23')
-    np.savetxt(time_gen23, timebpf.map(ts), fmt=fmt, header=str(dt), comments="")
+    np.savetxt(time_gen23, timebpf.map(ts), fmt=fmt, header=str(dt), comments='')
     _, pitch_gen23 = _tempfile.mkstemp(prefix='pitch-', suffix='.gen23')
-    np.savetxt(pitch_gen23, pitchbpf.map(ts), fmt=fmt, header=str(dt), comments="")
+    np.savetxt(pitch_gen23, pitchbpf.map(ts), fmt=fmt, header=str(dt), comments='')
     csd = f"""
     <CsoundSynthesizer>
     <CsOptions>
     -o {outfile}
     </CsOptions>
     <CsInstruments>
 
@@ -2641,15 +2655,15 @@
     {body}
 endin
 
     """.format(sr=sr, ksmps=ksmps, instrid=instrid, body=body, nchnls=nchnls, initstr=initstr)
     return orc
 
 
-def recInstr(body:str, events:list, init="", outfile:str=None,
+def recInstr(body: str, events: list, init='', outfile='',
              sr=44100, ksmps=64, nchnls=2, a4=442, samplefmt='float',
              dur=None
              ) -> tuple[str, _subprocess.Popen]:
     """
     Record one instrument for a given duration
 
     Args:
@@ -3281,15 +3295,15 @@
         lines = body
     docstart, docend = locateDocstring(lines)
     if docstart is not None:
         docstring = '\n'.join(lines[docstart:docend])
         rest = '\n'.join(lines[docend:])
     else:
         docstring = ''
-        rest = body
+        rest = body if isinstance(body, str) else '\n'.join(lines)
     return docstring, rest
 
 
 @_functools.cache
 def instrParseBody(body: str) -> ParsedInstrBody:
     """
     Parses the body of an instrument, returns pfields used, output channels, etc.
@@ -3319,19 +3333,19 @@
                           a1 = oscili:a(0.5, kfreq) * a0\\noutch 1, a1',
                         pfieldsDefaults={1: 0.0, 2: 0.0, 3: 0.0, 4: 1.0, 5: 1000.0},
                         pfieldsUsed={4, 5},
                         outChannels={1},
                         pfieldsNameToIndex={'ibus': 4, 'kfreq': 5})
     """
     if not body.strip():
-        return ParsedInstrBody(pfieldIndexToValue=EMPTYDICT,
+        return ParsedInstrBody(pfieldIndexToValue={},
                                pfieldLines=(),
                                body='',
                                lines=(),
-                               pfieldIndexToName=EMPTYDICT)
+                               pfieldIndexToName={})
 
     pfieldLines = []
     bodyLines = []
     pfieldIndexToValue = {}
     insideComment = False
     pfieldsUsed = set()
     pfieldIndexToName: dict[int, str] = {}
@@ -3408,15 +3422,15 @@
                            pfieldsUsed=pfieldsUsed,
                            outChannels=outchannels,
                            pfieldLines=pfieldLines,
                            body="\n".join(bodyLines),
                            lines=lines)
 
 
-def bestSampleEncodingForExtension(ext: str) -> str | None:
+def bestSampleEncodingForExtension(ext: str) -> str:
     """
     Given an extension, return the best sample encoding.
 
     .. note::
 
         float64 is not considered necessary for holding sound information
 
@@ -3537,17 +3551,18 @@
         tuples (bank, presetindex, name)
     """
     from sf2utils.sf2parse import Sf2File
     f = open(sfpath, 'rb')
     sf = Sf2File(f)
     instruments: list[tuple[int, str]] = [(num, instr.name.strip())
                                           for num, instr in enumerate(sf.instruments)
-                                          if instr.name != 'EOI']
+                                          if instr.name and instr.name != 'EOI']
     presets: list[tuple[int, int, str]] = [(p.bank, p.preset, p.name.strip())
-                                           for p in sf.presets if p.name != 'EOP']
+                                           for p in sf.presets
+                                           if p.name and p.name != 'EOP']
     presets.sort()
     return instruments, presets
 
 
 def soundfontInstruments(sfpath: str) -> list[tuple[int, str]]:
     """
     Get instruments for a soundfont
```

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libbeosc.so` & `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libbeosc.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libelse.so` & `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libelse.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libjsfx.so` & `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libjsfx.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libklib.so` & `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libklib.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libpathtools.so` & `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libpathtools.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libpoly.so` & `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libpoly.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/librisset.so` & `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/librisset.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so` & `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libelse.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libklib.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/libpoly.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-arm64/librisset.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libelse.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libklib.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/librisset.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/beosc.dll` & `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/beosc.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/else.dll` & `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/else.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/klib.dll` & `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/klib.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/pathtools.dll` & `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/pathtools.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins6/windows-x86_64/poly.dll` & `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/poly.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libbeosc.so` & `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libbeosc.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libelse.so` & `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libelse.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libjsfx.so` & `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libjsfx.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libklib.so` & `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libklib.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libpathtools.so` & `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libpathtools.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libpoly.so` & `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libpoly.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/librisset.so` & `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/librisset.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so` & `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libelse.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libklib.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/librisset.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib` & `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/beosc.dll` & `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/beosc.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/else.dll` & `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/else.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/klib.dll` & `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/klib.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/pathtools.dll` & `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/pathtools.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/data/plugins7/windows-x86_64/poly.dll` & `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/poly.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/dependencies.py` & `csoundengine-2.8.3/csoundengine/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from datetime import datetime
 import json
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import *
 
 
-logger = logging.getLogger("csoundengine")
+logger = logging.getLogger("csoundengine.dependencies")
+logger.setLevel("INFO")
 
 
 def _asVersionTriplet(tagname: str) -> Tuple[int, int, int]:
     assert isinstance(tagname, str)
     match = re.search(r"(\d+)\.(\d+)(.(\d+))?", tagname)
     if not match:
         raise ValueError(f"Could not parse tagname {tagname}")
@@ -111,24 +112,23 @@
         raise RuntimeError(f"No plugins released for platform {sys.platform}")
     version = pluginurls.get('version', None)
     if version:
         print(f"Downloading latest version ({version}) of csound-plugins...")
     return _download(pluginurl, destFolder)
 
 
-def _download(url: str, destFolder: Union[str, Path]) -> Path:
+def _download(url: str, destFolder: str | Path) -> Path:
     assert os.path.exists(destFolder) and os.path.isdir(destFolder)
     fileName = os.path.split(url)[1]
     dest = Path(destFolder) / fileName
     if dest.exists():
-        logger.warning(f"Destination {dest} already exists, overwriting")
+        logger.warning(f"Destination '{dest}' already exists, overwriting")
         os.remove(dest)
-    logger.info(f"Downloading {url}")
     urllib.request.urlretrieve(url, dest)
-    logger.info(f"   ... saved to {dest}")
+    logger.info(f"Downloaded '{url}', saved to '{dest}'")
     return dest
 
 
 def _zipExtract(zippedfile: Path) -> Path:
     import zipfile
     destFolder = tempfile.mktemp(prefix=zippedfile.name)
     os.mkdir(destFolder)
@@ -137,22 +137,20 @@
     return Path(destFolder)
 
 
 def _copyFiles(files: List[str], dest: str, verbose=False) -> None:
     assert os.path.isdir(dest)
     for f in files:
         if verbose:
-            print(f"Copying file {f} to {dest}")
+            print(f"Copying file '{f}' to '{dest}'")
         shutil.copy(f, dest)
 
 
-def pluginsInstalled(cached: bool) -> bool:
+def pluginsInstalled(cached=True) -> bool:
     """Returns True if the needed plugins are already installed"""
-    #opcodes = set(csoundlib.opcodesList(cached=cached,
-    #                                    opcodedir=csoundlib.userPluginsFolder(apiversion=apiversion)))
     opcodes = set(csoundlib.opcodesList(cached=cached))
     neededOpcodes = {
         "atstop", "pwrite", "pread", "initerror",
         "dict_new", "dict_set", "dict_get",
         "pool_gen", "pool_pop", "pool_push", "pool_isfull",
         'interp1d', 'bisect', 'ftsetparams', 'zeroarray',
         'panstereo', 'poly0'
@@ -183,19 +181,19 @@
 
     subfolder = str(platformid)
     pluginspath = rootfolder/f'data/plugins{apiversion}'/subfolder
     if not pluginspath.exists():
         raise RuntimeError(f"Could not find own csound plugins. Folder: {pluginspath}")
     plugins = list(pluginspath.glob(globpattern))
     if not plugins:
-        logger.error(f"Plugins not found. Plugins folder: {pluginspath}, "
-                     f"glob patter: {globpattern}")
+        logger.error(f"Plugins not found. Plugins folder: '{pluginspath}', "
+                     f"glob patter: '{globpattern}'")
         raise RuntimeError("Plugins not found")
     pluginsDest = csoundlib.userPluginsFolder(apiversion=f'{apiversion}.0')
-    logger.info(f"Installing plugins in folder: {pluginsDest}")
+    logger.info(f"Installing plugins in folder: '{pluginsDest}'")
     os.makedirs(pluginsDest, exist_ok=True)
     _copyFiles([plugin.as_posix() for plugin in plugins], pluginsDest, verbose=True)
     if platformid.osname == 'macos' and codesign:
         installedBinaries = [os.path.join(pluginsDest, plugin.name)
                              for plugin in plugins]
         assert all(os.path.exists(binary) for binary in installedBinaries)
         try:
@@ -215,15 +213,15 @@
     """
     logger.info("Trying to install plugins via risset")
     import risset
     idx = risset.MainIndex(update=True, majorversion=majorversion)
     for pluginname in ['else', 'beosc', 'klib', 'poly']:
         p = idx.plugins.get(pluginname)
         if p is None:
-            logger.error(f"Plugin '{pluginname}' not found in risset's index")
+            logger.error(f"Plugin '{pluginname}' not in risset's index")
             return False
         elif idx.is_plugin_installed(p):
             logger.debug(f"Plugin '{pluginname}' already installed, skipping")
         else:
             errmsg = idx.install_plugin(p)
             if errmsg:
                 logger.error(f"Error while installing plugin {pluginname}: {errmsg}")
@@ -242,17 +240,17 @@
             will detect the installed version and use that
         risset: if True, install plugins via risset (default). Otherwise, uses
             the bundled plugins
 
     Returns:
         True if installation succeeded. Any errors are logged
     """
-    logger.info("Installing external plugins via risset")
 
     if risset:
+        logger.info("Installing external plugins via risset")
         try:
             ok = _installPluginsViaRisset()
             pluginsok = pluginsInstalled(cached=False)
             if ok and pluginsok:
                 logger.info("Plugins installed successfully via risset")
                 return True
             else:
@@ -276,51 +274,51 @@
             logger.error("Plugins where installed but do not seem to be detected")
     except Exception as e:
         logger.error(f"Exception {e} while trying to install plugins from distribution")
         return False
     return True
 
 
-def _checkDependencies(fix=False, updateState=True, quiet=False) -> Optional[str]:
+def _checkDependencies(fix=False, quiet=False) -> Optional[str]:
     """
     Either returns None or an error message
     """
     if not csoundInstalled():
         return "csound not installed. See https://csound.com/download.html"
 
     version = csoundlib.getVersion(useApi=True)
+
     if version < (6, 16, 0):
         return f"Csound version ({version}) is too old, should be >= 6.16"
 
     if version[0] >= 7:
         print(f"WARNING: Csound 7 is not fully supported. Proceed at yout own risk")
 
-    binversion = csoundlib.getVersion(useApi=False)
-    if version[:2] != binversion[:2]:
-        print(f"WARNING: the csound library found reported a version {version}, different"
-              f" from the version reported by the csound binary {binversion}")
-
-    if not pluginsInstalled(cached=False):
+    # binversion = csoundlib.getVersion(useApi=False)
+    # if version[:2] != binversion[:2]:
+    #     print(f"WARNING: the csound library found reported a version {version}, different"
+    #           f" from the version reported by the csound binary {binversion}")
+    if not pluginsInstalled():
         if fix:
             print("** csoundengine: Csound external plugins are not installed or are too old."
                   " I will try to install them now")
             ok = installPlugins(version[0])
             if ok:
                 print("** csoundengine: csound external plugins installed ok")
             else:
                 print("** csoundengine: csound external plugins could not be installed")
                 return "csound external plugins could not be installed"
         else:
-            return ("Some plugins are not installed. They can be installed via 'import csoundengine; csoundengine.installDependencies()'. "
+            return ("Some plugins are not installed. They can be installed via "
+                    "'import csoundengine; csoundengine.installDependencies()'. "
                     "To install the plugins manually you will need risset installed. Install them via risset "
                     "(risset install \"*\"), or manually from "
                     "https://github.com/csound-plugins/csound-plugins/releases")
     logger.info("Dependencies OK")
-    if updateState:
-        state['last_run'] = datetime.now().isoformat()
+    state['last_check'] = datetime.now().isoformat()
 
 
 def installDependencies() -> bool:
     """
     Install any needed depencendies
 
     Any problems regarding installation of dependencies will be logged as
@@ -342,31 +340,33 @@
 
     Returns:
         True if all dependencies are fullfilled
 
     """
     # Skip checks if only building docs
     if 'sphinx' in sys.modules:
-        logger.info("Called by sphinx? Skipping dependency check")
+        logger.debug("Called by sphinx? Skipping dependency check")
         return True
 
-    timeSincelast_run = datetime.now() - datetime.fromisoformat(state['last_run'])
-    if force or timeSincelast_run.days > 30:
-        logger.warning("Checking dependencies")
+    okstatus = True
+    now = datetime.now()
+    timeSinceLastCheck = now - datetime.fromisoformat(state['last_check'])
+    if force or timeSinceLastCheck.days >= 30:
+        logger.info("Checking dependencies")
         errormsg = _checkDependencies(fix=fix)
         if errormsg:
             logger.error(f"*** checkDependencies: {errormsg}")
             if not fix:
                 logger.error("*** You can try to fix this by calling installDependencies()")
-            return False
-    return True
+            okstatus = False
+    return okstatus
 
 
 def _codesignBinaries(binaries: list[str]) -> None:
     """
     Calls codesign to sign the binaries with adhoc signature
 
     Raises RuntimeError on fail
     """
     import risset
-    logger.info(f"Codesigning macos binaries: {binaries}")
+    logger.warning(f"Codesigning macos binaries: {binaries}")
     risset.macos_codesign(binaries, signature='-')
```

### Comparing `csoundengine-2.8.2/csoundengine/engine.py` & `csoundengine-2.8.3/csoundengine/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,16 +331,16 @@
                  nchnls_i: int | None = None,
                  realtime=False,
                  buffersize: int | None = None,
                  numbuffers: int | None = None,
                  globalcode: str = "",
                  numAudioBuses: int | None = None,
                  numControlBuses: int | None = None,
-                 quiet: bool = None,
-                 udpserver: bool = None,
+                 quiet: bool | None = None,
+                 udpserver: bool | None = None,
                  udpport: int = 0,
                  commandlineOptions: list[str] | None = None,
                  includes: list[str] | None = None,
                  midibackend: str = 'default',
                  midiin: str | None = None,
                  autosync=False,
                  latency: float | None = None,
@@ -366,16 +366,18 @@
                 logger.error(f"Backend {backend} unknown. Available backends: "
                              f"{availableBackends}")
             else:
                 logger.error(f"Backend {backend} not available. Available backends: "
                              f"{availableBackends}")
 
         cascadingBackends = [b.strip() for b in backend.split(",")]
-        resolvedBackend = internal.resolveOption(cascadingBackends,
-                                                      availableBackends)
+        resolvedBackend = internal.resolveOption(cascadingBackends, availableBackends)
+        if resolvedBackend is None:
+            raise RuntimeError(f"No audio backends available")
+
         backendDef = csoundlib.getAudioBackend(resolvedBackend)
 
         if not backendDef:
             logger.error(f'Could not find any available backends for {backend}')
             logger.error(f'    Available backends: {", ".join(availableBackends)}')
             logger.error('To configure the default backends, do:\n'
                          '    from csoundengine import config\n'
@@ -399,23 +401,23 @@
             if selected is None:
                 raise RuntimeError("No output audio device selected")
             outdev, outdevName = selected.id, selected.name
             if not nchnls:
                 nchnls = selected.numchannels
         elif isinstance(outdev, int) or _re.search(r"\bdac[0-9]+\b", outdev):
             # dac1, dac8
-            if resolvedBackend == 'jack':
+            if backendDef.name == 'jack':
                 logger.warning(
                     "This way of setting the audio device is discouraged with jack"
                     ". Use a regex to select a specific client or None to connect"
                     "to the default client")
             if isinstance(outdev, int):
                 outdev = f"dac{outdev}"
         else:
-            if resolvedBackend == 'jack':
+            if backendDef.name == 'jack':
                 outdevName = outdev
             else:
                 selected = next((d for d in outdevs if _fnmatch.fnmatch(d.name, outdev)), None)
                 if not selected:
                     raise ValueError(f"Output device {outdev} not known. Possible devices: "
                                      f"{outdevs}")
                 outdev, outdevName = selected.id, selected.name
@@ -467,124 +469,128 @@
             if backendDef.hasSystemSr:
                 sr = backendsr
             else:
                 sr = 44100
                 logger.error(f"Asked for system sr, but backend '{resolvedBackend}', does not"
                              f"have a fixed sr. Using sr={sr}")
 
-        if a4 is None: a4 = cfg['A4']
+        if a4 is None:
+            a4 = cfg['A4']
         if numthreads == 0:
             numthreads = config['numthreads']
-        if ksmps is None: ksmps = cfg['ksmps']
+        if ksmps is None:
+            ksmps = cfg['ksmps']
         if nchnls_i is None:
             nchnls_i = cfg['nchnls_i']
         if nchnls is None:
             nchnls = cfg['nchnls']
         if nchnls == 0 or nchnls_i == 0:
             inchnls, outchnls = csoundlib.getNchnls(resolvedBackend,
                                                     outpattern=outdev, inpattern=indev)
             nchnls = nchnls or outchnls
             nchnls_i = nchnls_i or inchnls
-        assert nchnls > 0
-        assert nchnls_i >= 0
+        assert nchnls is not None and nchnls > 0
+        assert nchnls_i is not None and nchnls_i >= 0
+
+        if quiet is None:
+            quiet = cfg['suppress_output']
 
-        if quiet is None: quiet = cfg['suppress_output']
         if quiet:
             commandlineOptions.append('-m0')
             commandlineOptions.append('-d')
         self.name = name
         "Name of this Engine"
 
-        assert sr > 0
-        self.sr = sr
+        assert sr is not None and sr > 0
+        self.sr: int = sr
         "Sample rate"
 
         self.backend = resolvedBackend
         "Name of the backend used (jack, portaudio, etc)"
 
-        self.a4 = a4
+        self.a4: int | float = a4
         "Reference frequency for A4"
 
-        self.ksmps = ksmps
+        self.ksmps: int = ksmps
         "Number of samples per cycle"
 
-        self.onecycle = ksmps / sr
+        self.onecycle: float = ksmps / sr
         "Duration of one performance cycle (ksmps/sr)"
 
         self.outdev = outdev
         "Output device used"
 
         self.outdevName = outdevName
         "Long name of the output device"
 
         self.indev = indev
         "Input device"
 
         self.indevName = indevName
         "Long name of the input device"
 
-        self.nchnls = nchnls
+        self.nchnls: int = nchnls
         "Number of output channels"
 
-        self.nchnls_i = nchnls_i
+        self.nchnls_i: int = nchnls_i
         "Number of input channels"
 
-        self.globalCode = globalcode
+        self.globalCode: str = globalcode
         "Global (init) code to execute at the start of the Engine"
 
         self.started = False
         "Is this engine started?"
 
-        self.extraOptions = commandlineOptions
+        self.extraOptions: list[str] = commandlineOptions
         "Extra options passed to csound"
 
         self.commandlineOptions: list[str] = []
         """All command line options used to start the engine"""
 
         self.includes: list[str] = includes if includes is not None else []
         "List of include files"
 
-        self.extraLatency = latency if latency is not None else config['sched_latency']
+        self.extraLatency: float = latency if latency is not None else config['sched_latency']
         "Added latency for better synch"
 
-        self.numAudioBuses = numAudioBuses if numAudioBuses is not None else config['num_audio_buses']
+        self.numAudioBuses: int = numAudioBuses if numAudioBuses is not None else config['num_audio_buses']
         "Number of audio buses"
 
-        self.numControlBuses = numControlBuses if numControlBuses is not None else config['num_control_buses']
+        self.numControlBuses: int = numControlBuses if numControlBuses is not None else config['num_control_buses']
         "Number of control buses"
 
         self.udpPort = 0
         "UDP port used (0 if no udp port is active)"
 
         self.csound: None | ctcsound.Csound = None
         "The csound object"
 
-        self.autosync = autosync
+        self.autosync: bool = autosync
         """If True, call .sync whenever is needed"""
 
         backendBufferSize, backendNumBuffers = backendDef.bufferSizeAndNum()
         buffersize = (buffersize or backendBufferSize or config['buffersize'] or 256)
-        buffersize = max(ksmps * 2, buffersize)
+        buffersize = max(self.ksmps * 2, buffersize)
 
         numbuffers = (numbuffers or backendNumBuffers or config['numbuffers'] or
                       internal.determineNumbuffers(self.backend or "portaudio", buffersize=buffersize))
 
-        self.bufferSize = buffersize
+        self.bufferSize: int = buffersize
         "Buffer size"
 
-        self.numBuffers = numbuffers
+        self.numBuffers: int = numbuffers
         "Number of buffers to fill"
 
         self.midiBackend: None | str = midibackend
         "Midi backend used"
 
         self.started = False
         """Has this engine already started?"""
 
-        self.numthreads = numthreads
+        self.numthreads: int = numthreads
         """Number of threads to use in performance (corresponds to csound -j N)"""
 
         self._builtinInstrs: dict[str, int] = {}
         """Dict of built-in instrs, mapping instr name to number"""
 
         if midiin == 'all':
             midiindev = csoundlib.MidiDevice(deviceid='all', name='all')
@@ -763,15 +769,15 @@
         Get a unique token, to pass to csound for a sync response
         """
         assert self._responsesTable is not None
         token = self._tokens.pop()
         self._responsesTable[token] = _UNSET
         return token
 
-    def _waitOnToken(self, token: int, sleepfunc=time.sleep, period=0.001, timeout: float = None
+    def _waitOnToken(self, token: int, sleepfunc=time.sleep, period=0.001, timeout: float | None = None
                      ) -> float | None:
         if timeout is None:
             timeout = config['timeout']
         n = timeout // period
         table = self._responsesTable
         assert table is not None
         while n > 0:
@@ -956,18 +962,18 @@
 
     def stop(self):
         """
         Stop this Engine
         """
         if not hasattr(self, "name"):
             return
-        logger.info(f"stopping Engine {self.name}")
-        if not self.started or self._exited:
+        if self.csound is None or not self.started or self._exited:
             logger.debug(f"Engine {self.name} was not running, so can't stop it")
             return
+        logger.info(f"stopping Engine {self.name}")
         logger.info("... stopping thread")
         self._perfThread.stop()
         time.sleep(0.1)
         logger.info("... stopping csound")
         self.csound.stop()
         time.sleep(0.1)
         logger.info("... cleaning up")
@@ -1091,15 +1097,15 @@
 
         This is normally ``ksmps/sr * 2`` but the actual latency varies if
         the engine is being run in realtime (in that case init-pass is done
         async, which might result in longer latency).
         """
         return self.ksmps/self.sr * 2
 
-    def sync(self, timeout: float = None, force=False, threshold=2.) -> bool:
+    def sync(self, timeout: float | None = None, force=False, threshold=2.) -> bool:
         """
         Block until csound has processed its immediate events
 
         Args:
             timeout: a timeout in seconds; None = use default timeout as defined
                 in the configuration (TODO: add link to configuration docs)
             force: if True, sync even if not needed
@@ -1455,14 +1461,15 @@
         :meth:`Engine.elapsedTime`, :meth:`Engine.lockedClock`
 
         """
         if lock:
             if self.isClockLocked():
                 logger.debug("The elapsed time clock is already locked")
             else:
+                assert self.csound is not None
                 self._lockedElapsedTime = self.csound.currentTimeSamples()/self.sr
         else:
             if not self._lockedElapsedTime:
                 logger.info("Asked to unlock the elapsed time clock, but it was not locked")
             self._lockedElapsedTime = 0
 
     def isClockLocked(self) -> bool:
@@ -1874,17 +1881,17 @@
         :meth:`~csoundengine.engine.Engine.unschedFuture`
         """
         assert self.csound is not None
         self.csound.rewindScore()
         self._setupGlobalInstrs()
 
     def session(self,
-                priorities: int = None,
-                maxControlsPerInstr: int = None,
-                numControlSlots: int = None
+                priorities: int | None = None,
+                maxControlsPerInstr: int | None = None,
+                numControlSlots: int | None = None
                 ) -> _session.Session:
         """
         Return the Session corresponding to this Engine
 
         Since each Engine can have only one associated Session,
         the parameters passed are only valid for the creation of
         the Session. Any subsequent call to this method returns the
@@ -2178,33 +2185,34 @@
         if delay == 0:
             callback()
             return
         token = self._getSyncToken()
         pargs = [self._builtinInstrs['pingback'], delay, 0.01, token]
         self._eventWithCallback(token, pargs, lambda token: callback())
 
-    def _eventWait(self, token: int, pargs: Sequence[float], timeout: float = None
+    def _eventWait(self, token: int, pargs: Sequence[float], timeout: float | None = None
                    ) -> float | None:
         if timeout is None:
             timeout = config['timeout']
-        assert timeout > 0
+        else:
+            assert timeout > 0
         q = self._registerSync(token)
         self._perfThread.scoreEvent(0, "i", pargs)
         try:
             outvalue = q.get(block=True, timeout=timeout)
             self._modified(False)
             return outvalue if outvalue != _UNSET else None
         except _queue.Empty:
             raise TimeoutError(f"{token=}, {pargs=}")
 
     def plotTableSpectrogram(self,
                              tabnum: int,
                              fftsize=2048,
                              mindb=-90,
-                             maxfreq: int = None,
+                             maxfreq: int | None = None,
                              overlap: int = 4,
                              minfreq: int = 0,
                              sr: int = 44100,
                              chan=0
                              ) -> None:
         """
         Plot a spectrogram of the audio data in the given table
@@ -2593,25 +2601,25 @@
             if err:
                 raise RuntimeError(f"Error while trying to retrieve/create a channel pointer: {err}")
             self._channelPointers[channel] = ptr
         assert ptr is not None
         return ptr
 
     def setChannel(self, channel: str, value: float | str | np.ndarray,
-                   method: str = None, delay=0.
+                   method='', delay=0.
                    ) -> None:
         """
         Set the value of a software channel
 
         Args:
             channel: the name of the channel
             value: the new value, should match the type of the channel (a float for
                 a control channel, a string for a string channel or a numpy array
                 for an audio channel)
-            method: one of ``'api'``, ``'score'``, ``'udp'``. None will choose the most appropriate
+            method: one of ``'api'``, ``'score'``, ``'udp'``. An empty str will choose the most appropriate
                 method for the current engine/args
             delay: a delay to set the channel
 
         Example
         ~~~~~~~
 
         >>> from csoundengine import *
@@ -2629,15 +2637,15 @@
         """
         assert self.csound is not None
         isaudio = isinstance(value, np.ndarray)
         if isaudio:
             method = "api"
         elif delay > 0:
             method = "score"
-        elif method is None:
+        elif not method:
             if self.udpPort and config['prefer_udp']:
                 method = 'udp'
             else:
                 method = 'api'
 
         if method == 'api':
             if isinstance(value, (int, float)):
@@ -2901,15 +2909,15 @@
         """
         abspath = os.path.abspath(include)
         for f in self.includes:
             if abspath == f:
                 return
         self.includes.append(abspath)
 
-    def readSoundfile(self, path="?", tabnum: int = None, chan=0,
+    def readSoundfile(self, path="?", tabnum: int | None = None, chan=0,
                       callback=None, block=False, skiptime=0.) -> int:
         """
         Read a soundfile into a table (via GEN1), returns the table number
 
         Args:
             path: the path to the output -- **"?" to open file interactively**
             tabnum: if given, a table index. If None, an index is
@@ -2969,15 +2977,15 @@
         elif block:
             self._inputMessageWait(token, msg)
         else:
             self._perfThread.inputMessage(msg)
         return tabnum
 
     def soundfontPlay(self, index: int, pitch: float, amp=0.7, delay=0.,
-                      dur=-1., vel: int = None, chan=1
+                      dur=-1., vel: int | None = None, chan=1
                       ) -> float:
         """
         Play a note of a previously loaded soundfont
 
         The soundfont's program (bank, preset) must have been read before
         via :meth:`Engine.soundfontPreparePreset`
 
@@ -3031,22 +3039,23 @@
 
         :meth:`~Engine.soundfontPreparePreset`
         :meth:`~Engine.playSample`
 
         """
         assert index in self._soundfontPresets.values()
         if vel is None:
-            vel = amp/127
+            vel = amp*127
         args = [pitch, amp, index, vel, chan]
         return self.sched(self._builtinInstrs['soundfontPlay'], delay=delay, dur=dur,
                           args=args)
 
     def soundfontPreparePreset(self,
                                sf2path: str,
-                               preset: tuple[int, int] = None) -> int:
+                               preset: tuple[int, int] | None = None
+                               ) -> int:
         """
         Prepare a soundfont's preset to be used
 
         Assigns an index to a soundfont bank:preset to be used with sfplay or via
         :meth:`~Engine.soundfontPlay`
 
         The soundfont is loaded if it was not loaded before
@@ -3087,15 +3096,15 @@
         instrnum = self._builtinInstrs['sfPresetAssignIndex']
         s = f'i {instrnum} 0 0 "{sf2path}" {bank} {presetnum} {idx}'
         self._perfThread.inputMessage(s)
         return idx
 
     def _readSoundfileAsync(self,
                             path: str,
-                            tabnum: int = None,
+                            tabnum: int | None = None,
                             chan=0) -> int:
         assert self.started
         if tabnum is None:
             tabnum = self._assignTableNumber()
         s = f'f {tabnum} 0 0 -1 "{path}" 0 0 {chan}'
         self._perfThread.inputMessage(s)
         return tabnum
@@ -3730,15 +3739,15 @@
                        dur=pairs[-2] + self.ksmps/self.sr,
                        args=args)
         else:
             for subdelay, subgroup in internal.splitAutomation(pairs, maxDataSize // 2):
                 self.automateBus(bus=bus, pairs=subgroup, delay=delay+subdelay,
                                  mode=mode, overtake=overtake)
 
-    def readBus(self, bus: int, default=0.) -> float:
+    def readBus(self, bus: int, default: float | None = None) -> float | None:
         """
         Read the current value of a control bus
 
         Buses can be used to allow communication between instruments, or
         between a running csound instrument and python. Buses are useful
         for continuous streams; when using buses to communicate discrete
         values with python an opcode like trighold might be necessary.
@@ -3857,15 +3866,15 @@
         pargs = [self._builtinInstrs['busrelease'], 0, 0, int(bus)]
         self._perfThread.scoreEvent(0, "i", pargs)
 
     def _dumpbus(self, bus: int):
         pargs = [self._builtinInstrs['busdump'], 0, 0, int(bus)]
         self._perfThread.scoreEvent(0, "i", pargs)
 
-    def assignBus(self, kind='', value: float = None, persist=False
+    def assignBus(self, kind='', value: float | None = None, persist=False
                   ) -> int:
         """
         Assign one audio/control bus, returns the bus number.
 
         Audio buses are always mono.
 
         Args:
```

### Comparing `csoundengine-2.8.2/csoundengine/engineorc.py` & `csoundengine-2.8.3/csoundengine/engineorc.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/event.py` & `csoundengine-2.8.3/csoundengine/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,16 @@
                  interpolation='linear', overtake=False) -> None:
         if self.automations is None:
             self.automations = []
         autom = SchedAutomation(param=param, pairs=pairs, delay=delay,
                                 interpolation=interpolation, overtake=overtake)
         self.automations.append(autom)
 
-    def set(self, param: str = '', value: float = None, delay=0., **kws):
+    def set(self, param='', value=0., delay=0., **kws):
         if param:
-            assert value is not None
             self.automate(param=param, pairs=(0, value), delay=delay)
         if kws:
             for param, value in kws.items():
                 self.set(param=param, value=value, delay=delay)
 
     def stop(self, delay=0.):
         dur = delay - self.delay
```

### Comparing `csoundengine-2.8.2/csoundengine/instr.py` & `csoundengine-2.8.3/csoundengine/instr.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,22 +226,22 @@
         '_defaultPfieldValues'
     )
 
     def __init__(self,
                  name: str,
                  body: str,
                  args: dict[str, float | str] | None = None,
-                 init: str = '',
-                 numchans: int = 1,
+                 init='',
+                 numchans=1,
                  preschedCallback=None,
-                 doc: str = '',
+                 doc='',
                  includes: list[str] | None = None,
-                 aliases: dict[str, str] = None,
-                 maxNamedArgs: int = 0,
-                 useDynamicPfields: bool = None
+                 aliases: dict[str, str] | None = None,
+                 maxNamedArgs=0,
+                 useDynamicPfields: bool | None = None
                  ) -> None:
 
         assert isinstance(name, str)
 
         if errmsg := _checkInstr(body):
             raise CsoundError(errmsg)
 
@@ -688,15 +688,15 @@
         return frozenset(pfields)
 
     def paramValue(self, param: str) -> float | str | None:
         param2 = self.unaliasParam(param, param)
         defaults = self.paramDefaultValues(aliased=True)
         if param2 not in defaults:
             raise KeyError(f"Unknown parameter '{param}'. "
-                           f"Possible parameters: {default.keys()}")
+                           f"Possible parameters: {defaults.keys()}")
         return defaults[param2]
 
     @cache
     def paramDefaultValues(self, aliases=True, aliased=False) -> dict[str, float]:
         """
         A dict mapping named parameters to their default values
         
@@ -928,14 +928,16 @@
         """
         assert isinstance(args, (list, tuple))
         assert not kws or isinstance(kws, dict)
         maxidx = self.maxPfieldIndex() - 5
         if kws:
             kwsindexes = [k if isinstance(k, int) else self.pfieldIndex(k) for k in kws]
             maxidx = max(maxidx, max(kwsindexes) - 5)
+        else:
+            kwsindexes = []
 
         numpfields = maxidx + 1
         if not args:
             defaultvals = self.defaultPfieldValues()
             if len(defaultvals) >= numpfields:
                 pargs = defaultvals.copy()
             else:
@@ -956,20 +958,20 @@
         if kws:
             for idx, value in zip(kwsindexes, kws.values()):
                 pargs[idx-5] = value
         return pargs
 
     def rec(self,
             dur: float,
-            outfile: str | None = None,
+            outfile='',
             args: list[float] | dict[str, float] | None = None,
             sr: int | None = None,
             ksmps: int | None = None,
             encoding: str | None = None,
-            nchnls: int = 2,
+            nchnls=2,
             wait=True,
             a4: int | None = None,
             delay=0.,
             **kws
             ) -> str:
         """
         Record this Instr for a given duration
```

### Comparing `csoundengine-2.8.2/csoundengine/instrtools.py` & `csoundengine-2.8.3/csoundengine/instrtools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/interact.py` & `csoundengine-2.8.3/csoundengine/interact.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/internal.py` & `csoundengine-2.8.3/csoundengine/internal.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/jacktools.py` & `csoundengine-2.8.3/csoundengine/jacktools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/jupytertools.py` & `csoundengine-2.8.3/csoundengine/jupytertools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/linuxaudio.py` & `csoundengine-2.8.3/csoundengine/linuxaudio.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/magic.py` & `csoundengine-2.8.3/csoundengine/magic.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/offline.py` & `csoundengine-2.8.3/csoundengine/offline.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,23 +229,25 @@
 
     """
     def __init__(self,
                  sr: int | None = None,
                  nchnls: int = 2,
                  ksmps: int | None = None,
                  a4: float | None = None,
-                 priorities: int = None,
+                 priorities: int | None = None,
                  numAudioBuses=1000,
                  numControlBuses=10000,
                  dynamicArgsPerInstr: int = 16,
-                 dynamicArgsSlots: int = None):
+                 dynamicArgsSlots: int | None = None):
 
         if priorities is None:
             priorities = config['session_priorities']
 
+        assert isinstance(priorities, int)
+
         self.sr = sr or config['rec_sr']
         """Samplerate"""
 
         self.nchnls = nchnls
         """Number of output channels"""
 
         self.ksmps = ksmps or config['rec_ksmps']
@@ -272,15 +274,15 @@
 
         self.numPriorities: int = priorities
         """Number of priorities in this Renderer"""
 
         self._idCounter = 0
         self._nameAndPriorityToInstrnum: dict[tuple[str, int], int] = {}
         self._instrnumToNameAndPriority: dict[int, tuple[str, int]] = {}
-        self._numbuckets = priorities
+        self._numbuckets: int = priorities
         self._bucketCounters = [0] * priorities
         self._startUserInstrs = 50
         self._instanceCounters: dict[int, int] = {}
         self._numInstancesPerInstr = 10000
         self._numAudioBuses = numAudioBuses
         self._numControlBuses = numControlBuses
         self._ndarrayHashToTabproxy: dict[str, TableProxy] = {}
@@ -512,21 +514,21 @@
             return False
         self.instrs[instr.name] = instr
         return True
 
     def defInstr(self,
                  name: str,
                  body: str,
-                 args: dict[str, float|str] = None,
+                 args: dict[str, float|str] | None = None,
                  init: str = '',
-                 priority: int = None,
+                 priority: int | None = None,
                  doc: str = '',
                  includes: list[str] | None = None,
-                 aliases: dict[str, str] = None,
-                 useDynamicPfields: bool = None,
+                 aliases: dict[str, str] | None = None,
+                 useDynamicPfields: bool | None = None,
                  **kws) -> Instr:
         """
         Create an :class:`~csoundengine.instr.Instr` and register it with this renderer
 
         Args:
             name (str): the name of the created instr
             body (str): the body of the instrument. It can have named
@@ -653,15 +655,15 @@
 
     def sched(self,
               instrname: str,
               delay=0.,
               dur=-1.,
               priority=1,
               args: Sequence[float | str] | dict[str, float] | None = None,
-              whenfinished: Callable = None,
+              whenfinished: Callable | None = None,
               relative=True,
               **kwargs
               ) -> SchedEvent:
         """
         Schedule an event
 
         Args:
@@ -971,20 +973,20 @@
                outfile='',
                endtime=0.,
                encoding='',
                wait=True,
                verbose: bool | None = None,
                openWhenDone=False,
                starttime=0.,
-               compressionBitrate: int = None,
-               sr: int = None,
-               ksmps: int = None,
+               compressionBitrate: int | None = None,
+               sr: int | None = None,
+               ksmps: int | None = None,
                tail=0.,
                numthreads=0,
-               csoundoptions: list[str] = None
+               csoundoptions: list[str] | None = None
                ) -> RenderJob:
         """
         Render to a soundfile
 
         To further customize the render set any csound options via
         :meth:`Renderer.setCsoundOptions`
 
@@ -1190,15 +1192,15 @@
 
         Returns:
             a list of all scheduled events with the given p1
 
         """
         return [ev for ev in self.scheduledEvents.values() if ev.p1 == p1]
 
-    def strSet(self, s: str, index: int = None) -> int:
+    def strSet(self, s: str, index: int | None = None) -> int:
         """
         Set a string in this renderer.
 
         The string can be retrieved in any instrument via strget. The index is
         determined by the Renderer itself, and it is guaranteed that calling
         strSet with the same string will result in the same index
```

### Comparing `csoundengine-2.8.2/csoundengine/offlineorc.py` & `csoundengine-2.8.3/csoundengine/offlineorc.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/paramtable.py` & `csoundengine-2.8.3/csoundengine/paramtable.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/plotting.py` & `csoundengine-2.8.3/csoundengine/plotting.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/schedevent.py` & `csoundengine-2.8.3/csoundengine/schedevent.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/session.py` & `csoundengine-2.8.3/csoundengine/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,32 +245,32 @@
 class _RenderingSessionHandler(SessionHandler):
     """
     Adapts a Session for offline rendering
     """
     def __init__(self, renderer: offline.Renderer):
         self.renderer = renderer
 
-    def schedEvent(self, event: csoundengine.event.Event):
+    def schedEvent(self, event: Event):
         return self.renderer.schedEvent(event)
 
     def makeTable(self,
                   data: np.ndarray | list[float] | None = None,
                   size: int | tuple[int, int] = 0,
                   sr: int = 0,
                   ) -> TableProxy:
-        self.renderer.makeTable(data=data, size=size, sr=sr)
+        return self.renderer.makeTable(data=data, size=size, sr=sr)
 
     def readSoundfile(self,
                       path: str,
                       chan=0,
                       skiptime=0.,
                       delay=0.,
                       force=False,
                       ) -> TableProxy:
-        self.renderer.readSoundfile(path)
+        return self.renderer.readSoundfile(path)
 
 
 class Session(AbstractRenderer):
     """
     A Session is associated (exclusively) to a running
     :class:`~csoundengine.engine.Engine` and manages instrument declarations
     and scheduled events. An Engine can be thought of as a low-level interface
@@ -346,34 +346,34 @@
         ''')
         synth = s.sched('sine', kfreq=440)
 
 
     """
     def __new__(cls,
                 engine: str | Engine | None = None,
-                priorities: int = None,
-                dynamicArgsPerInstr: int = None,
-                dynamicArgsSlots: int = None,
+                priorities: int | None = None,
+                dynamicArgsPerInstr: int | None = None,
+                dynamicArgsSlots: int | None = None,
                 **enginekws):
 
         if isinstance(engine, str):
             _engine = Engine.activeEngines.get(engine)
             if not _engine:
                 raise KeyError(f"Engine {engine} does not exist!")
         else:
             _engine = engine if isinstance(engine, Engine) else None
         if _engine and _engine._session:
             return _engine._session
         return super().__new__(cls)
 
     def __init__(self,
                  engine: str | Engine | None = None,
-                 priorities: int = None,
-                 maxControlsPerInstr: int = None,
-                 numControlSlots: int = None,
+                 priorities: int | None = None,
+                 maxControlsPerInstr: int | None = None,
+                 numControlSlots: int | None = None,
                  **enginekws
                  ) -> None:
         """
         A Session controls a csound Engine
 
         Normally a user does not create a Session directly, but calls the
         :meth:`Engine.session() <csoundengine.engine.Engine.session>`` method
@@ -778,21 +778,21 @@
     #     oldcallback = self._schedCallback
     #     self._schedCallback = callback
     #     return oldcallback
 
     def defInstr(self,
                  name: str,
                  body: str,
-                 args: dict[str, float|str] = None,
-                 init: str = '',
-                 priority: int = None,
-                 doc: str = '',
+                 args: dict[str, float|str] | None = None,
+                 init='',
+                 priority: int | None = None,
+                 doc='',
                  includes: list[str] | None = None,
-                 aliases: dict[str, str] = None,
-                 useDynamicPfields: bool = None,
+                 aliases: dict[str, str] | None = None,
+                 useDynamicPfields: bool | None = None,
                  **kws) -> Instr:
         """
         Create an :class:`~csoundengine.instr.Instr` and register it at this session
 
         Any init code given is compiled and executed at this point
 
         Args:
@@ -982,14 +982,16 @@
         See Also
         ~~~~~~~~
 
         :meth:`~Session.defInstr`
         """
         if instrname == "?":
             instrname = _dialogs.selectItem(list(self.instrs.keys()))
+            if instrname is None:
+                return None
         return self.instrs.get(instrname)
 
     def _getReifiedInstr(self, name: str, priority: int) -> _ReifiedInstr | None:
         registry = self._reifiedInstrDefs.get(name)
         if not registry:
             return None
         return registry.get(priority)
@@ -1069,15 +1071,15 @@
         :meth:`~Session.defInstr`
         """
         assert isinstance(priority, int) and 1 <= priority <= 10
         assert instrname in self.instrs
         rinstr, needssync = self.prepareSched(instrname, priority)
         return rinstr.instrnum
 
-    def assignBus(self, kind='', value: float = None, persist=False
+    def assignBus(self, kind='', value: float | None = None, persist=False
                   ) -> busproxy.Bus:
         """
         Creates a bus in the engine
 
         This is a wrapper around
         :meth:`Engine.assignBus() <csoundengine.engine.Engine.assignBus>`. Instead of returning
         a raw bus token it returns a :class:`~csoundengine.busproxy.Bus`, which can be used
@@ -1228,15 +1230,15 @@
                            whenfinished=event.whenfinished,
                            relative=event.relative,
                            **kws)
         if event.automations:
             for automation in event.automations:
                 synth.automate(param=automation.param,
                                pairs=automation.pairs,
-                               delay=automation.delay,
+                               delay=automation.delay or 0.,
                                mode=automation.interpolation,
                                overtake=automation.overtake)
         return synth
 
     def lockedClock(self, latency: float | None) -> Session:
         """
         context manager to ensure sync
@@ -1256,24 +1258,25 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.engine.isClockLocked():
             self.engine.popLock()
         self._lockedLatency = None
 
     def rendering(self,
-                  outfile: str = '',
-                  sr: int | None = None,
+                  outfile='',
+                  sr=0,
                   nchnls: int | None = None,
-                  ksmps: int | None = None,
+                  ksmps=0,
                   encoding='',
                   starttime=0.,
                   endtime=0.,
                   tail=0.,
                   openWhenDone=False,
-                  verbose: bool = None) -> Renderer:
+                  verbose: bool | None = None
+                  ) -> offline.Renderer:
         """
         A context-manager for offline rendering
 
         All scheduled events are rendered to `outfile` when exiting the
         context. The :class:`~csoundengine.offline.Renderer` returned by the
         context manager has the same interface as a :class:`Session` and can
         be used as a drop-in replacement. Any instrument or resource declared
@@ -1292,16 +1295,14 @@
             starttime: start rendering at the given time. Any event ending previous to
                 this time will not be rendered and any event between starttime and
                 endtime will be cropped
             endtime: stop rendering at the given time. This will either extend or crop
                 the rendering.
             tail: extra render time at the end, to accomodate extended releases
             openWhenDone: open the file in the default application after rendering.
-            redirect: if True, within the context any call to .sched will be
-                redirected to the offline Renderer
             verbose: if True, output rendering information. If None uses the value
                 specified in the config (``config['rec_suppress_output']``)
 
         Returns:
             a :class:`csoundengine.offline.Renderer`
     
         Example
@@ -1326,15 +1327,15 @@
         """
         renderer = self.makeRenderer(sr=sr or self.engine.sr,
                                      nchnls=nchnls or self.engine.nchnls,
                                      ksmps=ksmps)
         handler = _RenderingSessionHandler(renderer=renderer)
         self.setHandler(handler)
 
-        def atexit(r: Renderer, _outfile=outfile):
+        def atexit(r: offline.Renderer, _outfile=outfile):
             r.render(outfile=_outfile, endtime=endtime, encoding=encoding,
                      starttime=starttime, openWhenDone=openWhenDone,
                      tail=tail, verbose=verbose)
             self._offlineRenderer = None
             self.setHandler(None)
 
         renderer._registerExitCallback(atexit)
@@ -1509,17 +1510,19 @@
             raise RuntimeError("Session blocked during rendering")
 
         assert isinstance(priority, int) and 1 <= priority <= self.numPriorities
         assert self._dynargsArray is not None
         abstime = delay if not relative else self.engine.elapsedTime() + delay + self.engine.extraLatency
 
         if instrname == "?":
-            instrname = _dialogs.selectItem(list(self.instrs.keys()),
-                                            title="Select Instr",
-                                            ensureSelection=True)
+            selected = _dialogs.selectItem(list(self.instrs.keys()),
+                                           title="Select Instr",
+                                           ensureSelection=True)
+            assert selected is not None
+            instrname = selected
 
         instr = self.getInstr(instrname)
         if instr is None:
             raise ValueError(f"Instrument '{instrname}' not defined. "
                              f"Known instruments: {', '.join(self.instrs.keys())}")
 
         rinstr, needssync = self.prepareSched(instrname, priority, block=True)
@@ -1641,15 +1644,15 @@
         is called by a :class:`~csoundengine.synth.Synth` when
         :meth:`~csoundengine.synth.Synth.stop` is called.
 
         Args:
             event: the event to stop, either a Synth or the p1
             delay: how long to wait before stopping them
         """
-        if self.isRendering() and self._blockWhileRendering:
+        if self.isRendering():
             raise RuntimeError("This Session is blocked while in rendering mode. Call .unsched on the renderer instead")
 
         synthid = event if isinstance(event, (int, float)) else event.p1
         assert isinstance(synthid, (int, float))
         synth = self._synths.get(synthid)
         if not synth:
             logger.error(f"Event {event} not found, cannot unschedule")
@@ -1738,15 +1741,15 @@
                        numframes=88200, path='path/to/soundfile.flac',
                        freeself=False)
             >>> table.duration()
             2.0
             >>> session.playSample(table)
 
         """
-        if self.isRendering() and self._blockWhileRendering:
+        if self.isRendering():
             raise RuntimeError("This Session is blocked during rendering. Call .readSoundFile on the offline "
                                "renderer instead")
         if path == "?":
             path = _state.openSoundfile()
         if (table := self._pathToTabproxy.get(path)) is not None and not force:
             return table
         tabnum = self.engine.readSoundfile(path=path, chan=chan, skiptime=skiptime, block=block)
@@ -1797,15 +1800,15 @@
             delay: when to allocate the table. This has little use in realtime but is here
                 to comply to the signature.
 
         Returns:
             a TableProxy object
 
         """
-        if self.isRendering() and self._blockWhileRendering:
+        if self.isRendering():
             raise RuntimeError("This Session is in rendering mode. Call .makeTable on the renderer instead "
                                "(with session.rendering() as r: ... r.makeTable(...)")
 
         if self._handler is not None:
             try:
                 return self._handler.makeTable(data=data, size=size, sr=sr)
             except NotImplementedError:
@@ -1972,15 +1975,15 @@
             >>> samples, sr = lt.util.sndread("/path/to/soundfile")
             >>> partials = lt.analyze(samples, sr, resolution=50)
             >>> lt.util.partials_save_matrix(partials, outfile='packed.mtx')
             >>> session = ce.Engine().session()
             >>> session.playPartials(source='packed.mtx', speed=0.5)
 
         """
-        if self.isRendering() and self._blockWhileRendering:
+        if self.isRendering():
             raise RuntimeError("This Session is blocked during rendering")
 
         iskip, inumrows, inumcols = -1, 0, 0
 
         if isinstance(source, int):
             tabnum = source
         elif isinstance(source, TableProxy):
@@ -2082,15 +2085,15 @@
             crossfade: if looping, this indicates the length of the crossfade
             blockread: block while reading the source (if needed) before playback is scheduled
 
         Returns:
             A Synth with the following mutable parameters: kgain, kspeed, kchan, kpan
 
         """
-        if self.isRendering() and self._blockWhileRendering:
+        if self.isRendering():
             raise RuntimeError("This Session is in rendering mode. Call .playSample on the renderer instead")
 
         if isinstance(source, int):
             tabnum = source
         elif isinstance(source, TableProxy):
             tabnum = source.tabnum
         elif isinstance(source, str):
@@ -2123,26 +2126,27 @@
                                     ifadeout=fadeout,
                                     kchan=chan,
                                     kspeed=speed,
                                     kpan=pan,
                                     kgain=gain,
                                     ixfade=crossfade))
 
-    def makeRenderer(self, sr: int = None, nchnls: int = None, ksmps: int = None,
-                     ) -> Renderer:
+    def makeRenderer(self, sr=0, nchnls: int | None = None, ksmps=0,
+                     ) -> offline.Renderer:
         """
         Create a :class:`~csoundengine.offline.Renderer` (to render offline) with
         the instruments defined in this Session
 
         To schedule events, use the :meth:`~csoundengine.offline.Renderer.sched` method
         of the renderer
 
         Args:
             sr: the samplerate (see config['rec_sr'])
-            ksmps: ksmps used for rendering (see also config['rec_ksmps'])
+            ksmps: ksmps used for rendering (see also config['rec_ksmps']). 0 uses
+                the default defined in the config
             nchnls: the number of output channels. If not given, nchnls is taken
                 from the session
 
         Returns:
             a Renderer
 
         Example
```

### Comparing `csoundengine-2.8.2/csoundengine/sessionhandler.py` & `csoundengine-2.8.3/csoundengine/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/sessioninstrs.py` & `csoundengine-2.8.3/csoundengine/sessioninstrs.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/state.py` & `csoundengine-2.8.3/csoundengine/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def _isofmt(t:datetime) -> str:
     """Returns the time in iso format"""
     return t.isoformat(':', 'minutes')
 
 
 _defaultState = {
-    'last_run': datetime(1900, 1, 1).isoformat(),
+    'last_check': datetime(1900, 1, 1).isoformat(),
     'soundfont_last_dir': _home,
     'soundfile_last_dir': _home,
     'soundfile_save_last_dir': _home,
 }
 
 
 state = ConfigDict("csoundengine.state", _defaultState, persistent=True)
@@ -64,9 +64,7 @@
 def openSoundfont(filter="Soundfont (*.sf2)", title="Open Soundfont", ensureSelection=False):
     out = openFile("soundfont_last_dir", filter=filter, title=title)
     if not out and ensureSelection:
         raise ValueError("No soundfont selected")
     return out
 
 
-
-
```

### Comparing `csoundengine-2.8.2/csoundengine/synth.py` & `csoundengine-2.8.3/csoundengine/synth.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
     def __repr__(self):
         playstr = _synthStatusIcon[self.playStatus()]
         parts = [f'{playstr} {self.instr.name}={self.p1} start={self.start:.3f} dur={self.dur:.3f}']
 
         if self.instr.hasControls():
             ctrlparts = []
             for k, v in self.instr.controls.items():
-                if k in self.controls:
+                if self.controls is not None and k in self.controls:
                     v = self.controls[k]
                 ctrlparts.append(f'{k}={v}')
             parts.append(f"|{' '.join(ctrlparts)}|")
         if self.args:
             showpidx = config['synth_repr_show_pfield_index']
             maxi = config['synth_repr_max_args']
             i2n = self.instr.pfieldIndexToName
@@ -531,15 +531,15 @@
 
     def stop(self, delay=0.) -> None:
         if self.finished():
             return
         self.session.unsched(self.p1, delay=delay)
 
 
-def _synthsCreateHtmlTable(synths: list[Synth], maxrows: int = None, tablestyle='',
+def _synthsCreateHtmlTable(synths: list[Synth], maxrows: int | None = None, tablestyle='',
                            ) -> str:
     synth0 = synths[0]
     instr0 = synth0.instr
     if any(synth.instr.name != instr0.name for synth in synths):
         # multiple instrs per group, not allowed here
         raise ValueError("Only synths of the same instr allowed here")
 
@@ -770,15 +770,15 @@
                     for synth in self
                     if param in synth.instr.dynamicPfieldNames()]
         if not eventids:
             raise ValueError(f"Parameter '{param}' unknown for group, possible "
                              f"parameters: {self.dynamicParamNames()}")
         return eventids
 
-    def _htmlTable(self, style='', maxrows: int = None) -> str:
+    def _htmlTable(self, style='', maxrows: int | None = None) -> str:
         subgroups = _iterlib.classify(self.synths, lambda synth: synth.instr.name)
         lines = []
         instrcol = jupytertools.defaultPalette["name.color"]
         for instrname, synths in subgroups.items():
             lines.append(f'<p><small>Instr: <strong style="color:{instrcol}">'
                          f'{instrname}'
                          f'</strong> - <b>{len(synths)}</b> synths</small></p>')
```

### Comparing `csoundengine-2.8.2/csoundengine/tableproxy.py` & `csoundengine-2.8.3/csoundengine/tableproxy.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/termui.py` & `csoundengine-2.8.3/csoundengine/termui.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine/tools.py` & `csoundengine-2.8.3/csoundengine/tools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/csoundengine.egg-info/PKG-INFO` & `csoundengine-2.8.3/csoundengine.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,40 @@
 Metadata-Version: 2.1
 Name: csoundengine
-Version: 2.8.2
+Version: 2.8.3
 Summary: A synthesis framework using csound
 Home-page: https://github.com/gesellkammer/csoundengine
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: cachetools
+Requires-Dist: JACK-client
+Requires-Dist: appdirs
+Requires-Dist: pygments
+Requires-Dist: sf2utils
+Requires-Dist: ipywidgets
+Requires-Dist: progressbar2
+Requires-Dist: xxhash
+Requires-Dist: docstring-parser
+Requires-Dist: ctcsound7>=0.4.6
+Requires-Dist: sndfileio>=1.9.4
+Requires-Dist: emlib>=1.14.1
+Requires-Dist: configdict>=2.10.0
+Requires-Dist: bpf4>=1.10.1
+Requires-Dist: numpyx>=1.3.3
+Requires-Dist: pitchtools>=1.14.0
+Requires-Dist: risset>=2.9.1
+Requires-Dist: sounddevice
 
 csoundengine
 ============
 
 |sh-month|
 
 .. |sh-month| image:: https://static.pepy.tech/badge/csoundengine/month
```

### Comparing `csoundengine-2.8.2/csoundengine.egg-info/SOURCES.txt` & `csoundengine-2.8.3/csoundengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/setup.py` & `csoundengine-2.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 import os
 
-version = (2, 8, 2)
+version = (2, 8, 3)
 
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 
@@ -49,18 +49,18 @@
         "xxhash",
         "docstring-parser",
 
         "ctcsound7>=0.4.6",
         "sndfileio>=1.9.4",
         "emlib>=1.14.1",
         "configdict>=2.10.0",
-        "bpf4>=1.8.6",
-        "numpyx>=1.3.1",
-        "pitchtools>=1.12.0",
-        "risset>=2.7.7",
+        "bpf4>=1.10.1",
+        "numpyx>=1.3.3",
+        "pitchtools>=1.14.0",
+        "risset>=2.9.1",
         "sounddevice"
     ],
     license="BSD",
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)'
     ],
```

### Comparing `csoundengine-2.8.2/test/test1.py` & `csoundengine-2.8.3/test/test1.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.2/test/test2.py` & `csoundengine-2.8.3/test/test2.py`

 * *Files identical despite different names*

