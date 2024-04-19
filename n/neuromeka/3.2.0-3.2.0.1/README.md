# Comparing `tmp/neuromeka-3.2.0.tar.gz` & `tmp/neuromeka-3.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\neuromeka-3.2.0.tar", last modified: Wed Apr 17 11:34:19 2024, max compression
+gzip compressed data, was "dist\neuromeka-3.2.0.1.tar", last modified: Fri Apr 19 08:49:13 2024, max compression
```

## Comparing `neuromeka-3.2.0.tar` & `neuromeka-3.2.0.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 11:34:19.388546 neuromeka-3.2.0/
--rw-rw-rw-   0        0        0     2498 2024-04-17 11:34:19.386593 neuromeka-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2024-02-03 06:42:52.000000 neuromeka-3.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 11:34:19.218689 neuromeka-3.2.0/neuromeka/
--rw-rw-rw-   0        0        0      154 2024-02-06 01:40:52.000000 neuromeka-3.2.0/neuromeka/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:34:19.250896 neuromeka-3.2.0/neuromeka/common/
--rw-rw-rw-   0        0        0      181 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/__init__.py
--rw-rw-rw-   0        0        0     6513 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/config.py
--rw-rw-rw-   0        0        0     8426 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/dcp_addr.py
--rw-rw-rw-   0        0        0     6425 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/global_timer.py
--rw-rw-rw-   0        0        0     8441 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/jsmin.py
--rw-rw-rw-   0        0        0     2011 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/limits.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:34:19.274331 neuromeka-3.2.0/neuromeka/common/property/
--rw-rw-rw-   0        0        0      279 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/property/Application.py
--rw-rw-rw-   0        0        0     1142 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/property/Collision.py
--rw-rw-rw-   0        0        0      122 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/property/Log.py
--rw-rw-rw-   0        0        0      346 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/property/Modbus.py
--rw-rw-rw-   0        0        0     3596 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/property/Motion.py
--rw-rw-rw-   0        0        0       69 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/property/Timer.py
--rw-rw-rw-   0        0        0       46 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/property/TrackConveyor.py
--rw-rw-rw-   0        0        0      462 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/property/Vision.py
--rw-rw-rw-   0        0        0      189 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/property/__init__.py
--rw-rw-rw-   0        0        0     1270 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/singleton_meta.py
--rw-rw-rw-   0        0        0     6633 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/common/utils.py
--rw-rw-rw-   0        0        0    22419 2024-04-11 06:51:20.000000 neuromeka-3.2.0/neuromeka/ecat.py
--rw-rw-rw-   0        0        0    14598 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/eye.py
--rw-rw-rw-   0        0        0    10651 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/indy.py
--rw-rw-rw-   0        0        0    74641 2024-04-12 12:54:16.000000 neuromeka-3.2.0/neuromeka/indydcp3.py
--rw-rw-rw-   0        0        0    13503 2024-04-11 06:51:20.000000 neuromeka-3.2.0/neuromeka/moby.py
--rw-rw-rw-   0        0        0    43010 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/motor.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:34:19.384607 neuromeka-3.2.0/neuromeka/proto/
--rw-rw-rw-   0        0        0        0 2024-02-06 00:57:07.000000 neuromeka-3.2.0/neuromeka/proto/__init__.py
--rw-rw-rw-   0        0        0    25861 2024-04-12 12:54:38.000000 neuromeka-3.2.0/neuromeka/proto/common_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:38.000000 neuromeka-3.2.0/neuromeka/proto/common_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    74073 2024-04-12 12:54:36.000000 neuromeka-3.2.0/neuromeka/proto/config_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:36.000000 neuromeka-3.2.0/neuromeka/proto/config_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    22023 2024-04-12 12:54:35.000000 neuromeka-3.2.0/neuromeka/proto/config_pb2.py
--rw-rw-rw-   0        0        0    72800 2024-04-12 12:54:35.000000 neuromeka-3.2.0/neuromeka/proto/config_pb2_grpc.py
--rw-rw-rw-   0        0        0   177549 2024-04-12 12:54:35.000000 neuromeka-3.2.0/neuromeka/proto/control_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:35.000000 neuromeka-3.2.0/neuromeka/proto/control_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    32755 2024-04-12 12:54:34.000000 neuromeka-3.2.0/neuromeka/proto/control_pb2.py
--rw-rw-rw-   0        0        0   111431 2024-04-12 12:54:34.000000 neuromeka-3.2.0/neuromeka/proto/control_pb2_grpc.py
--rw-rw-rw-   0        0        0    40034 2024-04-12 12:54:34.000000 neuromeka-3.2.0/neuromeka/proto/device_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:34.000000 neuromeka-3.2.0/neuromeka/proto/device_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    12386 2024-04-12 12:54:33.000000 neuromeka-3.2.0/neuromeka/proto/device_pb2.py
--rw-rw-rw-   0        0        0    39962 2024-04-12 12:54:33.000000 neuromeka-3.2.0/neuromeka/proto/device_pb2_grpc.py
--rw-rw-rw-   0        0        0    77288 2024-04-12 12:54:41.000000 neuromeka-3.2.0/neuromeka/proto/ethercat_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:41.000000 neuromeka-3.2.0/neuromeka/proto/ethercat_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    19026 2024-04-12 12:54:40.000000 neuromeka-3.2.0/neuromeka/proto/ethercat_pb2.py
--rw-rw-rw-   0        0        0    62864 2024-04-12 12:54:40.000000 neuromeka-3.2.0/neuromeka/proto/ethercat_pb2_grpc.py
--rw-rw-rw-   0        0        0    21736 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/proto/eyetask_pb2.py
--rw-rw-rw-   0        0        0     6787 2024-02-03 06:42:52.000000 neuromeka-3.2.0/neuromeka/proto/eyetask_pb2_grpc.py
--rw-rw-rw-   0        0        0      318 2024-02-06 01:43:37.000000 neuromeka-3.2.0/neuromeka/proto/grpc_wrapper.py
--rw-rw-rw-   0        0        0    17034 2024-04-12 12:54:37.000000 neuromeka-3.2.0/neuromeka/proto/linear_pb2.py
--rw-rw-rw-   0        0        0    10079 2024-04-12 12:54:37.000000 neuromeka-3.2.0/neuromeka/proto/linear_pb2_grpc.py
--rw-rw-rw-   0        0        0    73955 2024-04-12 12:54:42.000000 neuromeka-3.2.0/neuromeka/proto/moby_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:42.000000 neuromeka-3.2.0/neuromeka/proto/moby_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    16769 2024-04-12 12:54:41.000000 neuromeka-3.2.0/neuromeka/proto/moby_pb2.py
--rw-rw-rw-   0        0        0    55494 2024-04-12 12:54:41.000000 neuromeka-3.2.0/neuromeka/proto/moby_pb2_grpc.py
--rw-rw-rw-   0        0        0    12567 2024-04-12 12:54:38.000000 neuromeka-3.2.0/neuromeka/proto/plotting_pb2.py
--rw-rw-rw-   0        0        0     2569 2024-04-12 12:54:38.000000 neuromeka-3.2.0/neuromeka/proto/plotting_pb2_grpc.py
--rw-rw-rw-   0        0        0    45795 2024-04-12 12:54:37.000000 neuromeka-3.2.0/neuromeka/proto/rtde_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:37.000000 neuromeka-3.2.0/neuromeka/proto/rtde_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0     4929 2024-04-12 12:54:36.000000 neuromeka-3.2.0/neuromeka/proto/rtde_pb2.py
--rw-rw-rw-   0        0        0    13289 2024-04-12 12:54:36.000000 neuromeka-3.2.0/neuromeka/proto/rtde_pb2_grpc.py
--rw-rw-rw-   0        0        0    87158 2024-04-12 12:54:40.000000 neuromeka-3.2.0/neuromeka/proto/shared_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2024-04-12 12:54:40.000000 neuromeka-3.2.0/neuromeka/proto/shared_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0     6467 2024-04-12 12:54:42.000000 neuromeka-3.2.0/neuromeka/proto/teleop_dev_pb2.py
--rw-rw-rw-   0        0        0     4133 2024-04-12 12:54:42.000000 neuromeka-3.2.0/neuromeka/proto/teleop_dev_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:34:19.228457 neuromeka-3.2.0/neuromeka.egg-info/
--rw-rw-rw-   0        0        0     2498 2024-04-17 11:34:19.000000 neuromeka-3.2.0/neuromeka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2205 2024-04-17 11:34:19.000000 neuromeka-3.2.0/neuromeka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 11:34:19.000000 neuromeka-3.2.0/neuromeka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-04-17 11:34:19.000000 neuromeka-3.2.0/neuromeka.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 11:34:19.000000 neuromeka-3.2.0/neuromeka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 11:34:19.388546 neuromeka-3.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1249 2024-04-17 07:40:03.000000 neuromeka-3.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.207540 neuromeka-3.2.0.1/
+-rw-rw-rw-   0        0        0     2500 2024-04-19 08:49:13.205583 neuromeka-3.2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.037712 neuromeka-3.2.0.1/neuromeka/
+-rw-rw-rw-   0        0        0      152 2024-04-19 05:41:11.000000 neuromeka-3.2.0.1/neuromeka/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.070900 neuromeka-3.2.0.1/neuromeka/common/
+-rw-rw-rw-   0        0        0      181 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/__init__.py
+-rw-rw-rw-   0        0        0     6513 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/config.py
+-rw-rw-rw-   0        0        0     8426 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/dcp_addr.py
+-rw-rw-rw-   0        0        0     6425 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/global_timer.py
+-rw-rw-rw-   0        0        0     8441 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/jsmin.py
+-rw-rw-rw-   0        0        0     2011 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/limits.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.094324 neuromeka-3.2.0.1/neuromeka/common/property/
+-rw-rw-rw-   0        0        0      279 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Application.py
+-rw-rw-rw-   0        0        0     1142 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Collision.py
+-rw-rw-rw-   0        0        0      122 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Log.py
+-rw-rw-rw-   0        0        0      346 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Modbus.py
+-rw-rw-rw-   0        0        0     3596 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Motion.py
+-rw-rw-rw-   0        0        0       69 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Timer.py
+-rw-rw-rw-   0        0        0       46 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/TrackConveyor.py
+-rw-rw-rw-   0        0        0      462 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/Vision.py
+-rw-rw-rw-   0        0        0      189 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/property/__init__.py
+-rw-rw-rw-   0        0        0     1270 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/singleton_meta.py
+-rw-rw-rw-   0        0        0     6633 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/common/utils.py
+-rw-rw-rw-   0        0        0    22419 2024-04-11 06:51:20.000000 neuromeka-3.2.0.1/neuromeka/ecat.py
+-rw-rw-rw-   0        0        0    14613 2024-04-19 06:35:19.000000 neuromeka-3.2.0.1/neuromeka/eye.py
+-rw-rw-rw-   0        0        0    10651 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/indy.py
+-rw-rw-rw-   0        0        0    74641 2024-04-12 12:54:16.000000 neuromeka-3.2.0.1/neuromeka/indydcp3.py
+-rw-rw-rw-   0        0        0    13503 2024-04-11 06:51:20.000000 neuromeka-3.2.0.1/neuromeka/moby.py
+-rw-rw-rw-   0        0        0    43010 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/motor.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.202659 neuromeka-3.2.0.1/neuromeka/proto/
+-rw-rw-rw-   0        0        0        0 2024-02-06 00:57:07.000000 neuromeka-3.2.0.1/neuromeka/proto/__init__.py
+-rw-rw-rw-   0        0        0    25861 2024-04-12 12:54:38.000000 neuromeka-3.2.0.1/neuromeka/proto/common_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:38.000000 neuromeka-3.2.0.1/neuromeka/proto/common_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    74073 2024-04-12 12:54:36.000000 neuromeka-3.2.0.1/neuromeka/proto/config_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:36.000000 neuromeka-3.2.0.1/neuromeka/proto/config_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    22023 2024-04-12 12:54:35.000000 neuromeka-3.2.0.1/neuromeka/proto/config_pb2.py
+-rw-rw-rw-   0        0        0    72800 2024-04-12 12:54:35.000000 neuromeka-3.2.0.1/neuromeka/proto/config_pb2_grpc.py
+-rw-rw-rw-   0        0        0   177549 2024-04-12 12:54:35.000000 neuromeka-3.2.0.1/neuromeka/proto/control_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:35.000000 neuromeka-3.2.0.1/neuromeka/proto/control_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    32755 2024-04-12 12:54:34.000000 neuromeka-3.2.0.1/neuromeka/proto/control_pb2.py
+-rw-rw-rw-   0        0        0   111431 2024-04-12 12:54:34.000000 neuromeka-3.2.0.1/neuromeka/proto/control_pb2_grpc.py
+-rw-rw-rw-   0        0        0    40034 2024-04-12 12:54:34.000000 neuromeka-3.2.0.1/neuromeka/proto/device_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:34.000000 neuromeka-3.2.0.1/neuromeka/proto/device_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12386 2024-04-12 12:54:33.000000 neuromeka-3.2.0.1/neuromeka/proto/device_pb2.py
+-rw-rw-rw-   0        0        0    39962 2024-04-12 12:54:33.000000 neuromeka-3.2.0.1/neuromeka/proto/device_pb2_grpc.py
+-rw-rw-rw-   0        0        0    77288 2024-04-12 12:54:41.000000 neuromeka-3.2.0.1/neuromeka/proto/ethercat_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:41.000000 neuromeka-3.2.0.1/neuromeka/proto/ethercat_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    19026 2024-04-12 12:54:40.000000 neuromeka-3.2.0.1/neuromeka/proto/ethercat_pb2.py
+-rw-rw-rw-   0        0        0    62864 2024-04-12 12:54:40.000000 neuromeka-3.2.0.1/neuromeka/proto/ethercat_pb2_grpc.py
+-rw-rw-rw-   0        0        0    21736 2024-02-03 06:42:52.000000 neuromeka-3.2.0.1/neuromeka/proto/eyetask_pb2.py
+-rw-rw-rw-   0        0        0     6780 2024-04-19 05:39:52.000000 neuromeka-3.2.0.1/neuromeka/proto/eyetask_pb2_grpc.py
+-rw-rw-rw-   0        0        0      318 2024-02-06 01:43:37.000000 neuromeka-3.2.0.1/neuromeka/proto/grpc_wrapper.py
+-rw-rw-rw-   0        0        0    17034 2024-04-12 12:54:37.000000 neuromeka-3.2.0.1/neuromeka/proto/linear_pb2.py
+-rw-rw-rw-   0        0        0    10079 2024-04-12 12:54:37.000000 neuromeka-3.2.0.1/neuromeka/proto/linear_pb2_grpc.py
+-rw-rw-rw-   0        0        0    73955 2024-04-12 12:54:42.000000 neuromeka-3.2.0.1/neuromeka/proto/moby_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:42.000000 neuromeka-3.2.0.1/neuromeka/proto/moby_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    16769 2024-04-12 12:54:41.000000 neuromeka-3.2.0.1/neuromeka/proto/moby_pb2.py
+-rw-rw-rw-   0        0        0    55494 2024-04-12 12:54:41.000000 neuromeka-3.2.0.1/neuromeka/proto/moby_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12567 2024-04-12 12:54:38.000000 neuromeka-3.2.0.1/neuromeka/proto/plotting_pb2.py
+-rw-rw-rw-   0        0        0     2569 2024-04-12 12:54:38.000000 neuromeka-3.2.0.1/neuromeka/proto/plotting_pb2_grpc.py
+-rw-rw-rw-   0        0        0    45795 2024-04-12 12:54:37.000000 neuromeka-3.2.0.1/neuromeka/proto/rtde_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:37.000000 neuromeka-3.2.0.1/neuromeka/proto/rtde_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4929 2024-04-12 12:54:36.000000 neuromeka-3.2.0.1/neuromeka/proto/rtde_pb2.py
+-rw-rw-rw-   0        0        0    13289 2024-04-12 12:54:36.000000 neuromeka-3.2.0.1/neuromeka/proto/rtde_pb2_grpc.py
+-rw-rw-rw-   0        0        0    87158 2024-04-12 12:54:40.000000 neuromeka-3.2.0.1/neuromeka/proto/shared_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2024-04-12 12:54:40.000000 neuromeka-3.2.0.1/neuromeka/proto/shared_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6467 2024-04-12 12:54:42.000000 neuromeka-3.2.0.1/neuromeka/proto/teleop_dev_pb2.py
+-rw-rw-rw-   0        0        0     4133 2024-04-12 12:54:42.000000 neuromeka-3.2.0.1/neuromeka/proto/teleop_dev_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:49:13.048449 neuromeka-3.2.0.1/neuromeka.egg-info/
+-rw-rw-rw-   0        0        0     2500 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2205 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 08:49:12.000000 neuromeka-3.2.0.1/neuromeka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:49:13.207540 neuromeka-3.2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1251 2024-04-19 08:47:40.000000 neuromeka-3.2.0.1/setup.py
```

### Comparing `neuromeka-3.2.0/PKG-INFO` & `neuromeka-3.2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromeka
-Version: 3.2.0
+Version: 3.2.0.1
 Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients3
 Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuromeka-3.2.0/README.md` & `neuromeka-3.2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/common/config.py` & `neuromeka-3.2.0.1/neuromeka/common/config.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/common/dcp_addr.py` & `neuromeka-3.2.0.1/neuromeka/common/dcp_addr.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/common/global_timer.py` & `neuromeka-3.2.0.1/neuromeka/common/global_timer.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/common/jsmin.py` & `neuromeka-3.2.0.1/neuromeka/common/jsmin.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/common/limits.py` & `neuromeka-3.2.0.1/neuromeka/common/limits.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/common/property/Collision.py` & `neuromeka-3.2.0.1/neuromeka/common/property/Collision.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/common/property/Motion.py` & `neuromeka-3.2.0.1/neuromeka/common/property/Motion.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/common/singleton_meta.py` & `neuromeka-3.2.0.1/neuromeka/common/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/common/utils.py` & `neuromeka-3.2.0.1/neuromeka/common/utils.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/ecat.py` & `neuromeka-3.2.0.1/neuromeka/ecat.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/eye.py` & `neuromeka-3.2.0.1/neuromeka/eye.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import json
 import socket
 from io import BytesIO
 import pickle
 import time
 
 import grpc
-from .proto.EyeTask_pb2_grpc import EyeTaskStub
-from .proto import EyeTask_pb2
+from .proto.eyetask_pb2_grpc import EyeTaskStub
+from .proto import eyetask_pb2 as EyeTask_pb2
 
 ConnectUI = '/main/connect'
 GetVersion = '/main/version'
 GetApp = '/main/app'
 RobotStatus = '/main/robot/status'
 DisplayImage = '/main/robot/image'
 ImageSize = '/main/robot/image/size'
```

### Comparing `neuromeka-3.2.0/neuromeka/indy.py` & `neuromeka-3.2.0.1/neuromeka/indy.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/indydcp3.py` & `neuromeka-3.2.0.1/neuromeka/indydcp3.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/moby.py` & `neuromeka-3.2.0.1/neuromeka/moby.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/motor.py` & `neuromeka-3.2.0.1/neuromeka/motor.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/common_msgs_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/common_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/config_msgs_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/config_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/config_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/config_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/config_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/control_msgs_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/control_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/control_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/control_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/control_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/control_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/device_msgs_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/device_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/device_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/device_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/device_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/ethercat_msgs_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/ethercat_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/ethercat_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/ethercat_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/ethercat_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/ethercat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/eyetask_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/eyetask_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/eyetask_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/eyetask_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import eyetask_pb2 as eyetask__pb2
+import eyetask_pb2 as eyetask__pb2
 
 
 class EyeTaskStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `neuromeka-3.2.0/neuromeka/proto/linear_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/linear_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/linear_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/linear_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/moby_msgs_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/moby_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/moby_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/moby_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/moby_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/moby_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/plotting_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/plotting_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/plotting_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/plotting_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/rtde_msgs_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/rtde_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/rtde_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/rtde_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/rtde_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/rtde_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/shared_msgs_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/shared_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/teleop_dev_pb2.py` & `neuromeka-3.2.0.1/neuromeka/proto/teleop_dev_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka/proto/teleop_dev_pb2_grpc.py` & `neuromeka-3.2.0.1/neuromeka/proto/teleop_dev_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/neuromeka.egg-info/PKG-INFO` & `neuromeka-3.2.0.1/neuromeka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromeka
-Version: 3.2.0
+Version: 3.2.0.1
 Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients3
 Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuromeka-3.2.0/neuromeka.egg-info/SOURCES.txt` & `neuromeka-3.2.0.1/neuromeka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuromeka-3.2.0/setup.py` & `neuromeka-3.2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="neuromeka",
-    version="3.2.0",
+    version="3.2.0.1",
     author="Neuromeka",
     author_email="youngjin.heo@neuromeka.com",
     description="Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/neuromeka-robotics/neuromeka-clients3",
     packages=find_packages(),
```

