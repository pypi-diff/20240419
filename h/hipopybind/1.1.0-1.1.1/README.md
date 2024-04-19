# Comparing `tmp/hipopybind-1.1.0.tar.gz` & `tmp/hipopybind-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipopybind-1.1.0.tar", last modified: Fri Apr 19 15:54:30 2024, max compression
+gzip compressed data, was "hipopybind-1.1.1.tar", last modified: Fri Apr 19 18:06:12 2024, max compression
```

## Comparing `hipopybind-1.1.0.tar` & `hipopybind-1.1.1.tar`

### file list

```diff
@@ -1,548 +1,548 @@
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.403132 hipopybind-1.1.0/
--rw-r--r--   0 mfm45      (503) staff       (20)     1296 2024-04-17 20:52:18.000000 hipopybind-1.1.0/CMakeLists.txt
--rw-r--r--   0 mfm45      (503) staff       (20)     1098 2024-04-17 20:52:18.000000 hipopybind-1.1.0/LICENSE
--rw-r--r--   0 mfm45      (503) staff       (20)      146 2024-04-18 19:12:47.000000 hipopybind-1.1.0/MANIFEST.in
--rw-r--r--   0 mfm45      (503) staff       (20)     1136 2024-04-19 15:54:30.402489 hipopybind-1.1.0/PKG-INFO
--rw-r--r--   0 mfm45      (503) staff       (20)      738 2024-04-19 15:53:11.000000 hipopybind-1.1.0/README.md
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.474199 hipopybind-1.1.0/hipo/
--rw-r--r--   0 mfm45      (503) staff       (20)       29 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/.git
--rw-r--r--   0 mfm45      (503) staff       (20)       64 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/.gitmodules
--rw-r--r--   0 mfm45      (503) staff       (20)     5549 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/CMakeLists.txt
--rw-r--r--   0 mfm45      (503) staff       (20)     1772 2024-04-18 17:50:41.000000 hipopybind-1.1.0/hipo/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)      670 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/README.md
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.489876 hipopybind-1.1.0/hipo/ai/
--rw-r--r--   0 mfm45      (503) staff       (20)      865 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/ai/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     2796 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/ai/analyze.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     4425 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/ai/cluster.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     1582 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/ai/cluster.h
--rw-r--r--   0 mfm45      (503) staff       (20)     4224 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/ai/dcana.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     1112 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/ai/dcana.h
--rw-r--r--   0 mfm45      (503) staff       (20)     2804 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/ai/main.cc
--rw-r--r--   0 mfm45      (503) staff       (20)    15296 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/ai/track.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     4064 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/ai/track.h
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.493470 hipopybind-1.1.0/hipo/cmake/
--rw-r--r--   0 mfm45      (503) staff       (20)     1425 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/cmake/LZ4Config.cmake
--rw-r--r--   0 mfm45      (503) staff       (20)      278 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/cmake/hipo4Config.cmake.in
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.511751 hipopybind-1.1.0/hipo/examples/
--rw-r--r--   0 mfm45      (503) staff       (20)     1406 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/Makefile
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.515590 hipopybind-1.1.0/hipo/examples/benchmarks/
--rw-r--r--   0 mfm45      (503) staff       (20)      898 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/benchmarks/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     3929 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/benchmarks/ana_benchmark.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     5502 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/benchmarks/map_benchmark.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     2371 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/builder.cc
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.518213 hipopybind-1.1.0/hipo/examples/fortran/
--rw-r--r--   0 mfm45      (503) staff       (20)      930 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/fortran/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)      837 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/fortran/freader.F
--rw-r--r--   0 mfm45      (503) staff       (20)     2424 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/readEvents.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     2650 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/readFile.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     2029 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/readFileTags.cc
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.530242 hipopybind-1.1.0/hipo/examples/root/
--rw-r--r--   0 mfm45      (503) staff       (20)     1712 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/root/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     4530 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/root/benchmark_hipo.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     5399 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/root/benchmark_hipo_ana.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     4036 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/root/benchmark_hipo_cwise.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     4325 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/root/benchmark_root.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     6485 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/root/converter.cc
--rwxr-xr-x   0 mfm45      (503) staff       (20)      109 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/root/ramdisk.sh
--rw-r--r--   0 mfm45      (503) staff       (20)     2093 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/schema.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     2090 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/showFile.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     1697 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/writeEvents.cc
--rw-r--r--   0 mfm45      (503) staff       (20)     4858 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/writeFile.cc
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.532217 hipopybind-1.1.0/hipo/examples/xrootd/
--rw-r--r--   0 mfm45      (503) staff       (20)     1041 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/xrootd/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     1160 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/examples/xrootd/readFileXrootd.cc
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.568564 hipopybind-1.1.0/hipo/hipo4/
--rw-r--r--   0 mfm45      (503) staff       (20)      715 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     8242 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/bank.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    20013 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/bank.h
--rw-r--r--   0 mfm45      (503) staff       (20)     3693 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/datastream.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     4795 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/datastream.h
--rw-r--r--   0 mfm45      (503) staff       (20)     4504 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/dictionary.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     3858 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/dictionary.h
--rw-r--r--   0 mfm45      (503) staff       (20)     8726 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/event.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     4198 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/event.h
--rw-r--r--   0 mfm45      (503) staff       (20)      682 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/hipoexceptions.h
--rw-r--r--   0 mfm45      (503) staff       (20)    19589 2024-04-19 15:52:04.000000 hipopybind-1.1.0/hipo/hipo4/reader.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     8618 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/reader.h
--rw-r--r--   0 mfm45      (503) staff       (20)    24717 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/record.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     5919 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/record.h
--rw-r--r--   0 mfm45      (503) staff       (20)     6531 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/recordbuilder.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     1796 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/recordbuilder.h
--rw-r--r--   0 mfm45      (503) staff       (20)    10276 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/utils.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     2731 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/utils.h
--rw-r--r--   0 mfm45      (503) staff       (20)    13945 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/wrapper.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     8264 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/writer.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     6581 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/hipo4/writer.h
--rwxr-xr-x   0 mfm45      (503) staff       (20)   222928 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/libhipo4.dylib
--rwxr-xr-x   0 mfm45      (503) staff       (20)   367480 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/libhipo4.so
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.585823 hipopybind-1.1.0/hipo/lz4/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.586856 hipopybind-1.1.0/hipo/lz4/.circleci/
--rw-r--r--   0 mfm45      (503) staff       (20)     5030 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/.circleci/config.yml
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.416413 hipopybind-1.1.0/hipo/lz4/.circleci/images/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.591224 hipopybind-1.1.0/hipo/lz4/.circleci/images/primary/
--rw-r--r--   0 mfm45      (503) staff       (20)      644 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/.circleci/images/primary/Dockerfile
--rw-r--r--   0 mfm45      (503) staff       (20)       44 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/.git
--rw-r--r--   0 mfm45      (503) staff       (20)      348 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/.gitattributes
--rw-r--r--   0 mfm45      (503) staff       (20)      315 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/.gitignore
--rw-r--r--   0 mfm45      (503) staff       (20)     5714 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/.travis.yml
--rw-r--r--   0 mfm45      (503) staff       (20)      630 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/INSTALL
--rw-r--r--   0 mfm45      (503) staff       (20)      565 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/LICENSE
--rw-r--r--   0 mfm45      (503) staff       (20)     6663 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     1688 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/Makefile.inc
--rw-r--r--   0 mfm45      (503) staff       (20)    13759 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/NEWS
--rw-r--r--   0 mfm45      (503) staff       (20)     5534 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/README.md
--rw-r--r--   0 mfm45      (503) staff       (20)     5862 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/appveyor.yml
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.421434 hipopybind-1.1.0/hipo/lz4/contrib/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.593486 hipopybind-1.1.0/hipo/lz4/contrib/cmake_unofficial/
--rw-r--r--   0 mfm45      (503) staff       (20)       97 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/cmake_unofficial/.gitignore
--rw-r--r--   0 mfm45      (503) staff       (20)     8188 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/cmake_unofficial/CMakeLists.txt
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.605196 hipopybind-1.1.0/hipo/lz4/contrib/debian/
--rw-r--r--   0 mfm45      (503) staff       (20)      475 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/debian/changelog
--rw-r--r--   0 mfm45      (503) staff       (20)        2 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/debian/compat
--rw-r--r--   0 mfm45      (503) staff       (20)      612 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/debian/control
--rw-r--r--   0 mfm45      (503) staff       (20)      325 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/debian/copyright
--rw-r--r--   0 mfm45      (503) staff       (20)        8 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/debian/dirs
--rw-r--r--   0 mfm45      (503) staff       (20)        0 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/debian/docs
--rw-r--r--   0 mfm45      (503) staff       (20)       35 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/debian/liblz4-dev.install
--rw-r--r--   0 mfm45      (503) staff       (20)       30 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/debian/liblz4.install
--rwxr-xr-x   0 mfm45      (503) staff       (20)      188 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/debian/rules
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.611943 hipopybind-1.1.0/hipo/lz4/contrib/djgpp/
--rw-r--r--   0 mfm45      (503) staff       (20)     1292 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/djgpp/LICENSE
--rw-r--r--   0 mfm45      (503) staff       (20)     3524 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/djgpp/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     1125 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/djgpp/README.MD
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.618746 hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/
--rw-r--r--   0 mfm45      (503) staff       (20)       28 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/.gitignore
--rw-r--r--   0 mfm45      (503) staff       (20)     3020 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     1144 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/README.md
--rw-r--r--   0 mfm45      (503) staff       (20)      613 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/gen-lz4-manual.sh
--rw-r--r--   0 mfm45      (503) staff       (20)     8697 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/gen_manual.cpp
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.631018 hipopybind-1.1.0/hipo/lz4/contrib/meson/
--rw-r--r--   0 mfm45      (503) staff       (20)     1307 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/GetLz4LibraryVersion.py
--rw-r--r--   0 mfm45      (503) staff       (20)     2120 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/InstallSymlink.py
--rw-r--r--   0 mfm45      (503) staff       (20)      838 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/README.md
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.632614 hipopybind-1.1.0/hipo/lz4/contrib/meson/contrib/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.634539 hipopybind-1.1.0/hipo/lz4/contrib/meson/contrib/gen_manual/
--rw-r--r--   0 mfm45      (503) staff       (20)     1531 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/contrib/gen_manual/meson.build
--rw-r--r--   0 mfm45      (503) staff       (20)      495 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/contrib/meson.build
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.636068 hipopybind-1.1.0/hipo/lz4/contrib/meson/examples/
--rw-r--r--   0 mfm45      (503) staff       (20)     1975 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/examples/meson.build
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.638487 hipopybind-1.1.0/hipo/lz4/contrib/meson/lib/
--rw-r--r--   0 mfm45      (503) staff       (20)     2027 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/lib/meson.build
--rw-r--r--   0 mfm45      (503) staff       (20)     3953 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/meson.build
--rw-r--r--   0 mfm45      (503) staff       (20)     1196 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/meson_options.txt
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.643111 hipopybind-1.1.0/hipo/lz4/contrib/meson/programs/
--rw-r--r--   0 mfm45      (503) staff       (20)     2025 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/programs/meson.build
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.645219 hipopybind-1.1.0/hipo/lz4/contrib/meson/tests/
--rw-r--r--   0 mfm45      (503) staff       (20)     3306 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/meson/tests/meson.build
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.649657 hipopybind-1.1.0/hipo/lz4/contrib/snap/
--rw-r--r--   0 mfm45      (503) staff       (20)     1172 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/snap/README.md
--rw-r--r--   0 mfm45      (503) staff       (20)     1115 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/contrib/snap/snapcraft.yaml
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.656420 hipopybind-1.1.0/hipo/lz4/doc/
--rw-r--r--   0 mfm45      (503) staff       (20)     6422 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/doc/lz4_Block_format.md
--rw-r--r--   0 mfm45      (503) staff       (20)    14421 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/doc/lz4_Frame_format.md
--rw-r--r--   0 mfm45      (503) staff       (20)    30346 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/doc/lz4_manual.html
--rw-r--r--   0 mfm45      (503) staff       (20)    20733 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/doc/lz4frame_manual.html
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.680093 hipopybind-1.1.0/hipo/lz4/examples/
--rw-r--r--   0 mfm45      (503) staff       (20)      143 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/.gitignore
--rw-r--r--   0 mfm45      (503) staff       (20)    18092 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/COPYING
--rw-r--r--   0 mfm45      (503) staff       (20)     6057 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/HCStreaming_ringBuffer.c
--rw-r--r--   0 mfm45      (503) staff       (20)     3685 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)      313 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/README.md
--rw-r--r--   0 mfm45      (503) staff       (20)     4832 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_doubleBuffer.c
--rw-r--r--   0 mfm45      (503) staff       (20)     2749 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_doubleBuffer.md
--rw-r--r--   0 mfm45      (503) staff       (20)     5383 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_lineByLine.c
--rw-r--r--   0 mfm45      (503) staff       (20)     3648 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_lineByLine.md
--rw-r--r--   0 mfm45      (503) staff       (20)     4981 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_ringBuffer.c
--rw-r--r--   0 mfm45      (503) staff       (20)    27116 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/compress_functions.c
--rw-r--r--   0 mfm45      (503) staff       (20)     8116 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/dictionaryRandomAccess.c
--rw-r--r--   0 mfm45      (503) staff       (20)     2100 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/dictionaryRandomAccess.md
--rw-r--r--   0 mfm45      (503) staff       (20)    13397 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/frameCompress.c
--rw-r--r--   0 mfm45      (503) staff       (20)      269 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/printVersion.c
--rw-r--r--   0 mfm45      (503) staff       (20)     5496 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/simple_buffer.c
--rw-r--r--   0 mfm45      (503) staff       (20)     3615 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/examples/streaming_api_basics.md
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.716477 hipopybind-1.1.0/hipo/lz4/lib/
--rw-r--r--   0 mfm45      (503) staff       (20)       34 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/.gitignore
--rw-r--r--   0 mfm45      (503) staff       (20)     1311 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/LICENSE
--rw-r--r--   0 mfm45      (503) staff       (20)     8431 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     5149 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/README.md
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.423433 hipopybind-1.1.0/hipo/lz4/lib/dll/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.730407 hipopybind-1.1.0/hipo/lz4/lib/dll/example/
--rw-r--r--   0 mfm45      (503) staff       (20)     2031 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/dll/example/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     3013 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/dll/example/README.md
--rw-r--r--   0 mfm45      (503) staff       (20)     1269 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/dll/example/fullbench-dll.sln
--rw-r--r--   0 mfm45      (503) staff       (20)    10157 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/dll/example/fullbench-dll.vcxproj
--rw-r--r--   0 mfm45      (503) staff       (20)     1109 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/liblz4-dll.rc.in
--rw-r--r--   0 mfm45      (503) staff       (20)      385 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/liblz4.pc.in
--rw-r--r--   0 mfm45      (503) staff       (20)    97210 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/lz4.c
--rw-r--r--   0 mfm45      (503) staff       (20)    39943 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/lz4.h
--rw-r--r--   0 mfm45      (503) staff       (20)    77571 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/lz4frame.c
--rw-r--r--   0 mfm45      (503) staff       (20)    28657 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/lz4frame.h
--rw-r--r--   0 mfm45      (503) staff       (20)     2044 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/lz4frame_static.h
--rw-r--r--   0 mfm45      (503) staff       (20)    62843 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/lz4hc.c
--rw-r--r--   0 mfm45      (503) staff       (20)    21357 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/lz4hc.h
--rw-r--r--   0 mfm45      (503) staff       (20)    34045 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/xxhash.c
--rw-r--r--   0 mfm45      (503) staff       (20)    13466 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/lib/xxhash.h
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.810307 hipopybind-1.1.0/hipo/lz4/programs/
--rw-r--r--   0 mfm45      (503) staff       (20)      169 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/.gitignore
--rw-r--r--   0 mfm45      (503) staff       (20)    18092 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/COPYING
--rw-r--r--   0 mfm45      (503) staff       (20)     5681 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     3541 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/README.md
--rw-r--r--   0 mfm45      (503) staff       (20)    22491 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/bench.c
--rw-r--r--   0 mfm45      (503) staff       (20)     1484 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/bench.h
--rw-r--r--   0 mfm45      (503) staff       (20)     5938 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/datagen.c
--rw-r--r--   0 mfm45      (503) staff       (20)     1687 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/datagen.h
--rw-r--r--   0 mfm45      (503) staff       (20)      851 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/lz4-exe.rc.in
--rw-r--r--   0 mfm45      (503) staff       (20)     9011 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/lz4.1
--rw-r--r--   0 mfm45      (503) staff       (20)     8203 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/lz4.1.md
--rw-r--r--   0 mfm45      (503) staff       (20)    33979 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/lz4cli.c
--rw-r--r--   0 mfm45      (503) staff       (20)    61886 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/lz4io.c
--rw-r--r--   0 mfm45      (503) staff       (20)     5199 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/lz4io.h
--rw-r--r--   0 mfm45      (503) staff       (20)     6822 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/platform.h
--rw-r--r--   0 mfm45      (503) staff       (20)    20176 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/programs/util.h
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.840362 hipopybind-1.1.0/hipo/lz4/tests/
--rw-r--r--   0 mfm45      (503) staff       (20)      185 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/.gitignore
--rw-r--r--   0 mfm45      (503) staff       (20)    18092 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/COPYING
--rw-r--r--   0 mfm45      (503) staff       (20)    18428 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     3503 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/README.md
--rw-r--r--   0 mfm45      (503) staff       (20)    11005 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/checkFrame.c
--rw-r--r--   0 mfm45      (503) staff       (20)     2554 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/checkTag.c
--rw-r--r--   0 mfm45      (503) staff       (20)     5740 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/datagencli.c
--rw-r--r--   0 mfm45      (503) staff       (20)    51673 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/frametest.c
--rw-r--r--   0 mfm45      (503) staff       (20)    30685 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/fullbench.c
--rw-r--r--   0 mfm45      (503) staff       (20)    85263 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/fuzzer.c
--rw-r--r--   0 mfm45      (503) staff       (20)     7308 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/roundTripTest.c
--rw-r--r--   0 mfm45      (503) staff       (20)    12437 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/test-lz4-list.py
--rw-r--r--   0 mfm45      (503) staff       (20)    16792 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/test-lz4-speed.py
--rw-r--r--   0 mfm45      (503) staff       (20)     5376 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/test-lz4-versions.py
--rwxr-xr-x   0 mfm45      (503) staff       (20)     1901 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/test_custom_block_sizes.sh
--rwxr-xr-x   0 mfm45      (503) staff       (20)      789 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/tests/test_install.sh
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.845267 hipopybind-1.1.0/hipo/lz4/visual/
--rw-r--r--   0 mfm45      (503) staff       (20)       76 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/.gitignore
--rw-r--r--   0 mfm45      (503) staff       (20)     2887 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/README.md
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.846413 hipopybind-1.1.0/hipo/lz4/visual/VS2010/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.850666 hipopybind-1.1.0/hipo/lz4/visual/VS2010/datagen/
--rw-r--r--   0 mfm45      (503) staff       (20)     9272 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/datagen/datagen.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.851486 hipopybind-1.1.0/hipo/lz4/visual/VS2010/frametest/
--rw-r--r--   0 mfm45      (503) staff       (20)     9623 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/frametest/frametest.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.853388 hipopybind-1.1.0/hipo/lz4/visual/VS2010/fullbench/
--rw-r--r--   0 mfm45      (503) staff       (20)     9623 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/fullbench/fullbench.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.855763 hipopybind-1.1.0/hipo/lz4/visual/VS2010/fullbench-dll/
--rw-r--r--   0 mfm45      (503) staff       (20)    10445 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/fullbench-dll/fullbench-dll.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.858975 hipopybind-1.1.0/hipo/lz4/visual/VS2010/fuzzer/
--rw-r--r--   0 mfm45      (503) staff       (20)     9451 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/fuzzer/fuzzer.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.860892 hipopybind-1.1.0/hipo/lz4/visual/VS2010/liblz4/
--rw-r--r--   0 mfm45      (503) staff       (20)     9512 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/liblz4/liblz4.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.864783 hipopybind-1.1.0/hipo/lz4/visual/VS2010/liblz4-dll/
--rw-r--r--   0 mfm45      (503) staff       (20)     1388 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0 mfm45      (503) staff       (20)     9616 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/liblz4-dll/liblz4-dll.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.867308 hipopybind-1.1.0/hipo/lz4/visual/VS2010/lz4/
--rw-r--r--   0 mfm45      (503) staff       (20)     1388 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/lz4/lz4.rc
--rw-r--r--   0 mfm45      (503) staff       (20)    10285 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/lz4/lz4.vcxproj
--rw-r--r--   0 mfm45      (503) staff       (20)     6761 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2010/lz4.sln
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.868148 hipopybind-1.1.0/hipo/lz4/visual/VS2017/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.869136 hipopybind-1.1.0/hipo/lz4/visual/VS2017/datagen/
--rw-r--r--   0 mfm45      (503) staff       (20)     9454 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2017/datagen/datagen.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.870198 hipopybind-1.1.0/hipo/lz4/visual/VS2017/frametest/
--rw-r--r--   0 mfm45      (503) staff       (20)     9805 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2017/frametest/frametest.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.873064 hipopybind-1.1.0/hipo/lz4/visual/VS2017/fullbench/
--rw-r--r--   0 mfm45      (503) staff       (20)     9805 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2017/fullbench/fullbench.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.874181 hipopybind-1.1.0/hipo/lz4/visual/VS2017/fullbench-dll/
--rw-r--r--   0 mfm45      (503) staff       (20)    10626 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.874833 hipopybind-1.1.0/hipo/lz4/visual/VS2017/fuzzer/
--rw-r--r--   0 mfm45      (503) staff       (20)     9633 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.875641 hipopybind-1.1.0/hipo/lz4/visual/VS2017/liblz4/
--rw-r--r--   0 mfm45      (503) staff       (20)     9694 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2017/liblz4/liblz4.vcxproj
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.878327 hipopybind-1.1.0/hipo/lz4/visual/VS2017/liblz4-dll/
--rw-r--r--   0 mfm45      (503) staff       (20)     1388 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
--rw-r--r--   0 mfm45      (503) staff       (20)     9797 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
--rw-r--r--   0 mfm45      (503) staff       (20)     6193 2024-04-18 17:49:46.000000 hipopybind-1.1.0/hipo/lz4/visual/VS2017/lz4.sln
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.879118 hipopybind-1.1.0/hipo/python/
--rw-r--r--   0 mfm45      (503) staff       (20)     1068 2024-04-18 17:47:31.000000 hipopybind-1.1.0/hipo/python/hiporeader.py
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.401434 hipopybind-1.1.0/hipopybind.egg-info/
--rw-r--r--   0 mfm45      (503) staff       (20)     1136 2024-04-19 15:54:29.000000 hipopybind-1.1.0/hipopybind.egg-info/PKG-INFO
--rw-r--r--   0 mfm45      (503) staff       (20)    15284 2024-04-19 15:54:29.000000 hipopybind-1.1.0/hipopybind.egg-info/SOURCES.txt
--rw-r--r--   0 mfm45      (503) staff       (20)        1 2024-04-19 15:54:29.000000 hipopybind-1.1.0/hipopybind.egg-info/dependency_links.txt
--rw-r--r--   0 mfm45      (503) staff       (20)        1 2024-04-18 17:59:16.000000 hipopybind-1.1.0/hipopybind.egg-info/not-zip-safe
--rw-r--r--   0 mfm45      (503) staff       (20)       20 2024-04-19 15:54:29.000000 hipopybind-1.1.0/hipopybind.egg-info/requires.txt
--rw-r--r--   0 mfm45      (503) staff       (20)       11 2024-04-19 15:54:29.000000 hipopybind-1.1.0/hipopybind.egg-info/top_level.txt
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.922783 hipopybind-1.1.0/pybind11/
--rw-r--r--   0 mfm45      (503) staff       (20)     1271 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.appveyor.yml
--rw-r--r--   0 mfm45      (503) staff       (20)      996 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.clang-format
--rw-r--r--   0 mfm45      (503) staff       (20)     2605 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.clang-tidy
--rw-r--r--   0 mfm45      (503) staff       (20)     2196 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.cmake-format.yaml
--rw-r--r--   0 mfm45      (503) staff       (20)       33 2024-04-17 20:52:24.000000 hipopybind-1.1.0/pybind11/.git
--rw-r--r--   0 mfm45      (503) staff       (20)       18 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.gitattributes
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.947566 hipopybind-1.1.0/pybind11/.github/
--rw-r--r--   0 mfm45      (503) staff       (20)      182 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/CODEOWNERS
--rw-r--r--   0 mfm45      (503) staff       (20)    15271 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.988992 hipopybind-1.1.0/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mfm45      (503) staff       (20)     2016 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 mfm45      (503) staff       (20)      328 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 mfm45      (503) staff       (20)      162 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/dependabot.yml
--rw-r--r--   0 mfm45      (503) staff       (20)      116 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/labeler.yml
--rw-r--r--   0 mfm45      (503) staff       (20)       50 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/labeler_merged.yml
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.993884 hipopybind-1.1.0/pybind11/.github/matchers/
--rw-r--r--   0 mfm45      (503) staff       (20)      668 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/matchers/pylint.json
--rw-r--r--   0 mfm45      (503) staff       (20)      645 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.002105 hipopybind-1.1.0/pybind11/.github/workflows/
--rw-r--r--   0 mfm45      (503) staff       (20)    28217 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 mfm45      (503) staff       (20)     2095 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 mfm45      (503) staff       (20)     1419 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/workflows/format.yml
--rw-r--r--   0 mfm45      (503) staff       (20)      333 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 mfm45      (503) staff       (20)     2558 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 mfm45      (503) staff       (20)     2837 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0 mfm45      (503) staff       (20)      487 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.gitignore
--rw-r--r--   0 mfm45      (503) staff       (20)     4083 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 mfm45      (503) staff       (20)       62 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/.readthedocs.yml
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.003260 hipopybind-1.1.0/pybind11/CMakeFiles/
--rw-r--r--   0 mfm45      (503) staff       (20)      622 2024-04-17 20:53:03.000000 hipopybind-1.1.0/pybind11/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0 mfm45      (503) staff       (20)        2 2024-04-17 20:53:03.000000 hipopybind-1.1.0/pybind11/CMakeFiles/progress.marks
--rw-r--r--   0 mfm45      (503) staff       (20)    11687 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/CMakeLists.txt
--rw-r--r--   0 mfm45      (503) staff       (20)     1684 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/LICENSE
--rw-r--r--   0 mfm45      (503) staff       (20)      223 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/MANIFEST.in
--rw-r--r--   0 mfm45      (503) staff       (20)     6512 2024-04-17 20:53:02.000000 hipopybind-1.1.0/pybind11/Makefile
--rw-r--r--   0 mfm45      (503) staff       (20)     7686 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/README.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     1149 2024-04-17 20:53:03.000000 hipopybind-1.1.0/pybind11/cmake_install.cmake
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.067617 hipopybind-1.1.0/pybind11/docs/
--rw-r--r--   0 mfm45      (503) staff       (20)      607 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/Doxyfile
--rw-r--r--   0 mfm45      (503) staff       (20)     7417 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/Makefile
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.436093 hipopybind-1.1.0/pybind11/docs/_static/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.070599 hipopybind-1.1.0/pybind11/docs/_static/css/
--rw-r--r--   0 mfm45      (503) staff       (20)       37 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/_static/css/custom.css
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.093072 hipopybind-1.1.0/pybind11/docs/advanced/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.109963 hipopybind-1.1.0/pybind11/docs/advanced/cast/
--rw-r--r--   0 mfm45      (503) staff       (20)     3937 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     3429 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    14283 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     3889 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     1556 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    12371 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     9586 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     8863 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    47796 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     8453 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    17772 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    26729 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    12446 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.114669 hipopybind-1.1.0/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 mfm45      (503) staff       (20)      278 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    17161 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     9030 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     5710 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     6377 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     9240 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/basics.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     2856 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/benchmark.py
--rw-r--r--   0 mfm45      (503) staff       (20)     3168 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/benchmark.rst
--rw-r--r--   0 mfm45      (503) staff       (20)   105375 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/changelog.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    16380 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/classes.rst
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.115486 hipopybind-1.1.0/pybind11/docs/cmake/
--rw-r--r--   0 mfm45      (503) staff       (20)      273 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/cmake/index.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    25777 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/compiling.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    11559 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/conf.py
--rw-r--r--   0 mfm45      (503) staff       (20)    13177 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/faq.rst
--rw-r--r--   0 mfm45      (503) staff       (20)      613 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/index.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     3277 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/installing.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     3079 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/limitations.rst
--rw-r--r--   0 mfm45      (503) staff       (20)    61034 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 mfm45      (503) staff       (20)    44653 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 mfm45      (503) staff       (20)    87708 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 mfm45      (503) staff       (20)    41121 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 mfm45      (503) staff       (20)    85853 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 mfm45      (503) staff       (20)     2647 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/reference.rst
--rw-r--r--   0 mfm45      (503) staff       (20)     4414 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/release.rst
--rw-r--r--   0 mfm45      (503) staff       (20)      149 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/requirements.txt
--rw-r--r--   0 mfm45      (503) staff       (20)    23489 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:29.440415 hipopybind-1.1.0/pybind11/include/
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.153403 hipopybind-1.1.0/pybind11/include/pybind11/
--rw-r--r--   0 mfm45      (503) staff       (20)    23979 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/attr.h
--rw-r--r--   0 mfm45      (503) staff       (20)     7069 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 mfm45      (503) staff       (20)    65705 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/cast.h
--rw-r--r--   0 mfm45      (503) staff       (20)     8458 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 mfm45      (503) staff       (20)      120 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/common.h
--rw-r--r--   0 mfm45      (503) staff       (20)     2096 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.168658 hipopybind-1.1.0/pybind11/include/pybind11/detail/
--rw-r--r--   0 mfm45      (503) staff       (20)    27854 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 mfm45      (503) staff       (20)    50335 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 mfm45      (503) staff       (20)     5491 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 mfm45      (503) staff       (20)    17981 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 mfm45      (503) staff       (20)    24008 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 mfm45      (503) staff       (20)    42266 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 mfm45      (503) staff       (20)     1625 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 mfm45      (503) staff       (20)    32147 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 mfm45      (503) staff       (20)    11792 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/embed.h
--rw-r--r--   0 mfm45      (503) staff       (20)     4731 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/eval.h
--rw-r--r--   0 mfm45      (503) staff       (20)     4695 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/functional.h
--rw-r--r--   0 mfm45      (503) staff       (20)     6923 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/gil.h
--rw-r--r--   0 mfm45      (503) staff       (20)     8862 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 mfm45      (503) staff       (20)    79524 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 mfm45      (503) staff       (20)     9051 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/operators.h
--rw-r--r--   0 mfm45      (503) staff       (20)     2181 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/options.h
--rw-r--r--   0 mfm45      (503) staff       (20)   126301 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 mfm45      (503) staff       (20)    92159 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.169391 hipopybind-1.1.0/pybind11/include/pybind11/stl/
--rw-r--r--   0 mfm45      (503) staff       (20)     4185 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 mfm45      (503) staff       (20)    14606 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/stl.h
--rw-r--r--   0 mfm45      (503) staff       (20)    27013 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 mfm45      (503) staff       (20)     2765 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/noxfile.py
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.182650 hipopybind-1.1.0/pybind11/pybind11/
--rw-r--r--   0 mfm45      (503) staff       (20)      414 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/pybind11/__init__.py
--rw-r--r--   0 mfm45      (503) staff       (20)     1360 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/pybind11/__main__.py
--rw-r--r--   0 mfm45      (503) staff       (20)      233 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/pybind11/_version.py
--rw-r--r--   0 mfm45      (503) staff       (20)     1226 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/pybind11/commands.py
--rw-r--r--   0 mfm45      (503) staff       (20)        0 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/pybind11/py.typed
--rw-r--r--   0 mfm45      (503) staff       (20)    17609 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 mfm45      (503) staff       (20)     1261 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/pyproject.toml
--rw-r--r--   0 mfm45      (503) staff       (20)     1622 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/setup.cfg
--rw-r--r--   0 mfm45      (503) staff       (20)     4877 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/setup.py
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.346801 hipopybind-1.1.0/pybind11/tests/
--rw-r--r--   0 mfm45      (503) staff       (20)    20608 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 mfm45      (503) staff       (20)     4915 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/conftest.py
--rw-r--r--   0 mfm45      (503) staff       (20)    11734 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/constructor_stats.h
--rw-r--r--   0 mfm45      (503) staff       (20)     1486 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     1776 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)      940 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/env.py
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.348218 hipopybind-1.1.0/pybind11/tests/extra_python_package/
--rw-r--r--   0 mfm45      (503) staff       (20)        0 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 mfm45      (503) staff       (20)     8142 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.350808 hipopybind-1.1.0/pybind11/tests/extra_setuptools/
--rw-r--r--   0 mfm45      (503) staff       (20)        0 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 mfm45      (503) staff       (20)     4153 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 mfm45      (503) staff       (20)     2847 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/local_bindings.h
--rw-r--r--   0 mfm45      (503) staff       (20)     5743 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/object.h
--rw-r--r--   0 mfm45      (503) staff       (20)     6264 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     4384 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     2685 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 mfm45      (503) staff       (20)      768 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/pytest.ini
--rw-r--r--   0 mfm45      (503) staff       (20)      600 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/requirements.txt
--rw-r--r--   0 mfm45      (503) staff       (20)      855 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_async.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)      534 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_async.py
--rw-r--r--   0 mfm45      (503) staff       (20)     8567 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     4841 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_buffers.py
--rw-r--r--   0 mfm45      (503) staff       (20)    15990 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    17245 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 mfm45      (503) staff       (20)     4118 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     6549 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_call_policies.py
--rw-r--r--   0 mfm45      (503) staff       (20)     9243 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     5906 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_callbacks.py
--rw-r--r--   0 mfm45      (503) staff       (20)     3370 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     5695 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_chrono.py
--rw-r--r--   0 mfm45      (503) staff       (20)    23520 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_class.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    14326 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_class.py
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.356090 hipopybind-1.1.0/pybind11/tests/test_cmake_build/
--rw-r--r--   0 mfm45      (503) staff       (20)     2639 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 mfm45      (503) staff       (20)      673 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.359616 hipopybind-1.1.0/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 mfm45      (503) staff       (20)     1171 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.360393 hipopybind-1.1.0/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 mfm45      (503) staff       (20)     1293 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.360979 hipopybind-1.1.0/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 mfm45      (503) staff       (20)     1685 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 mfm45      (503) staff       (20)      152 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.362999 hipopybind-1.1.0/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 mfm45      (503) staff       (20)     1353 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.363854 hipopybind-1.1.0/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 mfm45      (503) staff       (20)     1163 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.364577 hipopybind-1.1.0/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 mfm45      (503) staff       (20)     1368 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 mfm45      (503) staff       (20)      198 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 mfm45      (503) staff       (20)     3831 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)      589 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_const_name.py
--rw-r--r--   0 mfm45      (503) staff       (20)     5853 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     1498 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 mfm45      (503) staff       (20)    10886 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     4796 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_copy_move.py
--rw-r--r--   0 mfm45      (503) staff       (20)     7280 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     3980 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 mfm45      (503) staff       (20)     1259 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     1089 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 mfm45      (503) staff       (20)     2816 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     1606 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 mfm45      (503) staff       (20)    18265 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_eigen.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    28454 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.372574 hipopybind-1.1.0/pybind11/tests/test_embed/
--rw-r--r--   0 mfm45      (503) staff       (20)     1798 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 mfm45      (503) staff       (20)     1338 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)      543 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    14310 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)      237 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 mfm45      (503) staff       (20)      275 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 mfm45      (503) staff       (20)     5722 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_enum.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     8903 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_enum.py
--rw-r--r--   0 mfm45      (503) staff       (20)     3168 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_eval.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     1143 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_eval.py
--rw-r--r--   0 mfm45      (503) staff       (20)      119 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_eval_call.py
--rw-r--r--   0 mfm45      (503) staff       (20)    12098 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)      399 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_exceptions.h
--rw-r--r--   0 mfm45      (503) staff       (20)    12326 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_exceptions.py
--rw-r--r--   0 mfm45      (503) staff       (20)    18155 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    16519 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 mfm45      (503) staff       (20)     1673 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     3104 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 mfm45      (503) staff       (20)     3960 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     7286 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_iostream.py
--rw-r--r--   0 mfm45      (503) staff       (20)     9535 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    13757 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 mfm45      (503) staff       (20)     4401 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     8049 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 mfm45      (503) staff       (20)    21388 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    18134 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 mfm45      (503) staff       (20)     4121 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_modules.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     4191 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_modules.py
--rw-r--r--   0 mfm45      (503) staff       (20)    12305 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    11874 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 mfm45      (503) staff       (20)    19800 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    20228 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 mfm45      (503) staff       (20)    21114 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    14394 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 mfm45      (503) staff       (20)     4487 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     9686 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 mfm45      (503) staff       (20)     2777 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     1847 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 mfm45      (503) staff       (20)     9463 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     4333 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 mfm45      (503) staff       (20)     6719 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     2720 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_pickling.py
--rw-r--r--   0 mfm45      (503) staff       (20)    29963 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    22310 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_pytypes.py
--rw-r--r--   0 mfm45      (503) staff       (20)    20580 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     7791 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 mfm45      (503) staff       (20)    18898 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     9530 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 mfm45      (503) staff       (20)    21587 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_stl.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    12235 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_stl.py
--rw-r--r--   0 mfm45      (503) staff       (20)     4622 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)     7912 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 mfm45      (503) staff       (20)     4617 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)      741 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 mfm45      (503) staff       (20)     1855 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_thread.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)      826 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_thread.py
--rw-r--r--   0 mfm45      (503) staff       (20)      603 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_union.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)      148 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_union.py
--rw-r--r--   0 mfm45      (503) staff       (20)    22983 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 mfm45      (503) staff       (20)    12919 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 mfm45      (503) staff       (20)     3226 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 mfm45      (503) staff       (20)     2657 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.395305 hipopybind-1.1.0/pybind11/tools/
--rw-r--r--   0 mfm45      (503) staff       (20)     2350 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 mfm45      (503) staff       (20)     3105 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 mfm45      (503) staff       (20)    10890 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 mfm45      (503) staff       (20)      817 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 mfm45      (503) staff       (20)     1423 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/check-style.sh
--rw-r--r--   0 mfm45      (503) staff       (20)      952 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 mfm45      (503) staff       (20)     1031 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/libsize.py
--rwxr-xr-x   0 mfm45      (503) staff       (20)     1282 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/make_changelog.py
--rw-r--r--   0 mfm45      (503) staff       (20)      196 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 mfm45      (503) staff       (20)    13487 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 mfm45      (503) staff       (20)     6930 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 mfm45      (503) staff       (20)     8955 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 mfm45      (503) staff       (20)     8359 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 mfm45      (503) staff       (20)       94 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/pyproject.toml
--rw-r--r--   0 mfm45      (503) staff       (20)     1965 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/setup_global.py.in
--rw-r--r--   0 mfm45      (503) staff       (20)     1139 2024-04-17 20:52:28.000000 hipopybind-1.1.0/pybind11/tools/setup_main.py.in
--rw-r--r--   0 mfm45      (503) staff       (20)      585 2024-04-18 14:15:16.000000 hipopybind-1.1.0/pyproject.toml
--rw-r--r--   0 mfm45      (503) staff       (20)       38 2024-04-19 15:54:30.403239 hipopybind-1.1.0/setup.cfg
--rw-r--r--   0 mfm45      (503) staff       (20)     6234 2024-04-19 15:52:46.000000 hipopybind-1.1.0/setup.py
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.398173 hipopybind-1.1.0/src/
--rw-r--r--   0 mfm45      (503) staff       (20)    55712 2024-04-19 15:35:53.000000 hipopybind-1.1.0/src/main.cpp
-drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 15:54:30.399338 hipopybind-1.1.0/tests/
--rw-r--r--   0 mfm45      (503) staff       (20)       77 2024-04-19 15:52:58.000000 hipopybind-1.1.0/tests/test_basic.py
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.326988 hipopybind-1.1.1/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1296 2024-04-17 20:52:18.000000 hipopybind-1.1.1/CMakeLists.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)     1098 2024-04-17 20:52:18.000000 hipopybind-1.1.1/LICENSE
+-rw-r--r--   0 mfm45      (503) staff       (20)      146 2024-04-18 19:12:47.000000 hipopybind-1.1.1/MANIFEST.in
+-rw-r--r--   0 mfm45      (503) staff       (20)     1136 2024-04-19 18:06:12.326288 hipopybind-1.1.1/PKG-INFO
+-rw-r--r--   0 mfm45      (503) staff       (20)      738 2024-04-19 15:53:11.000000 hipopybind-1.1.1/README.md
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.925550 hipopybind-1.1.1/hipo/
+-rw-r--r--   0 mfm45      (503) staff       (20)       29 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/.git
+-rw-r--r--   0 mfm45      (503) staff       (20)       64 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/.gitmodules
+-rw-r--r--   0 mfm45      (503) staff       (20)     5549 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/CMakeLists.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)     1772 2024-04-18 17:50:41.000000 hipopybind-1.1.1/hipo/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)      670 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/README.md
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.945560 hipopybind-1.1.1/hipo/ai/
+-rw-r--r--   0 mfm45      (503) staff       (20)      865 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/ai/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     2796 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/ai/analyze.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     4425 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/ai/cluster.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     1582 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/ai/cluster.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     4224 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/ai/dcana.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     1112 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/ai/dcana.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     2804 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/ai/main.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)    15296 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/ai/track.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     4064 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/ai/track.h
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.949334 hipopybind-1.1.1/hipo/cmake/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1425 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/cmake/LZ4Config.cmake
+-rw-r--r--   0 mfm45      (503) staff       (20)      278 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/cmake/hipo4Config.cmake.in
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.966204 hipopybind-1.1.1/hipo/examples/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1406 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/Makefile
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.972589 hipopybind-1.1.1/hipo/examples/benchmarks/
+-rw-r--r--   0 mfm45      (503) staff       (20)      898 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/benchmarks/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     3929 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/benchmarks/ana_benchmark.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     5502 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/benchmarks/map_benchmark.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     2371 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/builder.cc
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.981029 hipopybind-1.1.1/hipo/examples/fortran/
+-rw-r--r--   0 mfm45      (503) staff       (20)      930 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/fortran/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)      837 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/fortran/freader.F
+-rw-r--r--   0 mfm45      (503) staff       (20)     2424 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/readEvents.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     2650 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/readFile.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     2029 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/readFileTags.cc
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.001463 hipopybind-1.1.1/hipo/examples/root/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1712 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/root/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     4530 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/root/benchmark_hipo.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     5399 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/root/benchmark_hipo_ana.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     4036 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/root/benchmark_hipo_cwise.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     4325 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/root/benchmark_root.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     6485 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/root/converter.cc
+-rwxr-xr-x   0 mfm45      (503) staff       (20)      109 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/root/ramdisk.sh
+-rw-r--r--   0 mfm45      (503) staff       (20)     2093 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/schema.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     2090 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/showFile.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     1697 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/writeEvents.cc
+-rw-r--r--   0 mfm45      (503) staff       (20)     4858 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/writeFile.cc
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.004506 hipopybind-1.1.1/hipo/examples/xrootd/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1041 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/xrootd/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     1160 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/examples/xrootd/readFileXrootd.cc
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.042727 hipopybind-1.1.1/hipo/hipo4/
+-rw-r--r--   0 mfm45      (503) staff       (20)      715 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     8242 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/bank.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    20013 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/bank.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     3693 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/datastream.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     4795 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/datastream.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     4504 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/dictionary.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     3858 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/dictionary.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     8726 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/event.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     4198 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/event.h
+-rw-r--r--   0 mfm45      (503) staff       (20)      682 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/hipoexceptions.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    19589 2024-04-19 15:52:04.000000 hipopybind-1.1.1/hipo/hipo4/reader.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     8618 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/reader.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    24717 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/record.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     5919 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/record.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     6531 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/recordbuilder.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     1796 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/recordbuilder.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    10276 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/utils.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     2731 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/utils.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    13945 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/wrapper.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     8264 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/writer.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     6581 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/hipo4/writer.h
+-rwxr-xr-x   0 mfm45      (503) staff       (20)   222928 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/libhipo4.dylib
+-rwxr-xr-x   0 mfm45      (503) staff       (20)   367480 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/libhipo4.so
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.062950 hipopybind-1.1.1/hipo/lz4/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.063999 hipopybind-1.1.1/hipo/lz4/.circleci/
+-rw-r--r--   0 mfm45      (503) staff       (20)     5030 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/.circleci/config.yml
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.876278 hipopybind-1.1.1/hipo/lz4/.circleci/images/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.065404 hipopybind-1.1.1/hipo/lz4/.circleci/images/primary/
+-rw-r--r--   0 mfm45      (503) staff       (20)      644 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/.circleci/images/primary/Dockerfile
+-rw-r--r--   0 mfm45      (503) staff       (20)       44 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/.git
+-rw-r--r--   0 mfm45      (503) staff       (20)      348 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/.gitattributes
+-rw-r--r--   0 mfm45      (503) staff       (20)      315 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/.gitignore
+-rw-r--r--   0 mfm45      (503) staff       (20)     5714 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/.travis.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)      630 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/INSTALL
+-rw-r--r--   0 mfm45      (503) staff       (20)      565 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/LICENSE
+-rw-r--r--   0 mfm45      (503) staff       (20)     6663 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     1688 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/Makefile.inc
+-rw-r--r--   0 mfm45      (503) staff       (20)    13759 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/NEWS
+-rw-r--r--   0 mfm45      (503) staff       (20)     5534 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/README.md
+-rw-r--r--   0 mfm45      (503) staff       (20)     5862 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/appveyor.yml
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.881486 hipopybind-1.1.1/hipo/lz4/contrib/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.067973 hipopybind-1.1.1/hipo/lz4/contrib/cmake_unofficial/
+-rw-r--r--   0 mfm45      (503) staff       (20)       97 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/cmake_unofficial/.gitignore
+-rw-r--r--   0 mfm45      (503) staff       (20)     8188 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/cmake_unofficial/CMakeLists.txt
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.079138 hipopybind-1.1.1/hipo/lz4/contrib/debian/
+-rw-r--r--   0 mfm45      (503) staff       (20)      475 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/debian/changelog
+-rw-r--r--   0 mfm45      (503) staff       (20)        2 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/debian/compat
+-rw-r--r--   0 mfm45      (503) staff       (20)      612 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/debian/control
+-rw-r--r--   0 mfm45      (503) staff       (20)      325 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/debian/copyright
+-rw-r--r--   0 mfm45      (503) staff       (20)        8 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/debian/dirs
+-rw-r--r--   0 mfm45      (503) staff       (20)        0 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/debian/docs
+-rw-r--r--   0 mfm45      (503) staff       (20)       35 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/debian/liblz4-dev.install
+-rw-r--r--   0 mfm45      (503) staff       (20)       30 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/debian/liblz4.install
+-rwxr-xr-x   0 mfm45      (503) staff       (20)      188 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/debian/rules
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.083193 hipopybind-1.1.1/hipo/lz4/contrib/djgpp/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1292 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/djgpp/LICENSE
+-rw-r--r--   0 mfm45      (503) staff       (20)     3524 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/djgpp/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     1125 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/djgpp/README.MD
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.089050 hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/
+-rw-r--r--   0 mfm45      (503) staff       (20)       28 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/.gitignore
+-rw-r--r--   0 mfm45      (503) staff       (20)     3020 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     1144 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/README.md
+-rw-r--r--   0 mfm45      (503) staff       (20)      613 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/gen-lz4-manual.sh
+-rw-r--r--   0 mfm45      (503) staff       (20)     8697 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/gen_manual.cpp
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.103105 hipopybind-1.1.1/hipo/lz4/contrib/meson/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1307 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/GetLz4LibraryVersion.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     2120 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/InstallSymlink.py
+-rw-r--r--   0 mfm45      (503) staff       (20)      838 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/README.md
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.104066 hipopybind-1.1.1/hipo/lz4/contrib/meson/contrib/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.108023 hipopybind-1.1.1/hipo/lz4/contrib/meson/contrib/gen_manual/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1531 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/contrib/gen_manual/meson.build
+-rw-r--r--   0 mfm45      (503) staff       (20)      495 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/contrib/meson.build
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.109356 hipopybind-1.1.1/hipo/lz4/contrib/meson/examples/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1975 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/examples/meson.build
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.112177 hipopybind-1.1.1/hipo/lz4/contrib/meson/lib/
+-rw-r--r--   0 mfm45      (503) staff       (20)     2027 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/lib/meson.build
+-rw-r--r--   0 mfm45      (503) staff       (20)     3953 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/meson.build
+-rw-r--r--   0 mfm45      (503) staff       (20)     1196 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/meson_options.txt
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.119114 hipopybind-1.1.1/hipo/lz4/contrib/meson/programs/
+-rw-r--r--   0 mfm45      (503) staff       (20)     2025 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/programs/meson.build
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.120565 hipopybind-1.1.1/hipo/lz4/contrib/meson/tests/
+-rw-r--r--   0 mfm45      (503) staff       (20)     3306 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/meson/tests/meson.build
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.123101 hipopybind-1.1.1/hipo/lz4/contrib/snap/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1172 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/snap/README.md
+-rw-r--r--   0 mfm45      (503) staff       (20)     1115 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/contrib/snap/snapcraft.yaml
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.166389 hipopybind-1.1.1/hipo/lz4/doc/
+-rw-r--r--   0 mfm45      (503) staff       (20)     6422 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/doc/lz4_Block_format.md
+-rw-r--r--   0 mfm45      (503) staff       (20)    14421 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/doc/lz4_Frame_format.md
+-rw-r--r--   0 mfm45      (503) staff       (20)    30346 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/doc/lz4_manual.html
+-rw-r--r--   0 mfm45      (503) staff       (20)    20733 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/doc/lz4frame_manual.html
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.250968 hipopybind-1.1.1/hipo/lz4/examples/
+-rw-r--r--   0 mfm45      (503) staff       (20)      143 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/.gitignore
+-rw-r--r--   0 mfm45      (503) staff       (20)    18092 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/COPYING
+-rw-r--r--   0 mfm45      (503) staff       (20)     6057 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/HCStreaming_ringBuffer.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     3685 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)      313 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/README.md
+-rw-r--r--   0 mfm45      (503) staff       (20)     4832 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_doubleBuffer.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     2749 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_doubleBuffer.md
+-rw-r--r--   0 mfm45      (503) staff       (20)     5383 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_lineByLine.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     3648 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_lineByLine.md
+-rw-r--r--   0 mfm45      (503) staff       (20)     4981 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_ringBuffer.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    27116 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/compress_functions.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     8116 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/dictionaryRandomAccess.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     2100 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/dictionaryRandomAccess.md
+-rw-r--r--   0 mfm45      (503) staff       (20)    13397 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/frameCompress.c
+-rw-r--r--   0 mfm45      (503) staff       (20)      269 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/printVersion.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     5496 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/simple_buffer.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     3615 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/examples/streaming_api_basics.md
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.288381 hipopybind-1.1.1/hipo/lz4/lib/
+-rw-r--r--   0 mfm45      (503) staff       (20)       34 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/.gitignore
+-rw-r--r--   0 mfm45      (503) staff       (20)     1311 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/LICENSE
+-rw-r--r--   0 mfm45      (503) staff       (20)     8431 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     5149 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/README.md
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.884989 hipopybind-1.1.1/hipo/lz4/lib/dll/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.297673 hipopybind-1.1.1/hipo/lz4/lib/dll/example/
+-rw-r--r--   0 mfm45      (503) staff       (20)     2031 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/dll/example/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     3013 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/dll/example/README.md
+-rw-r--r--   0 mfm45      (503) staff       (20)     1269 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/dll/example/fullbench-dll.sln
+-rw-r--r--   0 mfm45      (503) staff       (20)    10157 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/dll/example/fullbench-dll.vcxproj
+-rw-r--r--   0 mfm45      (503) staff       (20)     1109 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/liblz4-dll.rc.in
+-rw-r--r--   0 mfm45      (503) staff       (20)      385 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/liblz4.pc.in
+-rw-r--r--   0 mfm45      (503) staff       (20)    97210 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/lz4.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    39943 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/lz4.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    77571 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/lz4frame.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    28657 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/lz4frame.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     2044 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/lz4frame_static.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    62843 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/lz4hc.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    21357 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/lz4hc.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    34045 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/xxhash.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    13466 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/lib/xxhash.h
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.326713 hipopybind-1.1.1/hipo/lz4/programs/
+-rw-r--r--   0 mfm45      (503) staff       (20)      169 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/.gitignore
+-rw-r--r--   0 mfm45      (503) staff       (20)    18092 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/COPYING
+-rw-r--r--   0 mfm45      (503) staff       (20)     5681 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     3541 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/README.md
+-rw-r--r--   0 mfm45      (503) staff       (20)    22491 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/bench.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     1484 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/bench.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     5938 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/datagen.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     1687 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/datagen.h
+-rw-r--r--   0 mfm45      (503) staff       (20)      851 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/lz4-exe.rc.in
+-rw-r--r--   0 mfm45      (503) staff       (20)     9011 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/lz4.1
+-rw-r--r--   0 mfm45      (503) staff       (20)     8203 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/lz4.1.md
+-rw-r--r--   0 mfm45      (503) staff       (20)    33979 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/lz4cli.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    61886 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/lz4io.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     5199 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/lz4io.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     6822 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/platform.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    20176 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/programs/util.h
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.351223 hipopybind-1.1.1/hipo/lz4/tests/
+-rw-r--r--   0 mfm45      (503) staff       (20)      185 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/.gitignore
+-rw-r--r--   0 mfm45      (503) staff       (20)    18092 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/COPYING
+-rw-r--r--   0 mfm45      (503) staff       (20)    18428 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     3503 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/README.md
+-rw-r--r--   0 mfm45      (503) staff       (20)    11005 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/checkFrame.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     2554 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/checkTag.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     5740 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/datagencli.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    51673 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/frametest.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    30685 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/fullbench.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    85263 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/fuzzer.c
+-rw-r--r--   0 mfm45      (503) staff       (20)     7308 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/roundTripTest.c
+-rw-r--r--   0 mfm45      (503) staff       (20)    12437 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/test-lz4-list.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    16792 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/test-lz4-speed.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     5376 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/test-lz4-versions.py
+-rwxr-xr-x   0 mfm45      (503) staff       (20)     1901 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/test_custom_block_sizes.sh
+-rwxr-xr-x   0 mfm45      (503) staff       (20)      789 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/tests/test_install.sh
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.352567 hipopybind-1.1.1/hipo/lz4/visual/
+-rw-r--r--   0 mfm45      (503) staff       (20)       76 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/.gitignore
+-rw-r--r--   0 mfm45      (503) staff       (20)     2887 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/README.md
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.354374 hipopybind-1.1.1/hipo/lz4/visual/VS2010/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.355451 hipopybind-1.1.1/hipo/lz4/visual/VS2010/datagen/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9272 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/datagen/datagen.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.358069 hipopybind-1.1.1/hipo/lz4/visual/VS2010/frametest/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9623 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/frametest/frametest.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.358985 hipopybind-1.1.1/hipo/lz4/visual/VS2010/fullbench/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9623 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/fullbench/fullbench.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.359880 hipopybind-1.1.1/hipo/lz4/visual/VS2010/fullbench-dll/
+-rw-r--r--   0 mfm45      (503) staff       (20)    10445 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/fullbench-dll/fullbench-dll.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.361072 hipopybind-1.1.1/hipo/lz4/visual/VS2010/fuzzer/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9451 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/fuzzer/fuzzer.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.364950 hipopybind-1.1.1/hipo/lz4/visual/VS2010/liblz4/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9512 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/liblz4/liblz4.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.368373 hipopybind-1.1.1/hipo/lz4/visual/VS2010/liblz4-dll/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1388 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0 mfm45      (503) staff       (20)     9616 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/liblz4-dll/liblz4-dll.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.370160 hipopybind-1.1.1/hipo/lz4/visual/VS2010/lz4/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1388 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/lz4/lz4.rc
+-rw-r--r--   0 mfm45      (503) staff       (20)    10285 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/lz4/lz4.vcxproj
+-rw-r--r--   0 mfm45      (503) staff       (20)     6761 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2010/lz4.sln
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.372250 hipopybind-1.1.1/hipo/lz4/visual/VS2017/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.373140 hipopybind-1.1.1/hipo/lz4/visual/VS2017/datagen/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9454 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2017/datagen/datagen.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.373964 hipopybind-1.1.1/hipo/lz4/visual/VS2017/frametest/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9805 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2017/frametest/frametest.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.375024 hipopybind-1.1.1/hipo/lz4/visual/VS2017/fullbench/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9805 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2017/fullbench/fullbench.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.376225 hipopybind-1.1.1/hipo/lz4/visual/VS2017/fullbench-dll/
+-rw-r--r--   0 mfm45      (503) staff       (20)    10626 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.378209 hipopybind-1.1.1/hipo/lz4/visual/VS2017/fuzzer/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9633 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.379104 hipopybind-1.1.1/hipo/lz4/visual/VS2017/liblz4/
+-rw-r--r--   0 mfm45      (503) staff       (20)     9694 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2017/liblz4/liblz4.vcxproj
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.382653 hipopybind-1.1.1/hipo/lz4/visual/VS2017/liblz4-dll/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1388 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc
+-rw-r--r--   0 mfm45      (503) staff       (20)     9797 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj
+-rw-r--r--   0 mfm45      (503) staff       (20)     6193 2024-04-18 17:49:46.000000 hipopybind-1.1.1/hipo/lz4/visual/VS2017/lz4.sln
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.383737 hipopybind-1.1.1/hipo/python/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1068 2024-04-18 17:47:31.000000 hipopybind-1.1.1/hipo/python/hiporeader.py
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.324500 hipopybind-1.1.1/hipopybind.egg-info/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1136 2024-04-19 18:06:09.000000 hipopybind-1.1.1/hipopybind.egg-info/PKG-INFO
+-rw-r--r--   0 mfm45      (503) staff       (20)    15284 2024-04-19 18:06:09.000000 hipopybind-1.1.1/hipopybind.egg-info/SOURCES.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)        1 2024-04-19 18:06:09.000000 hipopybind-1.1.1/hipopybind.egg-info/dependency_links.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)        1 2024-04-18 17:59:16.000000 hipopybind-1.1.1/hipopybind.egg-info/not-zip-safe
+-rw-r--r--   0 mfm45      (503) staff       (20)       20 2024-04-19 18:06:09.000000 hipopybind-1.1.1/hipopybind.egg-info/requires.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)       11 2024-04-19 18:06:09.000000 hipopybind-1.1.1/hipopybind.egg-info/top_level.txt
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.858868 hipopybind-1.1.1/pybind11/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1271 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.appveyor.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)      996 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.clang-format
+-rw-r--r--   0 mfm45      (503) staff       (20)     2605 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.clang-tidy
+-rw-r--r--   0 mfm45      (503) staff       (20)     2196 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.cmake-format.yaml
+-rw-r--r--   0 mfm45      (503) staff       (20)       33 2024-04-17 20:52:24.000000 hipopybind-1.1.1/pybind11/.git
+-rw-r--r--   0 mfm45      (503) staff       (20)       18 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.gitattributes
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.887183 hipopybind-1.1.1/pybind11/.github/
+-rw-r--r--   0 mfm45      (503) staff       (20)      182 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 mfm45      (503) staff       (20)    15271 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.889835 hipopybind-1.1.1/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mfm45      (503) staff       (20)     2016 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)      328 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)      162 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/dependabot.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)      116 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/labeler.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)       50 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.890821 hipopybind-1.1.1/pybind11/.github/matchers/
+-rw-r--r--   0 mfm45      (503) staff       (20)      668 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 mfm45      (503) staff       (20)      645 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.904803 hipopybind-1.1.1/pybind11/.github/workflows/
+-rw-r--r--   0 mfm45      (503) staff       (20)    28217 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)     2095 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)     1419 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)      333 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)     2558 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)     2837 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 mfm45      (503) staff       (20)      487 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.gitignore
+-rw-r--r--   0 mfm45      (503) staff       (20)     4083 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 mfm45      (503) staff       (20)       62 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/.readthedocs.yml
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:10.907059 hipopybind-1.1.1/pybind11/CMakeFiles/
+-rw-r--r--   0 mfm45      (503) staff       (20)      622 2024-04-17 20:53:03.000000 hipopybind-1.1.1/pybind11/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0 mfm45      (503) staff       (20)        2 2024-04-17 20:53:03.000000 hipopybind-1.1.1/pybind11/CMakeFiles/progress.marks
+-rw-r--r--   0 mfm45      (503) staff       (20)    11687 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/CMakeLists.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)     1684 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/LICENSE
+-rw-r--r--   0 mfm45      (503) staff       (20)      223 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/MANIFEST.in
+-rw-r--r--   0 mfm45      (503) staff       (20)     6512 2024-04-17 20:53:02.000000 hipopybind-1.1.1/pybind11/Makefile
+-rw-r--r--   0 mfm45      (503) staff       (20)     7686 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/README.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     1149 2024-04-17 20:53:03.000000 hipopybind-1.1.1/pybind11/cmake_install.cmake
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.164081 hipopybind-1.1.1/pybind11/docs/
+-rw-r--r--   0 mfm45      (503) staff       (20)      607 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/Doxyfile
+-rw-r--r--   0 mfm45      (503) staff       (20)     7417 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/Makefile
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.901221 hipopybind-1.1.1/pybind11/docs/_static/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.165880 hipopybind-1.1.1/pybind11/docs/_static/css/
+-rw-r--r--   0 mfm45      (503) staff       (20)       37 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.189851 hipopybind-1.1.1/pybind11/docs/advanced/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.203053 hipopybind-1.1.1/pybind11/docs/advanced/cast/
+-rw-r--r--   0 mfm45      (503) staff       (20)     3937 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     3429 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    14283 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     3889 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     1556 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    12371 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     9586 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     8863 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    47796 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     8453 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    17772 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    26729 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    12446 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.209933 hipopybind-1.1.1/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 mfm45      (503) staff       (20)      278 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    17161 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     9030 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     5710 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     6377 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     9240 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/basics.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     2856 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/benchmark.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     3168 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/benchmark.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)   105375 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/changelog.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    16380 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/classes.rst
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.213415 hipopybind-1.1.1/pybind11/docs/cmake/
+-rw-r--r--   0 mfm45      (503) staff       (20)      273 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    25777 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/compiling.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    11559 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/conf.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    13177 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/faq.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)      613 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/index.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     3277 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/installing.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     3079 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/limitations.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)    61034 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 mfm45      (503) staff       (20)    44653 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 mfm45      (503) staff       (20)    87708 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 mfm45      (503) staff       (20)    41121 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 mfm45      (503) staff       (20)    85853 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 mfm45      (503) staff       (20)     2647 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/reference.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)     4414 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/release.rst
+-rw-r--r--   0 mfm45      (503) staff       (20)      149 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/requirements.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)    23489 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:09.903222 hipopybind-1.1.1/pybind11/include/
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.619329 hipopybind-1.1.1/pybind11/include/pybind11/
+-rw-r--r--   0 mfm45      (503) staff       (20)    23979 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     7069 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    65705 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     8458 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 mfm45      (503) staff       (20)      120 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/common.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     2096 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.629160 hipopybind-1.1.1/pybind11/include/pybind11/detail/
+-rw-r--r--   0 mfm45      (503) staff       (20)    27854 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    50335 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     5491 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    17981 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    24008 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    42266 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     1625 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    32147 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    11792 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     4731 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     4695 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     6923 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     8862 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    79524 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     9051 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     2181 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/options.h
+-rw-r--r--   0 mfm45      (503) staff       (20)   126301 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    92159 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.629990 hipopybind-1.1.1/pybind11/include/pybind11/stl/
+-rw-r--r--   0 mfm45      (503) staff       (20)     4185 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    14606 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    27013 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     2765 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/noxfile.py
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:11.635750 hipopybind-1.1.1/pybind11/pybind11/
+-rw-r--r--   0 mfm45      (503) staff       (20)      414 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/pybind11/__init__.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     1360 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/pybind11/__main__.py
+-rw-r--r--   0 mfm45      (503) staff       (20)      233 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/pybind11/_version.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     1226 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/pybind11/commands.py
+-rw-r--r--   0 mfm45      (503) staff       (20)        0 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/pybind11/py.typed
+-rw-r--r--   0 mfm45      (503) staff       (20)    17609 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     1261 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/pyproject.toml
+-rw-r--r--   0 mfm45      (503) staff       (20)     1622 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/setup.cfg
+-rw-r--r--   0 mfm45      (503) staff       (20)     4877 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/setup.py
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.270620 hipopybind-1.1.1/pybind11/tests/
+-rw-r--r--   0 mfm45      (503) staff       (20)    20608 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)     4915 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/conftest.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    11734 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     1486 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     1776 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)      940 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/env.py
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.273764 hipopybind-1.1.1/pybind11/tests/extra_python_package/
+-rw-r--r--   0 mfm45      (503) staff       (20)        0 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 mfm45      (503) staff       (20)     8142 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.275113 hipopybind-1.1.1/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 mfm45      (503) staff       (20)        0 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 mfm45      (503) staff       (20)     4153 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     2847 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/local_bindings.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     5743 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/object.h
+-rw-r--r--   0 mfm45      (503) staff       (20)     6264 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     4384 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     2685 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 mfm45      (503) staff       (20)      768 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/pytest.ini
+-rw-r--r--   0 mfm45      (503) staff       (20)      600 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/requirements.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)      855 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_async.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)      534 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_async.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     8567 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     4841 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_buffers.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    15990 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    17245 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     4118 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     6549 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     9243 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     5906 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     3370 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     5695 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_chrono.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    23520 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_class.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    14326 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_class.py
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.281032 hipopybind-1.1.1/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 mfm45      (503) staff       (20)     2639 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)      673 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.282049 hipopybind-1.1.1/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1171 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.283000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1293 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.283819 hipopybind-1.1.1/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1685 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)      152 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.285402 hipopybind-1.1.1/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1353 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.287050 hipopybind-1.1.1/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1163 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.289736 hipopybind-1.1.1/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1368 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)      198 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     3831 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)      589 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_const_name.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     5853 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     1498 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    10886 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     4796 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     7280 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     3980 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     1259 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     1089 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     2816 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     1606 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    18265 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_eigen.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    28454 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_eigen.py
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.298259 hipopybind-1.1.1/pybind11/tests/test_embed/
+-rw-r--r--   0 mfm45      (503) staff       (20)     1798 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 mfm45      (503) staff       (20)     1338 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)      543 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    14310 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)      237 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 mfm45      (503) staff       (20)      275 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     5722 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     8903 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_enum.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     3168 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     1143 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_eval.py
+-rw-r--r--   0 mfm45      (503) staff       (20)      119 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    12098 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)      399 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 mfm45      (503) staff       (20)    12326 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    18155 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    16519 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     1673 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     3104 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     3960 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     7286 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_iostream.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     9535 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    13757 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     4401 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     8049 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    21388 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    18134 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     4121 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     4191 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_modules.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    12305 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    11874 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    19800 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    20228 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    21114 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    14394 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     4487 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     9686 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     2777 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     1847 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     9463 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     4333 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     6719 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     2720 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_pickling.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    29963 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    22310 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    20580 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     7791 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    18898 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     9530 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    21587 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    12235 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_stl.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     4622 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)     7912 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     4617 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)      741 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     1855 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)      826 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_thread.py
+-rw-r--r--   0 mfm45      (503) staff       (20)      603 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_union.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)      148 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_union.py
+-rw-r--r--   0 mfm45      (503) staff       (20)    22983 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 mfm45      (503) staff       (20)    12919 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 mfm45      (503) staff       (20)     3226 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 mfm45      (503) staff       (20)     2657 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.320762 hipopybind-1.1.1/pybind11/tools/
+-rw-r--r--   0 mfm45      (503) staff       (20)     2350 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 mfm45      (503) staff       (20)     3105 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 mfm45      (503) staff       (20)    10890 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 mfm45      (503) staff       (20)      817 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 mfm45      (503) staff       (20)     1423 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/check-style.sh
+-rw-r--r--   0 mfm45      (503) staff       (20)      952 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 mfm45      (503) staff       (20)     1031 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/libsize.py
+-rwxr-xr-x   0 mfm45      (503) staff       (20)     1282 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/make_changelog.py
+-rw-r--r--   0 mfm45      (503) staff       (20)      196 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 mfm45      (503) staff       (20)    13487 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 mfm45      (503) staff       (20)     6930 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 mfm45      (503) staff       (20)     8955 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 mfm45      (503) staff       (20)     8359 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 mfm45      (503) staff       (20)       94 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/pyproject.toml
+-rw-r--r--   0 mfm45      (503) staff       (20)     1965 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 mfm45      (503) staff       (20)     1139 2024-04-17 20:52:28.000000 hipopybind-1.1.1/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 mfm45      (503) staff       (20)      585 2024-04-18 14:15:16.000000 hipopybind-1.1.1/pyproject.toml
+-rw-r--r--   0 mfm45      (503) staff       (20)       38 2024-04-19 18:06:12.327132 hipopybind-1.1.1/setup.cfg
+-rw-r--r--   0 mfm45      (503) staff       (20)     6234 2024-04-19 18:03:24.000000 hipopybind-1.1.1/setup.py
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.321802 hipopybind-1.1.1/src/
+-rw-r--r--   0 mfm45      (503) staff       (20)    55834 2024-04-19 17:35:46.000000 hipopybind-1.1.1/src/main.cpp
+drwxr-xr-x   0 mfm45      (503) staff       (20)        0 2024-04-19 18:06:12.323349 hipopybind-1.1.1/tests/
+-rw-r--r--   0 mfm45      (503) staff       (20)       77 2024-04-19 18:03:21.000000 hipopybind-1.1.1/tests/test_basic.py
```

### Comparing `hipopybind-1.1.0/CMakeLists.txt` & `hipopybind-1.1.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/LICENSE` & `hipopybind-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/PKG-INFO` & `hipopybind-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipopybind
-Version: 1.1.0
+Version: 1.1.1
 Summary: A HIPO python library using PyBind11 and CMake
 Home-page: https://github.com/mfmceneaney/hipopybind.git
 Author: Matthew McEneaney
 Author-email: matthew.mceneaney@duke.edu
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `hipopybind-1.1.0/README.md` & `hipopybind-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/CMakeLists.txt` & `hipopybind-1.1.1/hipo/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/Makefile` & `hipopybind-1.1.1/hipo/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/README.md` & `hipopybind-1.1.1/hipo/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/ai/Makefile` & `hipopybind-1.1.1/hipo/ai/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/ai/analyze.cc` & `hipopybind-1.1.1/hipo/ai/analyze.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/ai/cluster.cpp` & `hipopybind-1.1.1/hipo/ai/cluster.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/ai/cluster.h` & `hipopybind-1.1.1/hipo/ai/cluster.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/ai/dcana.cpp` & `hipopybind-1.1.1/hipo/ai/dcana.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/ai/dcana.h` & `hipopybind-1.1.1/hipo/ai/dcana.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/ai/main.cc` & `hipopybind-1.1.1/hipo/ai/main.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/ai/track.cpp` & `hipopybind-1.1.1/hipo/ai/track.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/ai/track.h` & `hipopybind-1.1.1/hipo/ai/track.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/cmake/LZ4Config.cmake` & `hipopybind-1.1.1/hipo/cmake/LZ4Config.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/Makefile` & `hipopybind-1.1.1/hipo/examples/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/benchmarks/Makefile` & `hipopybind-1.1.1/hipo/examples/benchmarks/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/benchmarks/ana_benchmark.cc` & `hipopybind-1.1.1/hipo/examples/benchmarks/ana_benchmark.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/benchmarks/map_benchmark.cc` & `hipopybind-1.1.1/hipo/examples/benchmarks/map_benchmark.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/builder.cc` & `hipopybind-1.1.1/hipo/examples/builder.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/fortran/Makefile` & `hipopybind-1.1.1/hipo/examples/fortran/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/fortran/freader.F` & `hipopybind-1.1.1/hipo/examples/fortran/freader.F`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/readEvents.cc` & `hipopybind-1.1.1/hipo/examples/readEvents.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/readFile.cc` & `hipopybind-1.1.1/hipo/examples/readFile.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/readFileTags.cc` & `hipopybind-1.1.1/hipo/examples/readFileTags.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/root/Makefile` & `hipopybind-1.1.1/hipo/examples/root/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/root/benchmark_hipo.cc` & `hipopybind-1.1.1/hipo/examples/root/benchmark_hipo.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/root/benchmark_hipo_ana.cc` & `hipopybind-1.1.1/hipo/examples/root/benchmark_hipo_ana.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/root/benchmark_hipo_cwise.cc` & `hipopybind-1.1.1/hipo/examples/root/benchmark_hipo_cwise.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/root/benchmark_root.cc` & `hipopybind-1.1.1/hipo/examples/root/benchmark_root.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/root/converter.cc` & `hipopybind-1.1.1/hipo/examples/root/converter.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/schema.cc` & `hipopybind-1.1.1/hipo/examples/schema.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/showFile.cc` & `hipopybind-1.1.1/hipo/examples/showFile.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/writeEvents.cc` & `hipopybind-1.1.1/hipo/examples/writeEvents.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/writeFile.cc` & `hipopybind-1.1.1/hipo/examples/writeFile.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/xrootd/Makefile` & `hipopybind-1.1.1/hipo/examples/xrootd/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/examples/xrootd/readFileXrootd.cc` & `hipopybind-1.1.1/hipo/examples/xrootd/readFileXrootd.cc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/Makefile` & `hipopybind-1.1.1/hipo/hipo4/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/bank.cpp` & `hipopybind-1.1.1/hipo/hipo4/bank.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/bank.h` & `hipopybind-1.1.1/hipo/hipo4/bank.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/datastream.cpp` & `hipopybind-1.1.1/hipo/hipo4/datastream.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/datastream.h` & `hipopybind-1.1.1/hipo/hipo4/datastream.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/dictionary.cpp` & `hipopybind-1.1.1/hipo/hipo4/dictionary.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/dictionary.h` & `hipopybind-1.1.1/hipo/hipo4/dictionary.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/event.cpp` & `hipopybind-1.1.1/hipo/hipo4/event.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/event.h` & `hipopybind-1.1.1/hipo/hipo4/event.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/hipoexceptions.h` & `hipopybind-1.1.1/hipo/hipo4/hipoexceptions.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/reader.cpp` & `hipopybind-1.1.1/hipo/hipo4/reader.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/reader.h` & `hipopybind-1.1.1/hipo/hipo4/reader.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/record.cpp` & `hipopybind-1.1.1/hipo/hipo4/record.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/record.h` & `hipopybind-1.1.1/hipo/hipo4/record.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/recordbuilder.cpp` & `hipopybind-1.1.1/hipo/hipo4/recordbuilder.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/recordbuilder.h` & `hipopybind-1.1.1/hipo/hipo4/recordbuilder.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/utils.cpp` & `hipopybind-1.1.1/hipo/hipo4/utils.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/utils.h` & `hipopybind-1.1.1/hipo/hipo4/utils.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/wrapper.cpp` & `hipopybind-1.1.1/hipo/hipo4/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/writer.cpp` & `hipopybind-1.1.1/hipo/hipo4/writer.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/hipo4/writer.h` & `hipopybind-1.1.1/hipo/hipo4/writer.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/libhipo4.dylib` & `hipopybind-1.1.1/hipo/libhipo4.dylib`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/libhipo4.so` & `hipopybind-1.1.1/hipo/libhipo4.so`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/.circleci/config.yml` & `hipopybind-1.1.1/hipo/lz4/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/.circleci/images/primary/Dockerfile` & `hipopybind-1.1.1/hipo/lz4/.circleci/images/primary/Dockerfile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/.travis.yml` & `hipopybind-1.1.1/hipo/lz4/.travis.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/INSTALL` & `hipopybind-1.1.1/hipo/lz4/INSTALL`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/LICENSE` & `hipopybind-1.1.1/hipo/lz4/LICENSE`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/Makefile` & `hipopybind-1.1.1/hipo/lz4/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/Makefile.inc` & `hipopybind-1.1.1/hipo/lz4/Makefile.inc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/NEWS` & `hipopybind-1.1.1/hipo/lz4/NEWS`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/README.md` & `hipopybind-1.1.1/hipo/lz4/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/appveyor.yml` & `hipopybind-1.1.1/hipo/lz4/appveyor.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/cmake_unofficial/CMakeLists.txt` & `hipopybind-1.1.1/hipo/lz4/contrib/cmake_unofficial/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/debian/control` & `hipopybind-1.1.1/hipo/lz4/contrib/debian/control`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/djgpp/LICENSE` & `hipopybind-1.1.1/hipo/lz4/contrib/djgpp/LICENSE`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/djgpp/Makefile` & `hipopybind-1.1.1/hipo/lz4/contrib/djgpp/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/djgpp/README.MD` & `hipopybind-1.1.1/hipo/lz4/contrib/djgpp/README.MD`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/Makefile` & `hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/README.md` & `hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/gen-lz4-manual.sh` & `hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/gen-lz4-manual.sh`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/gen_manual/gen_manual.cpp` & `hipopybind-1.1.1/hipo/lz4/contrib/gen_manual/gen_manual.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/GetLz4LibraryVersion.py` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/GetLz4LibraryVersion.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/InstallSymlink.py` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/InstallSymlink.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/README.md` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/contrib/gen_manual/meson.build` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/contrib/gen_manual/meson.build`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/examples/meson.build` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/examples/meson.build`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/lib/meson.build` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/lib/meson.build`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/meson.build` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/meson.build`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/meson_options.txt` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/meson_options.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/programs/meson.build` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/programs/meson.build`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/meson/tests/meson.build` & `hipopybind-1.1.1/hipo/lz4/contrib/meson/tests/meson.build`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/snap/README.md` & `hipopybind-1.1.1/hipo/lz4/contrib/snap/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/contrib/snap/snapcraft.yaml` & `hipopybind-1.1.1/hipo/lz4/contrib/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/doc/lz4_Block_format.md` & `hipopybind-1.1.1/hipo/lz4/doc/lz4_Block_format.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/doc/lz4_Frame_format.md` & `hipopybind-1.1.1/hipo/lz4/doc/lz4_Frame_format.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/doc/lz4_manual.html` & `hipopybind-1.1.1/hipo/lz4/doc/lz4_manual.html`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/doc/lz4frame_manual.html` & `hipopybind-1.1.1/hipo/lz4/doc/lz4frame_manual.html`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/COPYING` & `hipopybind-1.1.1/hipo/lz4/examples/COPYING`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/HCStreaming_ringBuffer.c` & `hipopybind-1.1.1/hipo/lz4/examples/HCStreaming_ringBuffer.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/Makefile` & `hipopybind-1.1.1/hipo/lz4/examples/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_doubleBuffer.c` & `hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_doubleBuffer.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_doubleBuffer.md` & `hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_doubleBuffer.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_lineByLine.c` & `hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_lineByLine.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_lineByLine.md` & `hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_lineByLine.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/blockStreaming_ringBuffer.c` & `hipopybind-1.1.1/hipo/lz4/examples/blockStreaming_ringBuffer.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/compress_functions.c` & `hipopybind-1.1.1/hipo/lz4/examples/compress_functions.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/dictionaryRandomAccess.c` & `hipopybind-1.1.1/hipo/lz4/examples/dictionaryRandomAccess.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/dictionaryRandomAccess.md` & `hipopybind-1.1.1/hipo/lz4/examples/dictionaryRandomAccess.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/frameCompress.c` & `hipopybind-1.1.1/hipo/lz4/examples/frameCompress.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/simple_buffer.c` & `hipopybind-1.1.1/hipo/lz4/examples/simple_buffer.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/examples/streaming_api_basics.md` & `hipopybind-1.1.1/hipo/lz4/examples/streaming_api_basics.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/LICENSE` & `hipopybind-1.1.1/hipo/lz4/lib/LICENSE`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/Makefile` & `hipopybind-1.1.1/hipo/lz4/lib/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/README.md` & `hipopybind-1.1.1/hipo/lz4/lib/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/dll/example/Makefile` & `hipopybind-1.1.1/hipo/lz4/lib/dll/example/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/dll/example/README.md` & `hipopybind-1.1.1/hipo/lz4/lib/dll/example/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/dll/example/fullbench-dll.sln` & `hipopybind-1.1.1/hipo/lz4/lib/dll/example/fullbench-dll.sln`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/dll/example/fullbench-dll.vcxproj` & `hipopybind-1.1.1/hipo/lz4/lib/dll/example/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/liblz4-dll.rc.in` & `hipopybind-1.1.1/hipo/lz4/lib/liblz4-dll.rc.in`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/lz4.c` & `hipopybind-1.1.1/hipo/lz4/lib/lz4.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/lz4.h` & `hipopybind-1.1.1/hipo/lz4/lib/lz4.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/lz4frame.c` & `hipopybind-1.1.1/hipo/lz4/lib/lz4frame.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/lz4frame.h` & `hipopybind-1.1.1/hipo/lz4/lib/lz4frame.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/lz4frame_static.h` & `hipopybind-1.1.1/hipo/lz4/lib/lz4frame_static.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/lz4hc.c` & `hipopybind-1.1.1/hipo/lz4/lib/lz4hc.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/lz4hc.h` & `hipopybind-1.1.1/hipo/lz4/lib/lz4hc.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/xxhash.c` & `hipopybind-1.1.1/hipo/lz4/lib/xxhash.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/lib/xxhash.h` & `hipopybind-1.1.1/hipo/lz4/lib/xxhash.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/COPYING` & `hipopybind-1.1.1/hipo/lz4/programs/COPYING`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/Makefile` & `hipopybind-1.1.1/hipo/lz4/programs/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/README.md` & `hipopybind-1.1.1/hipo/lz4/programs/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/bench.c` & `hipopybind-1.1.1/hipo/lz4/programs/bench.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/bench.h` & `hipopybind-1.1.1/hipo/lz4/programs/bench.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/datagen.c` & `hipopybind-1.1.1/hipo/lz4/programs/datagen.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/datagen.h` & `hipopybind-1.1.1/hipo/lz4/programs/datagen.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/lz4-exe.rc.in` & `hipopybind-1.1.1/hipo/lz4/programs/lz4-exe.rc.in`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/lz4.1` & `hipopybind-1.1.1/hipo/lz4/programs/lz4.1`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/lz4.1.md` & `hipopybind-1.1.1/hipo/lz4/programs/lz4.1.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/lz4cli.c` & `hipopybind-1.1.1/hipo/lz4/programs/lz4cli.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/lz4io.c` & `hipopybind-1.1.1/hipo/lz4/programs/lz4io.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/lz4io.h` & `hipopybind-1.1.1/hipo/lz4/programs/lz4io.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/platform.h` & `hipopybind-1.1.1/hipo/lz4/programs/platform.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/programs/util.h` & `hipopybind-1.1.1/hipo/lz4/programs/util.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/COPYING` & `hipopybind-1.1.1/hipo/lz4/tests/COPYING`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/Makefile` & `hipopybind-1.1.1/hipo/lz4/tests/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/README.md` & `hipopybind-1.1.1/hipo/lz4/tests/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/checkFrame.c` & `hipopybind-1.1.1/hipo/lz4/tests/checkFrame.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/checkTag.c` & `hipopybind-1.1.1/hipo/lz4/tests/checkTag.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/datagencli.c` & `hipopybind-1.1.1/hipo/lz4/tests/datagencli.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/frametest.c` & `hipopybind-1.1.1/hipo/lz4/tests/frametest.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/fullbench.c` & `hipopybind-1.1.1/hipo/lz4/tests/fullbench.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/fuzzer.c` & `hipopybind-1.1.1/hipo/lz4/tests/fuzzer.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/roundTripTest.c` & `hipopybind-1.1.1/hipo/lz4/tests/roundTripTest.c`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/test-lz4-list.py` & `hipopybind-1.1.1/hipo/lz4/tests/test-lz4-list.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/test-lz4-speed.py` & `hipopybind-1.1.1/hipo/lz4/tests/test-lz4-speed.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/test-lz4-versions.py` & `hipopybind-1.1.1/hipo/lz4/tests/test-lz4-versions.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/test_custom_block_sizes.sh` & `hipopybind-1.1.1/hipo/lz4/tests/test_custom_block_sizes.sh`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/tests/test_install.sh` & `hipopybind-1.1.1/hipo/lz4/tests/test_install.sh`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/README.md` & `hipopybind-1.1.1/hipo/lz4/visual/README.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/datagen/datagen.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/frametest/frametest.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/fullbench/fullbench.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/fullbench-dll/fullbench-dll.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/fuzzer/fuzzer.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/liblz4/liblz4.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/liblz4-dll/liblz4-dll.rc` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/liblz4-dll/liblz4-dll.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/lz4/lz4.rc` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/lz4/lz4.rc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/lz4/lz4.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/lz4/lz4.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2010/lz4.sln` & `hipopybind-1.1.1/hipo/lz4/visual/VS2010/lz4.sln`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2017/datagen/datagen.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2017/datagen/datagen.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2017/frametest/frametest.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2017/frametest/frametest.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2017/fullbench/fullbench.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2017/fullbench/fullbench.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2017/fullbench-dll/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2017/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2017/liblz4/liblz4.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2017/liblz4/liblz4.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc` & `hipopybind-1.1.1/hipo/lz4/visual/VS2017/liblz4-dll/liblz4-dll.rc`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj` & `hipopybind-1.1.1/hipo/lz4/visual/VS2017/liblz4-dll/liblz4-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/lz4/visual/VS2017/lz4.sln` & `hipopybind-1.1.1/hipo/lz4/visual/VS2017/lz4.sln`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipo/python/hiporeader.py` & `hipopybind-1.1.1/hipo/python/hiporeader.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/hipopybind.egg-info/PKG-INFO` & `hipopybind-1.1.1/hipopybind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipopybind
-Version: 1.1.0
+Version: 1.1.1
 Summary: A HIPO python library using PyBind11 and CMake
 Home-page: https://github.com/mfmceneaney/hipopybind.git
 Author: Matthew McEneaney
 Author-email: matthew.mceneaney@duke.edu
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `hipopybind-1.1.0/hipopybind.egg-info/SOURCES.txt` & `hipopybind-1.1.1/hipopybind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.appveyor.yml` & `hipopybind-1.1.1/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.clang-format` & `hipopybind-1.1.1/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.clang-tidy` & `hipopybind-1.1.1/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.cmake-format.yaml` & `hipopybind-1.1.1/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.github/CONTRIBUTING.md` & `hipopybind-1.1.1/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `hipopybind-1.1.1/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.github/matchers/pylint.json` & `hipopybind-1.1.1/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.github/pull_request_template.md` & `hipopybind-1.1.1/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.github/workflows/ci.yml` & `hipopybind-1.1.1/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.github/workflows/configure.yml` & `hipopybind-1.1.1/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.github/workflows/format.yml` & `hipopybind-1.1.1/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.github/workflows/pip.yml` & `hipopybind-1.1.1/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.github/workflows/upstream.yml` & `hipopybind-1.1.1/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/.pre-commit-config.yaml` & `hipopybind-1.1.1/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/CMakeFiles/CMakeDirectoryInformation.cmake` & `hipopybind-1.1.1/pybind11/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/LICENSE` & `hipopybind-1.1.1/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/Makefile` & `hipopybind-1.1.1/pybind11/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/README.rst` & `hipopybind-1.1.1/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/cmake_install.cmake` & `hipopybind-1.1.1/pybind11/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/Doxyfile` & `hipopybind-1.1.1/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/Makefile` & `hipopybind-1.1.1/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/cast/chrono.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/cast/custom.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/cast/eigen.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/cast/functional.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/cast/index.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/cast/overview.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/cast/stl.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/cast/strings.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/classes.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/embedding.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/exceptions.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/functions.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/misc.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/pycpp/numpy.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/pycpp/object.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/pycpp/utilities.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/advanced/smart_ptrs.rst` & `hipopybind-1.1.1/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/basics.rst` & `hipopybind-1.1.1/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/benchmark.py` & `hipopybind-1.1.1/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/benchmark.rst` & `hipopybind-1.1.1/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/changelog.rst` & `hipopybind-1.1.1/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/classes.rst` & `hipopybind-1.1.1/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/compiling.rst` & `hipopybind-1.1.1/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/conf.py` & `hipopybind-1.1.1/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/faq.rst` & `hipopybind-1.1.1/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/index.rst` & `hipopybind-1.1.1/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/installing.rst` & `hipopybind-1.1.1/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/limitations.rst` & `hipopybind-1.1.1/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/pybind11-logo.png` & `hipopybind-1.1.1/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/pybind11_vs_boost_python1.png` & `hipopybind-1.1.1/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/pybind11_vs_boost_python1.svg` & `hipopybind-1.1.1/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/pybind11_vs_boost_python2.png` & `hipopybind-1.1.1/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/pybind11_vs_boost_python2.svg` & `hipopybind-1.1.1/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/reference.rst` & `hipopybind-1.1.1/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/release.rst` & `hipopybind-1.1.1/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/docs/upgrade.rst` & `hipopybind-1.1.1/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/attr.h` & `hipopybind-1.1.1/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/buffer_info.h` & `hipopybind-1.1.1/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/cast.h` & `hipopybind-1.1.1/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/chrono.h` & `hipopybind-1.1.1/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/complex.h` & `hipopybind-1.1.1/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/detail/class.h` & `hipopybind-1.1.1/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/detail/common.h` & `hipopybind-1.1.1/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/detail/descr.h` & `hipopybind-1.1.1/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/detail/init.h` & `hipopybind-1.1.1/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/detail/internals.h` & `hipopybind-1.1.1/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/detail/type_caster_base.h` & `hipopybind-1.1.1/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/detail/typeid.h` & `hipopybind-1.1.1/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/eigen.h` & `hipopybind-1.1.1/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/embed.h` & `hipopybind-1.1.1/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/eval.h` & `hipopybind-1.1.1/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/functional.h` & `hipopybind-1.1.1/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/gil.h` & `hipopybind-1.1.1/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/iostream.h` & `hipopybind-1.1.1/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/numpy.h` & `hipopybind-1.1.1/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/operators.h` & `hipopybind-1.1.1/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/options.h` & `hipopybind-1.1.1/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/pybind11.h` & `hipopybind-1.1.1/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/pytypes.h` & `hipopybind-1.1.1/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/stl/filesystem.h` & `hipopybind-1.1.1/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/stl.h` & `hipopybind-1.1.1/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/include/pybind11/stl_bind.h` & `hipopybind-1.1.1/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/noxfile.py` & `hipopybind-1.1.1/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/pybind11/__main__.py` & `hipopybind-1.1.1/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/pybind11/commands.py` & `hipopybind-1.1.1/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/pybind11/setup_helpers.py` & `hipopybind-1.1.1/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/pyproject.toml` & `hipopybind-1.1.1/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/setup.cfg` & `hipopybind-1.1.1/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/setup.py` & `hipopybind-1.1.1/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/conftest.py` & `hipopybind-1.1.1/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/constructor_stats.h` & `hipopybind-1.1.1/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/cross_module_gil_utils.cpp` & `hipopybind-1.1.1/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `hipopybind-1.1.1/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/env.py` & `hipopybind-1.1.1/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/extra_python_package/test_files.py` & `hipopybind-1.1.1/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/extra_setuptools/test_setuphelper.py` & `hipopybind-1.1.1/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/local_bindings.h` & `hipopybind-1.1.1/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/object.h` & `hipopybind-1.1.1/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/pybind11_cross_module_tests.cpp` & `hipopybind-1.1.1/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/pybind11_tests.cpp` & `hipopybind-1.1.1/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/pybind11_tests.h` & `hipopybind-1.1.1/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/pytest.ini` & `hipopybind-1.1.1/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/requirements.txt` & `hipopybind-1.1.1/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_async.cpp` & `hipopybind-1.1.1/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_async.py` & `hipopybind-1.1.1/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_buffers.cpp` & `hipopybind-1.1.1/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_buffers.py` & `hipopybind-1.1.1/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_builtin_casters.cpp` & `hipopybind-1.1.1/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_builtin_casters.py` & `hipopybind-1.1.1/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_call_policies.cpp` & `hipopybind-1.1.1/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_call_policies.py` & `hipopybind-1.1.1/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_callbacks.cpp` & `hipopybind-1.1.1/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_callbacks.py` & `hipopybind-1.1.1/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_chrono.cpp` & `hipopybind-1.1.1/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_chrono.py` & `hipopybind-1.1.1/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_class.cpp` & `hipopybind-1.1.1/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_class.py` & `hipopybind-1.1.1/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_cmake_build/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_cmake_build/embed.cpp` & `hipopybind-1.1.1/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_const_name.cpp` & `hipopybind-1.1.1/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_const_name.py` & `hipopybind-1.1.1/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_constants_and_functions.cpp` & `hipopybind-1.1.1/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_constants_and_functions.py` & `hipopybind-1.1.1/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_copy_move.cpp` & `hipopybind-1.1.1/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_copy_move.py` & `hipopybind-1.1.1/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_custom_type_casters.cpp` & `hipopybind-1.1.1/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_custom_type_casters.py` & `hipopybind-1.1.1/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_custom_type_setup.cpp` & `hipopybind-1.1.1/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_custom_type_setup.py` & `hipopybind-1.1.1/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_docstring_options.cpp` & `hipopybind-1.1.1/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_docstring_options.py` & `hipopybind-1.1.1/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_eigen.cpp` & `hipopybind-1.1.1/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_eigen.py` & `hipopybind-1.1.1/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_embed/CMakeLists.txt` & `hipopybind-1.1.1/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_embed/catch.cpp` & `hipopybind-1.1.1/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_embed/external_module.cpp` & `hipopybind-1.1.1/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_embed/test_interpreter.cpp` & `hipopybind-1.1.1/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_enum.cpp` & `hipopybind-1.1.1/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_enum.py` & `hipopybind-1.1.1/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_eval.cpp` & `hipopybind-1.1.1/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_eval.py` & `hipopybind-1.1.1/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_exceptions.cpp` & `hipopybind-1.1.1/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_exceptions.py` & `hipopybind-1.1.1/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_factory_constructors.cpp` & `hipopybind-1.1.1/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_factory_constructors.py` & `hipopybind-1.1.1/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_gil_scoped.cpp` & `hipopybind-1.1.1/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_gil_scoped.py` & `hipopybind-1.1.1/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_iostream.cpp` & `hipopybind-1.1.1/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_iostream.py` & `hipopybind-1.1.1/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_kwargs_and_defaults.cpp` & `hipopybind-1.1.1/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_kwargs_and_defaults.py` & `hipopybind-1.1.1/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_local_bindings.cpp` & `hipopybind-1.1.1/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_local_bindings.py` & `hipopybind-1.1.1/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_methods_and_attributes.cpp` & `hipopybind-1.1.1/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_methods_and_attributes.py` & `hipopybind-1.1.1/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_modules.cpp` & `hipopybind-1.1.1/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_modules.py` & `hipopybind-1.1.1/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_multiple_inheritance.cpp` & `hipopybind-1.1.1/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_multiple_inheritance.py` & `hipopybind-1.1.1/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_numpy_array.cpp` & `hipopybind-1.1.1/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_numpy_array.py` & `hipopybind-1.1.1/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_numpy_dtypes.cpp` & `hipopybind-1.1.1/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_numpy_dtypes.py` & `hipopybind-1.1.1/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_numpy_vectorize.cpp` & `hipopybind-1.1.1/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_numpy_vectorize.py` & `hipopybind-1.1.1/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_opaque_types.cpp` & `hipopybind-1.1.1/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_opaque_types.py` & `hipopybind-1.1.1/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_operator_overloading.cpp` & `hipopybind-1.1.1/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_operator_overloading.py` & `hipopybind-1.1.1/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_pickling.cpp` & `hipopybind-1.1.1/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_pickling.py` & `hipopybind-1.1.1/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_pytypes.cpp` & `hipopybind-1.1.1/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_pytypes.py` & `hipopybind-1.1.1/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_sequences_and_iterators.cpp` & `hipopybind-1.1.1/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_sequences_and_iterators.py` & `hipopybind-1.1.1/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_smart_ptr.cpp` & `hipopybind-1.1.1/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_smart_ptr.py` & `hipopybind-1.1.1/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_stl.cpp` & `hipopybind-1.1.1/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_stl.py` & `hipopybind-1.1.1/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_stl_binders.cpp` & `hipopybind-1.1.1/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_stl_binders.py` & `hipopybind-1.1.1/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_tagbased_polymorphic.cpp` & `hipopybind-1.1.1/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_tagbased_polymorphic.py` & `hipopybind-1.1.1/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_thread.cpp` & `hipopybind-1.1.1/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_thread.py` & `hipopybind-1.1.1/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_union.cpp` & `hipopybind-1.1.1/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_virtual_functions.cpp` & `hipopybind-1.1.1/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/test_virtual_functions.py` & `hipopybind-1.1.1/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/valgrind-numpy-scipy.supp` & `hipopybind-1.1.1/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tests/valgrind-python.supp` & `hipopybind-1.1.1/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/FindCatch.cmake` & `hipopybind-1.1.1/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/FindEigen3.cmake` & `hipopybind-1.1.1/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/FindPythonLibsNew.cmake` & `hipopybind-1.1.1/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/JoinPaths.cmake` & `hipopybind-1.1.1/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/check-style.sh` & `hipopybind-1.1.1/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/cmake_uninstall.cmake.in` & `hipopybind-1.1.1/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/libsize.py` & `hipopybind-1.1.1/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/make_changelog.py` & `hipopybind-1.1.1/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/pybind11Common.cmake` & `hipopybind-1.1.1/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/pybind11Config.cmake.in` & `hipopybind-1.1.1/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/pybind11NewTools.cmake` & `hipopybind-1.1.1/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/pybind11Tools.cmake` & `hipopybind-1.1.1/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/setup_global.py.in` & `hipopybind-1.1.1/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pybind11/tools/setup_main.py.in` & `hipopybind-1.1.1/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/pyproject.toml` & `hipopybind-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hipopybind-1.1.0/setup.py` & `hipopybind-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="hipopybind",
-    version="1.1.0",
+    version="1.1.1",
     author="Matthew McEneaney",
     author_email="matthew.mceneaney@duke.edu",
     license="MIT",
     url="https://github.com/mfmceneaney/hipopybind.git",
     description="A HIPO python library using PyBind11 and CMake",
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
```

### Comparing `hipopybind-1.1.0/src/main.cpp` & `hipopybind-1.1.1/src/main.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,18 @@
                             case 8: vec_long.at(entryindex).push_back(bank.getLongs(name)); break;
                             default: throw pybind11::type_error("HipoFileIterator: Invalid type int for entry: "+entrynames.at(j)+"\n");
                         }
                     } // for (int j = 0; j<nentries; j++)
 
                 } // for (int i = 0; i<nbanks; i++)
                 counter++;
-                if (counter>=batchsize) { return true; }
+                if (counter>=batchsize) {
+                    if (!reader.hasNext() && index>=filenames.size()-1) return false;
+                    return true;
+                }
             }
             // Move on to next file if batch is not yet complete
             if (open()) {
                 return next(counter); //NOTE: Recursive function //NOTE: If you do not return here, the original function keeps going after the recursive call and returns false and so ends iteration.
             }
             //TODO: NOTE: THIS SHOULD NOT RAISE A STOP ITERATION BECAUSE YOU STILL NEED TO GET THE BATCH DATA IN PYTHON
             return false; //NOTE: Only happens if you've reached the end of all files.
```

