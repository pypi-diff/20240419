# Comparing `tmp/blickfeld_qb2-2.0.7.tar.gz` & `tmp/blickfeld_qb2-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blickfeld_qb2-2.0.7.tar", last modified: Thu Apr  4 06:18:50 2024, max compression
+gzip compressed data, was "blickfeld_qb2-2.0.9.tar", last modified: Fri Apr 12 04:16:14 2024, max compression
```

## Comparing `blickfeld_qb2-2.0.7.tar` & `blickfeld_qb2-2.0.9.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2024-04-04 06:18:37.000000 blickfeld_qb2-2.0.7/LICENSE.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/PKG-INFO
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      493 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4464 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2253 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2411 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/geometry/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3394 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/geometry/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4319 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/channel.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/device_ca_cert.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      798 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1418 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4145 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    55198 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/_types.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/_version.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/casing.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/importing.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/naming.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/grpclib_client.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/grpclib_server.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/util/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/util/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/util/async_channel.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/__main__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/compiler.py
--rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/main.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)    28742 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/models.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     8046 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/parser.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       18 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/config/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      833 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/config/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2742 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    14010 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    21357 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      860 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3979 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/detector/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2566 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6691 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    12120 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/eye_safety/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       18 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/eye_safety/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/eye_safety/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1066 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/eye_safety/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1392 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    21734 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/flow/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      701 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7115 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.497414 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1855 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3845 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/laser/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    12464 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3652 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    27189 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    11738 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    21372 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      757 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10548 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/push/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/push/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/push/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3198 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/push/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/push/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2330 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/push/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/push/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    15034 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/push/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/client/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/client/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2725 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/client/token_factory.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     5345 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1291 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    38039 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/secure/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/system/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/system/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/system/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    15151 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/system/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/system/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     8720 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/system/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/blickfeld_qb2/system/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    40554 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2/system/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-04 06:18:50.493414 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/PKG-INFO
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3703 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/SOURCES.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/dependency_links.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/requires.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/top_level.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2024-04-04 06:18:50.501414 blickfeld_qb2-2.0.7/setup.cfg
--rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2024-04-04 06:18:50.000000 blickfeld_qb2-2.0.7/setup.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2024-04-12 04:16:09.000000 blickfeld_qb2-2.0.9/LICENSE.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/PKG-INFO
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      493 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/base/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4464 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/base/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/base/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2253 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/base/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/base/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2411 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/base/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/base/geometry/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3394 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/base/geometry/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/base/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/base/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4319 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/base/grpc/channel.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/base/grpc/device_ca_cert.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      798 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1418 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4145 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    55198 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/_types.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/_version.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/casing.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/compile/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/compile/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/compile/importing.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/compile/naming.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/grpclib_client.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/grpclib_server.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/util/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/util/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/util/async_channel.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/google/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/google/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/google/protobuf/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/__main__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/compiler.py
+-rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/main.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    28742 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/models.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     8046 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/parser.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       18 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/config/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      833 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/config/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2742 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    14010 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    21357 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/detector/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/detector/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/detector/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      860 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/detector/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/detector/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3979 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/detector/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2566 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6691 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    12120 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/eye_safety/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       18 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/eye_safety/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/eye_safety/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1066 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/eye_safety/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/flow/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/flow/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/flow/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1392 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/flow/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/flow/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    21734 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/flow/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/hardware/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/hardware/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/hardware/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      701 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/hardware/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/hardware/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7115 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/hardware/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/laser/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/laser/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/laser/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1855 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/laser/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/laser/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3845 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/laser/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    12806 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3652 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    27189 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    11738 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    21372 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_toolkit/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_toolkit/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_toolkit/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      757 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_toolkit/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_toolkit/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10548 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/percept_toolkit/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/push/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/push/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/push/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3198 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/push/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/push/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2330 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/push/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/push/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    15034 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/push/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/client/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/client/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2725 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/client/token_factory.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     5345 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1291 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    38039 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/secure/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/system/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/system/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/system/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    15151 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/system/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/system/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     8720 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/system/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/blickfeld_qb2/system/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    40554 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2/system/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2024-04-12 04:16:14.541156 blickfeld_qb2-2.0.9/blickfeld_qb2.egg-info/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2.egg-info/PKG-INFO
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3703 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2.egg-info/SOURCES.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2.egg-info/dependency_links.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2.egg-info/requires.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/blickfeld_qb2.egg-info/top_level.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2024-04-12 04:16:14.545157 blickfeld_qb2-2.0.9/setup.cfg
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2024-04-12 04:16:14.000000 blickfeld_qb2-2.0.9/setup.py
```

### Comparing `blickfeld_qb2-2.0.7/LICENSE.txt` & `blickfeld_qb2-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/base/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/base/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import data
-from . import config
 from . import geometry
+from . import config
 
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # sources: blickfeld/base/options/access_control.proto, blickfeld/base/options/misc.proto, blickfeld/base/options/protocol_maturity.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import blickfeld_qb2.betterproto as betterproto
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/base/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/base/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/base/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/base/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/base/geometry/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/base/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/channel.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/base/grpc/channel.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/base/grpc/device_ca_cert.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/base/grpc/device_ca_cert.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/beam_deflection_control/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/beam_deflection_control/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/casing.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/casing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/compile/importing.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/compile/importing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/grpclib_client.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/grpclib_client.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/grpclib_server.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/grpclib_server.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/grpc/util/async_channel.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/grpc/util/async_channel.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/compiler.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/compiler.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/main.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/main.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/models.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/models.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/betterproto/plugin/parser.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/betterproto/plugin/parser.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/config/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/config/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/config/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,33 @@
     """
     Sort returns by range. This can improve the SNR for outdoor applications
     with rain and snow.
     """
 
 
 @dataclass(eq=False, repr=False)
+class Health(betterproto.Message):
+    """Configuration parameters for the health message"""
+
+    point_rate_lower_limit: int = betterproto.uint32_field(1)
+    """
+    Set the point rate lower limit. If the point rate is lower than this limit,
+    the device is considered to be covered.
+    """
+
+    point_cloud_alignment_deviation_norm_upper_limit: float = betterproto.float_field(2)
+    """The limit to detect the alignment has changed."""
+
+    point_cloud_reference_alignment: "_data__.Acceleration" = betterproto.message_field(
+        3
+    )
+    """Set the point cloud reference alignment."""
+
+
+@dataclass(eq=False, repr=False)
 class PointCloud(betterproto.Message):
     """Configuration parameters for the point cloud"""
 
     pass
 
 
 @dataclass(eq=False, repr=False)
@@ -63,26 +82,7 @@
     """
     Set lower threshold for reflectivity. This can be tuned to improve the SNR
     when low-reflectivity targets have a lower priority.
     """
 
     minimum_range: float = betterproto.float_field(5)
     """Set lower threshold for range. Default value is 1m."""
-
-
-@dataclass(eq=False, repr=False)
-class Health(betterproto.Message):
-    """Configuration parameters for the health message"""
-
-    point_rate_lower_limit: int = betterproto.uint32_field(1)
-    """
-    Set the point rate lower limit. If the point rate is lower than this limit,
-    the device is considered to be covered.
-    """
-
-    point_cloud_alignment_deviation_norm_upper_limit: float = betterproto.float_field(2)
-    """The limit to detect the alignment has changed."""
-
-    point_cloud_reference_alignment: "_data__.Acceleration" = betterproto.message_field(
-        3
-    )
-    """Set the point cloud reference alignment."""
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/data/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,28 @@
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 import numpy as np
 
 from ...base import data as __base_data__
 
 
 @dataclass(eq=False, repr=False)
+class Acceleration(betterproto.Message):
+    """A measurement of the Accelerometer"""
+
+    x: float = betterproto.float_field(1)
+    """X component of acceleration vector"""
+
+    y: float = betterproto.float_field(2)
+    """Y component of acceleration vector"""
+
+    z: float = betterproto.float_field(3)
+    """Z component of acceleration vector"""
+
+
+@dataclass(eq=False, repr=False)
 class Frame(betterproto.Message):
     """This section describes the contents of a point cloud frame."""
 
     id: int = betterproto.uint64_field(1)
     """Incremental frame ID since startup of the device."""
 
     timestamp: int = betterproto.uint64_field(2)
@@ -57,25 +71,28 @@
     """
 
     timestamp: np.ndarray = betterproto.bytes_field(6, numpy_dtype="<u8")
     """Unix timestamp of points. Type: UInt64"""
 
 
 @dataclass(eq=False, repr=False)
-class Acceleration(betterproto.Message):
-    """A measurement of the Accelerometer"""
+class AccelerationBuffer(betterproto.Message):
+    """Buffer for multiple Acceleration samples"""
 
-    x: float = betterproto.float_field(1)
-    """X component of acceleration vector"""
+    timestamp: int = betterproto.uint64_field(1)
+    """Timestamp of the first sample in the buffer."""
 
-    y: float = betterproto.float_field(2)
-    """Y component of acceleration vector"""
+    sampling_period: int = betterproto.uint64_field(2)
+    """Sampling period of the acceleration samples"""
 
-    z: float = betterproto.float_field(3)
-    """Z component of acceleration vector"""
+    cartesian: bytes = betterproto.bytes_field(3)
+    """
+    Cartesian 3-dimensional array in row-major format with [x, y, z] tuples.
+    Type: Float32
+    """
 
 
 @dataclass(eq=False, repr=False)
 class Health(betterproto.Message):
     """Message representing health"""
 
     state: "__base_data__.HealthState" = betterproto.enum_field(1)
@@ -405,24 +422,7 @@
     point_cloud_alignment_changed: bool = betterproto.bool_field(12)
     """
     The point cloud alignment deviates from the reference alignment. This might
     have an impact on the point cloud processing as e.g. the ground alignment
     got incorrect. If this is expected, the alignment can be reconfigured with
     the Health.SetConfig API method.
     """
-
-
-@dataclass(eq=False, repr=False)
-class AccelerationBuffer(betterproto.Message):
-    """Buffer for multiple Acceleration samples"""
-
-    timestamp: int = betterproto.uint64_field(1)
-    """Timestamp of the first sample in the buffer."""
-
-    sampling_period: int = betterproto.uint64_field(2)
-    """Sampling period of the acceleration samples"""
-
-    cartesian: bytes = betterproto.bytes_field(3)
-    """
-    Cartesian 3-dimensional array in row-major format with [x, y, z] tuples.
-    Type: Float32
-    """
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/core_processing/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/core_processing/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,62 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """Response to health get request"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """Stream response to health watch request"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthSetConfigRequest(betterproto.Message):
+    """Health set config request"""
+
+    config: "_config__.Health" = betterproto.message_field(1)
+    """Health parameters"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthGetConfigResponse(betterproto.Message):
+    """Health get config response"""
+
+    config: "_config__.Health" = betterproto.message_field(1)
+    """Health parameters"""
+
+
+@dataclass(eq=False, repr=False)
+class AccelerationStreamResponse(betterproto.Message):
+    """Stream response to acceleration stream request"""
+
+    buffer: "_data__.AccelerationBuffer" = betterproto.message_field(1)
+    """Buffer with acceleration"""
+
+
+@dataclass(eq=False, repr=False)
+class AccelerationGetFilteredResponse(betterproto.Message):
+    """Response to acceleration get filtered request"""
+
+    acceleration: "_data__.Acceleration" = betterproto.message_field(1)
+    """Single filtered acceleration"""
+
+
+@dataclass(eq=False, repr=False)
 class PointCloudStreamRequest(betterproto.Message):
     """Request for point cloud stream request"""
 
     pass
 
 
 @dataclass(eq=False, repr=False)
@@ -76,106 +124,92 @@
 
     filter: "_config__.PointCloudFilter" = betterproto.message_field(1)
     """
     Filter configuration which is currently applied on the point cloud frames.
     """
 
 
-@dataclass(eq=False, repr=False)
-class AccelerationStreamResponse(betterproto.Message):
-    """Stream response to acceleration stream request"""
-
-    buffer: "_data__.AccelerationBuffer" = betterproto.message_field(1)
-    """Buffer with acceleration"""
-
-
-@dataclass(eq=False, repr=False)
-class AccelerationGetFilteredResponse(betterproto.Message):
-    """Response to acceleration get filtered request"""
-
-    acceleration: "_data__.Acceleration" = betterproto.message_field(1)
-    """Single filtered acceleration"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Response to health get request"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """Stream response to health watch request"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthSetConfigRequest(betterproto.Message):
-    """Health set config request"""
-
-    config: "_config__.Health" = betterproto.message_field(1)
-    """Health parameters"""
+class Health(betterproto.ServiceStub):
+    """
+    The health service provides methods to monitor operational status of the
+    core_processing module
+    """
 
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the core_processing module"""
 
-@dataclass(eq=False, repr=False)
-class HealthGetConfigResponse(betterproto.Message):
-    """Health get config response"""
+        request = betterproto_lib_google_protobuf.Empty()
 
-    config: "_config__.Health" = betterproto.message_field(1)
-    """Health parameters"""
+        return await self._unary_unary(
+            "/blickfeld.core_processing.services.Health/Get",
+            request,
+            HealthGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the core_processing module"""
 
-class PointCloud(betterproto.ServiceStub):
-    """
-    Point Cloud service for core point cloud stream. It is the direct result of
-    the internal processing pipeline. The output is not post-processed further.
-    The post-processed output can be retrieved from the percept-processing
-    PointCloud service.
-    """
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
-    async def async_stream(
+    async def async_watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["PointCloudStreamResponse"]:
+    ) -> AsyncIterator["HealthWatchResponse"]:
         """
-        Stream a point cloud stream NOTE: This activates the sensor if it is
-        currently idle.
+        Can be used to attach to the health monitoring status information of
+        the core_processing module
         """
 
-        request = PointCloudStreamRequest()
+        request = betterproto_lib_google_protobuf.Empty()
 
         async for response in self._unary_stream(
-            "/blickfeld.core_processing.services.PointCloud/Stream",
+            "/blickfeld.core_processing.services.Health/Watch",
             request,
-            PointCloudStreamResponse,
+            HealthWatchResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
-    def stream(
+    def watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["PointCloudStreamResponse"]:
+    ) -> Iterator["HealthWatchResponse"]:
         """
-        Stream a point cloud stream NOTE: This activates the sensor if it is
-        currently idle.
+        Can be used to attach to the health monitoring status information of
+        the core_processing module
         """
 
         loop = asyncio.get_event_loop()
-        ait = self.async_stream(
+        ait = self.async_watch(
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
@@ -186,141 +220,192 @@
 
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
-    async def async_get(
+    async def async_set_config(
         self,
+        *,
+        config: "_config__.Health" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetResponse":
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
         """
-        Get a single point cloud NOTE: This activates the sensor if it is
-        currently idle.
+        Set the necessary parameters to generate the health message. It could
+        be calibration flag, limits, etc.
         """
 
-        request = PointCloudGetRequest()
+        request = HealthSetConfigRequest()
+        if config is not None:
+            request.config = config
 
         return await self._unary_unary(
-            "/blickfeld.core_processing.services.PointCloud/Get",
+            "/blickfeld.core_processing.services.Health/SetConfig",
             request,
-            PointCloudGetResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def set_config(
         self,
+        *,
+        config: "_config__.Health" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetResponse":
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
         """
-        Get a single point cloud NOTE: This activates the sensor if it is
-        currently idle.
+        Set the necessary parameters to generate the health message. It could
+        be calibration flag, limits, etc.
         """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_set_config(
+                config=config,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_set_filter(
+    async def async_get_config(
         self,
-        *,
-        filter: "_config__.PointCloudFilter" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set the filter configuration which is to be applied on the point cloud
-        data
-        """
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetConfigResponse":
+        """Get the health config"""
 
-        request = PointCloudSetFilterRequest()
-        if filter is not None:
-            request.filter = filter
+        request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.core_processing.services.PointCloud/SetFilter",
+            "/blickfeld.core_processing.services.Health/GetConfig",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            HealthGetConfigResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def set_filter(
+    def get_config(
         self,
-        *,
-        filter: "_config__.PointCloudFilter" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set the filter configuration which is to be applied on the point cloud
-        data
-        """
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetConfigResponse":
+        """Get the health config"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_set_filter(
-                filter=filter,
+            self.async_get_config(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_get_filter(
+
+class Acceleration(betterproto.ServiceStub):
+    """
+    The Acceleration Service provides access to the accelerometer of the
+    device.
+    """
+
+    async def async_stream(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetFilterResponse":
+    ) -> AsyncIterator["AccelerationStreamResponse"]:
         """
-        Get the filter configuration which is currently applied on the point
-        cloud data
+        Streams raw data from accelerometer [WARNING] Raw data is acquired with
+        a high sampling frequency and sent out in larger chunks. To estimate
+        the static state of the device the GetFiltered method should be used.
         """
 
         request = betterproto_lib_google_protobuf.Empty()
 
-        return await self._unary_unary(
-            "/blickfeld.core_processing.services.PointCloud/GetFilter",
+        async for response in self._unary_stream(
+            "/blickfeld.core_processing.services.Acceleration/Stream",
             request,
-            PointCloudGetFilterResponse,
+            AccelerationStreamResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        )
+        ):
+            yield response
 
-    def get_filter(
+    def stream(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "PointCloudGetFilterResponse":
+    ) -> Iterator["AccelerationStreamResponse"]:
         """
-        Get the filter configuration which is currently applied on the point
-        cloud data
+        Streams raw data from accelerometer [WARNING] Raw data is acquired with
+        a high sampling frequency and sent out in larger chunks. To estimate
+        the static state of the device the GetFiltered method should be used.
         """
 
         loop = asyncio.get_event_loop()
+        ait = self.async_stream(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+    async def async_get_filtered(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "AccelerationGetFilteredResponse":
+        """Get filtered sample from accelerometer"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.core_processing.services.Acceleration/GetFiltered",
+            request,
+            AccelerationGetFilteredResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get_filtered(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "AccelerationGetFilteredResponse":
+        """Get filtered sample from accelerometer"""
+
+        loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get_filter(
+            self.async_get_filtered(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
@@ -416,54 +501,54 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class Acceleration(betterproto.ServiceStub):
+class PointCloud(betterproto.ServiceStub):
     """
-    The Acceleration Service provides access to the accelerometer of the
-    device.
+    Point Cloud service for core point cloud stream. It is the direct result of
+    the internal processing pipeline. The output is not post-processed further.
+    The post-processed output can be retrieved from the percept-processing
+    PointCloud service.
     """
 
     async def async_stream(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["AccelerationStreamResponse"]:
+    ) -> AsyncIterator["PointCloudStreamResponse"]:
         """
-        Streams raw data from accelerometer [WARNING] Raw data is acquired with
-        a high sampling frequency and sent out in larger chunks. To estimate
-        the static state of the device the GetFiltered method should be used.
+        Stream a point cloud stream NOTE: This activates the sensor if it is
+        currently idle.
         """
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = PointCloudStreamRequest()
 
         async for response in self._unary_stream(
-            "/blickfeld.core_processing.services.Acceleration/Stream",
+            "/blickfeld.core_processing.services.PointCloud/Stream",
             request,
-            AccelerationStreamResponse,
+            PointCloudStreamResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def stream(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["AccelerationStreamResponse"]:
+    ) -> Iterator["PointCloudStreamResponse"]:
         """
-        Streams raw data from accelerometer [WARNING] Raw data is acquired with
-        a high sampling frequency and sent out in larger chunks. To estimate
-        the static state of the device the GetFiltered method should be used.
+        Stream a point cloud stream NOTE: This activates the sensor if it is
+        currently idle.
         """
 
         loop = asyncio.get_event_loop()
         ait = self.async_stream(
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
@@ -478,224 +563,139 @@
 
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
-    async def async_get_filtered(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "AccelerationGetFilteredResponse":
-        """Get filtered sample from accelerometer"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.core_processing.services.Acceleration/GetFiltered",
-            request,
-            AccelerationGetFilteredResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get_filtered(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "AccelerationGetFilteredResponse":
-        """Get filtered sample from accelerometer"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get_filtered(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
-class Health(betterproto.ServiceStub):
-    """
-    The health service provides methods to monitor operational status of the
-    core_processing module
-    """
-
     async def async_get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the core_processing module"""
+    ) -> "PointCloudGetResponse":
+        """
+        Get a single point cloud NOTE: This activates the sensor if it is
+        currently idle.
+        """
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = PointCloudGetRequest()
 
         return await self._unary_unary(
-            "/blickfeld.core_processing.services.Health/Get",
+            "/blickfeld.core_processing.services.PointCloud/Get",
             request,
-            HealthGetResponse,
+            PointCloudGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
     def get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the core_processing module"""
+    ) -> "PointCloudGetResponse":
+        """
+        Get a single point cloud NOTE: This activates the sensor if it is
+        currently idle.
+        """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
             self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """
-        Can be used to attach to the health monitoring status information of
-        the core_processing module
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.core_processing.services.Health/Watch",
-            request,
-            HealthWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """
-        Can be used to attach to the health monitoring status information of
-        the core_processing module
-        """
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-    async def async_set_config(
+    async def async_set_filter(
         self,
         *,
-        config: "_config__.Health" = None,
+        filter: "_config__.PointCloudFilter" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
         """
-        Set the necessary parameters to generate the health message. It could
-        be calibration flag, limits, etc.
+        Set the filter configuration which is to be applied on the point cloud
+        data
         """
 
-        request = HealthSetConfigRequest()
-        if config is not None:
-            request.config = config
+        request = PointCloudSetFilterRequest()
+        if filter is not None:
+            request.filter = filter
 
         return await self._unary_unary(
-            "/blickfeld.core_processing.services.Health/SetConfig",
+            "/blickfeld.core_processing.services.PointCloud/SetFilter",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def set_config(
+    def set_filter(
         self,
         *,
-        config: "_config__.Health" = None,
+        filter: "_config__.PointCloudFilter" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
         """
-        Set the necessary parameters to generate the health message. It could
-        be calibration flag, limits, etc.
+        Set the filter configuration which is to be applied on the point cloud
+        data
         """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_set_config(
-                config=config,
+            self.async_set_filter(
+                filter=filter,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_get_config(
+    async def async_get_filter(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetConfigResponse":
-        """Get the health config"""
+    ) -> "PointCloudGetFilterResponse":
+        """
+        Get the filter configuration which is currently applied on the point
+        cloud data
+        """
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.core_processing.services.Health/GetConfig",
+            "/blickfeld.core_processing.services.PointCloud/GetFilter",
             request,
-            HealthGetConfigResponse,
+            PointCloudGetFilterResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get_config(
+    def get_filter(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetConfigResponse":
-        """Get the health config"""
+    ) -> "PointCloudGetFilterResponse":
+        """
+        Get the filter configuration which is currently applied on the point
+        cloud data
+        """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get_config(
+            self.async_get_filter(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/detector/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/detector/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/detector/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/detector/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/diagnostics/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/diagnostics/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,30 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """Response to health get request."""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Aggregated health"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """Response to health watch request."""
+
+    health: "_data__.Health" = betterproto.message_field(2)
+    """Aggregated health"""
+
+
+@dataclass(eq=False, repr=False)
 class SelfTestRunRequest(betterproto.Message):
     """The self test run can be configured with this request"""
 
     self_tests: List["_config__.SelfTest"] = betterproto.enum_field(1)
     """
     Specify self tests which should be executed. If not set, the default set
     will be executed.
@@ -51,38 +67,14 @@
     """
 
     report: "_data__.SelfTestReport" = betterproto.message_field(1)
     """Test report"""
 
 
 @dataclass(eq=False, repr=False)
-class ReportGenerateResponse(betterproto.Message):
-    """Stream of the encrypted report in chunks of binary data."""
-
-    binary_chunk: bytes = betterproto.bytes_field(1)
-    """Binary chunk of the diagnostics report."""
-
-
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Response to health get request."""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Aggregated health"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """Response to health watch request."""
-
-    health: "_data__.Health" = betterproto.message_field(2)
-    """Aggregated health"""
-
-
-@dataclass(eq=False, repr=False)
 class LogStreamRequest(betterproto.Message):
     """Stream request"""
 
     cursor: "_data__.LogEntryCursor" = betterproto.message_field(1)
     """
     The cursor pointing to the log entry from which to start the stream from.
     This field is optional. If it is not set the stream will start from the
@@ -106,119 +98,20 @@
 class LogStreamResponse(betterproto.Message):
     """Stream response"""
 
     entry: "_data__.LogEntry" = betterproto.message_field(1)
     """The requested log entry."""
 
 
-class SelfTest(betterproto.ServiceStub):
-    """
-    The SelfTest service offers methods to trigger test routines. The routines
-    focus on automatic self tests without user interaction. The reports give an
-    indication what the potential root cause for an found issue could be.
-    """
-
-    async def async_run(
-        self,
-        *,
-        self_tests: Optional[List["_config__.SelfTest"]] = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "SelfTestRunResponse":
-        """This triggers the default test case routine"""
-
-        self_tests = self_tests or []
-
-        request = SelfTestRunRequest()
-        request.self_tests = self_tests
-
-        return await self._unary_unary(
-            "/blickfeld.diagnostics.services.SelfTest/Run",
-            request,
-            SelfTestRunResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def run(
-        self,
-        *,
-        self_tests: Optional[List["_config__.SelfTest"]] = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "SelfTestRunResponse":
-        """This triggers the default test case routine"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_run(
-                self_tests=self_tests,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
-class Report(betterproto.ServiceStub):
-    """
-    The Report service generates an encrypted diagnostics report containing
-    information about the state and health information of the Qb2 device.
-    """
-
-    async def async_generate(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["ReportGenerateResponse"]:
-        """Returns a stream of the report's binary chunks."""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.diagnostics.services.Report/Generate",
-            request,
-            ReportGenerateResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def generate(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["ReportGenerateResponse"]:
-        """Returns a stream of the report's binary chunks."""
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_generate(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
+@dataclass(eq=False, repr=False)
+class ReportGenerateResponse(betterproto.Message):
+    """Stream of the encrypted report in chunks of binary data."""
 
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
+    binary_chunk: bytes = betterproto.bytes_field(1)
+    """Binary chunk of the diagnostics report."""
 
 
 class Health(betterproto.ServiceStub):
     """
     This service provides the aggregated health state information of all Qb2
     software modules (only state and state reason are included). Service can be
     used to get an instant overview of the overall Qb2 device health.
@@ -313,14 +206,66 @@
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
 
+class SelfTest(betterproto.ServiceStub):
+    """
+    The SelfTest service offers methods to trigger test routines. The routines
+    focus on automatic self tests without user interaction. The reports give an
+    indication what the potential root cause for an found issue could be.
+    """
+
+    async def async_run(
+        self,
+        *,
+        self_tests: Optional[List["_config__.SelfTest"]] = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "SelfTestRunResponse":
+        """This triggers the default test case routine"""
+
+        self_tests = self_tests or []
+
+        request = SelfTestRunRequest()
+        request.self_tests = self_tests
+
+        return await self._unary_unary(
+            "/blickfeld.diagnostics.services.SelfTest/Run",
+            request,
+            SelfTestRunResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def run(
+        self,
+        *,
+        self_tests: Optional[List["_config__.SelfTest"]] = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "SelfTestRunResponse":
+        """This triggers the default test case routine"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_run(
+                self_tests=self_tests,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+
 class Log(betterproto.ServiceStub):
     """
     The Log service provides methods to access the logs of selected software
     modules running on the device. Via this service, the client is able to
     monitor events that happen on the device during operation. This allows to
     asses the state of the device or to have additional information if the
     sensor is in a failed state.
@@ -374,14 +319,69 @@
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+
+class Report(betterproto.ServiceStub):
+    """
+    The Report service generates an encrypted diagnostics report containing
+    information about the state and health information of the Qb2 device.
+    """
+
+    async def async_generate(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["ReportGenerateResponse"]:
+        """Returns a stream of the report's binary chunks."""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.diagnostics.services.Report/Generate",
+            request,
+            ReportGenerateResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def generate(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["ReportGenerateResponse"]:
+        """Returns a stream of the report's binary chunks."""
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_generate(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
                 obj = await ait.__anext__()
                 return False, obj
             except StopAsyncIteration:
                 return True, None
 
         while True:
             done, obj = loop.run_until_complete(get_next())
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/eye_safety/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/eye_safety/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/flow/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/flow/config/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,14 @@
 from typing import List
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 
 @dataclass(eq=False, repr=False)
-class NodeRedJson(betterproto.Message):
-    """Simple container for the node red import / export format"""
-
-    nodes: List["betterproto_lib_google_protobuf.Struct"] = betterproto.message_field(1)
-    """List of JSON nodes"""
-
-
-@dataclass(eq=False, repr=False)
 class Flow(betterproto.Message):
     """
     Blickfeld Flow configuration This container is used to control high-level
     attributes of NodeRed flows.
     """
 
     name: str = betterproto.string_field(1)
@@ -38,7 +30,15 @@
     """Is it a subflow?"""
 
     metadata: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(5)
     """Other arbitrary metadata"""
 
     nodes: List["betterproto_lib_google_protobuf.Struct"] = betterproto.message_field(6)
     """All nodes contained in the flow"""
+
+
+@dataclass(eq=False, repr=False)
+class NodeRedJson(betterproto.Message):
+    """Simple container for the node red import / export format"""
+
+    nodes: List["betterproto_lib_google_protobuf.Struct"] = betterproto.message_field(1)
+    """List of JSON nodes"""
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/flow/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/flow/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,33 +45,14 @@
     """Settings get request"""
 
     settings: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
     """Current settings Generic JSON format which is defined by NodeRed."""
 
 
 @dataclass(eq=False, repr=False)
-class CredentialsSetRequest(betterproto.Message):
-    """Credentials set request"""
-
-    credentials: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
-    """
-    Credentials which should be stored Generic JSON format which is defined by
-    NodeRed.
-    """
-
-
-@dataclass(eq=False, repr=False)
-class CredentialsGetResponse(betterproto.Message):
-    """Credentails get response"""
-
-    credentials: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
-    """Current credentials Generic JSON format which is defined by NodeRed."""
-
-
-@dataclass(eq=False, repr=False)
 class FlowGetRequest(betterproto.Message):
     """Flow get request"""
 
     id: str = betterproto.string_field(1)
     """Flow id"""
 
     as_node_red_json: bool = betterproto.bool_field(2)
@@ -177,14 +158,33 @@
 class FlowWatchGlobalNodesResponse(betterproto.Message):
     """Flow watch global nodes response"""
 
     node_red_json: "_config__.NodeRedJson" = betterproto.message_field(1)
     """NodeRed JSON format of all global configuration nodes"""
 
 
+@dataclass(eq=False, repr=False)
+class CredentialsSetRequest(betterproto.Message):
+    """Credentials set request"""
+
+    credentials: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
+    """
+    Credentials which should be stored Generic JSON format which is defined by
+    NodeRed.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class CredentialsGetResponse(betterproto.Message):
+    """Credentails get response"""
+
+    credentials: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(1)
+    """Current credentials Generic JSON format which is defined by NodeRed."""
+
+
 class Settings(betterproto.ServiceStub):
     """
     Configuration service to store the NodeRed Settings. It is used to
     implement the custom storage API: https://nodered.org/docs/api/storage/
     """
 
     async def async_set(
@@ -275,112 +275,14 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class Credentials(betterproto.ServiceStub):
-    """
-    Service to store the NodeRed credentials. It is used to implement the
-    custom storage API: https://nodered.org/docs/api/storage/
-    """
-
-    async def async_set(
-        self,
-        *,
-        credentials: "betterproto_lib_google_protobuf.Struct" = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set credentials Used by https://nodered.org/docs/api/storage/methods/#s
-        toragesavecredentialscredentials
-        """
-
-        request = CredentialsSetRequest()
-        if credentials is not None:
-            request.credentials = credentials
-
-        return await self._unary_unary(
-            "/blickfeld.flow.services.Credentials/Set",
-            request,
-            betterproto_lib_google_protobuf.Empty,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def set(
-        self,
-        *,
-        credentials: "betterproto_lib_google_protobuf.Struct" = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Set credentials Used by https://nodered.org/docs/api/storage/methods/#s
-        toragesavecredentialscredentials
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_set(
-                credentials=credentials,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "CredentialsGetResponse":
-        """
-        Get credentials Used by
-        https://nodered.org/docs/api/storage/methods/#storagegetcredentials
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.flow.services.Credentials/Get",
-            request,
-            CredentialsGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "CredentialsGetResponse":
-        """
-        Get credentials Used by
-        https://nodered.org/docs/api/storage/methods/#storagegetcredentials
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
 class Flow(betterproto.ServiceStub):
     """
     Service to store and control Blickfeld flows. It is used to implement the
     custom storage API: https://nodered.org/docs/api/storage/
     """
 
     async def async_get(
@@ -723,7 +625,105 @@
         return loop.run_until_complete(
             self.async_watch_global_nodes(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
+
+
+class Credentials(betterproto.ServiceStub):
+    """
+    Service to store the NodeRed credentials. It is used to implement the
+    custom storage API: https://nodered.org/docs/api/storage/
+    """
+
+    async def async_set(
+        self,
+        *,
+        credentials: "betterproto_lib_google_protobuf.Struct" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Set credentials Used by https://nodered.org/docs/api/storage/methods/#s
+        toragesavecredentialscredentials
+        """
+
+        request = CredentialsSetRequest()
+        if credentials is not None:
+            request.credentials = credentials
+
+        return await self._unary_unary(
+            "/blickfeld.flow.services.Credentials/Set",
+            request,
+            betterproto_lib_google_protobuf.Empty,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def set(
+        self,
+        *,
+        credentials: "betterproto_lib_google_protobuf.Struct" = None,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Set credentials Used by https://nodered.org/docs/api/storage/methods/#s
+        toragesavecredentialscredentials
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_set(
+                credentials=credentials,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "CredentialsGetResponse":
+        """
+        Get credentials Used by
+        https://nodered.org/docs/api/storage/methods/#storagegetcredentials
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.flow.services.Credentials/Get",
+            request,
+            CredentialsGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "CredentialsGetResponse":
+        """
+        Get credentials Used by
+        https://nodered.org/docs/api/storage/methods/#storagegetcredentials
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/hardware/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/hardware/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/hardware/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -29,191 +29,191 @@
 class IdentificationGetResponse(betterproto.Message):
     """Response message for the identification get command"""
 
     identification: "_config__.Identification" = betterproto.message_field(1)
     """The current identification"""
 
 
-class DeviceOperation(betterproto.ServiceStub):
+class Identification(betterproto.ServiceStub):
     """
-    This service is used for starting and stopping the device operation.
-    Normally, the device is started and stopped based on the client
-    connections. If there is a client using the Qb2, the device will start and
-    stay in operation until all clients disconnected. The start function of
-    this service overrides this behaviour, i.e. when started using the start
-    function the device will stay operational even though no clients are
-    connected. This allows a faster retrieval of frames once a client connects
-    as the startup phase is skipped.
+    The identification service provides methods to set and read out
+    identification data of the Qb2 device.
     """
 
-    async def async_start(
+    async def async_get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Method to start the device operation. This starts the operation ot the
-        deflection mirrors and the laser triggering. When this call is used,
-        the device will stay in operation until stop is called (independent//
-        of clients being connected or not).
-        """
+    ) -> "IdentificationGetResponse":
+        """Gets identification configuration"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.hardware.services.DeviceOperation/Start",
+            "/blickfeld.hardware.services.Identification/Get",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            IdentificationGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def start(
+    def get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Method to start the device operation. This starts the operation ot the
-        deflection mirrors and the laser triggering. When this call is used,
-        the device will stay in operation until stop is called (independent//
-        of clients being connected or not).
-        """
+    ) -> "IdentificationGetResponse":
+        """Gets identification configuration"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_start(
+            self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_stop(
+
+class ComputeModule(betterproto.ServiceStub):
+    """
+    This service is used to control & observe the state of the compute module.
+    """
+
+    async def async_reboot(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Method to stop the device operation. This will stop the deflection
-        mirror operation and laser triggering.
-        """
+        """Reboots the CM4"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.hardware.services.DeviceOperation/Stop",
+            "/blickfeld.hardware.services.ComputeModule/Reboot",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def stop(
+    def reboot(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Method to stop the device operation. This will stop the deflection
-        mirror operation and laser triggering.
-        """
+        """Reboots the CM4"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_stop(
+            self.async_reboot(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class ComputeModule(betterproto.ServiceStub):
+class DeviceOperation(betterproto.ServiceStub):
     """
-    This service is used to control & observe the state of the compute module.
+    This service is used for starting and stopping the device operation.
+    Normally, the device is started and stopped based on the client
+    connections. If there is a client using the Qb2, the device will start and
+    stay in operation until all clients disconnected. The start function of
+    this service overrides this behaviour, i.e. when started using the start
+    function the device will stay operational even though no clients are
+    connected. This allows a faster retrieval of frames once a client connects
+    as the startup phase is skipped.
     """
 
-    async def async_reboot(
+    async def async_start(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Reboots the CM4"""
+        """
+        Method to start the device operation. This starts the operation ot the
+        deflection mirrors and the laser triggering. When this call is used,
+        the device will stay in operation until stop is called (independent//
+        of clients being connected or not).
+        """
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.hardware.services.ComputeModule/Reboot",
+            "/blickfeld.hardware.services.DeviceOperation/Start",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def reboot(
+    def start(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Reboots the CM4"""
+        """
+        Method to start the device operation. This starts the operation ot the
+        deflection mirrors and the laser triggering. When this call is used,
+        the device will stay in operation until stop is called (independent//
+        of clients being connected or not).
+        """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_reboot(
+            self.async_start(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-
-class Identification(betterproto.ServiceStub):
-    """
-    The identification service provides methods to set and read out
-    identification data of the Qb2 device.
-    """
-
-    async def async_get(
+    async def async_stop(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "IdentificationGetResponse":
-        """Gets identification configuration"""
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Method to stop the device operation. This will stop the deflection
+        mirror operation and laser triggering.
+        """
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.hardware.services.Identification/Get",
+            "/blickfeld.hardware.services.DeviceOperation/Stop",
             request,
-            IdentificationGetResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def stop(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "IdentificationGetResponse":
-        """Gets identification configuration"""
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Method to stop the device operation. This will stop the deflection
+        mirror operation and laser triggering.
+        """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_stop(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/laser/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/laser/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/laser/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/laser/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,137 +28,28 @@
     """Medium object size: free standing human, single human, etc"""
 
     OBJECT_SIZE_LARGE = 3
     """Large object size: cars, group of people, large animals, etc"""
 
 
 @dataclass(eq=False, repr=False)
-class PointCloudFilter(betterproto.Message):
-    """Algorithm for filtering point clouds"""
-
-    radius_outlier: "PointCloudFilterRadiusOutlier" = betterproto.message_field(
-        1, group="point_cloud_filter_type"
-    )
-    """Use radius outlier filter for noise reduction on point clouds"""
-
-
-@dataclass(eq=False, repr=False)
-class PointCloudFilterRadiusOutlier(betterproto.Message):
-    """Filter points based on the number of neighbors in a certain radius"""
-
-    min_neighbor_points: int = betterproto.uint32_field(1)
-    """Minimum number of neighbors a point has to have to be retained"""
-
-    neighbor_radius: float = betterproto.double_field(2)
-    """All points within this radius are considered neighbors of a point"""
-
-
-@dataclass(eq=False, repr=False)
-class DataSource(betterproto.Message):
-    """
-    The configuration storing the sources to retrieve the point cloud data for
-    further processing.
-    """
-
-    qb2_setup: "DataSourceQb2Setup" = betterproto.message_field(
-        3, group="data_source_type"
-    )
-    """Use Qb2 lidars to retrieve point clouds"""
-
-    geolocation_of_map: "__base_config__.Geolocation" = betterproto.message_field(4)
-    """
-    Geolocation of data source. This references the map coordinate system of
-    this data source to the world. Individual lidars are referenced to the map
-    coordinate system via their `map_from_lidar` transform. [NOTE] If the
-    map_from_lidar transform is not an identity transformation, this is not the
-    geolocation of an individual sensor.
-    """
-
-
-@dataclass(eq=False, repr=False)
-class DataSourceQb2(betterproto.Message):
-    """Configuration for retrieving point clouds from a Qb2"""
-
-    fqdn: str = betterproto.string_field(1)
-    """
-    The fully qualified domain name of the Qb2 device. For on-device
-    processing/configuration, 'fqdn' can be set to an empty string to request
-    the data of the current device.
-    """
-
-    map_from_lidar: "__base_geometry__.Transform" = betterproto.message_field(2)
-    """
-    Transformation from the lidar frame to the map frame. If this transform is
-    not set, this will be interpreted as identify transformation. Transforming
-    all point cloud topics into the map frame results in a globally consistent
-    combined point cloud in map frame.
-    """
-
-    application_key: str = betterproto.string_field(3)
-    """
-    Application key with authorized access level. Required if user-management
-    is enabled on externally connected devices.
-    """
-
-    serial_number: str = betterproto.string_field(4)
-    """
-    Serial number. Required if user-management is enabled on externally
-    connected devices.
-    """
-
-    metadata: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(100)
-    """Arbitrary metadata storage for client applications"""
-
-
-@dataclass(eq=False, repr=False)
-class DataSourceTrigger(betterproto.Message):
-    """
-    Configuration of Trigger Mode. In trigger mode the processing pipeline will
-    reduce the frequency at which point clouds and state lists are getting
-    computed to reduce the amount of data transmitted between the processing
-    device and configured 'lidars'.
-    """
-
-    frequency: float = betterproto.float_field(1)
-    """
-    The frequency at which data is getting requested from the lidars and
-    outputs are generated.
-    """
-
-
-@dataclass(eq=False, repr=False)
-class DataSourceQb2Setup(betterproto.Message):
-    """The configuration of a Qb2 setup of the LiDAR devices"""
-
-    lidars: List["DataSourceQb2"] = betterproto.message_field(1)
-    """the qb2 lidars to get the point clouds from"""
-
-    trigger: "DataSourceTrigger" = betterproto.message_field(2)
-    """
-    If the field is set trigger mode is enabled. If the field is not set, the
-    pipeline outputs are computed with the frequency of configured lidars, i.e.
-    the scan pattern configured on those.
-    """
-
-
-@dataclass(eq=False, repr=False)
 class BackgroundSubtraction(betterproto.Message):
     """
     Algorithms seperating the input point cloud into foreground and background.
     """
 
     mixture_of_gaussians: "BackgroundSubtractionMixtureOfGaussians" = (
         betterproto.message_field(1, group="background_subtraction_type")
     )
     """Use mixture of gaussians for foreground/background detection"""
 
-    octree: "BackgroundSubtractionOctree" = betterproto.message_field(
+    static: "BackgroundSubtractionStatic" = betterproto.message_field(
         3, group="background_subtraction_type"
     )
-    """Use a static octree for foreground/background detection."""
+    """Use a static tree structure for foreground/background detection."""
 
 
 @dataclass(eq=False, repr=False)
 class BackgroundSubtractionMixtureOfGaussians(betterproto.Message):
     """
     Dynamic background subtraction using a mixture of gaussians. The algorithm
     automatically slowly updates the background model if the scene changes. The
@@ -181,29 +72,41 @@
     """
     Controls how much noise the background/foreground is expected to have.
     Reasonable default: 0.25
     """
 
 
 @dataclass(eq=False, repr=False)
-class BackgroundSubtractionOctree(betterproto.Message):
+class BackgroundSubtractionStatic(betterproto.Message):
     """
     Uses the first received frames to build a static background map of the
     environment. The algorithm requires the scene to only contain the static
     parts of the scene on the start of the processing. The background model is
     not updated automatically afterwards. The ResetBackground grpc method
     allows to update the static map of the environment.
     """
 
     num_initialization_frames: int = betterproto.uint32_field(1)
     """
     How many frames of the first received frames are used to build the
     background Reasonable default: 10
     """
 
+    voxel_size: float = betterproto.float_field(3)
+    """
+    Size of voxels used for voxelization of the background during
+    initialization. Default: 0.05 m
+    """
+
+    min_distance: float = betterproto.float_field(4)
+    """
+    Minimum spatial distance to background to detect points as foreground
+    Default: 0.15 m
+    """
+
 
 @dataclass(eq=False, repr=False)
 class Clustering(betterproto.Message):
     """
     Algorithms for detecting objects as clustered points in the foreground
     scene.
     """
@@ -236,14 +139,35 @@
     Multiply the given radius with the range of a point and add it to the
     radius. This significantly improves the clustering for close-range scenes.
     Reasonable default: 0.025
     """
 
 
 @dataclass(eq=False, repr=False)
+class PointCloudFilter(betterproto.Message):
+    """Algorithm for filtering point clouds"""
+
+    radius_outlier: "PointCloudFilterRadiusOutlier" = betterproto.message_field(
+        1, group="point_cloud_filter_type"
+    )
+    """Use radius outlier filter for noise reduction on point clouds"""
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudFilterRadiusOutlier(betterproto.Message):
+    """Filter points based on the number of neighbors in a certain radius"""
+
+    min_neighbor_points: int = betterproto.uint32_field(1)
+    """Minimum number of neighbors a point has to have to be retained"""
+
+    neighbor_radius: float = betterproto.double_field(2)
+    """All points within this radius are considered neighbors of a point"""
+
+
+@dataclass(eq=False, repr=False)
 class Perception(betterproto.Message):
     """
     The configuration of perception algorithms used to run e.g. security zones
     """
 
     background_subtraction: "BackgroundSubtraction" = betterproto.message_field(1)
     """Extract the foreground point cloud of the scene"""
@@ -355,7 +279,95 @@
 
 
 @dataclass(eq=False, repr=False)
 class ZoneAlgorithmExclusion(betterproto.Message):
     """Algorithm that excludes points from the input point cloud"""
 
     pass
+
+
+@dataclass(eq=False, repr=False)
+class DataSource(betterproto.Message):
+    """
+    The configuration storing the sources to retrieve the point cloud data for
+    further processing.
+    """
+
+    qb2_setup: "DataSourceQb2Setup" = betterproto.message_field(
+        3, group="data_source_type"
+    )
+    """Use Qb2 lidars to retrieve point clouds"""
+
+    geolocation_of_map: "__base_config__.Geolocation" = betterproto.message_field(4)
+    """
+    Geolocation of data source. This references the map coordinate system of
+    this data source to the world. Individual lidars are referenced to the map
+    coordinate system via their `map_from_lidar` transform. [NOTE] If the
+    map_from_lidar transform is not an identity transformation, this is not the
+    geolocation of an individual sensor.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class DataSourceQb2(betterproto.Message):
+    """Configuration for retrieving point clouds from a Qb2"""
+
+    fqdn: str = betterproto.string_field(1)
+    """
+    The fully qualified domain name of the Qb2 device. For on-device
+    processing/configuration, 'fqdn' can be set to an empty string to request
+    the data of the current device.
+    """
+
+    map_from_lidar: "__base_geometry__.Transform" = betterproto.message_field(2)
+    """
+    Transformation from the lidar frame to the map frame. If this transform is
+    not set, this will be interpreted as identify transformation. Transforming
+    all point cloud topics into the map frame results in a globally consistent
+    combined point cloud in map frame.
+    """
+
+    application_key: str = betterproto.string_field(3)
+    """
+    Application key with authorized access level. Required if user-management
+    is enabled on externally connected devices.
+    """
+
+    serial_number: str = betterproto.string_field(4)
+    """
+    Serial number. Required if user-management is enabled on externally
+    connected devices.
+    """
+
+    metadata: "betterproto_lib_google_protobuf.Struct" = betterproto.message_field(100)
+    """Arbitrary metadata storage for client applications"""
+
+
+@dataclass(eq=False, repr=False)
+class DataSourceTrigger(betterproto.Message):
+    """
+    Configuration of Trigger Mode. In trigger mode the processing pipeline will
+    reduce the frequency at which point clouds and state lists are getting
+    computed to reduce the amount of data transmitted between the processing
+    device and configured 'lidars'.
+    """
+
+    frequency: float = betterproto.float_field(1)
+    """
+    The frequency at which data is getting requested from the lidars and
+    outputs are generated.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class DataSourceQb2Setup(betterproto.Message):
+    """The configuration of a Qb2 setup of the LiDAR devices"""
+
+    lidars: List["DataSourceQb2"] = betterproto.message_field(1)
+    """the qb2 lidars to get the point clouds from"""
+
+    trigger: "DataSourceTrigger" = betterproto.message_field(2)
+    """
+    If the field is set trigger mode is enabled. If the field is not set, the
+    pipeline outputs are computed with the frequency of configured lidars, i.e.
+    the scan pattern configured on those.
+    """
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/data/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,54 +7,14 @@
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 from ...base import data as __base_data__
 
 
-class PointCloudType(betterproto.Enum):
-    """The type of the point cloud"""
-
-    POINT_CLOUD_TYPE_UNSPECIFIED = 0
-    """The zero value that is not accepted"""
-
-    POINT_CLOUD_TYPE_FULL = 1
-    """
-    Full point cloud (combined point cloud of all devices or unfiltered point
-    cloud coming from one device)
-    """
-
-    POINT_CLOUD_TYPE_FOREGROUND = 2
-    """Point cloud containing only foreground/points from moving objects"""
-
-    POINT_CLOUD_TYPE_FULL_OPTIMIZED = 3
-    """
-    Same as 'POINT_CLOUD_TYPE_FULL' but with reduced point cloud density to
-    reduce the size of the point cloud
-    """
-
-    POINT_CLOUD_TYPE_FILTERED = 4
-    """
-    Same as 'POINT_CLOUD_TYPE_FULL' but with all points excluded that are in
-    exclusion zones
-    """
-
-    POINT_CLOUD_TYPE_FILTERED_FOREGROUND = 5
-    """
-    Same as 'POINT_CLOUD_TYPE_FOREGROUND' but with all points excluded that are
-    in exclusion zones
-    """
-
-    POINT_CLOUD_TYPE_BACKGROUND = 6
-    """
-    Point cloud containing the points representing the background model/point
-    cloud
-    """
-
-
 class State(betterproto.Enum):
     """The states of pipeline"""
 
     STATE_UNSPECIFIED = 0
     """State field is not set"""
 
     STATE_STARTING = 1
@@ -103,14 +63,54 @@
     The data is expressed in the coordiante system of the data-source/device
     """
 
     COORDINATE_SYSTEM_TRANSFORMED = 2
     """The data is expressed in a map coordinate system"""
 
 
+class PointCloudType(betterproto.Enum):
+    """The type of the point cloud"""
+
+    POINT_CLOUD_TYPE_UNSPECIFIED = 0
+    """The zero value that is not accepted"""
+
+    POINT_CLOUD_TYPE_FULL = 1
+    """
+    Full point cloud (combined point cloud of all devices or unfiltered point
+    cloud coming from one device)
+    """
+
+    POINT_CLOUD_TYPE_FOREGROUND = 2
+    """Point cloud containing only foreground/points from moving objects"""
+
+    POINT_CLOUD_TYPE_FULL_OPTIMIZED = 3
+    """
+    Same as 'POINT_CLOUD_TYPE_FULL' but with reduced point cloud density to
+    reduce the size of the point cloud
+    """
+
+    POINT_CLOUD_TYPE_FILTERED = 4
+    """
+    Same as 'POINT_CLOUD_TYPE_FULL' but with all points excluded that are in
+    exclusion zones
+    """
+
+    POINT_CLOUD_TYPE_FILTERED_FOREGROUND = 5
+    """
+    Same as 'POINT_CLOUD_TYPE_FOREGROUND' but with all points excluded that are
+    in exclusion zones
+    """
+
+    POINT_CLOUD_TYPE_BACKGROUND = 6
+    """
+    Point cloud containing the points representing the background model/point
+    cloud
+    """
+
+
 @dataclass(eq=False, repr=False)
 class Health(betterproto.Message):
     """
     A health message that contains information about the pipeline status and
     the module itself.
     """
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_pipeline/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/percept_pipeline/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,87 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """Stream response containing health of the module"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """The module health"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """Get response containing health of the module"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """The module health"""
+
+
+@dataclass(eq=False, repr=False)
+class PerceptionGetResponse(betterproto.Message):
+    """Response containing the current perception configuration"""
+
+    perception: "_config__.Perception" = betterproto.message_field(1)
+    """The current perception configuration"""
+
+
+@dataclass(eq=False, repr=False)
+class PerceptionSetRequest(betterproto.Message):
+    """Request for setting the perception configuration"""
+
+    template_name: str = betterproto.string_field(1, group="set_type")
+    """
+    Use a template to set the configuration, templates are predefined
+    perception configurations
+    """
+
+    perception: "_config__.Perception" = betterproto.message_field(2, group="set_type")
+    """Use the specified configuration"""
+
+
+@dataclass(eq=False, repr=False)
+class PerceptionWatchResponse(betterproto.Message):
+    """Continuous response on perception configuration changes"""
+
+    perception: "_config__.Perception" = betterproto.message_field(1)
+    """The current set perception configuration"""
+
+
+@dataclass(eq=False, repr=False)
+class PerceptionListTemplatesResponse(betterproto.Message):
+    """Response containing perception configuration templates"""
+
+    named_templates: Dict[str, "_config__.Perception"] = betterproto.map_field(
+        1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
+    )
+    """
+    Mapping from a template name to the template itself. The template can be
+    used to configure the perception algorithms for certain use-cases.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class PerceptionResetBackgroundRequest(betterproto.Message):
+    """
+    Request to reset the background model of one, multiple or all devices
+    """
+
+    fqdns: List[str] = betterproto.string_field(1)
+    """
+    If the list is empty, the background models of all data sources are reset.
+    If the background models of only specific devices should be rebuilt, the
+    'fqdn' of the respective devices has to be mentioned in the 'fqdns' list.
+    """
+
+
+@dataclass(eq=False, repr=False)
 class ZoneListResponse(betterproto.Message):
     """Response containing the configured list of zones"""
 
     zones: List["_config__.ZoneAlgorithm"] = betterproto.message_field(1)
     """The currently configured zones"""
 
 
@@ -107,241 +180,225 @@
 class DataSourceWatchResponse(betterproto.Message):
     """Continuous response on data source changes"""
 
     data_source: "_config__.DataSource" = betterproto.message_field(1)
     """The currently set data source"""
 
 
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """Stream response containing health of the module"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """The module health"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Get response containing health of the module"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """The module health"""
-
-
-@dataclass(eq=False, repr=False)
-class PerceptionGetResponse(betterproto.Message):
-    """Response containing the current perception configuration"""
-
-    perception: "_config__.Perception" = betterproto.message_field(1)
-    """The current perception configuration"""
-
-
-@dataclass(eq=False, repr=False)
-class PerceptionSetRequest(betterproto.Message):
-    """Request for setting the perception configuration"""
-
-    template_name: str = betterproto.string_field(1, group="set_type")
-    """
-    Use a template to set the configuration, templates are predefined
-    perception configurations
-    """
-
-    perception: "_config__.Perception" = betterproto.message_field(2, group="set_type")
-    """Use the specified configuration"""
-
-
-@dataclass(eq=False, repr=False)
-class PerceptionWatchResponse(betterproto.Message):
-    """Continuous response on perception configuration changes"""
-
-    perception: "_config__.Perception" = betterproto.message_field(1)
-    """The current set perception configuration"""
-
+class Health(betterproto.ServiceStub):
+    """Reports the health of the pipeline module."""
 
-@dataclass(eq=False, repr=False)
-class PerceptionListTemplatesResponse(betterproto.Message):
-    """Response containing perception configuration templates"""
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["HealthWatchResponse"]:
+        """
+        Streams health information on a regular cadence or if certain incidents
+        happen
+        """
 
-    named_templates: Dict[str, "_config__.Perception"] = betterproto.map_field(
-        1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
-    )
-    """
-    Mapping from a template name to the template itself. The template can be
-    used to configure the perception algorithms for certain use-cases.
-    """
+        request = betterproto_lib_google_protobuf.Empty()
 
+        async for response in self._unary_stream(
+            "/blickfeld.percept_pipeline.services.Health/Watch",
+            request,
+            HealthWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
 
-@dataclass(eq=False, repr=False)
-class PerceptionResetBackgroundRequest(betterproto.Message):
-    """
-    Request to reset the background model of one, multiple or all devices
-    """
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["HealthWatchResponse"]:
+        """
+        Streams health information on a regular cadence or if certain incidents
+        happen
+        """
 
-    fqdns: List[str] = betterproto.string_field(1)
-    """
-    If the list is empty, the background models of all data sources are reset.
-    If the background models of only specific devices should be rebuilt, the
-    'fqdn' of the respective devices has to be mentioned in the 'fqdns' list.
-    """
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
 
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
 
-class Zone(betterproto.ServiceStub):
-    """
-    The zone service allows getting, configuring, deleting and receiving
-    updates of the configured zones.
-    """
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
 
-    async def async_list(
+    async def async_get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "ZoneListResponse":
-        """Returns the configured zones"""
+    ) -> "HealthGetResponse":
+        """Returns the current health information"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Zone/List",
+            "/blickfeld.percept_pipeline.services.Health/Get",
             request,
-            ZoneListResponse,
+            HealthGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def list(
+    def get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "ZoneListResponse":
-        """Returns the configured zones"""
+    ) -> "HealthGetResponse":
+        """Returns the current health information"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_list(
+            self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_store(
+
+class Perception(betterproto.ServiceStub):
+    """
+    The perception service allows getting, configuring and receiving updates of
+    the perception configurations. Perception configurations specify the
+    algorithms used for e.g. for background subtraction etc.
+    """
+
+    async def async_get(
         self,
-        *,
-        zone: "_config__.ZoneAlgorithm" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Store / Update a zone"""
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PerceptionGetResponse":
+        """Get current perception configuration"""
 
-        request = ZoneStoreRequest()
-        if zone is not None:
-            request.zone = zone
+        request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Zone/Store",
+            "/blickfeld.percept_pipeline.services.Perception/Get",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            PerceptionGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def store(
+    def get(
         self,
-        *,
-        zone: "_config__.ZoneAlgorithm" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Store / Update a zone"""
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PerceptionGetResponse":
+        """Get current perception configuration"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_store(
-                zone=zone,
+            self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_delete(
+    async def async_set(
         self,
         *,
-        uuid: str = "",
+        template_name: str = "",
+        perception: "_config__.Perception" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Delete a zone"""
+        """Set the perception configuration"""
 
-        request = ZoneDeleteRequest()
-        request.uuid = uuid
+        request = PerceptionSetRequest()
+        request.template_name = template_name
+        if perception is not None:
+            request.perception = perception
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Zone/Delete",
+            "/blickfeld.percept_pipeline.services.Perception/Set",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def delete(
+    def set(
         self,
         *,
-        uuid: str = "",
+        template_name: str = "",
+        perception: "_config__.Perception" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Delete a zone"""
+        """Set the perception configuration"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_delete(
-                uuid=uuid,
+            self.async_set(
+                template_name=template_name,
+                perception=perception,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
     async def async_watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["ZoneWatchResponse"]:
-        """Watch configuration for zone list"""
+    ) -> AsyncIterator["PerceptionWatchResponse"]:
+        """Watch changes of perception configuration"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         async for response in self._unary_stream(
-            "/blickfeld.percept_pipeline.services.Zone/Watch",
+            "/blickfeld.percept_pipeline.services.Perception/Watch",
             request,
-            ZoneWatchResponse,
+            PerceptionWatchResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["ZoneWatchResponse"]:
-        """Watch configuration for zone list"""
+    ) -> Iterator["PerceptionWatchResponse"]:
+        """Watch changes of perception configuration"""
 
         loop = asyncio.get_event_loop()
         ait = self.async_watch(
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
@@ -355,207 +412,249 @@
 
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
-    async def async_get_tare_volume(
+    async def async_list_templates(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PerceptionListTemplatesResponse":
+        """Return list of names for named templates"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.percept_pipeline.services.Perception/ListTemplates",
+            request,
+            PerceptionListTemplatesResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def list_templates(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PerceptionListTemplatesResponse":
+        """Return list of names for named templates"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_list_templates(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_reset_background(
         self,
         *,
-        zone_uuid: str = "",
+        fqdns: Optional[List[str]] = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "ZoneGetTareVolumeResponse":
-        """Computes raw volume within a volume zone without any offsets."""
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Resets the background of one, multiple or all devices"""
 
-        request = ZoneGetTareVolumeRequest()
-        request.zone_uuid = zone_uuid
+        fqdns = fqdns or []
+
+        request = PerceptionResetBackgroundRequest()
+        request.fqdns = fqdns
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Zone/GetTareVolume",
+            "/blickfeld.percept_pipeline.services.Perception/ResetBackground",
             request,
-            ZoneGetTareVolumeResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get_tare_volume(
+    def reset_background(
         self,
         *,
-        zone_uuid: str = "",
+        fqdns: Optional[List[str]] = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "ZoneGetTareVolumeResponse":
-        """Computes raw volume within a volume zone without any offsets."""
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Resets the background of one, multiple or all devices"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get_tare_volume(
-                zone_uuid=zone_uuid,
+            self.async_reset_background(
+                fqdns=fqdns,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class DataSource(betterproto.ServiceStub):
+class Zone(betterproto.ServiceStub):
     """
-    The data source service allows getting, configuring and receiving updates
-    of the data source used for processing pipelines. The data source
-    configuration specifies where to retrieve the point cloud data for further
-    processing.
+    The zone service allows getting, configuring, deleting and receiving
+    updates of the configured zones.
     """
 
-    async def async_get(
+    async def async_list(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "DataSourceGetResponse":
-        """Get current data_source Configuration"""
+    ) -> "ZoneListResponse":
+        """Returns the configured zones"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.DataSource/Get",
+            "/blickfeld.percept_pipeline.services.Zone/List",
             request,
-            DataSourceGetResponse,
+            ZoneListResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def list(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "DataSourceGetResponse":
-        """Get current data_source Configuration"""
+    ) -> "ZoneListResponse":
+        """Returns the configured zones"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_list(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_set(
+    async def async_store(
         self,
         *,
-        data_source: "_config__.DataSource" = None,
+        zone: "_config__.ZoneAlgorithm" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Set configuration for data_source"""
+        """Store / Update a zone"""
 
-        request = DataSourceSetRequest()
-        if data_source is not None:
-            request.data_source = data_source
+        request = ZoneStoreRequest()
+        if zone is not None:
+            request.zone = zone
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.DataSource/Set",
+            "/blickfeld.percept_pipeline.services.Zone/Store",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def set(
+    def store(
         self,
         *,
-        data_source: "_config__.DataSource" = None,
+        zone: "_config__.ZoneAlgorithm" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Set configuration for data_source"""
+        """Store / Update a zone"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_set(
-                data_source=data_source,
+            self.async_store(
+                zone=zone,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_reset(
+    async def async_delete(
         self,
+        *,
+        uuid: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
+        metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Resets the data_source configuration to factory values"""
+        """Delete a zone"""
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = ZoneDeleteRequest()
+        request.uuid = uuid
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.DataSource/Reset",
+            "/blickfeld.percept_pipeline.services.Zone/Delete",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def reset(
+    def delete(
         self,
+        *,
+        uuid: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
+        metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Resets the data_source configuration to factory values"""
+        """Delete a zone"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_reset(
+            self.async_delete(
+                uuid=uuid,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
     async def async_watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["DataSourceWatchResponse"]:
-        """Watch configuration for data_source"""
+    ) -> AsyncIterator["ZoneWatchResponse"]:
+        """Watch configuration for zone list"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         async for response in self._unary_stream(
-            "/blickfeld.percept_pipeline.services.DataSource/Watch",
+            "/blickfeld.percept_pipeline.services.Zone/Watch",
             request,
-            DataSourceWatchResponse,
+            ZoneWatchResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["DataSourceWatchResponse"]:
-        """Watch configuration for data_source"""
+    ) -> Iterator["ZoneWatchResponse"]:
+        """Watch configuration for zone list"""
 
         loop = asyncio.get_event_loop()
         ait = self.async_watch(
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
@@ -569,226 +668,207 @@
 
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
-
-class Health(betterproto.ServiceStub):
-    """Reports the health of the pipeline module."""
-
-    async def async_watch(
+    async def async_get_tare_volume(
         self,
+        *,
+        zone_uuid: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """
-        Streams health information on a regular cadence or if certain incidents
-        happen
-        """
+        metadata: Optional["MetadataLike"] = None
+    ) -> "ZoneGetTareVolumeResponse":
+        """Computes raw volume within a volume zone without any offsets."""
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = ZoneGetTareVolumeRequest()
+        request.zone_uuid = zone_uuid
 
-        async for response in self._unary_stream(
-            "/blickfeld.percept_pipeline.services.Health/Watch",
+        return await self._unary_unary(
+            "/blickfeld.percept_pipeline.services.Zone/GetTareVolume",
             request,
-            HealthWatchResponse,
+            ZoneGetTareVolumeResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        ):
-            yield response
+        )
 
-    def watch(
+    def get_tare_volume(
         self,
+        *,
+        zone_uuid: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """
-        Streams health information on a regular cadence or if certain incidents
-        happen
-        """
+        metadata: Optional["MetadataLike"] = None
+    ) -> "ZoneGetTareVolumeResponse":
+        """Computes raw volume within a volume zone without any offsets."""
 
         loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
+        return loop.run_until_complete(
+            self.async_get_tare_volume(
+                zone_uuid=zone_uuid,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
 
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
+class DataSource(betterproto.ServiceStub):
+    """
+    The data source service allows getting, configuring and receiving updates
+    of the data source used for processing pipelines. The data source
+    configuration specifies where to retrieve the point cloud data for further
+    processing.
+    """
 
     async def async_get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health information"""
+    ) -> "DataSourceGetResponse":
+        """Get current data_source Configuration"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Health/Get",
+            "/blickfeld.percept_pipeline.services.DataSource/Get",
             request,
-            HealthGetResponse,
+            DataSourceGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
     def get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health information"""
+    ) -> "DataSourceGetResponse":
+        """Get current data_source Configuration"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
             self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-
-class Perception(betterproto.ServiceStub):
-    """
-    The perception service allows getting, configuring and receiving updates of
-    the perception configurations. Perception configurations specify the
-    algorithms used for e.g. for background subtraction etc.
-    """
-
-    async def async_get(
+    async def async_set(
         self,
+        *,
+        data_source: "_config__.DataSource" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PerceptionGetResponse":
-        """Get current perception configuration"""
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Set configuration for data_source"""
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = DataSourceSetRequest()
+        if data_source is not None:
+            request.data_source = data_source
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Perception/Get",
+            "/blickfeld.percept_pipeline.services.DataSource/Set",
             request,
-            PerceptionGetResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def set(
         self,
+        *,
+        data_source: "_config__.DataSource" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PerceptionGetResponse":
-        """Get current perception configuration"""
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Set configuration for data_source"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_set(
+                data_source=data_source,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_set(
+    async def async_reset(
         self,
-        *,
-        template_name: str = "",
-        perception: "_config__.Perception" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
+        metadata: Optional["MetadataLike"] = None,
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Set the perception configuration"""
+        """Resets the data_source configuration to factory values"""
 
-        request = PerceptionSetRequest()
-        request.template_name = template_name
-        if perception is not None:
-            request.perception = perception
+        request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Perception/Set",
+            "/blickfeld.percept_pipeline.services.DataSource/Reset",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def set(
+    def reset(
         self,
-        *,
-        template_name: str = "",
-        perception: "_config__.Perception" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
+        metadata: Optional["MetadataLike"] = None,
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Set the perception configuration"""
+        """Resets the data_source configuration to factory values"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_set(
-                template_name=template_name,
-                perception=perception,
+            self.async_reset(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
     async def async_watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["PerceptionWatchResponse"]:
-        """Watch changes of perception configuration"""
+    ) -> AsyncIterator["DataSourceWatchResponse"]:
+        """Watch configuration for data_source"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         async for response in self._unary_stream(
-            "/blickfeld.percept_pipeline.services.Perception/Watch",
+            "/blickfeld.percept_pipeline.services.DataSource/Watch",
             request,
-            PerceptionWatchResponse,
+            DataSourceWatchResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["PerceptionWatchResponse"]:
-        """Watch changes of perception configuration"""
+    ) -> Iterator["DataSourceWatchResponse"]:
+        """Watch configuration for data_source"""
 
         loop = asyncio.get_event_loop()
         ait = self.async_watch(
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
@@ -801,87 +881,7 @@
                 return True, None
 
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
-
-    async def async_list_templates(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PerceptionListTemplatesResponse":
-        """Return list of names for named templates"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Perception/ListTemplates",
-            request,
-            PerceptionListTemplatesResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def list_templates(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PerceptionListTemplatesResponse":
-        """Return list of names for named templates"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_list_templates(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_reset_background(
-        self,
-        *,
-        fqdns: Optional[List[str]] = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Resets the background of one, multiple or all devices"""
-
-        fqdns = fqdns or []
-
-        request = PerceptionResetBackgroundRequest()
-        request.fqdns = fqdns
-
-        return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Perception/ResetBackground",
-            request,
-            betterproto_lib_google_protobuf.Empty,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def reset_background(
-        self,
-        *,
-        fqdns: Optional[List[str]] = None,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Resets the background of one, multiple or all devices"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_reset_background(
-                fqdns=fqdns,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/percept_processing/data/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,102 @@
     """
 
     DATA_TYPE_OBJECTS = 7
     """Objects data type: a map of objects detected by the system"""
 
 
 @dataclass(eq=False, repr=False)
+class Health(betterproto.Message):
+    """
+    A health message that contains information about the pipeline status and
+    the module itself.
+    """
+
+    state: "__base_data__.HealthState" = betterproto.enum_field(1)
+    """High-level state of module."""
+
+    state_reason: str = betterproto.string_field(2)
+    """Reason for the given state. It is not set if state is STATE_OK."""
+
+    pipeline_state: "__percept_pipeline_data__.State" = betterproto.enum_field(4)
+    """
+    Current state of the pipeline. It indicates if the pipeline is stable,
+    unstable or broken, based on the frequency of the data that is processed
+    and published.
+    """
+
+    clients: List["HealthClient"] = betterproto.message_field(5)
+    """Health information of all connected clients"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthClient(betterproto.Message):
+    """Health information of connected clients"""
+
+    uuid: str = betterproto.string_field(1)
+    """Identifier of the client"""
+
+    peer_uri: str = betterproto.string_field(2)
+    """The client peer uri"""
+
+    connection_timestamp: int = betterproto.uint64_field(3)
+    """The timestamp of the moment the client connected to processing"""
+
+    lost_frames: int = betterproto.uint64_field(4)
+    """The number of total lost frames since the start of the stream"""
+
+    point_cloud: "HealthClientPointCloud" = betterproto.message_field(
+        5, group="stream_type"
+    )
+    """The client receives point cloud stream data"""
+
+    states: "HealthClientStates" = betterproto.message_field(6, group="stream_type")
+    """The client receives states stream data"""
+
+    volume_map: "HealthClientVolumeMap" = betterproto.message_field(
+        7, group="stream_type"
+    )
+    """The client receives volume map stream data"""
+
+    objects: "HealthClientObjects" = betterproto.message_field(8, group="stream_type")
+    """The client receives objects stream data"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthClientPointCloud(betterproto.Message):
+    """Point Cloud specific information"""
+
+    point_cloud_type: "__percept_pipeline_data__.PointCloudType" = (
+        betterproto.enum_field(1)
+    )
+    """The point cloud type the client is receiving"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthClientStates(betterproto.Message):
+    """States specific information"""
+
+    pass
+
+
+@dataclass(eq=False, repr=False)
+class HealthClientVolumeMap(betterproto.Message):
+    """Volume Map specific information"""
+
+    pass
+
+
+@dataclass(eq=False, repr=False)
+class HealthClientObjects(betterproto.Message):
+    """Objects specific information"""
+
+    pass
+
+
+@dataclass(eq=False, repr=False)
 class VolumeMap(betterproto.Message):
     """A message containing the volume map of one volume zone."""
 
     timestamp: int = betterproto.uint64_field(1)
     """Timestamp of the lidar frame in which the volume map was calculated"""
 
     generator_uuid: str = betterproto.string_field(2)
@@ -223,129 +311,41 @@
     """The current numerical volume of the zone."""
 
     coverage: float = betterproto.float_field(5)
     """The current zone volume surface coverage"""
 
 
 @dataclass(eq=False, repr=False)
-class Objects(betterproto.Message):
+class States(betterproto.Message):
     """
-    A message that contains a map of objects. An object contains the
-    information regarding the detected object by the system.
+    A message that contains a map of states. A state is an information
+    generated by the system based on the select zone type or device. For
+    example, a state can contain information about the volume or the intrusion
+    in the zone.
     """
 
     timestamp: int = betterproto.uint64_field(1)
-    """The timestamp of the measurement(s) used to compute the objects."""
+    """The timestamp of the measurement(s) used to compute the states."""
 
-    objects: Dict[str, "DetectedObject"] = betterproto.map_field(
+    states: Dict[str, "State"] = betterproto.map_field(
         2, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
-    """
-    Map of objects where the key is the UUID of the object. These objects
-    should contain the point cloud of each object.
-    """
-
-
-@dataclass(eq=False, repr=False)
-class Health(betterproto.Message):
-    """
-    A health message that contains information about the pipeline status and
-    the module itself.
-    """
-
-    state: "__base_data__.HealthState" = betterproto.enum_field(1)
-    """High-level state of module."""
-
-    state_reason: str = betterproto.string_field(2)
-    """Reason for the given state. It is not set if state is STATE_OK."""
-
-    pipeline_state: "__percept_pipeline_data__.State" = betterproto.enum_field(4)
-    """
-    Current state of the pipeline. It indicates if the pipeline is stable,
-    unstable or broken, based on the frequency of the data that is processed
-    and published.
-    """
-
-    clients: List["HealthClient"] = betterproto.message_field(5)
-    """Health information of all connected clients"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthClient(betterproto.Message):
-    """Health information of connected clients"""
-
-    uuid: str = betterproto.string_field(1)
-    """Identifier of the client"""
-
-    peer_uri: str = betterproto.string_field(2)
-    """The client peer uri"""
-
-    connection_timestamp: int = betterproto.uint64_field(3)
-    """The timestamp of the moment the client connected to processing"""
-
-    lost_frames: int = betterproto.uint64_field(4)
-    """The number of total lost frames since the start of the stream"""
-
-    point_cloud: "HealthClientPointCloud" = betterproto.message_field(
-        5, group="stream_type"
-    )
-    """The client receives point cloud stream data"""
-
-    states: "HealthClientStates" = betterproto.message_field(6, group="stream_type")
-    """The client receives states stream data"""
-
-    volume_map: "HealthClientVolumeMap" = betterproto.message_field(
-        7, group="stream_type"
-    )
-    """The client receives volume map stream data"""
-
-    objects: "HealthClientObjects" = betterproto.message_field(8, group="stream_type")
-    """The client receives objects stream data"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthClientPointCloud(betterproto.Message):
-    """Point Cloud specific information"""
-
-    point_cloud_type: "__percept_pipeline_data__.PointCloudType" = (
-        betterproto.enum_field(1)
-    )
-    """The point cloud type the client is receiving"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthClientStates(betterproto.Message):
-    """States specific information"""
-
-    pass
-
-
-@dataclass(eq=False, repr=False)
-class HealthClientVolumeMap(betterproto.Message):
-    """Volume Map specific information"""
-
-    pass
-
-
-@dataclass(eq=False, repr=False)
-class HealthClientObjects(betterproto.Message):
-    """Objects specific information"""
-
-    pass
+    """Map of states where the key is the generator UUID of the state."""
 
 
 @dataclass(eq=False, repr=False)
-class States(betterproto.Message):
+class Objects(betterproto.Message):
     """
-    A message that contains a map of states. A state is an information
-    generated by the system based on the select zone type or device. For
-    example, a state can contain information about the volume or the intrusion
-    in the zone.
+    A message that contains a map of objects. An object contains the
+    information regarding the detected object by the system.
     """
 
     timestamp: int = betterproto.uint64_field(1)
-    """The timestamp of the measurement(s) used to compute the states."""
+    """The timestamp of the measurement(s) used to compute the objects."""
 
-    states: Dict[str, "State"] = betterproto.map_field(
+    objects: Dict[str, "DetectedObject"] = betterproto.map_field(
         2, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
     )
-    """Map of states where the key is the generator UUID of the state."""
+    """
+    Map of objects where the key is the UUID of the object. These objects
+    should contain the point cloud of each object.
+    """
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_processing/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/percept_processing/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,36 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """
+    A response for getting a stream of health messages about the pipeline
+    """
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """
+    The current health message with information about the state of the pipeline
+    """
+
+
+@dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """A response for getting an health message about the pipeline"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """
+    The current health message with information about the state of the pipeline
+    """
+
+
+@dataclass(eq=False, repr=False)
 class VolumeMapStreamRequest(betterproto.Message):
     """A request to receive a stream of state list messages"""
 
     zone_uuid: str = betterproto.string_field(2)
     """Volume zone uuid"""
 
 
@@ -76,14 +98,36 @@
     """
 
     data_types: List["_data__.DataType"] = betterproto.enum_field(1)
     """A list of the data types available for streaming"""
 
 
 @dataclass(eq=False, repr=False)
+class StatesStreamResponse(betterproto.Message):
+    """
+    A response for getting a stream of states messages from the running
+    pipeline
+    """
+
+    states: "_data__.States" = betterproto.message_field(1)
+    """The current states with the information detected in the scene."""
+
+
+@dataclass(eq=False, repr=False)
+class ObjectsStreamResponse(betterproto.Message):
+    """
+    A response for getting a stream of objects messages from the running
+    pipeline
+    """
+
+    objects: "_data__.Objects" = betterproto.message_field(1)
+    """The current objects detected in the scene."""
+
+
+@dataclass(eq=False, repr=False)
 class PointCloudStreamRequest(betterproto.Message):
     """
     A request to receive a stream of point cloud messages. Different point
     clouds can be streamed depending on the set fields: - combined point cloud
     (the full point cloud of all the available devices combined) in the map
     coordinate system - the foreground of the combined point cloud in the map
     coordinate system - the complete raw point cloud coming from one device,
@@ -114,56 +158,115 @@
 class PointCloudStreamResponse(betterproto.Message):
     """A response for getting a stream of point cloud messages"""
 
     point_cloud: "__core_processing_data__.Frame" = betterproto.message_field(1)
     """The required point cloud, based on the fields set in the request"""
 
 
-@dataclass(eq=False, repr=False)
-class ObjectsStreamResponse(betterproto.Message):
+class Health(betterproto.ServiceStub):
     """
-    A response for getting a stream of objects messages from the running
-    pipeline
+    An RPC service to request information about the state of the pipeline and
+    of the module.
     """
 
-    objects: "_data__.Objects" = betterproto.message_field(1)
-    """The current objects detected in the scene."""
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["HealthWatchResponse"]:
+        """
+        A method to get a stream of health messages, containing information
+        about the state of the pipeline
+        """
 
+        request = betterproto_lib_google_protobuf.Empty()
 
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """
-    A response for getting a stream of health messages about the pipeline
-    """
+        async for response in self._unary_stream(
+            "/blickfeld.percept_processing.services.Health/Watch",
+            request,
+            HealthWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
 
-    health: "_data__.Health" = betterproto.message_field(1)
-    """
-    The current health message with information about the state of the pipeline
-    """
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["HealthWatchResponse"]:
+        """
+        A method to get a stream of health messages, containing information
+        about the state of the pipeline
+        """
 
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
 
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """A response for getting an health message about the pipeline"""
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
 
-    health: "_data__.Health" = betterproto.message_field(1)
-    """
-    The current health message with information about the state of the pipeline
-    """
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
 
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """
+        A method to get one health message, containing information about the
+        state of the pipeline
+        """
 
-@dataclass(eq=False, repr=False)
-class StatesStreamResponse(betterproto.Message):
-    """
-    A response for getting a stream of states messages from the running
-    pipeline
-    """
+        request = betterproto_lib_google_protobuf.Empty()
 
-    states: "_data__.States" = betterproto.message_field(1)
-    """The current states with the information detected in the scene."""
+        return await self._unary_unary(
+            "/blickfeld.percept_processing.services.Health/Get",
+            request,
+            HealthGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """
+        A method to get one health message, containing information about the
+        state of the pipeline
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
 
 class VolumeMap(betterproto.ServiceStub):
     """An RPC service to request a stream of volume map messages."""
 
     async def async_stream(
         self,
@@ -359,81 +462,53 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class PointCloud(betterproto.ServiceStub):
+class States(betterproto.ServiceStub):
     """
-    An RPC service to request a stream of point cloud messages. If a pipeline
-    is already running, it will be used to stream the data. If no pipeline is
+    An RPC service to request a stream of states messages. If a pipeline is
+    already running, it will be used to stream the data. If no pipeline is
     running, it will be started first and then the stream will start. NOTE: in
-    this second case, the pipeline will also be automatically stopped once the
     this second case, the pipeline will also be automatically stopped once
     there are no more clients requesting any stream type from the module.
     """
 
     async def async_stream(
         self,
-        *,
-        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
-        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
-        fqdn: str = "",
-        crop: "__base_geometry__.Shape" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> AsyncIterator["PointCloudStreamResponse"]:
-        """
-        A method to get a stream of point cloud messages from the pipeline. It
-        is possible to stream different point clouds, depending on the fields
-        set in the request
-        """
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["StatesStreamResponse"]:
+        """A method to get a stream of states messages from the pipeline"""
 
-        request = PointCloudStreamRequest()
-        request.point_cloud_type = point_cloud_type
-        request.coordinate_system = coordinate_system
-        request.fqdn = fqdn
-        if crop is not None:
-            request.crop = crop
+        request = betterproto_lib_google_protobuf.Empty()
 
         async for response in self._unary_stream(
-            "/blickfeld.percept_processing.services.PointCloud/Stream",
+            "/blickfeld.percept_processing.services.States/Stream",
             request,
-            PointCloudStreamResponse,
+            StatesStreamResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def stream(
         self,
-        *,
-        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
-        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
-        fqdn: str = "",
-        crop: "__base_geometry__.Shape" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> Iterator["PointCloudStreamResponse"]:
-        """
-        A method to get a stream of point cloud messages from the pipeline. It
-        is possible to stream different point clouds, depending on the fields
-        set in the request
-        """
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["StatesStreamResponse"]:
+        """A method to get a stream of states messages from the pipeline"""
 
         loop = asyncio.get_event_loop()
         ait = self.async_stream(
-            point_cloud_type=point_cloud_type,
-            coordinate_system=coordinate_system,
-            fqdn=fqdn,
-            crop=crop,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
@@ -503,156 +578,81 @@
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
 
-class Health(betterproto.ServiceStub):
-    """
-    An RPC service to request information about the state of the pipeline and
-    of the module.
-    """
-
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """
-        A method to get a stream of health messages, containing information
-        about the state of the pipeline
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.percept_processing.services.Health/Watch",
-            request,
-            HealthWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """
-        A method to get a stream of health messages, containing information
-        about the state of the pipeline
-        """
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """
-        A method to get one health message, containing information about the
-        state of the pipeline
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.percept_processing.services.Health/Get",
-            request,
-            HealthGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """
-        A method to get one health message, containing information about the
-        state of the pipeline
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
-class States(betterproto.ServiceStub):
+class PointCloud(betterproto.ServiceStub):
     """
-    An RPC service to request a stream of states messages. If a pipeline is
-    already running, it will be used to stream the data. If no pipeline is
+    An RPC service to request a stream of point cloud messages. If a pipeline
+    is already running, it will be used to stream the data. If no pipeline is
     running, it will be started first and then the stream will start. NOTE: in
+    this second case, the pipeline will also be automatically stopped once the
     this second case, the pipeline will also be automatically stopped once
     there are no more clients requesting any stream type from the module.
     """
 
     async def async_stream(
         self,
+        *,
+        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
+        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
+        fqdn: str = "",
+        crop: "__base_geometry__.Shape" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["StatesStreamResponse"]:
-        """A method to get a stream of states messages from the pipeline"""
+        metadata: Optional["MetadataLike"] = None
+    ) -> AsyncIterator["PointCloudStreamResponse"]:
+        """
+        A method to get a stream of point cloud messages from the pipeline. It
+        is possible to stream different point clouds, depending on the fields
+        set in the request
+        """
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = PointCloudStreamRequest()
+        request.point_cloud_type = point_cloud_type
+        request.coordinate_system = coordinate_system
+        request.fqdn = fqdn
+        if crop is not None:
+            request.crop = crop
 
         async for response in self._unary_stream(
-            "/blickfeld.percept_processing.services.States/Stream",
+            "/blickfeld.percept_processing.services.PointCloud/Stream",
             request,
-            StatesStreamResponse,
+            PointCloudStreamResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def stream(
         self,
+        *,
+        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
+        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
+        fqdn: str = "",
+        crop: "__base_geometry__.Shape" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["StatesStreamResponse"]:
-        """A method to get a stream of states messages from the pipeline"""
+        metadata: Optional["MetadataLike"] = None
+    ) -> Iterator["PointCloudStreamResponse"]:
+        """
+        A method to get a stream of point cloud messages from the pipeline. It
+        is possible to stream different point clouds, depending on the fields
+        set in the request
+        """
 
         loop = asyncio.get_event_loop()
         ait = self.async_stream(
+            point_cloud_type=point_cloud_type,
+            coordinate_system=coordinate_system,
+            fqdn=fqdn,
+            crop=crop,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/percept_toolkit/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/percept_toolkit/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/percept_toolkit/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/push/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/push/config/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,25 +24,14 @@
     """json representation of protobuf messages"""
 
     ENCODING_JSON_FLATTENED = 3
     """flattened json representation of protobuf messages"""
 
 
 @dataclass(eq=False, repr=False)
-class Payload(betterproto.Message):
-    """defines what type of data stream to use as payload"""
-
-    encoding: "PayloadEncoding" = betterproto.enum_field(1)
-    """payload encoding"""
-
-    data_type: "__percept_processing_data__.DataType" = betterproto.enum_field(3)
-    """payload data type to stream"""
-
-
-@dataclass(eq=False, repr=False)
 class Authentication(betterproto.Message):
     """Authentication definition"""
 
     user: str = betterproto.string_field(1)
     """the user name used for authentication"""
 
     password: str = betterproto.string_field(2)
@@ -89,14 +78,25 @@
     mqtt topic - if empty the
     'blickfeld/{data_type}/{encoding_type}/{config_name}' pattern is used as a
     default
     """
 
 
 @dataclass(eq=False, repr=False)
+class Payload(betterproto.Message):
+    """defines what type of data stream to use as payload"""
+
+    encoding: "PayloadEncoding" = betterproto.enum_field(1)
+    """payload encoding"""
+
+    data_type: "__percept_processing_data__.DataType" = betterproto.enum_field(3)
+    """payload data type to stream"""
+
+
+@dataclass(eq=False, repr=False)
 class Push(betterproto.Message):
     """defines a combination of stream and destination"""
 
     name: str = betterproto.string_field(1)
     """name of push"""
 
     payload: "Payload" = betterproto.message_field(2)
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/push/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/push/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/push/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/push/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,30 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """request get the health of the configured publisher"""
+
+    health: "_data__.Health" = betterproto.message_field(2)
+    """health of push configurations"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """request watch the health of the configured publisher"""
+
+    health: "_data__.Health" = betterproto.message_field(2)
+    """health of push configurations"""
+
+
+@dataclass(eq=False, repr=False)
 class PushStoreRequest(betterproto.Message):
     """request to add a push configuration"""
 
     uuid: str = betterproto.string_field(1)
     """the uuid of the configuration (has to be generated on client side!)"""
 
     push_config: "_config__.Push" = betterproto.message_field(2)
@@ -82,35 +98,107 @@
     """request to disable the push configuration with the given uuid"""
 
     uuid: str = betterproto.string_field(1)
     """configuration uuid to disable"""
 
 
 @dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """request get the health of the configured publisher"""
+class DestinationValidateRequest(betterproto.Message):
+    """request to validate a configured destination"""
 
-    health: "_data__.Health" = betterproto.message_field(2)
-    """health of push configurations"""
+    destination: "_config__.Destination" = betterproto.message_field(1)
+    """the current (possibly incomplete) configuration entered"""
 
 
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """request watch the health of the configured publisher"""
+class Health(betterproto.ServiceStub):
+    """An gRPC service to request the status of push configurations"""
 
-    health: "_data__.Health" = betterproto.message_field(2)
-    """health of push configurations"""
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Get Status for all configured push configurations"""
 
+        request = betterproto_lib_google_protobuf.Empty()
 
-@dataclass(eq=False, repr=False)
-class DestinationValidateRequest(betterproto.Message):
-    """request to validate a configured destination"""
+        return await self._unary_unary(
+            "/blickfeld.push.services.Health/Get",
+            request,
+            HealthGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
-    destination: "_config__.Destination" = betterproto.message_field(1)
-    """the current (possibly incomplete) configuration entered"""
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Get Status for all configured push configurations"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["HealthWatchResponse"]:
+        """Watch status changes for configured push configurations"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.push.services.Health/Watch",
+            request,
+            HealthWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["HealthWatchResponse"]:
+        """Watch status changes for configured push configurations"""
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
 
 
 class Push(betterproto.ServiceStub):
     """An gRPC service to configure multiple push settings"""
 
     async def async_store(
         self,
@@ -366,102 +454,14 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class Health(betterproto.ServiceStub):
-    """An gRPC service to request the status of push configurations"""
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Get Status for all configured push configurations"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.push.services.Health/Get",
-            request,
-            HealthGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Get Status for all configured push configurations"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """Watch status changes for configured push configurations"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.push.services.Health/Watch",
-            request,
-            HealthWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """Watch status changes for configured push configurations"""
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-
 class Destination(betterproto.ServiceStub):
     """An gRPC service to configure multiple push settings"""
 
     async def async_validate(
         self,
         *,
         destination: "_config__.Destination" = None,
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/secure/client/token_factory.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/secure/client/token_factory.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/secure/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/secure/config/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,77 @@
     """active, account can be used to authenticate."""
 
     STATE_BLOCKED = 3
     """blocked, account can not be used for authentication."""
 
 
 @dataclass(eq=False, repr=False)
+class ApplicationKey(betterproto.Message):
+    """An application key is linked to a user account."""
+
+    purpose: str = betterproto.string_field(1)
+    """
+    Human readable purpose for this application key. It is recommended to
+    briefly describe the purpose of the application key here. The field should
+    help users to quickly identify different application keys but can also be
+    left empty.
+    """
+
+    access_level: "__base__.AccessControlLevel" = betterproto.enum_field(2)
+    """Access level which is granted to this application key."""
+
+    access_read_only: bool = betterproto.bool_field(7)
+    """If true, this application key has read-only access permissions."""
+
+    last_login_ts: int = betterproto.uint64_field(4)
+    """
+    Last time the application key was used to authenticate. This is just for
+    information purposes and might not be reliable.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class Firewall(betterproto.Message):
+    """Configuration options for the firewall"""
+
+    disable_insecure_network_ports: bool = betterproto.bool_field(1)
+    """
+    Disable all insecure, unencrypted & unauthenticated, network interface
+    ports. [NOTE] This might break compatibility with client applications e.g.
+    a normal  HTTP call to http://qb2-xxxxx will fail.
+    """
+
+
+@dataclass(eq=False, repr=False)
+class Account(betterproto.Message):
+    """
+    An account identifies a single user defined on the Qb2 device. By
+    presenting credentials linked to an account a client can be authenticated.
+    """
+
+    name: str = betterproto.string_field(1)
+    """Account name. This field is used as the username during login."""
+
+    access_level: "__base__.AccessControlLevel" = betterproto.enum_field(2)
+    """Access level which is granted to this account."""
+
+    access_read_only: bool = betterproto.bool_field(8)
+    """If true, this account has read-only access permissions."""
+
+    last_login_ts: int = betterproto.uint64_field(4)
+    """
+    Last time the account was used to login as observed on system time. This is
+    just for information purposes and might not be reliable.
+    """
+
+    state: "AccountState" = betterproto.enum_field(6)
+    """The account state."""
+
+
+@dataclass(eq=False, repr=False)
 class Certificate(betterproto.Message):
     """Public key certificate during the TLS handshake process"""
 
     binary: bytes = betterproto.bytes_field(1)
     """Certificate bytes (DER format)"""
 
     type: str = betterproto.string_field(2)
@@ -91,70 +154,7 @@
     """
 
     binary: bytes = betterproto.bytes_field(1)
     """Key bytes as binary"""
 
     type: str = betterproto.string_field(2)
     """String giving information about which key type is used"""
-
-
-@dataclass(eq=False, repr=False)
-class ApplicationKey(betterproto.Message):
-    """An application key is linked to a user account."""
-
-    purpose: str = betterproto.string_field(1)
-    """
-    Human readable purpose for this application key. It is recommended to
-    briefly describe the purpose of the application key here. The field should
-    help users to quickly identify different application keys but can also be
-    left empty.
-    """
-
-    access_level: "__base__.AccessControlLevel" = betterproto.enum_field(2)
-    """Access level which is granted to this application key."""
-
-    access_read_only: bool = betterproto.bool_field(7)
-    """If true, this application key has read-only access permissions."""
-
-    last_login_ts: int = betterproto.uint64_field(4)
-    """
-    Last time the application key was used to authenticate. This is just for
-    information purposes and might not be reliable.
-    """
-
-
-@dataclass(eq=False, repr=False)
-class Firewall(betterproto.Message):
-    """Configuration options for the firewall"""
-
-    disable_insecure_network_ports: bool = betterproto.bool_field(1)
-    """
-    Disable all insecure, unencrypted & unauthenticated, network interface
-    ports. [NOTE] This might break compatibility with client applications e.g.
-    a normal  HTTP call to http://qb2-xxxxx will fail.
-    """
-
-
-@dataclass(eq=False, repr=False)
-class Account(betterproto.Message):
-    """
-    An account identifies a single user defined on the Qb2 device. By
-    presenting credentials linked to an account a client can be authenticated.
-    """
-
-    name: str = betterproto.string_field(1)
-    """Account name. This field is used as the username during login."""
-
-    access_level: "__base__.AccessControlLevel" = betterproto.enum_field(2)
-    """Access level which is granted to this account."""
-
-    access_read_only: bool = betterproto.bool_field(8)
-    """If true, this account has read-only access permissions."""
-
-    last_login_ts: int = betterproto.uint64_field(4)
-    """
-    Last time the account was used to login as observed on system time. This is
-    just for information purposes and might not be reliable.
-    """
-
-    state: "AccountState" = betterproto.enum_field(6)
-    """The account state."""
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/secure/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/secure/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/secure/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/secure/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -28,66 +28,76 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
-class SessionGetNonceResponse(betterproto.Message):
-    """Response for GetNonce request."""
+class AuthenticationLoginRequest(betterproto.Message):
+    """Request for authentication"""
 
-    nonce: str = betterproto.string_field(1)
-    """Cryptographic session nonce."""
+    user: "AuthenticationLoginRequestUser" = betterproto.message_field(
+        1, group="credentials"
+    )
+    """Authenticate with user credentials"""
+
+    application: "AuthenticationLoginRequestApplication" = betterproto.message_field(
+        2, group="credentials"
+    )
+    """Authenticate with application key credentials"""
 
 
 @dataclass(eq=False, repr=False)
-class DeviceCredentialsSetFactoryRequest(betterproto.Message):
-    """
-    Request with device credentials The device credentials should only be set
-    once in production.
-    """
+class AuthenticationLoginRequestUser(betterproto.Message):
+    """User credentials"""
 
-    device_credentials: "_config__.DeviceCredentials" = betterproto.message_field(1)
-    """
-    Cryptographic device credentials which were generated by the blickfeld-
-    secure-authority.
-    """
+    name: str = betterproto.string_field(1)
+    """the username (can be left out in case of default factory state)"""
+
+    password: str = betterproto.string_field(2)
+    """the password of the user in plain text"""
 
 
 @dataclass(eq=False, repr=False)
-class DeviceCredentialsSetRequest(betterproto.Message):
-    """Request with device credentials"""
+class AuthenticationLoginRequestApplication(betterproto.Message):
+    """Application Key credentials"""
 
-    device_credentials: "_config__.DeviceCredentials" = betterproto.message_field(1)
-    """
-    Cryptographic device credentials used to establish secured TLS connection
-    between client and Qb2 device.
-    """
+    key: str = betterproto.string_field(1, group="type")
+    """the key in plain text"""
+
+    http_digest: str = betterproto.string_field(2, group="type")
+    """the key as md5 checksum"""
 
 
 @dataclass(eq=False, repr=False)
-class DeviceCredentialsGetResponse(betterproto.Message):
-    """Response with device credentials"""
+class AuthenticationLoginResponse(betterproto.Message):
+    """Response containing the issued JWT token."""
 
-    device_credentials: "_config__.DeviceCredentials" = betterproto.message_field(1)
+    token: str = betterproto.string_field(1)
     """
-    Cryptographic device credentials used to establish secured TLS connection
-    between client and Qb2 device.
+    The JWT token which needs to be sent with the key "token" in the metadata
+    of a gRPC call. The token is bound to a
+    xref:blickfeld/secure/services/session.adoc[].
     """
 
 
 @dataclass(eq=False, repr=False)
-class DeviceCredentialsGetCertificatesResponse(betterproto.Message):
-    """Response message which delivers public device certificate"""
+class HealthGetResponse(betterproto.Message):
+    """Response to Health Get request"""
 
-    certificates: List["_config__.Certificate"] = betterproto.message_field(1)
-    """
-    Certificate chain which is deployed at Qb2 device and is used during the
-    TLS handshake.
-    """
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """Response to Health Watch request"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
 
 
 @dataclass(eq=False, repr=False)
 class ApplicationKeyListRequest(betterproto.Message):
     """Request to list applicaion keys"""
 
     account_uuid: str = betterproto.string_field(1)
@@ -168,27 +178,19 @@
     """Get configuration response"""
 
     config: "_config__.Firewall" = betterproto.message_field(1)
     """Configuration"""
 
 
 @dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Response to Health Get request"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """Response to Health Watch request"""
+class SessionGetNonceResponse(betterproto.Message):
+    """Response for GetNonce request."""
 
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
+    nonce: str = betterproto.string_field(1)
+    """Cryptographic session nonce."""
 
 
 @dataclass(eq=False, repr=False)
 class AccountListResponse(betterproto.Message):
     """Response for list of accounts"""
 
     account: Dict[str, "_config__.Account"] = betterproto.map_field(
@@ -296,289 +298,215 @@
     """the current password"""
 
     new: str = betterproto.string_field(2)
     """the new password"""
 
 
 @dataclass(eq=False, repr=False)
-class AuthenticationLoginRequest(betterproto.Message):
-    """Request for authentication"""
-
-    user: "AuthenticationLoginRequestUser" = betterproto.message_field(
-        1, group="credentials"
-    )
-    """Authenticate with user credentials"""
-
-    application: "AuthenticationLoginRequestApplication" = betterproto.message_field(
-        2, group="credentials"
-    )
-    """Authenticate with application key credentials"""
-
-
-@dataclass(eq=False, repr=False)
-class AuthenticationLoginRequestUser(betterproto.Message):
-    """User credentials"""
-
-    name: str = betterproto.string_field(1)
-    """the username (can be left out in case of default factory state)"""
+class DeviceCredentialsSetFactoryRequest(betterproto.Message):
+    """
+    Request with device credentials The device credentials should only be set
+    once in production.
+    """
 
-    password: str = betterproto.string_field(2)
-    """the password of the user in plain text"""
+    device_credentials: "_config__.DeviceCredentials" = betterproto.message_field(1)
+    """
+    Cryptographic device credentials which were generated by the blickfeld-
+    secure-authority.
+    """
 
 
 @dataclass(eq=False, repr=False)
-class AuthenticationLoginRequestApplication(betterproto.Message):
-    """Application Key credentials"""
-
-    key: str = betterproto.string_field(1, group="type")
-    """the key in plain text"""
+class DeviceCredentialsSetRequest(betterproto.Message):
+    """Request with device credentials"""
 
-    http_digest: str = betterproto.string_field(2, group="type")
-    """the key as md5 checksum"""
+    device_credentials: "_config__.DeviceCredentials" = betterproto.message_field(1)
+    """
+    Cryptographic device credentials used to establish secured TLS connection
+    between client and Qb2 device.
+    """
 
 
 @dataclass(eq=False, repr=False)
-class AuthenticationLoginResponse(betterproto.Message):
-    """Response containing the issued JWT token."""
+class DeviceCredentialsGetResponse(betterproto.Message):
+    """Response with device credentials"""
 
-    token: str = betterproto.string_field(1)
+    device_credentials: "_config__.DeviceCredentials" = betterproto.message_field(1)
     """
-    The JWT token which needs to be sent with the key "token" in the metadata
-    of a gRPC call. The token is bound to a
-    xref:blickfeld/secure/services/session.adoc[].
+    Cryptographic device credentials used to establish secured TLS connection
+    between client and Qb2 device.
     """
 
 
-class Session(betterproto.ServiceStub):
+@dataclass(eq=False, repr=False)
+class DeviceCredentialsGetCertificatesResponse(betterproto.Message):
+    """Response message which delivers public device certificate"""
+
+    certificates: List["_config__.Certificate"] = betterproto.message_field(1)
     """
-    Session service which implements all methods for session-bound security
-    features. A session is recreated after the following events: * Power-cycle
-    of the device * Every day (UTC) * Manual invalidation via gRPC call
+    Certificate chain which is deployed at Qb2 device and is used during the
+    TLS handshake.
     """
 
-    async def async_get_nonce(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "SessionGetNonceResponse":
-        """Get cryptographic session nonce."""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.secure.services.Session/GetNonce",
-            request,
-            SessionGetNonceResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
 
-    def get_nonce(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "SessionGetNonceResponse":
-        """Get cryptographic session nonce."""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get_nonce(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_invalidate(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Invalidates the current session. A new session will be created
-        automatically.
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.secure.services.Session/Invalidate",
-            request,
-            betterproto_lib_google_protobuf.Empty,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def invalidate(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """
-        Invalidates the current session. A new session will be created
-        automatically.
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_invalidate(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
-class DeviceCredentials(betterproto.ServiceStub):
-    """
-    Set device credentials for the secure TLS connection of the Qb2 device.
-    """
+class Authentication(betterproto.ServiceStub):
+    """Service for authentication to the Qb2 device."""
 
-    async def async_set(
+    async def async_login(
         self,
         *,
-        device_credentials: "_config__.DeviceCredentials" = None,
+        user: "AuthenticationLoginRequestUser" = None,
+        application: "AuthenticationLoginRequestApplication" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
+    ) -> "AuthenticationLoginResponse":
         """
-        Set device credentials. [WARN] This will override the factory SSL
-        certificate which is provided by the device. It will cause problems
-        with inter-device communication, authentication, and Blickfeld client
-        libraries. Blickfeld client libraries expect a root certificate which
-        is signed by the Blickfeld device root authority. The expected root
-        certificate must then be manually provided via configuration options in
-        the client libraries.
+        User-Accounts managed by Qb2 have to use the Login method with an
+        existing account in order to receive a JWT Token for access to
+        priviliged parts of the device API. The factory user has the username
+        "admin". The password is printed on the device label.
         """
 
-        request = DeviceCredentialsSetRequest()
-        if device_credentials is not None:
-            request.device_credentials = device_credentials
+        request = AuthenticationLoginRequest()
+        if user is not None:
+            request.user = user
+        if application is not None:
+            request.application = application
 
         return await self._unary_unary(
-            "/blickfeld.secure.services.DeviceCredentials/Set",
+            "/blickfeld.secure.services.Authentication/Login",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            AuthenticationLoginResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def set(
+    def login(
         self,
         *,
-        device_credentials: "_config__.DeviceCredentials" = None,
+        user: "AuthenticationLoginRequestUser" = None,
+        application: "AuthenticationLoginRequestApplication" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
+    ) -> "AuthenticationLoginResponse":
         """
-        Set device credentials. [WARN] This will override the factory SSL
-        certificate which is provided by the device. It will cause problems
-        with inter-device communication, authentication, and Blickfeld client
-        libraries. Blickfeld client libraries expect a root certificate which
-        is signed by the Blickfeld device root authority. The expected root
-        certificate must then be manually provided via configuration options in
-        the client libraries.
+        User-Accounts managed by Qb2 have to use the Login method with an
+        existing account in order to receive a JWT Token for access to
+        priviliged parts of the device API. The factory user has the username
+        "admin". The password is printed on the device label.
         """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_set(
-                device_credentials=device_credentials,
+            self.async_login(
+                user=user,
+                application=application,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_get_certificates(
+
+class Health(betterproto.ServiceStub):
+    """
+    The health service provides methods to monitor operational status of the
+    secure module
+    """
+
+    async def async_get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "DeviceCredentialsGetCertificatesResponse":
-        """Get device credentials certificates."""
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the secure module"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.secure.services.DeviceCredentials/GetCertificates",
+            "/blickfeld.secure.services.Health/Get",
             request,
-            DeviceCredentialsGetCertificatesResponse,
+            HealthGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get_certificates(
+    def get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "DeviceCredentialsGetCertificatesResponse":
-        """Get device credentials certificates."""
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the secure module"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get_certificates(
+            self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_clear(
+    async def async_watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
+    ) -> AsyncIterator["HealthWatchResponse"]:
         """
-        Clear device credentials. The device credentials will reset to the
-        factory device credentials.
+        Continously returns the current health status of the secure module
         """
 
         request = betterproto_lib_google_protobuf.Empty()
 
-        return await self._unary_unary(
-            "/blickfeld.secure.services.DeviceCredentials/Clear",
+        async for response in self._unary_stream(
+            "/blickfeld.secure.services.Health/Watch",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            HealthWatchResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        )
+        ):
+            yield response
 
-    def clear(
+    def watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
+    ) -> Iterator["HealthWatchResponse"]:
         """
-        Clear device credentials. The device credentials will reset to the
-        factory device credentials.
+        Continously returns the current health status of the secure module
         """
 
         loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_clear(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
 
 
 class ApplicationKey(betterproto.ServiceStub):
     """Service for managing application keys."""
 
     async def async_list(
         self,
@@ -791,107 +719,98 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class Health(betterproto.ServiceStub):
+class Session(betterproto.ServiceStub):
     """
-    The health service provides methods to monitor operational status of the
-    secure module
+    Session service which implements all methods for session-bound security
+    features. A session is recreated after the following events: * Power-cycle
+    of the device * Every day (UTC) * Manual invalidation via gRPC call
     """
 
-    async def async_get(
+    async def async_get_nonce(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the secure module"""
+    ) -> "SessionGetNonceResponse":
+        """Get cryptographic session nonce."""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.secure.services.Health/Get",
+            "/blickfeld.secure.services.Session/GetNonce",
             request,
-            HealthGetResponse,
+            SessionGetNonceResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def get_nonce(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the secure module"""
+    ) -> "SessionGetNonceResponse":
+        """Get cryptographic session nonce."""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_get_nonce(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_watch(
+    async def async_invalidate(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
+    ) -> "betterproto_lib_google_protobuf.Empty":
         """
-        Continously returns the current health status of the secure module
+        Invalidates the current session. A new session will be created
+        automatically.
         """
 
         request = betterproto_lib_google_protobuf.Empty()
 
-        async for response in self._unary_stream(
-            "/blickfeld.secure.services.Health/Watch",
+        return await self._unary_unary(
+            "/blickfeld.secure.services.Session/Invalidate",
             request,
-            HealthWatchResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        ):
-            yield response
+        )
 
-    def watch(
+    def invalidate(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
+    ) -> "betterproto_lib_google_protobuf.Empty":
         """
-        Continously returns the current health status of the secure module
+        Invalidates the current session. A new session will be created
+        automatically.
         """
 
         loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
+        return loop.run_until_complete(
+            self.async_invalidate(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
 
 class Account(betterproto.ServiceStub):
     """
     This service supports the complete lifecycle of accounts which are managed
     by the current Qb2 device.
     """
@@ -1166,67 +1085,148 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class Authentication(betterproto.ServiceStub):
-    """Service for authentication to the Qb2 device."""
+class DeviceCredentials(betterproto.ServiceStub):
+    """
+    Set device credentials for the secure TLS connection of the Qb2 device.
+    """
 
-    async def async_login(
+    async def async_set(
         self,
         *,
-        user: "AuthenticationLoginRequestUser" = None,
-        application: "AuthenticationLoginRequestApplication" = None,
+        device_credentials: "_config__.DeviceCredentials" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "AuthenticationLoginResponse":
+    ) -> "betterproto_lib_google_protobuf.Empty":
         """
-        User-Accounts managed by Qb2 have to use the Login method with an
-        existing account in order to receive a JWT Token for access to
-        priviliged parts of the device API. The factory user has the username
-        "admin". The password is printed on the device label.
+        Set device credentials. [WARN] This will override the factory SSL
+        certificate which is provided by the device. It will cause problems
+        with inter-device communication, authentication, and Blickfeld client
+        libraries. Blickfeld client libraries expect a root certificate which
+        is signed by the Blickfeld device root authority. The expected root
+        certificate must then be manually provided via configuration options in
+        the client libraries.
         """
 
-        request = AuthenticationLoginRequest()
-        if user is not None:
-            request.user = user
-        if application is not None:
-            request.application = application
+        request = DeviceCredentialsSetRequest()
+        if device_credentials is not None:
+            request.device_credentials = device_credentials
 
         return await self._unary_unary(
-            "/blickfeld.secure.services.Authentication/Login",
+            "/blickfeld.secure.services.DeviceCredentials/Set",
             request,
-            AuthenticationLoginResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def login(
+    def set(
         self,
         *,
-        user: "AuthenticationLoginRequestUser" = None,
-        application: "AuthenticationLoginRequestApplication" = None,
+        device_credentials: "_config__.DeviceCredentials" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "AuthenticationLoginResponse":
+    ) -> "betterproto_lib_google_protobuf.Empty":
         """
-        User-Accounts managed by Qb2 have to use the Login method with an
-        existing account in order to receive a JWT Token for access to
-        priviliged parts of the device API. The factory user has the username
-        "admin". The password is printed on the device label.
+        Set device credentials. [WARN] This will override the factory SSL
+        certificate which is provided by the device. It will cause problems
+        with inter-device communication, authentication, and Blickfeld client
+        libraries. Blickfeld client libraries expect a root certificate which
+        is signed by the Blickfeld device root authority. The expected root
+        certificate must then be manually provided via configuration options in
+        the client libraries.
         """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_login(
-                user=user,
-                application=application,
+            self.async_set(
+                device_credentials=device_credentials,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_get_certificates(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "DeviceCredentialsGetCertificatesResponse":
+        """Get device credentials certificates."""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.secure.services.DeviceCredentials/GetCertificates",
+            request,
+            DeviceCredentialsGetCertificatesResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get_certificates(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "DeviceCredentialsGetCertificatesResponse":
+        """Get device credentials certificates."""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get_certificates(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_clear(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Clear device credentials. The device credentials will reset to the
+        factory device credentials.
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.secure.services.DeviceCredentials/Clear",
+            request,
+            betterproto_lib_google_protobuf.Empty,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def clear(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        Clear device credentials. The device credentials will reset to the
+        factory device credentials.
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_clear(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/system/config/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/system/config/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,23 +9,14 @@
 
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 from ...eye_safety import data as __eye_safety_data__
 
 
-class DeviceClass(betterproto.Enum):
-    """Enum to distinguish different device classes"""
-
-    CLASS_UNKNOWN = 0
-    CUBE = 1
-    CUBE_RANGE = 2
-    QB2 = 3
-
-
 class ScanPatternFrameMode(betterproto.Enum):
     """
     The frame mode specifies the point cloud frame's composition and can be
     used to fine tune the LiDAR to specific use cases.
     """
 
     FRAME_MODE_UNSPECIFIED = 0
@@ -50,14 +41,23 @@
     FRAME_MODE_SEPARATE = 3
     """
     The laser will trigger both during up and downramping phase but separate
     point cloud frames will be emitted, which maximizes frame rate.
     """
 
 
+class DeviceClass(betterproto.Enum):
+    """Enum to distinguish different device classes"""
+
+    CLASS_UNKNOWN = 0
+    CUBE = 1
+    CUBE_RANGE = 2
+    QB2 = 3
+
+
 @dataclass(eq=False, repr=False)
 class Network(betterproto.Message):
     """
     * The "Network" protocol message allows to define and setup the network
     configuration of the Qb2 device which can be further applied by
     "SetConfig()" service API. The message specifies the desired network
     configuration mode: "dhcp", "link-local","static" or their combination, and
@@ -180,37 +180,14 @@
     Password of the wireless network [NOTE] If the password is not set and the
     SSID did not change, the existing password is used. This mechanism is
     applied as the password is never returned via the GetConfig API.
     """
 
 
 @dataclass(eq=False, repr=False)
-class Device(betterproto.Message):
-    """This message describes a Blickfeld Lidar device"""
-
-    fqdn_or_ip: str = betterproto.string_field(1)
-    """Fully-qualified-domain-name / Hostname or IP address"""
-
-    name: str = betterproto.string_field(2)
-    """
-    Human-readable name of the device Optional: Is filled out by the service if
-    not given.
-    """
-
-    serial_number: str = betterproto.string_field(3)
-    """
-    Serial number of the device Optional: Is filled out by the service if not
-    given.
-    """
-
-    class_: "DeviceClass" = betterproto.enum_field(4)
-    """Device class Optional: Is filled out by the service if not given."""
-
-
-@dataclass(eq=False, repr=False)
 class ScanPattern(betterproto.Message):
     """
     * The scan pattern defines the movement of the mirrors. The key parameters
     of the pattern are the horizontal and vertical fields of view (FoV) as well
     as the number of scan lines per frame. The frame rate is defined by the
     total number of scan lines and the oscillation frequency of the mirrors
     which is fixed and device-specific.
@@ -407,7 +384,30 @@
 
 @dataclass(eq=False, repr=False)
 class TimeSynchronizationNtp(betterproto.Message):
     """Configuration message for NTP time synchronization"""
 
     servers: List[str] = betterproto.string_field(1)
     """List of NTP time servers which are to be used"""
+
+
+@dataclass(eq=False, repr=False)
+class Device(betterproto.Message):
+    """This message describes a Blickfeld Lidar device"""
+
+    fqdn_or_ip: str = betterproto.string_field(1)
+    """Fully-qualified-domain-name / Hostname or IP address"""
+
+    name: str = betterproto.string_field(2)
+    """
+    Human-readable name of the device Optional: Is filled out by the service if
+    not given.
+    """
+
+    serial_number: str = betterproto.string_field(3)
+    """
+    Serial number of the device Optional: Is filled out by the service if not
+    given.
+    """
+
+    class_: "DeviceClass" = betterproto.enum_field(4)
+    """Device class Optional: Is filled out by the service if not given."""
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/system/data/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/system/data/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,150 +12,89 @@
     config as __base_config__,
     data as __base_data__,
 )
 from .. import config as _config__
 
 
 @dataclass(eq=False, repr=False)
-class Firmware(betterproto.Message):
-    """
-    The Firmware data message contains all relevant information about the
-    current firmware, uploaded firmware and the status of an firmware
-    installation.
-    """
-
-    pass
-
-
-@dataclass(eq=False, repr=False)
-class FirmwareInfo(betterproto.Message):
-    """
-    contains information about rauc bundle parsed from the associated manifest
-    file
-    """
-
-    label: str = betterproto.string_field(1)
-    """Human-readable label / version of the firmware"""
-
-    version: "__base_data__.Version" = betterproto.message_field(2)
-    """Version"""
-
-    allowed_downgrade_version: "__base_data__.Version" = betterproto.message_field(3)
+class NetworkStatus(betterproto.Message):
     """
-    Lowest allowed version which can be downgraded to if this firmware is
-    installed
+    Carries information about active connection: current statistics and network
+    configuration
     """
 
+    active_config: "_config__.Network" = betterproto.message_field(1)
+    """Brings configuration information about currently active connection"""
 
-@dataclass(eq=False, repr=False)
-class FirmwareStatus(betterproto.Message):
-    """contains information about rauc bridge status"""
-
-    idle: "FirmwareStatusIdle" = betterproto.message_field(1, group="status")
-    """no bundle is available and no installation is happenning"""
-
-    ready_to_install: "FirmwareStatusReadyToInstall" = betterproto.message_field(
-        2, group="status"
-    )
-    """bundle is verified and available for installation"""
-
-    installation: "FirmwareStatusInstallation" = betterproto.message_field(
-        3, group="status"
-    )
-    """the installation process is ongoing"""
-
-    failure: "FirmwareStatusFailure" = betterproto.message_field(4, group="status")
-    """installation failed"""
-
-    reboot: "FirmwareStatusReboot" = betterproto.message_field(5, group="status")
-    """reboot has been triggered after successfull installation"""
-
-    installed_firmware_info: "FirmwareInfo" = betterproto.message_field(6)
-    """Currently installed firmware"""
+    statistics: "NetworkStatusStatistics" = betterproto.message_field(2)
+    """Brings statistical information about currently active connection"""
 
 
 @dataclass(eq=False, repr=False)
-class FirmwareStatusIdle(betterproto.Message):
+class NetworkStatusStatistics(betterproto.Message):
     """
-    initial state when no bundle is available and no installation is happenning
+    (WIP) Carries statistical information about currently active connection
     """
 
-    pass
+    speed: str = betterproto.string_field(1)
+    """Link speed"""
 
 
 @dataclass(eq=False, repr=False)
-class FirmwareStatusReadyToInstall(betterproto.Message):
-    """state when bundle is verified and available for installation"""
-
-    uploaded_firmware_info: "FirmwareInfo" = betterproto.message_field(1)
-    """Firmware info of bundle which has been uploaded"""
+class Health(betterproto.Message):
+    """Message representing health"""
 
+    state: "__base_data__.HealthState" = betterproto.enum_field(1)
+    """High-level state of module"""
 
-@dataclass(eq=False, repr=False)
-class FirmwareStatusInstallation(betterproto.Message):
-    """state when the installation process is ongoing"""
+    state_reason: str = betterproto.string_field(2)
+    """Reason for given state. Is not set if state is STATE_OK."""
 
-    progress: "FirmwareStatusInstallationProgress" = betterproto.message_field(1)
-    """Current installation progress"""
+    time_synchronization: "HealthTimeSynchronization" = betterproto.message_field(3)
+    """Time synchronization status"""
 
 
 @dataclass(eq=False, repr=False)
-class FirmwareStatusInstallationProgress(betterproto.Message):
-    """
-    Contains information about current state of installation procedure inside
-    the tree of progress
-    """
-
-    percent: int = betterproto.uint32_field(1)
-    """progress of installation in percents (0%-100%)"""
+class HealthTimeSynchronization(betterproto.Message):
+    """Status message for time synchronization"""
 
-    message: str = betterproto.string_field(2)
-    """log message describing the current installation step"""
+    state: "__base_data__.HealthState" = betterproto.enum_field(1)
+    """High-level state of the time synchronization"""
 
+    state_reason: str = betterproto.string_field(2)
+    """Reason for given state. Is not set if state is STATE_OK."""
 
-@dataclass(eq=False, repr=False)
-class FirmwareStatusFailure(betterproto.Message):
-    """state when installation failed"""
+    current_system_timestamp: int = betterproto.uint64_field(3)
+    """Current timestamp"""
 
-    reason: str = betterproto.string_field(1)
-    """Human-readable reason for installation failure"""
+    ntp: "HealthTimeSynchronizationNtp" = betterproto.message_field(4, group="type")
+    """Status for NTP time synchronization"""
 
 
 @dataclass(eq=False, repr=False)
-class FirmwareStatusReboot(betterproto.Message):
-    """
-    state when reboot of the device has been triggered after successfull
-    installation
-    """
-
-    pass
-
+class HealthTimeSynchronizationNtp(betterproto.Message):
+    """Status message representing the NTP time synchronization status"""
 
-@dataclass(eq=False, repr=False)
-class NetworkStatus(betterproto.Message):
-    """
-    Carries information about active connection: current statistics and network
-    configuration
-    """
+    synchronized: bool = betterproto.bool_field(1)
+    """Flag indicating that the system time is synchronized with NTP"""
 
-    active_config: "_config__.Network" = betterproto.message_field(1)
-    """Brings configuration information about currently active connection"""
+    server: str = betterproto.string_field(2)
+    """The server NTP time server which is used"""
 
-    statistics: "NetworkStatusStatistics" = betterproto.message_field(2)
-    """Brings statistical information about currently active connection"""
+    offset: float = betterproto.float_field(3)
+    """Time offset between Qb2 system time and time server"""
 
+    delay: float = betterproto.float_field(4)
+    """Time delay from NTP request until server response is received"""
 
-@dataclass(eq=False, repr=False)
-class NetworkStatusStatistics(betterproto.Message):
-    """
-    (WIP) Carries statistical information about currently active connection
-    """
+    jitter: float = betterproto.float_field(5)
+    """Jitter between multiple time comparisons"""
 
-    speed: str = betterproto.string_field(1)
-    """Link speed"""
+    precision: float = betterproto.float_field(6)
+    """Precision of the NTP time synchronization"""
 
 
 @dataclass(eq=False, repr=False)
 class ScanPatternLimits(betterproto.Message):
     """
     This section contains limits for configurable parameters of a scan pattern
     """
@@ -212,58 +151,119 @@
     """
 
     target: "__base_config__.RangeDouble" = betterproto.message_field(1)
     """The target frame rate limit"""
 
 
 @dataclass(eq=False, repr=False)
-class Health(betterproto.Message):
-    """Message representing health"""
+class Firmware(betterproto.Message):
+    """
+    The Firmware data message contains all relevant information about the
+    current firmware, uploaded firmware and the status of an firmware
+    installation.
+    """
 
-    state: "__base_data__.HealthState" = betterproto.enum_field(1)
-    """High-level state of module"""
+    pass
 
-    state_reason: str = betterproto.string_field(2)
-    """Reason for given state. Is not set if state is STATE_OK."""
 
-    time_synchronization: "HealthTimeSynchronization" = betterproto.message_field(3)
-    """Time synchronization status"""
+@dataclass(eq=False, repr=False)
+class FirmwareInfo(betterproto.Message):
+    """
+    contains information about rauc bundle parsed from the associated manifest
+    file
+    """
+
+    label: str = betterproto.string_field(1)
+    """Human-readable label / version of the firmware"""
+
+    version: "__base_data__.Version" = betterproto.message_field(2)
+    """Version"""
+
+    allowed_downgrade_version: "__base_data__.Version" = betterproto.message_field(3)
+    """
+    Lowest allowed version which can be downgraded to if this firmware is
+    installed
+    """
 
 
 @dataclass(eq=False, repr=False)
-class HealthTimeSynchronization(betterproto.Message):
-    """Status message for time synchronization"""
+class FirmwareStatus(betterproto.Message):
+    """contains information about rauc bridge status"""
 
-    state: "__base_data__.HealthState" = betterproto.enum_field(1)
-    """High-level state of the time synchronization"""
+    idle: "FirmwareStatusIdle" = betterproto.message_field(1, group="status")
+    """no bundle is available and no installation is happenning"""
 
-    state_reason: str = betterproto.string_field(2)
-    """Reason for given state. Is not set if state is STATE_OK."""
+    ready_to_install: "FirmwareStatusReadyToInstall" = betterproto.message_field(
+        2, group="status"
+    )
+    """bundle is verified and available for installation"""
 
-    current_system_timestamp: int = betterproto.uint64_field(3)
-    """Current timestamp"""
+    installation: "FirmwareStatusInstallation" = betterproto.message_field(
+        3, group="status"
+    )
+    """the installation process is ongoing"""
 
-    ntp: "HealthTimeSynchronizationNtp" = betterproto.message_field(4, group="type")
-    """Status for NTP time synchronization"""
+    failure: "FirmwareStatusFailure" = betterproto.message_field(4, group="status")
+    """installation failed"""
+
+    reboot: "FirmwareStatusReboot" = betterproto.message_field(5, group="status")
+    """reboot has been triggered after successfull installation"""
+
+    installed_firmware_info: "FirmwareInfo" = betterproto.message_field(6)
+    """Currently installed firmware"""
 
 
 @dataclass(eq=False, repr=False)
-class HealthTimeSynchronizationNtp(betterproto.Message):
-    """Status message representing the NTP time synchronization status"""
+class FirmwareStatusIdle(betterproto.Message):
+    """
+    initial state when no bundle is available and no installation is happenning
+    """
 
-    synchronized: bool = betterproto.bool_field(1)
-    """Flag indicating that the system time is synchronized with NTP"""
+    pass
 
-    server: str = betterproto.string_field(2)
-    """The server NTP time server which is used"""
 
-    offset: float = betterproto.float_field(3)
-    """Time offset between Qb2 system time and time server"""
+@dataclass(eq=False, repr=False)
+class FirmwareStatusReadyToInstall(betterproto.Message):
+    """state when bundle is verified and available for installation"""
 
-    delay: float = betterproto.float_field(4)
-    """Time delay from NTP request until server response is received"""
+    uploaded_firmware_info: "FirmwareInfo" = betterproto.message_field(1)
+    """Firmware info of bundle which has been uploaded"""
 
-    jitter: float = betterproto.float_field(5)
-    """Jitter between multiple time comparisons"""
 
-    precision: float = betterproto.float_field(6)
-    """Precision of the NTP time synchronization"""
+@dataclass(eq=False, repr=False)
+class FirmwareStatusInstallation(betterproto.Message):
+    """state when the installation process is ongoing"""
+
+    progress: "FirmwareStatusInstallationProgress" = betterproto.message_field(1)
+    """Current installation progress"""
+
+
+@dataclass(eq=False, repr=False)
+class FirmwareStatusInstallationProgress(betterproto.Message):
+    """
+    Contains information about current state of installation procedure inside
+    the tree of progress
+    """
+
+    percent: int = betterproto.uint32_field(1)
+    """progress of installation in percents (0%-100%)"""
+
+    message: str = betterproto.string_field(2)
+    """log message describing the current installation step"""
+
+
+@dataclass(eq=False, repr=False)
+class FirmwareStatusFailure(betterproto.Message):
+    """state when installation failed"""
+
+    reason: str = betterproto.string_field(1)
+    """Human-readable reason for installation failure"""
+
+
+@dataclass(eq=False, repr=False)
+class FirmwareStatusReboot(betterproto.Message):
+    """
+    state when reboot of the device has been triggered after successfull
+    installation
+    """
+
+    pass
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2/system/services/__init__.py` & `blickfeld_qb2-2.0.9/blickfeld_qb2/system/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,105 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """Response to health get request"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """Stream response to health watch request"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternGetResponse(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternSetRequest(betterproto.Message):
+    name: str = betterproto.string_field(1, group="type_oneof")
+    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(
+        2, group="type_oneof"
+    )
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternWatchResponse(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternListResponse(betterproto.Message):
+    named_scan_patterns: Dict[str, "_config__.ScanPattern"] = betterproto.map_field(
+        1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
+    )
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternStoreRequest(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternDeleteRequest(betterproto.Message):
+    name: str = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternGetLimitsRequest(betterproto.Message):
+    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class ScanPatternGetLimitsResponse(betterproto.Message):
+    scan_pattern_limits: "_data__.ScanPatternLimits" = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class NetworkValidateRequest(betterproto.Message):
+    """Request to validate method"""
+
+    config: "_config__.Network" = betterproto.message_field(1)
+    """Configuration which should be validated"""
+
+
+@dataclass(eq=False, repr=False)
+class NetworkValidateResponse(betterproto.Message):
+    """Response to validate method"""
+
+    status: "_data__.NetworkStatus" = betterproto.message_field(1)
+    """Status message with allocated IP addresses"""
+
+
+@dataclass(eq=False, repr=False)
+class NetworkGetMacAddressesResponse(betterproto.Message):
+    """Response with mac addresses"""
+
+    ethernet: str = betterproto.string_field(1)
+    """Mac address of ethernet / LAN interface"""
+
+    wireless: str = betterproto.string_field(2)
+    """Mac address of wireless / WiFi interface"""
+
+
+@dataclass(eq=False, repr=False)
 class FirmwareUploadRequest(betterproto.Message):
     """
     This request is sent multiple times to upload a full complete bundle. End
     the stream with the last chunk of the bundle.
     """
 
     binary_chunk: bytes = betterproto.bytes_field(1)
@@ -144,105 +235,14 @@
     """Continuous response with status"""
 
     status: "_data__.FirmwareStatus" = betterproto.message_field(1)
     """Current firmware status"""
 
 
 @dataclass(eq=False, repr=False)
-class ScanPatternGetResponse(betterproto.Message):
-    name: str = betterproto.string_field(1)
-    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class ScanPatternSetRequest(betterproto.Message):
-    name: str = betterproto.string_field(1, group="type_oneof")
-    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(
-        2, group="type_oneof"
-    )
-
-
-@dataclass(eq=False, repr=False)
-class ScanPatternWatchResponse(betterproto.Message):
-    name: str = betterproto.string_field(1)
-    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class ScanPatternListResponse(betterproto.Message):
-    named_scan_patterns: Dict[str, "_config__.ScanPattern"] = betterproto.map_field(
-        1, betterproto.TYPE_STRING, betterproto.TYPE_MESSAGE
-    )
-
-
-@dataclass(eq=False, repr=False)
-class ScanPatternStoreRequest(betterproto.Message):
-    name: str = betterproto.string_field(1)
-    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class ScanPatternDeleteRequest(betterproto.Message):
-    name: str = betterproto.string_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class ScanPatternGetLimitsRequest(betterproto.Message):
-    scan_pattern: "_config__.ScanPattern" = betterproto.message_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class ScanPatternGetLimitsResponse(betterproto.Message):
-    scan_pattern_limits: "_data__.ScanPatternLimits" = betterproto.message_field(1)
-
-
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Response to health get request"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """Stream response to health watch request"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
-
-
-@dataclass(eq=False, repr=False)
-class NetworkValidateRequest(betterproto.Message):
-    """Request to validate method"""
-
-    config: "_config__.Network" = betterproto.message_field(1)
-    """Configuration which should be validated"""
-
-
-@dataclass(eq=False, repr=False)
-class NetworkValidateResponse(betterproto.Message):
-    """Response to validate method"""
-
-    status: "_data__.NetworkStatus" = betterproto.message_field(1)
-    """Status message with allocated IP addresses"""
-
-
-@dataclass(eq=False, repr=False)
-class NetworkGetMacAddressesResponse(betterproto.Message):
-    """Response with mac addresses"""
-
-    ethernet: str = betterproto.string_field(1)
-    """Mac address of ethernet / LAN interface"""
-
-    wireless: str = betterproto.string_field(2)
-    """Mac address of wireless / WiFi interface"""
-
-
-@dataclass(eq=False, repr=False)
 class TimeSynchronizationSetRequest(betterproto.Message):
     """Request which is sent together with a SetConfig API call"""
 
     config: "_config__.TimeSynchronization" = betterproto.message_field(1)
     """Time synchronization config to be used"""
 
 
@@ -250,319 +250,92 @@
 class TimeSynchronizationGetResponse(betterproto.Message):
     """Response which is sent as answer for a GetConfig call"""
 
     config: "_config__.TimeSynchronization" = betterproto.message_field(1)
     """Currently used time synchronization config"""
 
 
-class Firmware(betterproto.ServiceStub):
+class Health(betterproto.ServiceStub):
     """
-    The firmware service offers methods to fetch the currently installed
-    firmware, upgrade it, downgrade it and also configure auto-update
-    mechanisms.
+    The health service provides methods to monitor operational status of the
+    systen module
     """
 
-    async def async_upload(
-        self,
-        request_iterator: Union[
-            AsyncIterable["FirmwareUploadRequest"], Iterable["FirmwareUploadRequest"]
-        ],
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "FirmwareUploadResponse":
-        """
-        Upload the firmware bundle from the client to the device. Fails if the
-        uploaded firmware bundle is not valid.
-        """
-
-        return await self._stream_unary(
-            "/blickfeld.system.services.Firmware/Upload",
-            request_iterator,
-            FirmwareUploadRequest,
-            FirmwareUploadResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def upload(
-        self,
-        request_iterator: Iterable["FirmwareUploadRequest"],
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "FirmwareUploadResponse":
-        """
-        Upload the firmware bundle from the client to the device. Fails if the
-        uploaded firmware bundle is not valid.
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_upload(
-                request_iterator,
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_install(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["FirmwareInstallResponse"]:
-        """
-        Trigger the installation process of an uploaded firmware. A status
-        stream with the installation progress is returned and ends with
-        installation completion.
-        """
-
-        request = FirmwareInstallRequest()
-
-        async for response in self._unary_stream(
-            "/blickfeld.system.services.Firmware/Install",
-            request,
-            FirmwareInstallResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def install(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["FirmwareInstallResponse"]:
-        """
-        Trigger the installation process of an uploaded firmware. A status
-        stream with the installation progress is returned and ends with
-        installation completion.
-        """
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_install(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-    async def async_upload_and_install(
-        self,
-        request_iterator: Union[
-            AsyncIterable["FirmwareUploadAndInstallRequest"],
-            Iterable["FirmwareUploadAndInstallRequest"],
-        ],
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["FirmwareUploadAndInstallResponse"]:
-        """Combines the Upload and Install steps in a single method."""
-
-        async for response in self._stream_stream(
-            "/blickfeld.system.services.Firmware/UploadAndInstall",
-            request_iterator,
-            FirmwareUploadAndInstallRequest,
-            FirmwareUploadAndInstallResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def upload_and_install(
-        self,
-        request_iterator: Iterable["FirmwareUploadAndInstallRequest"],
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["FirmwareUploadAndInstallResponse"]:
-        """Combines the Upload and Install steps in a single method."""
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_upload_and_install(
-            request_iterator,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-    async def async_fetch_and_install(
-        self,
-        *,
-        version: "__base_data__.Version" = None,
-        url: str = "",
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> AsyncIterator["FirmwareFetchAndInstallResponse"]:
-        """
-        Fetch a firmware bundle from a static file server and perform
-        installation.
-        """
-
-        request = FirmwareFetchAndInstallRequest()
-        if version is not None:
-            request.version = version
-        request.url = url
-
-        async for response in self._unary_stream(
-            "/blickfeld.system.services.Firmware/FetchAndInstall",
-            request,
-            FirmwareFetchAndInstallResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def fetch_and_install(
-        self,
-        *,
-        version: "__base_data__.Version" = None,
-        url: str = "",
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> Iterator["FirmwareFetchAndInstallResponse"]:
-        """
-        Fetch a firmware bundle from a static file server and perform
-        installation.
-        """
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_fetch_and_install(
-            version=version,
-            url=url,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-    async def async_get_status(
+    async def async_get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "FirmwareGetStatusResponse":
-        """
-        Get the current firmware status which includes the currently installed
-        firmware but also ongoing or failed installations.
-        """
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the systen module"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.system.services.Firmware/GetStatus",
+            "/blickfeld.system.services.Health/Get",
             request,
-            FirmwareGetStatusResponse,
+            HealthGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get_status(
+    def get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "FirmwareGetStatusResponse":
-        """
-        Get the current firmware status which includes the currently installed
-        firmware but also ongoing or failed installations.
-        """
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the systen module"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get_status(
+            self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_watch_status(
+    async def async_watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["FirmwareWatchStatusResponse"]:
+    ) -> AsyncIterator["HealthWatchResponse"]:
         """
-        Continously watch the status stream and get updates on changes. This
-        can be used to attach to an ongoing installation.
+        Can be used to attach to the health monitoring status information of
+        the systen module
         """
 
         request = betterproto_lib_google_protobuf.Empty()
 
         async for response in self._unary_stream(
-            "/blickfeld.system.services.Firmware/WatchStatus",
+            "/blickfeld.system.services.Health/Watch",
             request,
-            FirmwareWatchStatusResponse,
+            HealthWatchResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
-    def watch_status(
+    def watch(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["FirmwareWatchStatusResponse"]:
+    ) -> Iterator["HealthWatchResponse"]:
         """
-        Continously watch the status stream and get updates on changes. This
-        can be used to attach to an ongoing installation.
+        Can be used to attach to the health monitoring status information of
+        the systen module
         """
 
         loop = asyncio.get_event_loop()
-        ait = self.async_watch_status(
+        ait = self.async_watch(
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
@@ -875,111 +648,14 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class Health(betterproto.ServiceStub):
-    """
-    The health service provides methods to monitor operational status of the
-    systen module
-    """
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the systen module"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.system.services.Health/Get",
-            request,
-            HealthGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the systen module"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """
-        Can be used to attach to the health monitoring status information of
-        the systen module
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.system.services.Health/Watch",
-            request,
-            HealthWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """
-        Can be used to attach to the health monitoring status information of
-        the systen module
-        """
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-
 class Network(betterproto.ServiceStub):
     """
     The network service allows to setup network configuration of Qb2 device.
     The exact structure of configuration settings is defined by "Network"
     protocol message. Service provides "SetConfig()" and "GetConfig()" API
     which allow to apply and read out configuration settings at run-time. The
     "GetStatus()" API brings configuration and statistical information about
@@ -1210,14 +886,338 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
+class Firmware(betterproto.ServiceStub):
+    """
+    The firmware service offers methods to fetch the currently installed
+    firmware, upgrade it, downgrade it and also configure auto-update
+    mechanisms.
+    """
+
+    async def async_upload(
+        self,
+        request_iterator: Union[
+            AsyncIterable["FirmwareUploadRequest"], Iterable["FirmwareUploadRequest"]
+        ],
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "FirmwareUploadResponse":
+        """
+        Upload the firmware bundle from the client to the device. Fails if the
+        uploaded firmware bundle is not valid.
+        """
+
+        return await self._stream_unary(
+            "/blickfeld.system.services.Firmware/Upload",
+            request_iterator,
+            FirmwareUploadRequest,
+            FirmwareUploadResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def upload(
+        self,
+        request_iterator: Iterable["FirmwareUploadRequest"],
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "FirmwareUploadResponse":
+        """
+        Upload the firmware bundle from the client to the device. Fails if the
+        uploaded firmware bundle is not valid.
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_upload(
+                request_iterator,
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_install(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["FirmwareInstallResponse"]:
+        """
+        Trigger the installation process of an uploaded firmware. A status
+        stream with the installation progress is returned and ends with
+        installation completion.
+        """
+
+        request = FirmwareInstallRequest()
+
+        async for response in self._unary_stream(
+            "/blickfeld.system.services.Firmware/Install",
+            request,
+            FirmwareInstallResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def install(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["FirmwareInstallResponse"]:
+        """
+        Trigger the installation process of an uploaded firmware. A status
+        stream with the installation progress is returned and ends with
+        installation completion.
+        """
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_install(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+    async def async_upload_and_install(
+        self,
+        request_iterator: Union[
+            AsyncIterable["FirmwareUploadAndInstallRequest"],
+            Iterable["FirmwareUploadAndInstallRequest"],
+        ],
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["FirmwareUploadAndInstallResponse"]:
+        """Combines the Upload and Install steps in a single method."""
+
+        async for response in self._stream_stream(
+            "/blickfeld.system.services.Firmware/UploadAndInstall",
+            request_iterator,
+            FirmwareUploadAndInstallRequest,
+            FirmwareUploadAndInstallResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def upload_and_install(
+        self,
+        request_iterator: Iterable["FirmwareUploadAndInstallRequest"],
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["FirmwareUploadAndInstallResponse"]:
+        """Combines the Upload and Install steps in a single method."""
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_upload_and_install(
+            request_iterator,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+    async def async_fetch_and_install(
+        self,
+        *,
+        version: "__base_data__.Version" = None,
+        url: str = "",
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> AsyncIterator["FirmwareFetchAndInstallResponse"]:
+        """
+        Fetch a firmware bundle from a static file server and perform
+        installation.
+        """
+
+        request = FirmwareFetchAndInstallRequest()
+        if version is not None:
+            request.version = version
+        request.url = url
+
+        async for response in self._unary_stream(
+            "/blickfeld.system.services.Firmware/FetchAndInstall",
+            request,
+            FirmwareFetchAndInstallResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def fetch_and_install(
+        self,
+        *,
+        version: "__base_data__.Version" = None,
+        url: str = "",
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None
+    ) -> Iterator["FirmwareFetchAndInstallResponse"]:
+        """
+        Fetch a firmware bundle from a static file server and perform
+        installation.
+        """
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_fetch_and_install(
+            version=version,
+            url=url,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+    async def async_get_status(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "FirmwareGetStatusResponse":
+        """
+        Get the current firmware status which includes the currently installed
+        firmware but also ongoing or failed installations.
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.system.services.Firmware/GetStatus",
+            request,
+            FirmwareGetStatusResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get_status(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "FirmwareGetStatusResponse":
+        """
+        Get the current firmware status which includes the currently installed
+        firmware but also ongoing or failed installations.
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get_status(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_watch_status(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["FirmwareWatchStatusResponse"]:
+        """
+        Continously watch the status stream and get updates on changes. This
+        can be used to attach to an ongoing installation.
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.system.services.Firmware/WatchStatus",
+            request,
+            FirmwareWatchStatusResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def watch_status(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["FirmwareWatchStatusResponse"]:
+        """
+        Continously watch the status stream and get updates on changes. This
+        can be used to attach to an ongoing installation.
+        """
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch_status(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+
 class TimeSynchronization(betterproto.ServiceStub):
     """
     This service provides methods to configure the time synchronization of the
     device.
     """
 
     async def async_set(
```

### Comparing `blickfeld_qb2-2.0.7/blickfeld_qb2.egg-info/SOURCES.txt` & `blickfeld_qb2-2.0.9/blickfeld_qb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-2.0.7/setup.py` & `blickfeld_qb2-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="blickfeld_qb2",
-    version="2.0.7",
+    version="2.0.9",
     author="Blickfeld GmbH",
     author_email="opensource@blickfeld.com",
     url="https://github.com/Blickfeld/blickfeld-qb2",
     description="Python package to communicate securely with Qb2 LiDAR devices of the Blickfeld GmbH",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

