# Comparing `tmp/pyflann_ibeis-2.3.0.tar.gz` & `tmp/pyflann_ibeis-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflann_ibeis-2.3.0.tar", last modified: Sun Jan 29 03:12:14 2023, max compression
+gzip compressed data, was "pyflann_ibeis-2.4.0.tar", last modified: Fri Apr 19 03:23:30 2024, max compression
```

## Comparing `pyflann_ibeis-2.3.0.tar` & `pyflann_ibeis-2.4.0.tar`

### file list

```diff
@@ -1,168 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.248260 pyflann_ibeis-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.240260 pyflann_ibeis-2.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.240260 pyflann_ibeis-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/.github/workflows/test_binaries.yml
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.240260 pyflann_ibeis-2.3.0/CMake/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/CMake/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/CMake/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/CMake/FindFlann.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/CMake/flann.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/CMake/flann_utils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/CMake/python_utils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/CMake/uninstall_target.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-01-29 03:12:14.248260 pyflann_ibeis-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.240260 pyflann_ibeis-2.3.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/bin/download_checkmd5.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/bin/indent.sh
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/bin/parse_authors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/bin/run_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/bin/uncrustify.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/build_wheels.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/clean.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.240260 pyflann_ibeis-2.3.0/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/ci_public_gpg_key.pgp.enc
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/ci_secret_gpg_subkeys.pgp.enc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.240260 pyflann_ibeis-2.3.0/dev/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6625 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/docker/make_base_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/gpg_owner_trust.enc
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/make_strict_req.sh
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/public_gpg_key
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/secrets_configuration.sh
--rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/setup_secrets.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/travis_public_gpg_key.pgp.enc
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/dev/travis_secret_gpg_key.pgp.enc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.236260 pyflann_ibeis-2.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.240260 pyflann_ibeis-2.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.240260 pyflann_ibeis-2.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/examples/README
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/examples/flann_example.c
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/examples/flann_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/examples/flann_example_mpi.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)    14127 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/publish.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.240260 pyflann_ibeis-2.3.0/pyflann_ibeis/
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/__main__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/flann_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/flann_ctypes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22057 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/index.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/pyflann_ibeis/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyflann_ibeis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/pyflann_ibeis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-01-29 03:12:14.000000 pyflann_ibeis-2.3.0/pyflann_ibeis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-01-29 03:12:14.000000 pyflann_ibeis-2.3.0/pyflann_ibeis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 03:12:14.000000 pyflann_ibeis-2.3.0/pyflann_ibeis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-29 03:12:14.000000 pyflann_ibeis-2.3.0/pyflann_ibeis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-29 03:12:14.000000 pyflann_ibeis-2.3.0/pyflann_ibeis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/run_developer_setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/run_doctests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4740 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 03:12:14.248260 pyflann_ibeis-2.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8360 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/src/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/src/cpp/flann/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/all_indices.h
--rw-r--r--   0 runner    (1001) docker     (123)    26390 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/autotuned_index.h
--rw-r--r--   0 runner    (1001) docker     (123)    12523 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/center_chooser.h
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/composite_index.h
--rw-r--r--   0 runner    (1001) docker     (123)    26081 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/dist.h
--rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/hierarchical_clustering_index.h
--rw-r--r--   0 runner    (1001) docker     (123)    53147 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_cuda_3d_index.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_cuda_3d_index.h
--rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_cuda_builder.h
--rw-r--r--   0 runner    (1001) docker     (123)    24308 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_index.h
--rw-r--r--   0 runner    (1001) docker     (123)    21535 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_single_index.h
--rw-r--r--   0 runner    (1001) docker     (123)    33192 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kmeans_index.h
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/linear_index.h
--rw-r--r--   0 runner    (1001) docker     (123)    20234 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/lsh_index.h
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/nn_index.h
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/config.h
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/config.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/defines.h
--rw-r--r--   0 runner    (1001) docker     (123)    49595 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/flann.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28980 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/flann.h
--rw-r--r--   0 runner    (1001) docker     (123)    13647 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/flann.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/flann_cpp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/general.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/src/cpp/flann/io/
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/io/hdf5.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/src/cpp/flann/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/mpi/client.h
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/mpi/flann_mpi_client.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/mpi/flann_mpi_server.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/mpi/index.h
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/mpi/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/mpi/queries.h
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/mpi/server.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.244260 pyflann_ibeis-2.3.0/src/cpp/flann/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/nn/ground_truth.h
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/nn/index_testing.h
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/nn/simplex_downhill.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.248260 pyflann_ibeis-2.3.0/src/cpp/flann/util/
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/allocator.h
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/any.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.248260 pyflann_ibeis-2.3.0/src/cpp/flann/util/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/cuda/heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    15962 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/cuda/result_set.h
--rw-r--r--   0 runner    (1001) docker     (123)    36730 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/cutil_math.h
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/dynamic_bitset.h
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/heap.h
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/logger.h
--rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/lsh_table.h
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/object_factory.h
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/params.h
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/random.h
--rw-r--r--   0 runner    (1001) docker     (123)    24047 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/result_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/sampling.h
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/saving.h
--rw-r--r--   0 runner    (1001) docker     (123)    20545 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/serialization.h
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/src/cpp/flann/util/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 03:12:14.248260 pyflann_ibeis-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_autotuned_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_cuda_test.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_hierarchical_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_kdtree_single_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_kdtree_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_kmeans_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_linear_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_lsh_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_multithreaded_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/flann_tests.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/memusage_clustering.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/memusage_nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3496 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/test_import.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4009 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/test_index_save.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4143 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/test_nn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2530 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/test_nn_autotune.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2380 2023-01-29 03:12:05.000000 pyflann_ibeis-2.3.0/tests/test_nn_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:30.009707 pyflann_ibeis-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.961707 pyflann_ibeis-2.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.961707 pyflann_ibeis-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    19751 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.961707 pyflann_ibeis-2.4.0/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/CMake/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/CMake/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/CMake/FindFlann.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/CMake/flann.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/CMake/flann_utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/CMake/python_utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/CMake/uninstall_target.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-04-19 03:23:30.009707 pyflann_ibeis-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.961707 pyflann_ibeis-2.4.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1969 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/bin/download_checkmd5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/bin/indent.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/bin/parse_authors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      254 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/bin/run_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/bin/uncrustify.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      668 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/build_wheels.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/clean.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.965707 pyflann_ibeis-2.4.0/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/ci_public_gpg_key.pgp.enc
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/ci_secret_gpg_subkeys.pgp.enc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.965707 pyflann_ibeis-2.4.0/dev/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6671 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/docker/make_base_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/gpg_owner_trust.enc
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/make_strict_req.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/public_gpg_key
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/secrets_configuration.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    20071 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/setup_secrets.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/travis_public_gpg_key.pgp.enc
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/dev/travis_secret_gpg_key.pgp.enc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.965707 pyflann_ibeis-2.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.965707 pyflann_ibeis-2.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)    35731 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.965707 pyflann_ibeis-2.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/examples/README
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/examples/flann_example.c
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/examples/flann_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/examples/flann_example_mpi.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15899 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/publish.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.965707 pyflann_ibeis-2.4.0/pyflann_ibeis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/__main__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15106 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/flann_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/flann_ctypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22057 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/index.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.969708 pyflann_ibeis-2.4.0/pyflann_ibeis/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyflann_ibeis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.981707 pyflann_ibeis-2.4.0/pyflann_ibeis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-04-19 03:23:29.000000 pyflann_ibeis-2.4.0/pyflann_ibeis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-19 03:23:29.000000 pyflann_ibeis-2.4.0/pyflann_ibeis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:23:29.000000 pyflann_ibeis-2.4.0/pyflann_ibeis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-19 03:23:29.000000 pyflann_ibeis-2.4.0/pyflann_ibeis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 03:23:29.000000 pyflann_ibeis-2.4.0/pyflann_ibeis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.969708 pyflann_ibeis-2.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/requirements/linting.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      161 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/run_developer_setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/run_doctests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/run_linter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4785 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:23:30.009707 pyflann_ibeis-2.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9972 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.969708 pyflann_ibeis-2.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.969708 pyflann_ibeis-2.4.0/src/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.969708 pyflann_ibeis-2.4.0/src/cpp/flann/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.973708 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/all_indices.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26390 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/autotuned_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12523 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/center_chooser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/composite_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26081 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/dist.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21319 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/hierarchical_clustering_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53147 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_cuda_3d_index.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_cuda_3d_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29646 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_cuda_builder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24308 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21535 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_single_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33192 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kmeans_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/linear_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/lsh_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/nn_index.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/defines.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49595 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/flann.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28980 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/flann.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13647 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/flann.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/flann_cpp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/general.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.973708 pyflann_ibeis-2.4.0/src/cpp/flann/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/io/hdf5.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.973708 pyflann_ibeis-2.4.0/src/cpp/flann/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/mpi/client.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/mpi/flann_mpi_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/mpi/flann_mpi_server.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/mpi/index.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/mpi/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/mpi/queries.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/mpi/server.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.973708 pyflann_ibeis-2.4.0/src/cpp/flann/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/nn/ground_truth.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/nn/index_testing.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/nn/simplex_downhill.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.977707 pyflann_ibeis-2.4.0/src/cpp/flann/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/allocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/any.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.977707 pyflann_ibeis-2.4.0/src/cpp/flann/util/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/cuda/heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15962 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/cuda/result_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36730 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/cutil_math.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/dynamic_bitset.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/logger.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/lsh_table.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/object_factory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/params.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24047 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/result_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/sampling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/saving.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/serialization.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/src/cpp/flann/util/timer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:23:29.981707 pyflann_ibeis-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_autotuned_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16011 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_cuda_test.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_hierarchical_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_kdtree_single_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_kdtree_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_kmeans_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_linear_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_lsh_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_multithreaded_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23477 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/flann_tests.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1683 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/memusage_clustering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1752 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/memusage_nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3496 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/test_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4009 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/test_index_save.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4143 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/test_nn.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2530 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/test_nn_autotune.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-19 03:23:12.000000 pyflann_ibeis-2.4.0/tests/test_nn_index.py
```

### Comparing `pyflann_ibeis-2.3.0/CMake/FindFlann.cmake` & `pyflann_ibeis-2.4.0/CMake/FindFlann.cmake`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/CMake/flann_utils.cmake` & `pyflann_ibeis-2.4.0/CMake/flann_utils.cmake`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/CMake/python_utils.cmake` & `pyflann_ibeis-2.4.0/CMake/python_utils.cmake`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/CMake/uninstall_target.cmake.in` & `pyflann_ibeis-2.4.0/CMake/uninstall_target.cmake.in`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/CMakeLists.txt` & `pyflann_ibeis-2.4.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/COPYING` & `pyflann_ibeis-2.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/ChangeLog` & `pyflann_ibeis-2.4.0/ChangeLog`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/README.rst` & `pyflann_ibeis-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/bin/download_checkmd5.py` & `pyflann_ibeis-2.4.0/bin/download_checkmd5.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/bin/parse_authors.py` & `pyflann_ibeis-2.4.0/bin/parse_authors.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/bin/uncrustify.cfg` & `pyflann_ibeis-2.4.0/bin/uncrustify.cfg`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/dev/docker/make_base_image.py` & `pyflann_ibeis-2.4.0/dev/docker/make_base_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         # 'cp27-cp27m'
         # 'cp35-cp35m'
         # 'cp36-cp36m',
         'cp37-cp37m',
         'cp38-cp38',
         'cp39-cp39',
         'cp310-cp310',
+        'cp311-cp311',
+        'cp312-cp312',
     ]
 
     pyinstall_cmds = []
     for tag in tags:
         pyinstall_cmds.append(ub.codeblock(
             fr'''
             RUN MB_PYTHON_TAG={tag} && \
```

### Comparing `pyflann_ibeis-2.3.0/dev/make_strict_req.sh` & `pyflann_ibeis-2.4.0/dev/make_strict_req.sh`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/dev/setup_secrets.sh` & `pyflann_ibeis-2.4.0/dev/setup_secrets.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/bin/bash
+#!/usr/bin/env bash
 __doc__='
 ============================
 SETUP CI SECRET INSTRUCTIONS
 ============================
 
 TODO: These instructions are currently pieced together from old disparate
 instances, and are not yet fully organized.
@@ -21,15 +21,15 @@
 ../.circleci/config.yml
 
 
 =========================
 GITHUB ACTION INSTRUCTIONS
 =========================
 
-* `PERSONAL_GITHUB_PUSH_TOKEN` - 
+* `PERSONAL_GITHUB_PUSH_TOKEN` -
     This is only needed if you want to automatically git-tag release branches.
 
     To make a API token go to:
         https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/creating-a-personal-access-token
 
 
 =========================
@@ -43,37 +43,37 @@
         sed "s|travis-ci-Erotemic|<YOUR-GPG-ID>|g" | \
         sed "s|CI_SECRET|<YOUR_CI_SECRET>|g" | \
         sed "s|GITLAB_ORG_PUSH_TOKEN|<YOUR_GIT_ORG_PUSH_TOKEN>|g" | \
         sed "s|gitlab.org.com|gitlab.your-instance.com|g" | \
     tee /tmp/repl && colordiff .setup_secrets.sh /tmp/repl
     ```
 
-    * Make sure you add Runners to your project 
-    https://gitlab.org.com/utils/xcookie/-/settings/ci_cd 
+    * Make sure you add Runners to your project
+    https://gitlab.org.com/utils/xcookie/-/settings/ci_cd
     in Runners-> Shared Runners
     and Runners-> Available specific runners
 
     * Ensure that you are auto-cancel redundant pipelines.
     Navigate to https://gitlab.kitware.com/utils/xcookie/-/settings/ci_cd and ensure "Auto-cancel redundant pipelines" is checked.
 
     More details are here https://docs.gitlab.com/ee/ci/pipelines/settings.html#auto-cancel-redundant-pipelines
 
     * TWINE_USERNAME - this is your pypi username
         twine info is only needed if you want to automatically publish to pypi
 
-    * TWINE_PASSWORD - this is your pypi password 
+    * TWINE_PASSWORD - this is your pypi password
 
-    * CI_SECRET - We will use this as a secret key to encrypt/decrypt gpg secrets 
+    * CI_SECRET - We will use this as a secret key to encrypt/decrypt gpg secrets
         This is only needed if you want to automatically sign published
         wheels with a gpg key.
 
-    * GITLAB_ORG_PUSH_TOKEN - 
+    * GITLAB_ORG_PUSH_TOKEN -
         This is only needed if you want to automatically git-tag release branches.
 
-        Create a new personal access token in User->Settings->Tokens, 
+        Create a new personal access token in User->Settings->Tokens,
         You can name the token GITLAB_ORG_PUSH_TOKEN_VALUE
         Give it api and write repository permissions
 
         SeeAlso: https://gitlab.org.com/profile/personal_access_tokens
 
         Take this variable and record its value somewhere safe. I put it in my secrets file as such:
 
@@ -119,62 +119,92 @@
 }
 
 ### FIXME: Should be configurable for general use
 
 setup_package_environs_gitlab_kitware(){
     echo '
     export VARNAME_CI_SECRET="CI_KITWARE_SECRET"
-    export VARNAME_TWINE_USERNAME="TWINE_USERNAME"
-    export VARNAME_TWINE_PASSWORD="TWINE_PASSWORD"
-    export VARNAME_TEST_TWINE_USERNAME="TEST_TWINE_USERNAME"
-    export VARNAME_TEST_TWINE_PASSWORD="TEST_TWINE_PASSWORD"
+    export VARNAME_TWINE_PASSWORD="EROTEMIC_PYPI_MASTER_TOKEN"
+    export VARNAME_TEST_TWINE_PASSWORD="EROTEMIC_TEST_PYPI_MASTER_TOKEN"
     export VARNAME_PUSH_TOKEN="GITLAB_KITWARE_TOKEN"
+    export VARNAME_TWINE_USERNAME="EROTEMIC_PYPI_MASTER_TOKEN_USERNAME"
+    export VARNAME_TEST_TWINE_USERNAME="EROTEMIC_TEST_PYPI_MASTER_TOKEN_USERNAME"
     export GPG_IDENTIFIER="=Erotemic-CI <erotemic@gmail.com>"
     ' | python -c "import sys; from textwrap import dedent; print(dedent(sys.stdin.read()).strip(chr(10)))" > dev/secrets_configuration.sh
     git add dev/secrets_configuration.sh
 }
 
 setup_package_environs_github_erotemic(){
     echo '
     export VARNAME_CI_SECRET="EROTEMIC_CI_SECRET"
-    export VARNAME_TWINE_USERNAME="TWINE_USERNAME"
-    export VARNAME_TWINE_PASSWORD="TWINE_PASSWORD"
-    export VARNAME_TEST_TWINE_USERNAME="TEST_TWINE_USERNAME"
-    export VARNAME_TEST_TWINE_PASSWORD="TEST_TWINE_PASSWORD"
+    export VARNAME_TWINE_PASSWORD="EROTEMIC_PYPI_MASTER_TOKEN"
+    export VARNAME_TEST_TWINE_PASSWORD="EROTEMIC_TEST_PYPI_MASTER_TOKEN"
+    export VARNAME_TWINE_USERNAME="EROTEMIC_PYPI_MASTER_TOKEN_USERNAME"
+    export VARNAME_TEST_TWINE_USERNAME="EROTEMIC_TEST_PYPI_MASTER_TOKEN_USERNAME"
     export GPG_IDENTIFIER="=Erotemic-CI <erotemic@gmail.com>"
     ' | python -c "import sys; from textwrap import dedent; print(dedent(sys.stdin.read()).strip(chr(10)))" > dev/secrets_configuration.sh
     git add dev/secrets_configuration.sh
 }
 
 setup_package_environs_github_pyutils(){
     echo '
     export VARNAME_CI_SECRET="PYUTILS_CI_SECRET"
+    export VARNAME_TWINE_PASSWORD="PYUTILS_PYPI_MASTER_TOKEN"
+    export VARNAME_TEST_TWINE_PASSWORD="PYUTILS_TEST_PYPI_MASTER_TOKEN"
+    export VARNAME_TWINE_USERNAME="PYUTILS_PYPI_MASTER_TOKEN_USERNAME"
+    export VARNAME_TEST_TWINE_USERNAME="PYUTILS_TEST_PYPI_MASTER_TOKEN_USERNAME"
     export GPG_IDENTIFIER="=PyUtils-CI <openpyutils@gmail.com>"
-    export VARNAME_TWINE_PASSWORD="PYUTILS_TWINE_PASSWORD"
-    export VARNAME_TWINE_PASSWORD="PYUTILS_TWINE_PASSWORD"
     ' | python -c "import sys; from textwrap import dedent; print(dedent(sys.stdin.read()).strip(chr(10)))" > dev/secrets_configuration.sh
     git add dev/secrets_configuration.sh
 
     #echo '
     #export VARNAME_CI_SECRET="PYUTILS_CI_SECRET"
     #export GPG_IDENTIFIER="=PyUtils-CI <openpyutils@gmail.com>"
     #' | python -c "import sys; from textwrap import dedent; print(dedent(sys.stdin.read()).strip(chr(10)))" > dev/secrets_configuration.sh
 }
 
 upload_github_secrets(){
     load_secrets
     unset GITHUB_TOKEN
-    gh auth login
+    #printf "%s" "$GITHUB_TOKEN" | gh auth login --hostname Github.com --with-token
+    if ! gh auth status ; then
+        gh auth login
+    fi
     source dev/secrets_configuration.sh
-    gh secret set "$VARNAME_CI_SECRET" -b"${!VARNAME_CI_SECRET}"
-    gh secret set "$VARNAME_TWINE_USERNAME" -b"${!VARNAME_TWINE_USERNAME}"
-    gh secret set "$VARNAME_TWINE_PASSWORD" -b"${!VARNAME_TWINE_PASSWORD}"
-    gh secret set "$VARNAME_TEST_TWINE_PASSWORD" -b"${!VARNAME_TEST_TWINE_PASSWORD}"
-    gh secret set "$VARNAME_TEST_TWINE_USERNAME" -b"${!VARNAME_TEST_TWINE_USERNAME}"
+    gh secret set "TWINE_USERNAME" -b"${!VARNAME_TWINE_USERNAME}"
+    gh secret set "TEST_TWINE_USERNAME" -b"${!VARNAME_TEST_TWINE_USERNAME}"
+    toggle_setx_enter
+    gh secret set "CI_SECRET" -b"${!VARNAME_CI_SECRET}"
+    gh secret set "TWINE_PASSWORD" -b"${!VARNAME_TWINE_PASSWORD}"
+    gh secret set "TEST_TWINE_PASSWORD" -b"${!VARNAME_TEST_TWINE_PASSWORD}"
+    toggle_setx_exit
+}
 
+
+toggle_setx_enter(){
+    # Can we do something like a try/finally?
+    # https://stackoverflow.com/questions/15656492/writing-try-catch-finally-in-shell
+    echo "Enter sensitive area"
+    if [[ -n "${-//[^x]/}" ]]; then
+        __context_1_toggle_setx=1
+    else
+        __context_1_toggle_setx=0
+    fi
+    if [[ "$__context_1_toggle_setx" == "1" ]]; then
+        echo "Setx was on, disable temporarilly"
+        set +x
+    fi
+}
+
+toggle_setx_exit(){
+    echo "Exit sensitive area"
+    # Can we guarentee this will happen?
+    if [[ "$__context_1_toggle_setx" == "1" ]]; then
+        set -x
+    fi
 }
 
 
 upload_gitlab_group_secrets(){
     __doc__="
     Use the gitlab API to modify group-level secrets
     "
@@ -191,59 +221,64 @@
     if [[ "$PRIVATE_GITLAB_TOKEN" == "ERROR" ]]; then
         echo "Failed to load authentication key"
         return 1
     fi
 
     TMP_DIR=$(mktemp -d -t ci-XXXXXXXXXX)
     curl --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups" > "$TMP_DIR/all_group_info"
-    GROUP_ID=$(cat "$TMP_DIR/all_group_info" | jq ". | map(select(.path==\"$GROUP_NAME\")) | .[0].id")
+    GROUP_ID=$(< "$TMP_DIR/all_group_info" jq ". | map(select(.path==\"$GROUP_NAME\")) | .[0].id")
     echo "GROUP_ID = $GROUP_ID"
 
     curl --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups/$GROUP_ID" > "$TMP_DIR/group_info"
-    cat "$TMP_DIR/group_info" | jq
+    < "$TMP_DIR/group_info" jq
 
     # Get group-level secret variables
     curl --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups/$GROUP_ID/variables" > "$TMP_DIR/group_vars"
-    cat "$TMP_DIR/group_vars" | jq '.[] | .key'
+    < "$TMP_DIR/group_vars" jq '.[] | .key'
 
     if [[ "$?" != "0" ]]; then
         echo "Failed to access group level variables. Probably a permission issue"
     fi
 
     source dev/secrets_configuration.sh
-    SECRET_VARNAME_ARR=(VARNAME_CI_SECRET VARNAME_TWINE_USERNAME VARNAME_TWINE_PASSWORD VARNAME_TEST_TWINE_PASSWORD VARNAME_TEST_TWINE_USERNAME VARNAME_PUSH_TOKEN)
+    SECRET_VARNAME_ARR=(VARNAME_CI_SECRET VARNAME_TWINE_PASSWORD VARNAME_TEST_TWINE_PASSWORD VARNAME_TWINE_USERNAME VARNAME_TEST_TWINE_USERNAME VARNAME_PUSH_TOKEN)
     for SECRET_VARNAME_PTR in "${SECRET_VARNAME_ARR[@]}"; do
         SECRET_VARNAME=${!SECRET_VARNAME_PTR}
         echo ""
         echo " ---- "
         LOCAL_VALUE=${!SECRET_VARNAME}
-        REMOTE_VALUE=$(cat "$TMP_DIR/group_vars" | jq -r ".[] | select(.key==\"$SECRET_VARNAME\") | .value")
+        REMOTE_VALUE=$(< "$TMP_DIR/group_vars" jq -r ".[] | select(.key==\"$SECRET_VARNAME\") | .value")
 
         # Print current local and remote value of a variable
         echo "SECRET_VARNAME_PTR = $SECRET_VARNAME_PTR"
         echo "SECRET_VARNAME = $SECRET_VARNAME"
         echo "(local)  $SECRET_VARNAME = $LOCAL_VALUE"
         echo "(remote) $SECRET_VARNAME = $REMOTE_VALUE"
 
         #curl --request GET --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups/$GROUP_ID/variables/SECRET_VARNAME" | jq -r .message
         if [[ "$REMOTE_VALUE" == "" ]]; then
             # New variable
             echo "Remove variable does not exist, posting"
+
+            toggle_setx_enter
             curl --request POST --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups/$GROUP_ID/variables" \
                     --form "key=${SECRET_VARNAME}" \
                     --form "value=${LOCAL_VALUE}" \
                     --form "protected=true" \
                     --form "masked=true" \
                     --form "environment_scope=*" \
-                    --form "variable_type=env_var" 
+                    --form "variable_type=env_var"
+            toggle_setx_exit
         elif [[ "$REMOTE_VALUE" != "$LOCAL_VALUE" ]]; then
             echo "Remove variable does not agree, putting"
             # Update variable value
+            toggle_setx_enter
             curl --request PUT --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups/$GROUP_ID/variables/$SECRET_VARNAME" \
-                    --form "value=${LOCAL_VALUE}" 
+                    --form "value=${LOCAL_VALUE}"
+            toggle_setx_exit
         else
             echo "Remote value agrees with local"
         fi
     done
     rm "$TMP_DIR/group_vars"
 }
 
@@ -265,40 +300,47 @@
     PRIVATE_GITLAB_TOKEN=$(git_token_for "$HOST")
     if [[ "$PRIVATE_GITLAB_TOKEN" == "ERROR" ]]; then
         echo "Failed to load authentication key"
         return 1
     fi
 
     TMP_DIR=$(mktemp -d -t ci-XXXXXXXXXX)
+    toggle_setx_enter
     curl --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups" > "$TMP_DIR/all_group_info"
-    GROUP_ID=$(cat "$TMP_DIR/all_group_info" | jq ". | map(select(.path==\"$GROUP_NAME\")) | .[0].id")
+    toggle_setx_exit
+    GROUP_ID=$(< "$TMP_DIR/all_group_info" jq ". | map(select(.path==\"$GROUP_NAME\")) | .[0].id")
     echo "GROUP_ID = $GROUP_ID"
 
+    toggle_setx_enter
     curl --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups/$GROUP_ID" > "$TMP_DIR/group_info"
-    cat "$TMP_DIR/group_info" | jq
+    toggle_setx_exit
+    GROUP_ID=$(< "$TMP_DIR/all_group_info" jq ". | map(select(.path==\"$GROUP_NAME\")) | .[0].id")
+    < "$TMP_DIR/group_info" jq
 
-    PROJECT_ID=$(cat "$TMP_DIR/group_info" | jq ".projects | map(select(.path==\"$PROJECT_NAME\")) | .[0].id")
+    PROJECT_ID=$(< "$TMP_DIR/group_info" jq ".projects | map(select(.path==\"$PROJECT_NAME\")) | .[0].id")
     echo "PROJECT_ID = $PROJECT_ID"
 
     # Get group-level secret variables
+    toggle_setx_enter
     curl --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/projects/$PROJECT_ID/variables" > "$TMP_DIR/project_vars"
-    cat "$TMP_DIR/project_vars" | jq '.[] | .key'
+    toggle_setx_exit
+    < "$TMP_DIR/project_vars" jq '.[] | .key'
     if [[ "$?" != "0" ]]; then
         echo "Failed to access project level variables. Probably a permission issue"
     fi
 
     LIVE_MODE=1
     source dev/secrets_configuration.sh
-    SECRET_VARNAME_ARR=(VARNAME_CI_SECRET VARNAME_TWINE_USERNAME VARNAME_TWINE_PASSWORD VARNAME_TEST_TWINE_PASSWORD VARNAME_TEST_TWINE_USERNAME VARNAME_PUSH_TOKEN)
+    SECRET_VARNAME_ARR=(VARNAME_CI_SECRET VARNAME_TWINE_PASSWORD VARNAME_TEST_TWINE_PASSWORD VARNAME_TWINE_USERNAME VARNAME_TEST_TWINE_USERNAME VARNAME_PUSH_TOKEN)
     for SECRET_VARNAME_PTR in "${SECRET_VARNAME_ARR[@]}"; do
         SECRET_VARNAME=${!SECRET_VARNAME_PTR}
         echo ""
         echo " ---- "
         LOCAL_VALUE=${!SECRET_VARNAME}
-        REMOTE_VALUE=$(cat "$TMP_DIR/project_vars" | jq -r ".[] | select(.key==\"$SECRET_VARNAME\") | .value")
+        REMOTE_VALUE=$(< "$TMP_DIR/project_vars" jq -r ".[] | select(.key==\"$SECRET_VARNAME\") | .value")
 
         # Print current local and remote value of a variable
         echo "SECRET_VARNAME_PTR = $SECRET_VARNAME_PTR"
         echo "SECRET_VARNAME = $SECRET_VARNAME"
         echo "(local)  $SECRET_VARNAME = $LOCAL_VALUE"
         echo "(remote) $SECRET_VARNAME = $REMOTE_VALUE"
 
@@ -309,24 +351,24 @@
             if [[ "$LIVE_MODE" == "1" ]]; then
                 curl --request POST --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/projects/$PROJECT_ID/variables" \
                         --form "key=${SECRET_VARNAME}" \
                         --form "value=${LOCAL_VALUE}" \
                         --form "protected=true" \
                         --form "masked=true" \
                         --form "environment_scope=*" \
-                        --form "variable_type=env_var" 
+                        --form "variable_type=env_var"
             else
                 echo "dry run, not posting"
             fi
         elif [[ "$REMOTE_VALUE" != "$LOCAL_VALUE" ]]; then
             echo "Remove variable does not agree, putting"
             # Update variable value
             if [[ "$LIVE_MODE" == "1" ]]; then
                 curl --request PUT --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/projects/$PROJECT_ID/variables/$SECRET_VARNAME" \
-                        --form "value=${LOCAL_VALUE}" 
+                        --form "value=${LOCAL_VALUE}"
             else
                 echo "dry run, not putting"
             fi
         else
             echo "Remote value agrees with local"
         fi
     done
@@ -349,18 +391,27 @@
 
     # ADD RELEVANT VARIABLES TO THE CI SECRET VARIABLES
     # HOW TO ENCRYPT YOUR SECRET GPG KEY
     # You need to have a known public gpg key for this to make any sense
 
     MAIN_GPG_KEYID=$(gpg --list-keys --keyid-format LONG "$GPG_IDENTIFIER" | head -n 2 | tail -n 1 | awk '{print $1}')
     GPG_SIGN_SUBKEY=$(gpg --list-keys --with-subkey-fingerprints "$GPG_IDENTIFIER" | grep "\[S\]" -A 1 | tail -n 1 | awk '{print $1}')
+    # Careful, if you don't have a subkey, requesting it will export more than you want.
+    # Export the main key instead (its better to have subkeys, but this is a lesser evil)
+    if [[ "$GPG_SIGN_SUBKEY" == "" ]]; then
+        # NOTE: if you get here this probably means your subkeys expired (and
+        # wont even be visible), so we probably should check for that here and
+        # thrown an error instead of using this hack, which likely wont work
+        # anyway.
+        GPG_SIGN_SUBKEY=$(gpg --list-keys --with-subkey-fingerprints "$GPG_IDENTIFIER" | grep "\[C\]" -A 1 | tail -n 1 | awk '{print $1}')
+    fi
     echo "MAIN_GPG_KEYID  = $MAIN_GPG_KEYID"
     echo "GPG_SIGN_SUBKEY = $GPG_SIGN_SUBKEY"
 
-    # Only export the signing secret subkey 
+    # Only export the signing secret subkey
     # Export plaintext gpg public keys, private sign key, and trust info
     mkdir -p dev
     gpg --armor --export-options export-backup --export-secret-subkeys "${GPG_SIGN_SUBKEY}!" > dev/ci_secret_gpg_subkeys.pgp
     gpg --armor --export "${GPG_SIGN_SUBKEY}" > dev/ci_public_gpg_key.pgp
     gpg --export-ownertrust > dev/gpg_owner_trust
 
     # Encrypt gpg keys and trust with CI secret
@@ -368,15 +419,15 @@
     GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -e -a -in dev/ci_secret_gpg_subkeys.pgp > dev/ci_secret_gpg_subkeys.pgp.enc
     GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -e -a -in dev/gpg_owner_trust > dev/gpg_owner_trust.enc
     echo "$MAIN_GPG_KEYID" > dev/public_gpg_key
 
     # Test decrpyt
     GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/ci_public_gpg_key.pgp.enc | gpg --list-packets --verbose
     GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/ci_secret_gpg_subkeys.pgp.enc  | gpg --list-packets --verbose
-    GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/gpg_owner_trust.enc 
+    GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/gpg_owner_trust.enc
     cat dev/public_gpg_key
 
     unload_secrets
 
     # Look at what we did, clean up, and add it to git
     ls dev/*.enc
     rm dev/*.pgp
@@ -384,31 +435,36 @@
     git status
     git add dev/*.enc
     git add dev/gpg_owner_trust
     git add dev/public_gpg_key
 }
 
 
+# See the xcookie module gitlab python API
+#gitlab_set_protected_branches(){
+#}
+
+
 _test_gnu(){
     # shellcheck disable=SC2155
     export GNUPGHOME=$(mktemp -d -t)
     ls -al "$GNUPGHOME"
     chmod 700 -R "$GNUPGHOME"
 
     source dev/secrets_configuration.sh
 
     gpg -k
-    
+
     load_secrets
     CI_SECRET="${!VARNAME_CI_SECRET}"
     echo "CI_SECRET = $CI_SECRET"
 
     cat dev/public_gpg_key
-    GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/ci_public_gpg_key.pgp.enc 
-    GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/gpg_owner_trust.enc 
+    GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/ci_public_gpg_key.pgp.enc
+    GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/gpg_owner_trust.enc
     GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/ci_secret_gpg_subkeys.pgp.enc
 
     GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/ci_public_gpg_key.pgp.enc | gpg --import
     GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/gpg_owner_trust.enc | gpg --import-ownertrust
     GLKWS=$CI_SECRET openssl enc -aes-256-cbc -pbkdf2 -md SHA512 -pass env:GLKWS -d -a -in dev/ci_secret_gpg_subkeys.pgp.enc | gpg --import
 
     gpg -k
```

### Comparing `pyflann_ibeis-2.3.0/dev/travis_public_gpg_key.pgp.enc` & `pyflann_ibeis-2.4.0/dev/travis_public_gpg_key.pgp.enc`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/dev/travis_secret_gpg_key.pgp.enc` & `pyflann_ibeis-2.4.0/dev/travis_secret_gpg_key.pgp.enc`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/docs/source/index.rst` & `pyflann_ibeis-2.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/examples/CMakeLists.txt` & `pyflann_ibeis-2.4.0/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/examples/flann_example.c` & `pyflann_ibeis-2.4.0/examples/flann_example.c`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/examples/flann_example.cpp` & `pyflann_ibeis-2.4.0/examples/flann_example.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/examples/flann_example_mpi.cpp` & `pyflann_ibeis-2.4.0/examples/flann_example_mpi.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/publish.sh` & `pyflann_ibeis-2.4.0/publish.sh`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-#!/bin/bash
-__doc__='''
-Script to publish a new version of this library on PyPI. 
+#!/usr/bin/env bash
+__doc__='
+Script to publish a new version of this library on PyPI.
 
 If your script has binary dependencies then we assume that you have built a
 proper binary wheel with auditwheel and it exists in the wheelhouse directory.
 Otherwise, for source tarballs and wheels this script runs the
 setup.py script to create the wheels as well.
 
 Running this script with the default arguments will perform any builds and gpg
 signing, but nothing will be uploaded to pypi unless the user explicitly sets
 DO_UPLOAD=True or answers yes to the prompts.
 
 Args:
-    TWINE_USERNAME (str) : 
+    TWINE_USERNAME (str) :
         username for pypi. This must be set if uploading to pypi.
         Defaults to "".
 
-    TWINE_PASSWORD (str) : 
+    TWINE_PASSWORD (str) :
         password for pypi. This must be set if uploading to pypi.
         Defaults to "".
 
-    DO_GPG (bool) : 
+    DO_GPG (bool) :
         If True, sign the packages with a GPG key specified by `GPG_KEYID`.
         defaults to auto.
 
-    DO_UPLOAD (bool) : 
+    DO_OTS (bool) :
+        If True, make an opentimestamp for the package and signature (if
+        available)
+
+    DO_UPLOAD (bool) :
         If True, upload the packages to the pypi server specified by
         `TWINE_REPOSITORY_URL`.
 
-    DO_BUILD (bool) : 
+    DO_BUILD (bool) :
         If True, will execute the setup.py build script, which is
         expected to use setuptools. In the future we may add support for other
         build systems. If False, this script will expect the pre-built packages
         to exist in "wheelhouse/{NAME}-{VERSION}-{SUFFIX}.{EXT}".
 
-        Defaults to "auto". 
+        Defaults to "auto".
 
-    DO_TAG (bool) : 
-        if True, will "git tag" the current HEAD with 
+    DO_TAG (bool) :
+        if True, will "git tag" the current HEAD with
 
-    TWINE_REPOSITORY_URL (url) : 
-         The URL of the pypi server to upload to. 
+    TWINE_REPOSITORY_URL (url) :
+         The URL of the pypi server to upload to.
          Defaults to "auto", which if on the release branch, this will default
          to the live pypi server `https://upload.pypi.org/legacy` otherwise
          this will default to the test.pypi server:
          `https://test.pypi.org/legacy`
 
      GPG_KEYID (str) :
         The keyid of the gpg key to sign with. (if DO_GPG=True). Defaults to
         the local git config user.signingkey
 
-    DEPLOY_REMOTE (str) : 
+    DEPLOY_REMOTE (str) :
         The git remote to push any tags to. Defaults to "origin"
 
-    GPG_EXECUTABLE (path) : 
-        Path to the GPG executable. 
+    GPG_EXECUTABLE (path) :
+        Path to the GPG executable.
         Defaults to "auto", which chooses "gpg2" if it exists, otherwise "gpg".
 
     MODE (str):
         Can be pure, binary, or all. Defaults to pure unless a CMakeLists.txt
         exists in which case it defaults to binary.
 
 Requirements:
@@ -80,16 +84,16 @@
 Usage:
     load_secrets
     # TODO: set a trap to unload secrets?
     cd <YOUR REPO>
     # Set your variables or load your secrets
     export TWINE_USERNAME=<pypi-username>
     export TWINE_PASSWORD=<pypi-password>
-    TWINE_REPOSITORY_URL="https://test.pypi.org/legacy/" 
-'''
+    TWINE_REPOSITORY_URL="https://test.pypi.org/legacy/"
+'
 
 DEBUG=${DEBUG:=''}
 if [[ "${DEBUG}" != "" ]]; then
     set -x
 fi
 
 check_variable(){
@@ -107,17 +111,17 @@
     fi
 }
 
 
 normalize_boolean(){
     ARG=$1
     ARG=$(echo "$ARG" | awk '{print tolower($0)}')
-    if [ "$ARG" = "true" ] || [ "$ARG" = "1" ] || [ "$ARG" = "yes" ] || [ "$ARG" = "on" ]; then
+    if [ "$ARG" = "true" ] || [ "$ARG" = "1" ] || [ "$ARG" = "yes" ] || [ "$ARG" = "y" ] || [ "$ARG" = "on" ]; then
         echo "True"
-    elif [ "$ARG" = "false" ] || [ "$ARG" = "0" ] || [ "$ARG" = "no" ] || [ "$ARG" = "off" ]; then
+    elif [ "$ARG" = "false" ] || [ "$ARG" = "0" ] || [ "$ARG" = "no" ] || [ "$ARG" = "n" ] || [ "$ARG" = "off" ]; then
         echo "False"
     else
         echo "$ARG"
     fi
 }
 
 
@@ -134,39 +138,50 @@
 
 ARG_1=$1
 
 DO_UPLOAD=${DO_UPLOAD:=$ARG_1}
 DO_TAG=${DO_TAG:=$ARG_1}
 
 DO_GPG=${DO_GPG:="auto"}
-# Verify that we want to build
 if [ "$DO_GPG" == "auto" ]; then
     DO_GPG="True"
 fi
 
+DO_OTS=${DO_OTS:="auto"}
+if [ "$DO_OTS" == "auto" ]; then
+    # Do opentimestamp if it is available
+    # python -m pip install opentimestamps-client
+    if type ots ; then
+        DO_OTS="True"
+    else
+        DO_OTS="False"
+    fi
+fi
+
 DO_BUILD=${DO_BUILD:="auto"}
 # Verify that we want to build
 if [ "$DO_BUILD" == "auto" ]; then
     DO_BUILD="True"
 fi
 
 DO_GPG=$(normalize_boolean "$DO_GPG")
+DO_OTS=$(normalize_boolean "$DO_OTS")
 DO_BUILD=$(normalize_boolean "$DO_BUILD")
 DO_UPLOAD=$(normalize_boolean "$DO_UPLOAD")
 DO_TAG=$(normalize_boolean "$DO_TAG")
 
 TWINE_USERNAME=${TWINE_USERNAME:=""}
 TWINE_PASSWORD=${TWINE_PASSWORD:=""}
 
 DEFAULT_TEST_TWINE_REPO_URL="https://test.pypi.org/legacy/"
 DEFAULT_LIVE_TWINE_REPO_URL="https://upload.pypi.org/legacy/"
 
 TWINE_REPOSITORY_URL=${TWINE_REPOSITORY_URL:="auto"}
 if [[ "${TWINE_REPOSITORY_URL}" == "auto" ]]; then
-    #if [[ "$(cat .git/HEAD)" != "ref: refs/heads/release" ]]; then 
+    #if [[ "$(cat .git/HEAD)" != "ref: refs/heads/release" ]]; then
     #    # If we are not on release, then default to the test pypi upload repo
     #    TWINE_REPOSITORY_URL=${TWINE_REPOSITORY_URL:="https://test.pypi.org/legacy/"}
     #else
     if [[ "$DEBUG" == "" ]]; then
         TWINE_REPOSITORY_URL="live"
     else
         TWINE_REPOSITORY_URL="test"
@@ -233,25 +248,26 @@
 TWINE_USERNAME='$TWINE_USERNAME'
 TWINE_REPOSITORY_URL = $TWINE_REPOSITORY_URL
 GPG_KEYID = '$GPG_KEYID'
 
 DO_UPLOAD=${DO_UPLOAD}
 DO_TAG=${DO_TAG}
 DO_GPG=${DO_GPG}
+DO_OTS=${DO_OTS}
 DO_BUILD=${DO_BUILD}
 MODE_LIST_STR=${MODE_LIST_STR}
 "
 
 
 # Verify that we want to tag
 if [[ "$DO_TAG" == "True" ]]; then
-    echo "About to tag VERSION='$VERSION'" 
+    echo "About to tag VERSION='$VERSION'"
 else
     if [[ "$DO_TAG" == "False" ]]; then
-        echo "We are NOT about to tag VERSION='$VERSION'" 
+        echo "We are NOT about to tag VERSION='$VERSION'"
     else
         # shellcheck disable=SC2162
         read -p "Do you want to git tag and push version='$VERSION'? (input 'yes' to confirm)" ANS
         echo "ANS = $ANS"
         WAS_INTERACTION="True"
         DO_TAG="$ANS"
         DO_TAG=$(normalize_boolean "$DO_TAG")
@@ -278,18 +294,18 @@
         DO_BUILD=$(normalize_boolean "$DO_BUILD")
     fi
 fi
 
 
 # Verify that we want to publish
 if [[ "$DO_UPLOAD" == "True" ]]; then
-    echo "About to directly publish VERSION='$VERSION'" 
+    echo "About to directly publish VERSION='$VERSION'"
 else
     if [[ "$DO_UPLOAD" == "False" ]]; then
-        echo "We are NOT about to directly publish VERSION='$VERSION'" 
+        echo "We are NOT about to directly publish VERSION='$VERSION'"
     else
         # shellcheck disable=SC2162
         read -p "Are you ready to directly publish version='$VERSION'? ('yes' will twine upload)" ANS
         echo "ANS = $ANS"
         WAS_INTERACTION="True"
         DO_UPLOAD="$ANS"
         DO_UPLOAD=$(normalize_boolean "$DO_UPLOAD")
@@ -371,138 +387,187 @@
     # FIXME; for some reason this doesnt always work properly
     # Copy the array into the dynamically named variable
     # shellcheck disable=SC2086
     readarray -t $arr_name < <(printf '%s\n' "${array[@]}")
 }
 
 
-WHEEL_PATHS=()
+WHEEL_FPATHS=()
 for _MODE in "${MODE_LIST[@]}"
 do
     if [[ "$_MODE" == "sdist" ]]; then
         ls_array "_NEW_WHEEL_PATHS" "dist/${NAME}-${VERSION}*.tar.gz"
     elif [[ "$_MODE" == "native" ]]; then
         ls_array "_NEW_WHEEL_PATHS" "dist/${NAME}-${VERSION}*.whl"
     elif [[ "$_MODE" == "bdist" ]]; then
         ls_array "_NEW_WHEEL_PATHS" "wheelhouse/${NAME}-${VERSION}-*.whl"
     else
         echo "ERROR: bad mode"
         exit 1
     fi
-    # hacky CONCAT because for some reason ls_array will return 
+    # hacky CONCAT because for some reason ls_array will return
     # something that looks empty but has one empty element
     for new_item in "${_NEW_WHEEL_PATHS[@]}"
     do
         if [[ "$new_item" != "" ]]; then
-            WHEEL_PATHS+=("$new_item")
+            WHEEL_FPATHS+=("$new_item")
         fi
     done
 done
 
 # Dedup the paths
-readarray -t WHEEL_PATHS < <(printf '%s\n' "${WHEEL_PATHS[@]}" | sort -u)
+readarray -t WHEEL_FPATHS < <(printf '%s\n' "${WHEEL_FPATHS[@]}" | sort -u)
 
-WHEEL_PATHS_STR=$(printf '"%s" ' "${WHEEL_PATHS[@]}")
+WHEEL_PATHS_STR=$(printf '"%s" ' "${WHEEL_FPATHS[@]}")
 echo "WHEEL_PATHS_STR = $WHEEL_PATHS_STR"
 
 echo "
-
-GLOBED
-------
 MODE=$MODE
 VERSION='$VERSION'
-WHEEL_PATHS='$WHEEL_PATHS_STR'
-
+WHEEL_FPATHS='$WHEEL_PATHS_STR'
 "
 
 
-
+WHEEL_SIGNATURE_FPATHS=()
 if [ "$DO_GPG" == "True" ]; then
 
     echo "
     === <GPG SIGN> ===
     "
 
-    for WHEEL_PATH in "${WHEEL_PATHS[@]}"
+    for WHEEL_FPATH in "${WHEEL_FPATHS[@]}"
     do
-        echo "WHEEL_PATH = $WHEEL_PATH"
-        check_variable WHEEL_PATH
+        echo "WHEEL_FPATH = $WHEEL_FPATH"
+        check_variable WHEEL_FPATH
             # https://stackoverflow.com/questions/45188811/how-to-gpg-sign-a-file-that-is-built-by-travis-ci
             # secure gpg --export-secret-keys > all.gpg
 
             # REQUIRES GPG >= 2.2
             check_variable GPG_EXECUTABLE || { echo 'failed no gpg exe' ; exit 1; }
             check_variable GPG_KEYID || { echo 'failed no gpg key' ; exit 1; }
 
             echo "Signing wheels"
             GPG_SIGN_CMD="$GPG_EXECUTABLE --batch --yes --detach-sign --armor --local-user $GPG_KEYID"
             echo "GPG_SIGN_CMD = $GPG_SIGN_CMD"
-            $GPG_SIGN_CMD --output "$WHEEL_PATH".asc "$WHEEL_PATH"
+            $GPG_SIGN_CMD --output "$WHEEL_FPATH".asc "$WHEEL_FPATH"
 
             echo "Checking wheels"
-            twine check "$WHEEL_PATH".asc "$WHEEL_PATH" || { echo 'could not check wheels' ; exit 1; }
+            twine check "$WHEEL_FPATH".asc "$WHEEL_FPATH" || { echo 'could not check wheels' ; exit 1; }
 
             echo "Verifying wheels"
-            $GPG_EXECUTABLE --verify "$WHEEL_PATH".asc "$WHEEL_PATH" || { echo 'could not verify wheels' ; exit 1; }
+            $GPG_EXECUTABLE --verify "$WHEEL_FPATH".asc "$WHEEL_FPATH" || { echo 'could not verify wheels' ; exit 1; }
+
+            WHEEL_SIGNATURE_FPATHS+=("$WHEEL_FPATH".asc)
     done
     echo "
     === <END GPG SIGN> ===
     "
 else
     echo "DO_GPG=False, Skipping GPG sign"
 fi
 
 
+
+if [ "$DO_OTS" == "True" ]; then
+
+    echo "
+    === <OTS SIGN> ===
+    "
+    if [ "$DO_GPG" == "True" ]; then
+        # Stamp the wheels and the signatures
+        ots stamp "${WHEEL_FPATHS[@]}" "${WHEEL_SIGNATURE_FPATHS[@]}"
+    else
+        # Stamp only the wheels
+        ots stamp "${WHEEL_FPATHS[@]}"
+    fi
+    echo "
+    === <END OTS SIGN> ===
+    "
+else
+    echo "DO_OTS=False, Skipping OTS sign"
+fi
+
+
 if [[ "$DO_TAG" == "True" ]]; then
     TAG_NAME="v${VERSION}"
     # if we messed up we can delete the tag
     # git push origin :refs/tags/$TAG_NAME
     # and then tag with -f
-    # 
+    #
     git tag "$TAG_NAME" -m "tarball tag $VERSION"
-    git push --tags $DEPLOY_REMOTE
+    git push --tags "$DEPLOY_REMOTE"
     echo "Should also do a: git push $DEPLOY_REMOTE main:release"
     echo "For github should draft a new release: https://github.com/PyUtils/line_profiler/releases/new"
 else
     echo "Not tagging"
 fi
 
 
 if [[ "$DO_UPLOAD" == "True" ]]; then
     check_variable TWINE_USERNAME
     check_variable TWINE_PASSWORD "hide"
 
-    for WHEEL_PATH in "${WHEEL_PATHS[@]}"
+    for WHEEL_FPATH in "${WHEEL_FPATHS[@]}"
     do
-        if [ "$DO_GPG" == "True" ]; then
-            twine upload --username "$TWINE_USERNAME" --password=$TWINE_PASSWORD  \
-                --repository-url "$TWINE_REPOSITORY_URL" \
-                --sign "$WHEEL_PATH".asc "$WHEEL_PATH" --skip-existing --verbose || { echo 'failed to twine upload' ; exit 1; }
-        else
-            twine upload --username "$TWINE_USERNAME" --password=$TWINE_PASSWORD \
-                --repository-url "$TWINE_REPOSITORY_URL" \
-                "$WHEEL_PATH" --skip-existing --verbose || { echo 'failed to twine upload' ; exit 1; }
-        fi
+        twine upload --username "$TWINE_USERNAME" "--password=$TWINE_PASSWORD" \
+            --repository-url "$TWINE_REPOSITORY_URL" \
+            "$WHEEL_FPATH" --skip-existing --verbose || { echo 'failed to twine upload' ; exit 1; }
     done
     echo """
         !!! FINISH: LIVE RUN !!!
     """
 else
     echo """
         DRY RUN ... Skipping upload
 
         DEPLOY_REMOTE = '$DEPLOY_REMOTE'
         DO_UPLOAD = '$DO_UPLOAD'
-        WHEEL_PATH = '$WHEEL_PATH'
+        WHEEL_FPATH = '$WHEEL_FPATH'
         WHEEL_PATHS_STR = '$WHEEL_PATHS_STR'
         MODE_LIST_STR = '$MODE_LIST_STR'
 
         VERSION='$VERSION'
         NAME='$NAME'
         TWINE_USERNAME='$TWINE_USERNAME'
         GPG_KEYID = '$GPG_KEYID'
 
         To do live run set DO_UPLOAD=1 and ensure deploy and current branch are the same
 
         !!! FINISH: DRY RUN !!!
     """
 fi
+
+__devel__='
+# Checking to see how easy it is to upload packages to gitlab.
+# This logic should go in the CI script, not sure if it belongs here.
+
+
+export HOST=https://gitlab.kitware.com
+export GROUP_NAME=computer-vision
+export PROJECT_NAME=geowatch
+PROJECT_VERSION=$(geowatch --version)
+echo "$PROJECT_VERSION"
+
+load_secrets
+export PRIVATE_GITLAB_TOKEN=$(git_token_for "$HOST")
+TMP_DIR=$(mktemp -d -t ci-XXXXXXXXXX)
+
+curl --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups" > "$TMP_DIR/all_group_info"
+GROUP_ID=$(cat "$TMP_DIR/all_group_info" | jq ". | map(select(.name==\"$GROUP_NAME\")) | .[0].id")
+echo "GROUP_ID = $GROUP_ID"
+
+curl --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" "$HOST/api/v4/groups/$GROUP_ID" > "$TMP_DIR/group_info"
+PROJ_ID=$(cat "$TMP_DIR/group_info" | jq ".projects | map(select(.name==\"$PROJECT_NAME\")) | .[0].id")
+echo "PROJ_ID = $PROJ_ID"
+
+ls_array DIST_FPATHS "dist/*"
+
+for FPATH in "${DIST_FPATHS[@]}"
+do
+    FNAME=$(basename $FPATH)
+    echo $FNAME
+    curl --header "PRIVATE-TOKEN: $PRIVATE_GITLAB_TOKEN" \
+         --upload-file $FPATH \
+         "https://gitlab.kitware.com/api/v4/projects/$PROJ_ID/packages/generic/$PROJECT_NAME/$PROJECT_VERSION/$FNAME"
+done
+
+'
```

### Comparing `pyflann_ibeis-2.3.0/pyflann_ibeis/__init__.py` & `pyflann_ibeis-2.4.0/pyflann_ibeis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,27 +20,23 @@
 #INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
 #NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 #DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 #THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
 #THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-#import sys
-#import os
-#sys.path.insert(0, os.path.split(__file__)[0]) # make python3 happy
+__version__ = '2.4.0'
+__author__ = 'Marius Muja, David G. Lowe, Jon Crall'
+__author_email__ = 'erotemic@gmail.com'
+__url__ = 'https://github.com/Erotemic/pyflann_ibeis'
 
-"""
+__autogen__ = """
 mkinit pyflann_ibeis
 """
 
-__version__ = '2.3.0'
-__author__ = 'Jon Crall'
-__author_email__ = 'erotemic@gmail.com'
-__url__ = 'https://github.com/Erotemic/pyflan_ibeis'
-
 
 from pyflann_ibeis import exceptions
 from pyflann_ibeis import flann_ctypes
 from pyflann_ibeis import index
 
 from pyflann_ibeis.exceptions import (FLANNException,)
 from pyflann_ibeis.flann_ctypes import (CustomStructure, FLANNParameters,
```

### Comparing `pyflann_ibeis-2.3.0/pyflann_ibeis/__main__.py` & `pyflann_ibeis-2.4.0/pyflann_ibeis/__main__.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/pyflann_ibeis/exceptions.py` & `pyflann_ibeis-2.4.0/pyflann_ibeis/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/pyflann_ibeis/flann_ctypes.py` & `pyflann_ibeis-2.4.0/pyflann_ibeis/flann_ctypes.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/pyflann_ibeis/flann_ctypes.pyi` & `pyflann_ibeis-2.4.0/pyflann_ibeis/flann_ctypes.pyi`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/pyflann_ibeis/index.py` & `pyflann_ibeis-2.4.0/pyflann_ibeis/index.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/pyflann_ibeis/index.pyi` & `pyflann_ibeis-2.4.0/pyflann_ibeis/index.pyi`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/pyflann_ibeis.egg-info/SOURCES.txt` & `pyflann_ibeis-2.4.0/pyflann_ibeis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 build_wheels.sh
 clean.sh
 publish.sh
 pyproject.toml
 requirements.txt
 run_developer_setup.sh
 run_doctests.sh
+run_linter.sh
 run_tests.py
 setup.py
 .github/dependabot.yml
-.github/workflows/test_binaries.yml
+.github/workflows/tests.yml
 CMake/CMakeLists.txt
 CMake/Config.cmake.in
 CMake/FindFlann.cmake
 CMake/flann.pc.in
 CMake/flann_utils.cmake
 CMake/python_utils.cmake
 CMake/uninstall_target.cmake.in
@@ -35,14 +36,16 @@
 dev/make_strict_req.sh
 dev/public_gpg_key
 dev/secrets_configuration.sh
 dev/setup_secrets.sh
 dev/travis_public_gpg_key.pgp.enc
 dev/travis_secret_gpg_key.pgp.enc
 dev/docker/make_base_image.py
+docs/Makefile
+docs/make.bat
 docs/source/conf.py
 docs/source/index.rst
 examples/CMakeLists.txt
 examples/README
 examples/flann_example.c
 examples/flann_example.cpp
 examples/flann_example_mpi.cpp
@@ -60,14 +63,15 @@
 pyflann_ibeis.egg-info/SOURCES.txt
 pyflann_ibeis.egg-info/dependency_links.txt
 pyflann_ibeis.egg-info/requires.txt
 pyflann_ibeis.egg-info/top_level.txt
 pyflann_ibeis/lib/__init__.py
 requirements/build.txt
 requirements/docs.txt
+requirements/linting.txt
 requirements/optional.txt
 requirements/runtime.txt
 requirements/tests.txt
 src/CMakeLists.txt
 src/cpp/CMakeLists.txt
 src/cpp/flann/config.h
 src/cpp/flann/config.h.in
```

### Comparing `pyflann_ibeis-2.3.0/pyproject.toml` & `pyflann_ibeis-2.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 [build-system]
 requires = [ "setuptools>=41.0.1", "wheel", "scikit-build>=0.9.0", "numpy", "ninja", "cmake"]
 
+[tool.xcookie]
+tags = [ "erotemic", "github", "binpy",]
+mod_name = "pyflann_ibeis"
+repo_name = "pyflann_ibeis"
+os = [ "linux" ]
+url = "https://github.com/Erotemic/pyflann_ibeis"
+description = "pyflann fork for IBEIS"
+author = ['Jon Crall', 'Marius Muja']
+author_email="erotemic@gmail.com"
+min_python = 3.8
+license = "BSD"
+dev_status = "stable"
+
 [tool.cibuildwheel]
-build = "cp37-* cp38-* cp39-* cp310-* cp311-*"
+build = "cp38-* cp39-* cp310-* cp311-* cp312-*"
+#build = "cp312-*"
 build-frontend = "build"
-skip = "pp* cp27-* cp34-* cp35-* cp36-* *-musllinux_*"
+skip = "pp* cp27-* cp34-* cp35-* cp36-* cp37-* *-musllinux_*"
 build-verbosity = 1
 test-requires = [ "-r requirements/tests.txt",]
 test-command = "python {project}/run_tests.py"
 
-# See: ~/code/vtool_ibeis_ext/dev/build_base_docker2.py
+
+# See: ~/code/vtool_ibeis_ext/dev/build_base_docker.py
 manylinux-x86_64-image = "quay.io/erotemic/manylinux2014_x86_64_for:lz4"
 manylinux-i686-image = "quay.io/erotemic/manylinux2014_i686_for:lz4"
 
-[tool.xcookie]
-tags = [ "erotemic", "github", "binpy",]
-mod_name = "pyflann_ibeis"
-repo_name = "pyflann_ibeis"
-
-#[tool.cibuildwheel.linux]
+[tool.cibuildwheel.linux]
 #before-all = "yum install epel-release lz4 lz4-devel -y"
+before-all = "yum update -y && yum install lz4-devel -y"
 
 #[tool.cibuildwheel.windows]
 #before-all = "choco install lz4 -y"
 
 #[tool.cibuildwheel.macos]
 #before-all = "brew install lz4"
```

### Comparing `pyflann_ibeis-2.3.0/run_tests.py` & `pyflann_ibeis-2.4.0/run_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,24 +109,25 @@
         print(f'No installed version of {package_name} found')
 
     try:
         print('Changing dirs to test_dir={!r}'.format(test_dir))
         os.chdir(test_dir)
 
         pytest_args = [
-            '--cov-config', '../pyproject.toml',
-            '--cov-report', 'html',
-            '--cov-report', 'term',
-            '--cov-report', 'xml',
-            '--cov=' + package_name,
+            # '--cov-config', '../pyproject.toml',
+            # '--cov-report', 'html',
+            # '--cov-report', 'term',
+            # '--cov-report', 'xml',
+            # '--cov=' + package_name,
+            modpath, '.'
         ]
-        if is_cibuildwheel():
-            pytest_args.append('--cov-append')
+        # if is_cibuildwheel():
+        #     pytest_args.append('--cov-append')
 
         pytest_args = pytest_args + sys.argv[1:]
         sys.exit(pytest.main(pytest_args))
     finally:
         os.chdir(cwd)
-        if is_cibuildwheel():
-            # for CIBW under linux
-            copy_coverage_cibuildwheel_docker(f'/home/runner/work/{package_name}/{package_name}')
+        # if is_cibuildwheel():
+        #     # for CIBW under linux
+        #     copy_coverage_cibuildwheel_docker(f'/home/runner/work/{package_name}/{package_name}')
         print('Restoring cwd = {!r}'.format(cwd))
```

### Comparing `pyflann_ibeis-2.3.0/setup.py` & `pyflann_ibeis-2.4.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,157 +11,173 @@
     CIBW_SKIP='pp*' \
         cibuildwheel --config-file pyproject.toml --platform linux --arch x86_64
 
 
 """
 from __future__ import absolute_import, division, print_function
 import sys
-from os.path import exists
 from collections import OrderedDict
+import re
+from os.path import exists, dirname, join
 
 
-def native_mb_python_tag(plat_impl=None, version_info=None):
-    """
-    Example:
-        >>> print(native_mb_python_tag())
-        >>> print(native_mb_python_tag('PyPy', (2, 7)))
-        >>> print(native_mb_python_tag('CPython', (3, 8)))
-    """
-    if plat_impl is None:
-        import platform
-        plat_impl = platform.python_implementation()
-
-    if version_info is None:
-        import sys
-        version_info = sys.version_info
-
-    major, minor = version_info[0:2]
-    ver = '{}{}'.format(major, minor)
-
-    if plat_impl == 'CPython':
-        # TODO: get if cp27m or cp27mu
-        impl = 'cp'
-        if ver == '27':
-            IS_27_BUILT_WITH_UNICODE = True  # how to determine this?
-            if IS_27_BUILT_WITH_UNICODE:
-                abi = 'mu'
-            else:
-                abi = 'm'
-        else:
-            if ver == '38':
-                # no abi in 38?
-                abi = ''
-            else:
-                abi = 'm'
-        mb_tag = '{impl}{ver}-{impl}{ver}{abi}'.format(**locals())
-    elif plat_impl == 'PyPy':
-        abi = ''
-        impl = 'pypy'
-        ver = '{}{}'.format(major, minor)
-        mb_tag = '{impl}-{ver}'.format(**locals())
-    else:
-        raise NotImplementedError(plat_impl)
-    return mb_tag
-
-
-def parse_version(fpath='pyflann_ibeis/__init__.py'):
+def parse_version(fpath):
     """
     Statically parse the version number from a python file
+    """
+    value = static_parse("__version__", fpath)
+    return value
 
 
+def static_parse(varname, fpath):
+    """
+    Statically parse the a constant variable from a python file
     """
     import ast
+
     if not exists(fpath):
-        raise ValueError('fpath={!r} does not exist'.format(fpath))
-    with open(fpath, 'r') as file_:
+        raise ValueError("fpath={!r} does not exist".format(fpath))
+    with open(fpath, "r") as file_:
         sourcecode = file_.read()
     pt = ast.parse(sourcecode)
-    class VersionVisitor(ast.NodeVisitor):
+
+    class StaticVisitor(ast.NodeVisitor):
         def visit_Assign(self, node):
             for target in node.targets:
-                if getattr(target, 'id', None) == '__version__':
-                    self.version = node.value.s
-    visitor = VersionVisitor()
+                if getattr(target, "id", None) == varname:
+                    self.static_value = node.value.s
+
+    visitor = StaticVisitor()
     visitor.visit(pt)
-    return visitor.version
+    try:
+        value = visitor.static_value
+    except AttributeError:
+        import warnings
 
+        value = "Unknown {}".format(varname)
+        warnings.warn(value)
+    return value
 
-def parse_long_description(fpath='README.rst'):
+
+def parse_description():
     """
-    Reads README text, but doesn't break if README does not exist.
+    Parse the description in the README file
+
+    CommandLine:
+        pandoc --from=markdown --to=rst --output=README.rst README.md
+        python -c "import setup; print(setup.parse_description())"
     """
-    if exists(fpath):
-        with open(fpath, 'r') as file:
-            return file.read()
-    return ''
+    readme_fpath = join(dirname(__file__), "README.rst")
+    # This breaks on pip install, so check that it exists.
+    if exists(readme_fpath):
+        with open(readme_fpath, "r") as f:
+            text = f.read()
+        return text
+    return ""
 
 
-def parse_requirements(fname='requirements.txt'):
+def parse_requirements(fname="requirements.txt", versions=False):
     """
-    Parse the package dependencies listed in a requirements file but
-    strips specific versioning information.
+    Parse the package dependencies listed in a requirements file but strips
+    specific versioning information.
+
+    Args:
+        fname (str): path to requirements file
+        versions (bool | str, default=False):
+            If true include version specs.
+            If strict, then pin to the minimum version.
+
+    Returns:
+        List[str]: list of requirements items
 
     CommandLine:
-        python -c "import setup; print(setup.parse_requirements())"
+        python -c "import setup, ubelt; print(ubelt.urepr(setup.parse_requirements()))"
     """
-    import re
     require_fpath = fname
 
-    def parse_line(line):
+    def parse_line(line, dpath=""):
         """
         Parse information from a line in a requirements text file
+
+        line = 'git+https://a.com/somedep@sometag#egg=SomeDep'
+        line = '-e git+https://a.com/somedep@sometag#egg=SomeDep'
         """
-        if line.startswith('-r '):
+        # Remove inline comments
+        comment_pos = line.find(" #")
+        if comment_pos > -1:
+            line = line[:comment_pos]
+
+        if line.startswith("-r "):
             # Allow specifying requirements in other files
-            target = line.split(' ')[1]
+            target = join(dpath, line.split(" ")[1])
             for info in parse_require_file(target):
                 yield info
-        elif line.startswith('-e '):
-            info = {}
-            info['package'] = line.split('#egg=')[1]
-            yield info
         else:
-            # Remove versioning from the package
-            pat = '(' + '|'.join(['>=', '==', '>']) + ')'
-            parts = re.split(pat, line, maxsplit=1)
-            parts = [p.strip() for p in parts]
-
-            info = {}
-            info['package'] = parts[0]
-            if len(parts) > 1:
-                op, rest = parts[1:]
-                if ';' in rest:
+            # See: https://www.python.org/dev/peps/pep-0508/
+            info = {"line": line}
+            if line.startswith("-e "):
+                info["package"] = line.split("#egg=")[1]
+            else:
+                if "--find-links" in line:
+                    # setuptools doesnt seem to handle find links
+                    line = line.split("--find-links")[0]
+                if ";" in line:
+                    pkgpart, platpart = line.split(";")
                     # Handle platform specific dependencies
-                    # http://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-platform-specific-dependencies
-                    version, platform_deps = map(str.strip, rest.split(';'))
-                    info['platform_deps'] = platform_deps
+                    # setuptools.readthedocs.io/en/latest/setuptools.html
+                    # #declaring-platform-specific-dependencies
+                    plat_deps = platpart.strip()
+                    info["platform_deps"] = plat_deps
                 else:
+                    pkgpart = line
+                    platpart = None
+
+                # Remove versioning from the package
+                pat = "(" + "|".join([">=", "==", ">"]) + ")"
+                parts = re.split(pat, pkgpart, maxsplit=1)
+                parts = [p.strip() for p in parts]
+
+                info["package"] = parts[0]
+                if len(parts) > 1:
+                    op, rest = parts[1:]
                     version = rest  # NOQA
-                info['version'] = (op, version)
+                    info["version"] = (op, version)
             yield info
 
     def parse_require_file(fpath):
-        with open(fpath, 'r') as f:
+        dpath = dirname(fpath)
+        with open(fpath, "r") as f:
             for line in f.readlines():
                 line = line.strip()
-                if line and not line.startswith('#'):
-                    for info in parse_line(line):
+                if line and not line.startswith("#"):
+                    for info in parse_line(line, dpath=dpath):
                         yield info
 
-    # This breaks on pip install, so check that it exists.
-    packages = []
-    if exists(require_fpath):
-        for info in parse_require_file(require_fpath):
-            package = info['package']
-            if not sys.version.startswith('3.4'):
-                # apparently package_deps are broken in 3.4
-                platform_deps = info.get('platform_deps')
-                if platform_deps is not None:
-                    package += ';' + platform_deps
-            packages.append(package)
+    def gen_packages_items():
+        if exists(require_fpath):
+            for info in parse_require_file(require_fpath):
+                parts = [info["package"]]
+                if versions and "version" in info:
+                    if versions == "strict":
+                        # In strict mode, we pin to the minimum version
+                        if info["version"]:
+                            # Only replace the first >= instance
+                            verstr = "".join(info["version"]).replace(">=", "==", 1)
+                            parts.append(verstr)
+                    else:
+                        parts.extend(info["version"])
+                if not sys.version.startswith("3.4"):
+                    # apparently package_deps are broken in 3.4
+                    plat_deps = info.get("platform_deps")
+                    if plat_deps is not None:
+                        parts.append(";" + plat_deps)
+                item = "".join(parts)
+                yield item
+
+    packages = list(gen_packages_items())
     return packages
 
 
 try:
     class EmptyListWithLength(list):
         def __len__(self):
             return 1
@@ -174,41 +190,58 @@
 except Exception:
     raise RuntimeError('FAILED TO ADD BUILD CONSTRUCTS')
 
 
 NAME = 'pyflann_ibeis'
 
 
-MB_PYTHON_TAG = native_mb_python_tag()  # NOQA
 VERSION = version = parse_version('pyflann_ibeis/__init__.py')  # must be global for git tags
 
 AUTHORS = ['Jon Crall', 'Marius Muja']
 AUTHOR_EMAIL = 'erotemic@gmail.com'
 URL = 'https://github.com/Erotemic/pyflann_ibeis'
 LICENSE = 'BSD'
 DESCRIPTION = 'FLANN (for IBEIS) - Fast Library for Approximate Nearest Neighbors'
 
 
+setupkw = {}
+setupkw["install_requires"] = parse_requirements(
+    "requirements/runtime.txt", versions="loose"
+)
+setupkw["extras_require"] = {
+    "all": parse_requirements("requirements.txt", versions="loose"),
+    "runtime": parse_requirements("requirements/runtime.txt", versions="loose"),
+    "tests": parse_requirements("requirements/tests.txt", versions="loose"),
+    "optional": parse_requirements("requirements/optional.txt", versions="loose"),
+    "build": parse_requirements("requirements/build.txt", versions="loose"),
+    "docs": parse_requirements("requirements/docs.txt", versions="loose"),
+    "all-strict": parse_requirements("requirements.txt", versions="strict"),
+    "runtime-strict": parse_requirements(
+        "requirements/runtime.txt", versions="strict"
+    ),
+    "tests-strict": parse_requirements("requirements/tests.txt", versions="strict"),
+    "optional-strict": parse_requirements(
+        "requirements/optional.txt", versions="strict"
+    ),
+    "build-strict": parse_requirements("requirements/build.txt", versions="strict"),
+    "docs-strict": parse_requirements("requirements/docs.txt", versions="strict"),
+}
+
+
 KWARGS = OrderedDict(
     name=NAME,
     version=VERSION,
     author=', '.join(AUTHORS),
     author_email=AUTHOR_EMAIL,
     description=DESCRIPTION,
-    long_description=parse_long_description('README.rst'),
+    long_description=parse_description(),
     long_description_content_type='text/x-rst',
     url=URL,
     license=LICENSE,
-    install_requires=parse_requirements('requirements/runtime.txt'),
-    extras_require={
-        'all': parse_requirements('requirements.txt'),
-        'tests': parse_requirements('requirements/tests.txt'),
-        'build': parse_requirements('requirements/build.txt'),
-        'runtime': parse_requirements('requirements/runtime.txt'),
-    },
+    **setupkw,
 
     # --- PACKAGES ---
     # The combination of packages and package_dir is how scikit-build will
     # know that the cmake installed files belong in the pyflann module and
     # not the data directory.
 
     packages=[
@@ -225,28 +258,28 @@
     package_data={
         'pyflann_ibeis': ['py.typed', '*.pyi'],
     },
 
     include_package_data=False,
     # List of classifiers available at:
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 6 - Mature',
         'License :: OSI Approved :: BSD License',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
-        'Operating System :: MacOS :: MacOS X',
+        # 'Operating System :: MacOS :: MacOS X',
         'Operating System :: Unix',
         'Topic :: Software Development :: Libraries :: Python Modules',
-        # 'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Recognition'
     ],
     cmake_args=[
         '-DBUILD_C_BINDINGS=ON',
         '-DBUILD_MATLAB_BINDINGS=OFF',
         '-DBUILD_EXAMPLES=OFF',
```

### Comparing `pyflann_ibeis-2.3.0/src/cpp/CMakeLists.txt` & `pyflann_ibeis-2.4.0/src/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/all_indices.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/all_indices.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/autotuned_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/autotuned_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/center_chooser.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/center_chooser.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/composite_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/composite_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/dist.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/dist.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/hierarchical_clustering_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/hierarchical_clustering_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_cuda_3d_index.cu` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_cuda_3d_index.cu`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_cuda_3d_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_cuda_3d_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_cuda_builder.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_cuda_builder.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kdtree_single_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kdtree_single_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/kmeans_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/kmeans_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/linear_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/linear_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/lsh_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/lsh_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/algorithms/nn_index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/algorithms/nn_index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/config.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/config.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/config.h.in` & `pyflann_ibeis-2.4.0/src/cpp/flann/config.h.in`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/defines.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/defines.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/flann.cpp` & `pyflann_ibeis-2.4.0/src/cpp/flann/flann.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/flann.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/flann.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/flann.hpp` & `pyflann_ibeis-2.4.0/src/cpp/flann/flann.hpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/flann_cpp.cpp` & `pyflann_ibeis-2.4.0/src/cpp/flann/flann_cpp.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/general.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/general.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/io/hdf5.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/io/hdf5.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/mpi/client.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/mpi/client.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/mpi/flann_mpi_client.cpp` & `pyflann_ibeis-2.4.0/src/cpp/flann/mpi/flann_mpi_client.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/mpi/flann_mpi_server.cpp` & `pyflann_ibeis-2.4.0/src/cpp/flann/mpi/flann_mpi_server.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/mpi/index.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/mpi/index.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/mpi/matrix.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/mpi/matrix.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/mpi/queries.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/mpi/queries.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/mpi/server.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/mpi/server.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/nn/ground_truth.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/nn/ground_truth.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/nn/index_testing.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/nn/index_testing.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/nn/simplex_downhill.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/nn/simplex_downhill.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/allocator.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/allocator.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/any.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/any.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/cuda/heap.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/cuda/heap.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/cuda/result_set.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/cuda/result_set.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/cutil_math.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/cutil_math.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/dynamic_bitset.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/dynamic_bitset.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/heap.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/heap.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/logger.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/logger.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/lsh_table.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/lsh_table.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/matrix.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/matrix.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/object_factory.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/object_factory.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/params.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/params.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/random.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/random.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/result_set.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/result_set.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/sampling.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/sampling.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/saving.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/saving.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/serialization.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/serialization.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/src/cpp/flann/util/timer.h` & `pyflann_ibeis-2.4.0/src/cpp/flann/util/timer.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/CMakeLists.txt` & `pyflann_ibeis-2.4.0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_autotuned_test.cpp` & `pyflann_ibeis-2.4.0/tests/flann_autotuned_test.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_cuda_test.cu` & `pyflann_ibeis-2.4.0/tests/flann_cuda_test.cu`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_hierarchical_test.cpp` & `pyflann_ibeis-2.4.0/tests/flann_hierarchical_test.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_kdtree_single_test.cpp` & `pyflann_ibeis-2.4.0/tests/flann_kdtree_single_test.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_kdtree_test.cpp` & `pyflann_ibeis-2.4.0/tests/flann_kdtree_test.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_kmeans_test.cpp` & `pyflann_ibeis-2.4.0/tests/flann_kmeans_test.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_linear_test.cpp` & `pyflann_ibeis-2.4.0/tests/flann_linear_test.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_lsh_test.cpp` & `pyflann_ibeis-2.4.0/tests/flann_lsh_test.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_multithreaded_test.cpp` & `pyflann_ibeis-2.4.0/tests/flann_multithreaded_test.cpp`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/flann_tests.h` & `pyflann_ibeis-2.4.0/tests/flann_tests.h`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/memusage_clustering.py` & `pyflann_ibeis-2.4.0/tests/memusage_clustering.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/memusage_nn.py` & `pyflann_ibeis-2.4.0/tests/memusage_nn.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/test_clustering.py` & `pyflann_ibeis-2.4.0/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/test_index_save.py` & `pyflann_ibeis-2.4.0/tests/test_index_save.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/test_nn.py` & `pyflann_ibeis-2.4.0/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/test_nn_autotune.py` & `pyflann_ibeis-2.4.0/tests/test_nn_autotune.py`

 * *Files identical despite different names*

### Comparing `pyflann_ibeis-2.3.0/tests/test_nn_index.py` & `pyflann_ibeis-2.4.0/tests/test_nn_index.py`

 * *Files identical despite different names*

