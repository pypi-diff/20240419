# Comparing `tmp/ni_measurementlink_service-1.4.0.dev1.tar.gz` & `tmp/ni_measurementlink_service-1.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_service-1.4.0.dev1.tar", max compression
+gzip compressed data, was "ni_measurementlink_service-1.5.0.dev0.tar", max compression
```

## Comparing `ni_measurementlink_service-1.4.0.dev1.tar` & `ni_measurementlink_service-1.5.0.dev0.tar`

### file list

```diff
@@ -1,102 +1,101 @@
--rw-r--r--   0        0        0     1071 2024-03-08 14:27:02.753118 ni_measurementlink_service-1.4.0.dev1/LICENSE
--rw-r--r--   0        0        0    17180 2024-03-08 14:27:02.753118 ni_measurementlink_service-1.4.0.dev1/README.md
--rw-r--r--   0        0        0      513 2024-03-08 14:27:02.765118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/__init__.py
--rw-r--r--   0        0        0      187 2024-03-08 14:27:02.765118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_annotations.py
--rw-r--r--   0        0        0     3843 2024-03-08 14:27:02.765118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_configuration.py
--rw-r--r--   0        0        0     3323 2024-03-08 14:27:02.765118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_datatypeinfo.py
--rw-r--r--   0        0        0     2724 2024-03-08 14:27:02.765118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_dotenvpath.py
--rw-r--r--   0        0        0     1667 2024-03-08 14:27:02.765118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/__init__.py
--rw-r--r--   0        0        0     3359 2024-03-08 14:27:02.765118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_grpcdevice.py
--rw-r--r--   0        0        0     2226 2024-03-08 14:27:02.765118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nidaqmx.py
--rw-r--r--   0        0        0     2577 2024-03-08 14:27:02.765118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nidcpower.py
--rw-r--r--   0        0        0     2662 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nidigital.py
--rw-r--r--   0        0        0     2614 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nidmm.py
--rw-r--r--   0        0        0     2576 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nifgen.py
--rw-r--r--   0        0        0     2638 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_niscope.py
--rw-r--r--   0        0        0     3377 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_niswitch.py
--rw-r--r--   0        0        0     4666 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_featuretoggles.py
--rw-r--r--   0        0        0       62 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/__init__.py
--rw-r--r--   0        0        0      558 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/discovery_client.py
--rw-r--r--   0        0        0    15671 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/grpc_servicer.py
--rw-r--r--   0        0        0       58 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/__init__.py
--rw-r--r--   0        0        0     6575 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/_message.py
--rw-r--r--   0        0        0      933 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/_serializer_types.py
--rw-r--r--   0        0        0     5621 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/metadata.py
--rw-r--r--   0        0        0     9948 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
--rw-r--r--   0        0        0     8515 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/serializer.py
--rw-r--r--   0        0        0     5555 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/service_manager.py
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/__init__.py
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/__init__.py
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
--rw-r--r--   0        0        0     4742 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
--rw-r--r--   0        0        0    10451 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
--rw-r--r--   0        0        0    10817 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
--rw-r--r--   0        0        0     9907 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.pyi
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
--rw-r--r--   0        0        0     5345 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
--rw-r--r--   0        0        0    13678 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
--rw-r--r--   0        0        0     5546 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
--rw-r--r--   0        0        0     3783 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.pyi
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/__init__.py
--rw-r--r--   0        0        0     5861 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py
--rw-r--r--   0        0        0    15950 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi
--rw-r--r--   0        0        0     5549 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py
--rw-r--r--   0        0        0     3815 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     1532 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
--rw-r--r--   0        0        0     1314 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.pyi
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
--rw-r--r--   0        0        0     7166 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
--rw-r--r--   0        0        0    20974 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
--rw-r--r--   0        0        0    14078 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
--rw-r--r--   0        0        0    10884 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.pyi
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
--rw-r--r--   0        0        0    10207 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
--rw-r--r--   0        0        0    24186 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
--rw-r--r--   0        0        0    23860 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    19345 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.pyi
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/protobuf/__init__.py
--rw-r--r--   0        0        0       33 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/__init__.py
--rw-r--r--   0        0        0     1474 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.py
--rw-r--r--   0        0        0     1563 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2_grpc.py
--rw-r--r--   0        0        0      540 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2_grpc.pyi
--rw-r--r--   0        0        0      709 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/README.md
--rw-r--r--   0        0        0     6729 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
--rw-r--r--   0        0        0     6650 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
--rw-r--r--   0        0        0     7826 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto
--rw-r--r--   0        0        0      712 2024-03-08 14:27:02.769118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
--rw-r--r--   0        0        0    10349 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
--rw-r--r--   0        0        0    13150 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
--rw-r--r--   0        0        0     1109 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/protobuf/types/xydata.proto
--rw-r--r--   0        0        0     2426 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/session.proto
--rw-r--r--   0        0        0     4196 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.py
--rw-r--r--   0        0        0     8735 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
--rw-r--r--   0        0        0     8948 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
--rw-r--r--   0        0        0     4720 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.pyi
--rw-r--r--   0        0        0     7396 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_tracelogging.py
--rw-r--r--   0        0        0      266 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/discovery/__init__.py
--rw-r--r--   0        0        0     9177 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/discovery/_client.py
--rw-r--r--   0        0        0     6430 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/discovery/_support.py
--rw-r--r--   0        0        0      634 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/discovery/_types.py
--rw-r--r--   0        0        0       23 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/grpc/__init__.py
--rw-r--r--   0        0        0     2262 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/grpc/channelpool.py
--rw-r--r--   0        0        0    17549 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/grpc/loggers.py
--rw-r--r--   0        0        0       37 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/measurement/__init__.py
--rw-r--r--   0        0        0     2927 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/measurement/info.py
--rw-r--r--   0        0        0    22489 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/measurement/service.py
--rw-r--r--   0        0        0        0 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/py.typed
--rw-r--r--   0        0        0     3141 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/__init__.py
--rw-r--r--   0        0        0    17084 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/_client.py
--rw-r--r--   0        0        0     1243 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/_constants.py
--rw-r--r--   0        0        0   111102 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/_reservation.py
--rw-r--r--   0        0        0    18001 2024-03-08 14:27:02.773118 ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/_types.py
--rw-r--r--   0        0        0     5360 2024-03-08 14:27:20.521209 ni_measurementlink_service-1.4.0.dev1/pyproject.toml
--rw-r--r--   0        0        0    21065 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.4.0.dev1/setup.py
--rw-r--r--   0        0        0    19356 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.4.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-19 19:40:07.036515 ni_measurementlink_service-1.5.0.dev0/LICENSE
+-rw-r--r--   0        0        0    17206 2024-04-19 19:40:07.036515 ni_measurementlink_service-1.5.0.dev0/README.md
+-rw-r--r--   0        0        0      513 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_annotations.py
+-rw-r--r--   0        0        0     3843 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_configuration.py
+-rw-r--r--   0        0        0     3567 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_datatypeinfo.py
+-rw-r--r--   0        0        0     2724 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_dotenvpath.py
+-rw-r--r--   0        0        0     1667 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/__init__.py
+-rw-r--r--   0        0        0     3359 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_grpcdevice.py
+-rw-r--r--   0        0        0     2226 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nidaqmx.py
+-rw-r--r--   0        0        0     2577 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nidcpower.py
+-rw-r--r--   0        0        0     2662 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nidigital.py
+-rw-r--r--   0        0        0     2614 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nidmm.py
+-rw-r--r--   0        0        0     2576 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nifgen.py
+-rw-r--r--   0        0        0     2638 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_niscope.py
+-rw-r--r--   0        0        0     3377 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_niswitch.py
+-rw-r--r--   0        0        0     4564 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_featuretoggles.py
+-rw-r--r--   0        0        0       62 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/__init__.py
+-rw-r--r--   0        0        0      558 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/discovery_client.py
+-rw-r--r--   0        0        0    15671 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/grpc_servicer.py
+-rw-r--r--   0        0        0       58 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/__init__.py
+-rw-r--r--   0        0        0     6575 2024-04-19 19:40:07.048515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/_message.py
+-rw-r--r--   0        0        0      933 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/_serializer_types.py
+-rw-r--r--   0        0        0     5621 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/metadata.py
+-rw-r--r--   0        0        0     9948 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
+-rw-r--r--   0        0        0     8515 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/serializer.py
+-rw-r--r--   0        0        0     5555 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/service_manager.py
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
+-rw-r--r--   0        0        0     4742 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
+-rw-r--r--   0        0        0    10134 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
+-rw-r--r--   0        0        0    10817 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9929 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
+-rw-r--r--   0        0        0     5345 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
+-rw-r--r--   0        0        0    13333 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5546 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3799 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/__init__.py
+-rw-r--r--   0        0        0     5861 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py
+-rw-r--r--   0        0        0    15584 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5549 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3831 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1532 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
+-rw-r--r--   0        0        0     1191 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
+-rw-r--r--   0        0        0      413 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
+-rw-r--r--   0        0        0     7166 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
+-rw-r--r--   0        0        0    20479 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
+-rw-r--r--   0        0        0    14078 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10912 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
+-rw-r--r--   0        0        0    10207 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
+-rw-r--r--   0        0        0    23596 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23860 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    19382 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/__init__.py
+-rw-r--r--   0        0        0     1474 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.py
+-rw-r--r--   0        0        0     1439 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2_grpc.py
+-rw-r--r--   0        0        0      553 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2_grpc.pyi
+-rw-r--r--   0        0        0      709 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/README.md
+-rw-r--r--   0        0        0     6729 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
+-rw-r--r--   0        0        0     6650 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
+-rw-r--r--   0        0        0     7826 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto
+-rw-r--r--   0        0        0      704 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
+-rw-r--r--   0        0        0    10059 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
+-rw-r--r--   0        0        0    12818 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
+-rw-r--r--   0        0        0     1105 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/protobuf/types/xydata.proto
+-rw-r--r--   0        0        0     2426 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/session.proto
+-rw-r--r--   0        0        0     4196 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.py
+-rw-r--r--   0        0        0     8461 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
+-rw-r--r--   0        0        0     8948 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
+-rw-r--r--   0        0        0     4745 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7396 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_tracelogging.py
+-rw-r--r--   0        0        0      266 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/discovery/__init__.py
+-rw-r--r--   0        0        0     9177 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/discovery/_client.py
+-rw-r--r--   0        0        0     6430 2024-04-19 19:40:07.052515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/discovery/_support.py
+-rw-r--r--   0        0        0      634 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/discovery/_types.py
+-rw-r--r--   0        0        0       23 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/grpc/__init__.py
+-rw-r--r--   0        0        0     2262 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/grpc/channelpool.py
+-rw-r--r--   0        0        0    17322 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/grpc/loggers.py
+-rw-r--r--   0        0        0       37 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/measurement/__init__.py
+-rw-r--r--   0        0        0     3005 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/measurement/info.py
+-rw-r--r--   0        0        0    23522 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/measurement/service.py
+-rw-r--r--   0        0        0        0 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/py.typed
+-rw-r--r--   0        0        0     3141 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/__init__.py
+-rw-r--r--   0        0        0    16866 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/_client.py
+-rw-r--r--   0        0        0     1243 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/_constants.py
+-rw-r--r--   0        0        0   109789 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/_reservation.py
+-rw-r--r--   0        0        0    18001 2024-04-19 19:40:07.056515 ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/_types.py
+-rw-r--r--   0        0        0     5546 2024-04-19 19:40:21.172610 ni_measurementlink_service-1.5.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    19442 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.5.0.dev0/PKG-INFO
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/LICENSE` & `ni_measurementlink_service-1.5.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/README.md` & `ni_measurementlink_service-1.5.0.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,18 @@
   - [Developing Measurements: Quick Start](#developing-measurements-quick-start)
     - [Installation](#installation)
     - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)
   - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)
   - [Static Registration of Python Measurements](#static-registration-of-python-measurements)
     - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)
     - [Create Executable for Python Scripts](#create-executable-for-python-scripts)
-  - [Appendix: Managing Measurement as Python Package (Project)](#appendix-managing-measurement-as-python-package-project)
-    - [Create and Manage Python Measurement Package using Poetry](#create-and-manage-python-measurement-package-using-poetry)
-    - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)
-    - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)
+  - [Appendix: Managing Measurement with Python](#appendix-managing-measurement-with-python)
+    - [Create and Manage Python Measurement using Poetry](#create-and-manage-python-measurement-using-poetry)
+    - [Create and Manage Python Measurement using `venv`](#create-and-manage-python-measurement-using-venv)
+    - [Create and Manage Python Measurement by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)
 
 ---
 
 ## Introduction
 
 MeasurementLink Support for Python (`ni-measurementlink-service`) is a Python
 framework that helps you create reusable measurement plug-ins using gRPC
@@ -66,14 +66,16 @@
 you are using a previous version of MeasurementLink, download the appropriate examples:
 
 - MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
 - MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
 - MeasurementLink 2023 Q3: [measurementlink-python-examples-1.1.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.1.0/measurementlink-python-examples-1.1.0.zip)
 - MeasurementLink 2023 Q4: [measurementlink-python-examples-1.2.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.2.0/measurementlink-python-examples-1.2.0.zip)
 - MeasurementLink 2024 Q1: [measurementlink-python-examples-1.3.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.3.0/measurementlink-python-examples-1.3.0.zip)
+- MeasurementLink 2024 Q2: [measurementlink-python-examples-1.4.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.4.0/measurementlink-python-examples-1.4.0.zip)
+
 
 For more information on setting up and running the example measurements, see the included `README.md` file.
 
 For best results, use the example measurements corresponding to the version of MeasurementLink
 that you are using. Newer examples may demonstrate features that are not available in older
 versions of MeasurementLink.
 
@@ -158,15 +160,15 @@
 
 ---
 
 ## Steps to run/debug the measurement service
 
 1. Start the discovery service if not already started.
 
-2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)
+2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-using-poetry)
 
     ```cmd
     .venv\scripts\activate
     ```
 
     - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.
     - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:
@@ -175,15 +177,15 @@
         Set-ExecutionPolicy RemoteSigned 
         ```
 
 3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.
 
 4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.
 
-5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)
+5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-using-poetry)
 
     ```cmd
     deactivate
     ```
 
 ---
 
@@ -243,31 +245,31 @@
 
 ## Troubleshooting
 
 ### "File not found" or "No such file or directory" errors when copying or running a measurement service
 
 If copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.
 
-## Appendix: Managing Measurement as Python Package (Project)
+## Appendix: Managing Measurement with Python
 
-Measurement and its related files can be maintained as a Python package. The basic components of any Python measurement package are:
+A measurement and its related files can be maintained in different ways in Python. The basic components of any Python measurement are:
 
 1. Measurement Python module (`.py` file)
     - This file contains all the details related to the measurement and also contains the logic for the measurement execution.
     - This file is run to start the measurement as a service.
 
 2. UI File
     - UI file for the measurement. Types of supported UI files are:
         - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.
         - LabVIEW UI (`.vi`)
     - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).
 
-Python communities have different ways of managing Python packages and their dependencies. It is up to the measurement developer to decide how to maintain the package and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.
+Python communities have different ways of managing Python projects and their dependencies. It is up to the measurement developer to decide how to maintain the project and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.
 
-### Create and Manage Python Measurement Package using Poetry
+### Create and Manage Python Measurement using Poetry
 
 1. Install `poetry` (one-time setup)
 
     1. Make sure the system has the recommended Python version installed.
 
     2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.
 
@@ -275,15 +277,15 @@
 
     1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.
 
         ``` cmd
         cd <path_of_directory_of_your_choice>
         ```
 
-    2. Create a Python package (project) using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.
+    2. Create a Poetry project using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.
 
         ``` cmd
         poetry new <name_of_the_project>
         ```
 
     3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.
 
@@ -299,15 +301,15 @@
 
             ``` cmd
             poetry add <dependency_package_name>
             ```
 
 For detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).
 
-### Create and Manage Python Measurement Package using `venv`
+### Create and Manage Python Measurement using `venv`
 
 1. Make sure the system has the recommended Python version installed.
 
 2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.
 
     ``` cmd
     cd <path_of_directory_of_your_choice>
@@ -339,15 +341,15 @@
 
         ``` cmd
         pip install <dependency_package_name>
         ```
 
 For detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).
 
-### Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package
+### Create and Manage Python Measurement by directly installing `ni-measurementlink-service` as a system-level package
 
 Measurement developers can also install `ni-measurementlink-service` as a system package if necessary.
 
 1. Install the `ni-measurementlink-service` package from the command prompt
 
     ``` cmd
     pip install ni-measurementlink-service
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/__init__.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/__init__.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_configuration.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_configuration.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_datatypeinfo.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_datatypeinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     DataType.Path: DataTypeInfo(type_pb2.Field.TYPE_STRING, False, TypeSpecialization.Path),
     DataType.Enum: DataTypeInfo(type_pb2.Field.TYPE_ENUM, False, TypeSpecialization.Enum),
     DataType.DoubleXYData: DataTypeInfo(
         type_pb2.Field.TYPE_MESSAGE,
         False,
         message_type=xydata_pb2.DoubleXYData.DESCRIPTOR.full_name,
     ),
+    DataType.IOResource: DataTypeInfo(
+        type_pb2.Field.TYPE_STRING, False, TypeSpecialization.IOResource
+    ),
     DataType.Int32Array1D: DataTypeInfo(type_pb2.Field.TYPE_INT32, True),
     DataType.Int64Array1D: DataTypeInfo(type_pb2.Field.TYPE_INT64, True),
     DataType.UInt32Array1D: DataTypeInfo(type_pb2.Field.TYPE_UINT32, True),
     DataType.UInt64Array1D: DataTypeInfo(type_pb2.Field.TYPE_UINT64, True),
     DataType.FloatArray1D: DataTypeInfo(type_pb2.Field.TYPE_FLOAT, True),
     DataType.DoubleArray1D: DataTypeInfo(type_pb2.Field.TYPE_DOUBLE, True),
     DataType.BooleanArray1D: DataTypeInfo(type_pb2.Field.TYPE_BOOL, True),
@@ -63,8 +66,11 @@
     DataType.PathArray1D: DataTypeInfo(type_pb2.Field.TYPE_STRING, True, TypeSpecialization.Path),
     DataType.EnumArray1D: DataTypeInfo(type_pb2.Field.TYPE_ENUM, True, TypeSpecialization.Enum),
     DataType.DoubleXYDataArray1D: DataTypeInfo(
         type_pb2.Field.TYPE_MESSAGE,
         True,
         message_type=xydata_pb2.DoubleXYData.DESCRIPTOR.full_name,
     ),
+    DataType.IOResourceArray1D: DataTypeInfo(
+        type_pb2.Field.TYPE_STRING, True, TypeSpecialization.IOResource
+    ),
 }
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_dotenvpath.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_dotenvpath.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/__init__.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_grpcdevice.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_grpcdevice.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nidaqmx.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nidaqmx.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nidcpower.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nidcpower.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nidigital.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nidigital.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nidmm.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nidmm.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_nifgen.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_nifgen.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_niscope.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_niscope.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_drivers/_niswitch.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_drivers/_niswitch.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_featuretoggles.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_featuretoggles.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,9 +142,7 @@
 
     return decorator
 
 
 # --------------------------------------
 # Define feature toggle constants here:
 # --------------------------------------
-
-MULTIPLEXER_SUPPORT_2024Q2 = FeatureToggle("MULTIPLEXER_SUPPORT_2024Q2", CodeReadiness.NEXT_RELEASE)
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/discovery_client.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/discovery_client.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/grpc_servicer.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/grpc_servicer.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/_message.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/_message.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/_serializer_types.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/_serializer_types.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/metadata.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/metadata.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/serialization_strategy.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/serialization_strategy.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/parameter/serializer.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/parameter/serializer.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/service_manager.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/service_manager.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 ---------------------------------------------------------------------
 ---------------------------------------------------------------------
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ServiceDescriptor(google.protobuf.message.Message):
     """Description of a registered service. This information can be used to display information to the user
     about the service when services are being developed for a plugin architecture
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class AnnotationsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     DESCRIPTION_URL_FIELD_NUMBER: builtins.int
     PROVIDED_INTERFACES_FIELD_NUMBER: builtins.int
     SERVICE_CLASS_FIELD_NUMBER: builtins.int
     ANNOTATIONS_FIELD_NUMBER: builtins.int
     display_name: builtins.str
     """Required. The user visible name of the service."""
     description_url: builtins.str
     """Optional. Url which provides descriptive information about the service"""
+    service_class: builtins.str
+    """Required. The "class" of a service. The value of this field should be unique for a given interface in provided_interfaces.
+    In effect, the .proto service declaration defines the interface, and this field defines a class or concrete type of the interface.
+    """
     @property
     def provided_interfaces(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Required. The service interfaces provided by the service. This is the gRPC Full Name of the service.
         Registration can use the gRPC metadata to provide these names.
         """
-    service_class: builtins.str
-    """Required. The "class" of a service. The value of this field should be unique for a given interface in provided_interfaces.
-    In effect, the .proto service declaration defines the interface, and this field defines a class or concrete type of the interface.
-    """
+
     @property
     def annotations(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Optional. Represents a set of annotations on the service.
         Well-known annotations:
         - Description
           - Key: "ni/service.description"
           - Expected format: string
@@ -73,28 +70,29 @@
           - Expected format: "." delimited namespace/hierarchy case-insensitive string
           - Example: "CurrentTests.Inrush"
         - Tags
           - Key: "ni/service.tags"
           - Expected format: serialized JSON string of an array of strings
           - Example: "[\\"powerup\\", \\"current\\"]"
         """
+
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         description_url: builtins.str = ...,
         provided_interfaces: collections.abc.Iterable[builtins.str] | None = ...,
         service_class: builtins.str = ...,
         annotations: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["annotations", b"annotations", "description_url", b"description_url", "display_name", b"display_name", "provided_interfaces", b"provided_interfaces", "service_class", b"service_class"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["annotations", b"annotations", "description_url", b"description_url", "display_name", b"display_name", "provided_interfaces", b"provided_interfaces", "service_class", b"service_class"]) -> None: ...
 
 global___ServiceDescriptor = ServiceDescriptor
 
-@typing_extensions.final
+@typing.final
 class ServiceLocation(google.protobuf.message.Message):
     """Represents the location of a service. The location generally includes the IP address and port number for the service
     which can be used to establish communication with the service.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -114,119 +112,122 @@
     def __init__(
         self,
         *,
         location: builtins.str = ...,
         insecure_port: builtins.str = ...,
         ssl_authenticated_port: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["insecure_port", b"insecure_port", "location", b"location", "ssl_authenticated_port", b"ssl_authenticated_port"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["insecure_port", b"insecure_port", "location", b"location", "ssl_authenticated_port", b"ssl_authenticated_port"]) -> None: ...
 
 global___ServiceLocation = ServiceLocation
 
-@typing_extensions.final
+@typing.final
 class RegisterServiceRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVICE_DESCRIPTION_FIELD_NUMBER: builtins.int
     LOCATION_FIELD_NUMBER: builtins.int
     @property
     def service_description(self) -> global___ServiceDescriptor:
         """Required. The description of the service."""
+
     @property
     def location(self) -> global___ServiceLocation:
         """Required. The canonical location information for the service."""
+
     def __init__(
         self,
         *,
         service_description: global___ServiceDescriptor | None = ...,
         location: global___ServiceLocation | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["location", b"location", "service_description", b"service_description"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["location", b"location", "service_description", b"service_description"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["location", b"location", "service_description", b"service_description"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["location", b"location", "service_description", b"service_description"]) -> None: ...
 
 global___RegisterServiceRequest = RegisterServiceRequest
 
-@typing_extensions.final
+@typing.final
 class RegisterServiceResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     REGISTRATION_ID_FIELD_NUMBER: builtins.int
     registration_id: builtins.str
     """ID that can be used to unregister the service."""
     def __init__(
         self,
         *,
         registration_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["registration_id", b"registration_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["registration_id", b"registration_id"]) -> None: ...
 
 global___RegisterServiceResponse = RegisterServiceResponse
 
-@typing_extensions.final
+@typing.final
 class UnregisterServiceRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     REGISTRATION_ID_FIELD_NUMBER: builtins.int
     registration_id: builtins.str
     """Required. The registration ID of the service that should be unregistered."""
     def __init__(
         self,
         *,
         registration_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["registration_id", b"registration_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["registration_id", b"registration_id"]) -> None: ...
 
 global___UnregisterServiceRequest = UnregisterServiceRequest
 
-@typing_extensions.final
+@typing.final
 class UnregisterServiceResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___UnregisterServiceResponse = UnregisterServiceResponse
 
-@typing_extensions.final
+@typing.final
 class EnumerateServicesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROVIDED_INTERFACE_FIELD_NUMBER: builtins.int
     provided_interface: builtins.str
     """Optional. The gRPC full name of the service interface that is needed. If empty,
     information for all services registered with the discovery service will be returned.
     """
     def __init__(
         self,
         *,
         provided_interface: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["provided_interface", b"provided_interface"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["provided_interface", b"provided_interface"]) -> None: ...
 
 global___EnumerateServicesRequest = EnumerateServicesRequest
 
-@typing_extensions.final
+@typing.final
 class EnumerateServicesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AVAILABLE_SERVICES_FIELD_NUMBER: builtins.int
     @property
     def available_services(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServiceDescriptor]:
         """The list of available services which implement the specified service interface."""
+
     def __init__(
         self,
         *,
         available_services: collections.abc.Iterable[global___ServiceDescriptor] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["available_services", b"available_services"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["available_services", b"available_services"]) -> None: ...
 
 global___EnumerateServicesResponse = EnumerateServicesResponse
 
-@typing_extensions.final
+@typing.final
 class ResolveServiceRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROVIDED_INTERFACE_FIELD_NUMBER: builtins.int
     SERVICE_CLASS_FIELD_NUMBER: builtins.int
     provided_interface: builtins.str
     """Required. This corresponds to the gRPC Full Name of the service and should match the information
@@ -238,10 +239,10 @@
     """
     def __init__(
         self,
         *,
         provided_interface: builtins.str = ...,
         service_class: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["provided_interface", b"provided_interface", "service_class", b"service_class"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["provided_interface", b"provided_interface", "service_class", b"service_class"]) -> None: ...
 
 global___ResolveServiceRequest = ResolveServiceRequest
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 ---------------------------------------------------------------------
 ---------------------------------------------------------------------
 """
+
 import abc
 import collections.abc
 import grpc
 import grpc.aio
 import ni_measurementlink_service._internal.stubs.ni.measurementlink.discovery.v1.discovery_service_pb2 as ni_measurementlink_discovery_v1_discovery_service_pb2
 import typing
 
-_T = typing.TypeVar('_T')
+_T = typing.TypeVar("_T")
 
-class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
-    ...
+class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta): ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore[misc, type-arg]
     ...
 
 class DiscoveryServiceStub:
     """The service used as a registry for other services. This service can be used to discover
     and activate other services present in the system.
     """
 
@@ -35,26 +35,29 @@
       - ServiceDescriptor.display_name is empty
       - ServiceDescriptor.provided_interfaces is empty
       - ServiceDescriptor.service_class is empty
       - ServiceLocation.location is empty
       - Both ServiceLocation.insecure_port and ServiceLocation.ssl_authenticated_port are empty
       - Either ServiceLocation.insecure_port or ServiceLocation.ssl_authenticated_port contain an invalid port number
     """
+
     UnregisterService: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_discovery_v1_discovery_service_pb2.UnregisterServiceRequest,
         ni_measurementlink_discovery_v1_discovery_service_pb2.UnregisterServiceResponse,
     ]
     """Unregisters a service instance with the discovery service."""
+
     EnumerateServices: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_discovery_v1_discovery_service_pb2.EnumerateServicesRequest,
         ni_measurementlink_discovery_v1_discovery_service_pb2.EnumerateServicesResponse,
     ]
     """Enumerate all services which implement a specific service interface.
     This is useful for plugin type systems where the possible services are not known ahead of time.
     """
+
     ResolveService: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_discovery_v1_discovery_service_pb2.ResolveServiceRequest,
         ni_measurementlink_discovery_v1_discovery_service_pb2.ServiceLocation,
     ]
     """Given a description of a service, returns information that can be used to establish communication
     with that service. If necessary, the service will be started by the discovery service if it has not
     already been started. Activation of the service is accomplished through use of a .serviceconfig file
@@ -82,26 +85,29 @@
       - ServiceDescriptor.display_name is empty
       - ServiceDescriptor.provided_interfaces is empty
       - ServiceDescriptor.service_class is empty
       - ServiceLocation.location is empty
       - Both ServiceLocation.insecure_port and ServiceLocation.ssl_authenticated_port are empty
       - Either ServiceLocation.insecure_port or ServiceLocation.ssl_authenticated_port contain an invalid port number
     """
+
     UnregisterService: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_discovery_v1_discovery_service_pb2.UnregisterServiceRequest,
         ni_measurementlink_discovery_v1_discovery_service_pb2.UnregisterServiceResponse,
     ]
     """Unregisters a service instance with the discovery service."""
+
     EnumerateServices: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_discovery_v1_discovery_service_pb2.EnumerateServicesRequest,
         ni_measurementlink_discovery_v1_discovery_service_pb2.EnumerateServicesResponse,
     ]
     """Enumerate all services which implement a specific service interface.
     This is useful for plugin type systems where the possible services are not known ahead of time.
     """
+
     ResolveService: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_discovery_v1_discovery_service_pb2.ResolveServiceRequest,
         ni_measurementlink_discovery_v1_discovery_service_pb2.ServiceLocation,
     ]
     """Given a description of a service, returns information that can be used to establish communication
     with that service. If necessary, the service will be started by the discovery service if it has not
     already been started. Activation of the service is accomplished through use of a .serviceconfig file
@@ -131,30 +137,33 @@
           - ServiceDescriptor.display_name is empty
           - ServiceDescriptor.provided_interfaces is empty
           - ServiceDescriptor.service_class is empty
           - ServiceLocation.location is empty
           - Both ServiceLocation.insecure_port and ServiceLocation.ssl_authenticated_port are empty
           - Either ServiceLocation.insecure_port or ServiceLocation.ssl_authenticated_port contain an invalid port number
         """
+
     @abc.abstractmethod
     def UnregisterService(
         self,
         request: ni_measurementlink_discovery_v1_discovery_service_pb2.UnregisterServiceRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_discovery_v1_discovery_service_pb2.UnregisterServiceResponse, collections.abc.Awaitable[ni_measurementlink_discovery_v1_discovery_service_pb2.UnregisterServiceResponse]]:
         """Unregisters a service instance with the discovery service."""
+
     @abc.abstractmethod
     def EnumerateServices(
         self,
         request: ni_measurementlink_discovery_v1_discovery_service_pb2.EnumerateServicesRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_discovery_v1_discovery_service_pb2.EnumerateServicesResponse, collections.abc.Awaitable[ni_measurementlink_discovery_v1_discovery_service_pb2.EnumerateServicesResponse]]:
         """Enumerate all services which implement a specific service interface.
         This is useful for plugin type systems where the possible services are not known ahead of time.
         """
+
     @abc.abstractmethod
     def ResolveService(
         self,
         request: ni_measurementlink_discovery_v1_discovery_service_pb2.ResolveServiceRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_discovery_v1_discovery_service_pb2.ServiceLocation, collections.abc.Awaitable[ni_measurementlink_discovery_v1_discovery_service_pb2.ServiceLocation]]:
         """Given a description of a service, returns information that can be used to establish communication
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,119 +1,121 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 ---------------------------------------------------------------------
 ---------------------------------------------------------------------
 """
+
 import builtins
 import collections.abc
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.type_pb2
 import ni_measurementlink_service._internal.stubs.ni.measurementlink.pin_map_context_pb2 as ni_measurementlink_pin_map_context_pb2
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GetMetadataRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetMetadataRequest = GetMetadataRequest
 
-@typing_extensions.final
+@typing.final
 class GetMetadataResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MEASUREMENT_DETAILS_FIELD_NUMBER: builtins.int
     MEASUREMENT_SIGNATURE_FIELD_NUMBER: builtins.int
     USER_INTERFACE_DETAILS_FIELD_NUMBER: builtins.int
     @property
     def measurement_details(self) -> global___MeasurementDetails:
         """Required. Specifies basic information about the measurement."""
+
     @property
     def measurement_signature(self) -> global___MeasurementSignature:
         """Required. Specifies the signature of the measurement."""
+
     @property
     def user_interface_details(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UserInterfaceDetails]:
         """Optional. Specifies the user interfaces available for use with the measurement, if any."""
+
     def __init__(
         self,
         *,
         measurement_details: global___MeasurementDetails | None = ...,
         measurement_signature: global___MeasurementSignature | None = ...,
         user_interface_details: collections.abc.Iterable[global___UserInterfaceDetails] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature", "user_interface_details", b"user_interface_details"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature", "user_interface_details", b"user_interface_details"]) -> None: ...
 
 global___GetMetadataResponse = GetMetadataResponse
 
-@typing_extensions.final
+@typing.final
 class MeasureRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONFIGURATION_PARAMETERS_FIELD_NUMBER: builtins.int
     PIN_MAP_CONTEXT_FIELD_NUMBER: builtins.int
     @property
     def configuration_parameters(self) -> google.protobuf.any_pb2.Any:
         """Required. Specifies the configuration to be used for the measurement. Each measurement will define its own set
         of required and optional parameters and generate errors as appropriate if the configuration does not conform
         to valid input ranges.
         """
+
     @property
     def pin_map_context(self) -> ni_measurementlink_pin_map_context_pb2.PinMapContext:
         """Optional. Specifies the pin map context for the measurement, if any. This field is optional in that callers
         may not always have a pin map context available to include in the request message. Each measurement will
         define if a valid pin map context is required in order to run or not and generate errors appropriately.
         """
+
     def __init__(
         self,
         *,
         configuration_parameters: google.protobuf.any_pb2.Any | None = ...,
         pin_map_context: ni_measurementlink_pin_map_context_pb2.PinMapContext | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> None: ...
 
 global___MeasureRequest = MeasureRequest
 
-@typing_extensions.final
+@typing.final
 class MeasureResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OUTPUTS_FIELD_NUMBER: builtins.int
     @property
     def outputs(self) -> google.protobuf.any_pb2.Any:
         """Required. Includes the output results from running the measurement. This field is required in that all measurements
         should return a valid output message even if it is just an empty message with no fields. Each measurement will define
         which of its output fields are required and which are optional based on the configuration for the measurement.
         """
+
     def __init__(
         self,
         *,
         outputs: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["outputs", b"outputs"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["outputs", b"outputs"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["outputs", b"outputs"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["outputs", b"outputs"]) -> None: ...
 
 global___MeasureResponse = MeasureResponse
 
-@typing_extensions.final
+@typing.final
 class MeasurementDetails(google.protobuf.message.Message):
     """Message that contains standard information reported by a measurement."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
@@ -123,102 +125,105 @@
     """Optional. The current version of the measurement."""
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         version: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["display_name", b"display_name", "version", b"version"]) -> None: ...
 
 global___MeasurementDetails = MeasurementDetails
 
-@typing_extensions.final
+@typing.final
 class MeasurementSignature(google.protobuf.message.Message):
     """Message that defines the signature of a measurement."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONFIGURATION_PARAMETERS_MESSAGE_TYPE_FIELD_NUMBER: builtins.int
     CONFIGURATION_PARAMETERS_FIELD_NUMBER: builtins.int
     CONFIGURATION_DEFAULTS_FIELD_NUMBER: builtins.int
     OUTPUTS_MESSAGE_TYPE_FIELD_NUMBER: builtins.int
     OUTPUTS_FIELD_NUMBER: builtins.int
     configuration_parameters_message_type: builtins.str
     """Required. The type name of the message used to define the measurement's configuration.
     This is the gRPC full name for the message.
     """
+    outputs_message_type: builtins.str
+    """Required. The type name of the message used to define the measurement's outputs.
+    This is the gRPC full name for the message.
+    """
     @property
     def configuration_parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ConfigurationParameter]:
         """Required. Defines the configuration parameters for the measurement."""
+
     @property
     def configuration_defaults(self) -> google.protobuf.any_pb2.Any:
         """Optional. The default values to use for the configuration parameters. Caller can use these default values
         rather than specifying their own. These values should be supplied using the message type defined by
         configuration_parameters_message_type.
         """
-    outputs_message_type: builtins.str
-    """Required. The type name of the message used to define the measurement's outputs.
-    This is the gRPC full name for the message.
-    """
+
     @property
     def outputs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Output]:
         """Required. Defines the outputs for the measurement."""
+
     def __init__(
         self,
         *,
         configuration_parameters_message_type: builtins.str = ...,
         configuration_parameters: collections.abc.Iterable[global___ConfigurationParameter] | None = ...,
         configuration_defaults: google.protobuf.any_pb2.Any | None = ...,
         outputs_message_type: builtins.str = ...,
         outputs: collections.abc.Iterable[global___Output] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["configuration_defaults", b"configuration_defaults"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["configuration_defaults", b"configuration_defaults", "configuration_parameters", b"configuration_parameters", "configuration_parameters_message_type", b"configuration_parameters_message_type", "outputs", b"outputs", "outputs_message_type", b"outputs_message_type"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["configuration_defaults", b"configuration_defaults"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["configuration_defaults", b"configuration_defaults", "configuration_parameters", b"configuration_parameters", "configuration_parameters_message_type", b"configuration_parameters_message_type", "outputs", b"outputs", "outputs_message_type", b"outputs_message_type"]) -> None: ...
 
 global___MeasurementSignature = MeasurementSignature
 
-@typing_extensions.final
+@typing.final
 class UserInterfaceDetails(google.protobuf.message.Message):
     """Contains measurement User Interface details."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FILE_URL_FIELD_NUMBER: builtins.int
     file_url: builtins.str
     """Optional. The URL to the file (such as .measui or .vi) providing a user interface for the measurement."""
     def __init__(
         self,
         *,
         file_url: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file_url", b"file_url"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["file_url", b"file_url"]) -> None: ...
 
 global___UserInterfaceDetails = UserInterfaceDetails
 
-@typing_extensions.final
+@typing.final
 class ConfigurationParameter(google.protobuf.message.Message):
     """Message that defines a configuration parameter for the measurement."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class AnnotationsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FIELD_NUMBER_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     REPEATED_FIELD_NUMBER: builtins.int
     ANNOTATIONS_FIELD_NUMBER: builtins.int
     field_number: builtins.int
@@ -240,28 +245,29 @@
         - Type specialization. The keys to other annotations will be read based on the value of `ni/type_specialization` annotation.
           - Key: "ni/type_specialization"
           - Common Values: "pin" ...    
         - For string parameter with ni/type_specialization annotation equals "pin"
           - Key: "ni/pin.instrument_type"
           - Common Values: "niDCPower", "niScope"...
         """
+
     def __init__(
         self,
         *,
         field_number: builtins.int = ...,
         type: google.protobuf.type_pb2.Field.Kind.ValueType = ...,
         name: builtins.str = ...,
         repeated: builtins.bool = ...,
         annotations: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["annotations", b"annotations", "field_number", b"field_number", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["annotations", b"annotations", "field_number", b"field_number", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
 
 global___ConfigurationParameter = ConfigurationParameter
 
-@typing_extensions.final
+@typing.final
 class Output(google.protobuf.message.Message):
     """Message that defines an output of the measurement."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FIELD_NUMBER_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
@@ -283,10 +289,10 @@
         self,
         *,
         field_number: builtins.int = ...,
         type: google.protobuf.type_pb2.Field.Kind.ValueType = ...,
         name: builtins.str = ...,
         repeated: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["field_number", b"field_number", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["field_number", b"field_number", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
 
 global___Output = Output
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 ---------------------------------------------------------------------
 ---------------------------------------------------------------------
 """
+
 import abc
 import collections.abc
 import grpc
 import grpc.aio
 import ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v1.measurement_service_pb2 as ni_measurementlink_measurement_v1_measurement_service_pb2
 import typing
 
-_T = typing.TypeVar('_T')
+_T = typing.TypeVar("_T")
 
-class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
-    ...
+class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta): ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore[misc, type-arg]
     ...
 
 class MeasurementServiceStub:
     """Service that implements a measurement. Unlike other services, a MeasurementService is designed to be a plugin
     where there can be multiple implementations of the service that provide different measurement capabilities.
     """
 
     def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None: ...
     GetMetadata: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_measurement_v1_measurement_service_pb2.GetMetadataRequest,
         ni_measurementlink_measurement_v1_measurement_service_pb2.GetMetadataResponse,
     ]
     """Returns information that describes the measurement."""
+
     Measure: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_measurement_v1_measurement_service_pb2.MeasureRequest,
         ni_measurementlink_measurement_v1_measurement_service_pb2.MeasureResponse,
     ]
     """API used to perform a measurement."""
 
 class MeasurementServiceAsyncStub:
@@ -42,14 +43,15 @@
     """
 
     GetMetadata: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_measurement_v1_measurement_service_pb2.GetMetadataRequest,
         ni_measurementlink_measurement_v1_measurement_service_pb2.GetMetadataResponse,
     ]
     """Returns information that describes the measurement."""
+
     Measure: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_measurement_v1_measurement_service_pb2.MeasureRequest,
         ni_measurementlink_measurement_v1_measurement_service_pb2.MeasureResponse,
     ]
     """API used to perform a measurement."""
 
 class MeasurementServiceServicer(metaclass=abc.ABCMeta):
@@ -60,14 +62,15 @@
     @abc.abstractmethod
     def GetMetadata(
         self,
         request: ni_measurementlink_measurement_v1_measurement_service_pb2.GetMetadataRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_measurement_v1_measurement_service_pb2.GetMetadataResponse, collections.abc.Awaitable[ni_measurementlink_measurement_v1_measurement_service_pb2.GetMetadataResponse]]:
         """Returns information that describes the measurement."""
+
     @abc.abstractmethod
     def Measure(
         self,
         request: ni_measurementlink_measurement_v1_measurement_service_pb2.MeasureRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_measurement_v1_measurement_service_pb2.MeasureResponse, collections.abc.Awaitable[ni_measurementlink_measurement_v1_measurement_service_pb2.MeasureResponse]]:
         """API used to perform a measurement."""
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,119 +1,121 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 ---------------------------------------------------------------------
 ---------------------------------------------------------------------
 """
+
 import builtins
 import collections.abc
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.type_pb2
 import ni_measurementlink_service._internal.stubs.ni.measurementlink.pin_map_context_pb2 as ni_measurementlink_pin_map_context_pb2
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GetMetadataRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetMetadataRequest = GetMetadataRequest
 
-@typing_extensions.final
+@typing.final
 class GetMetadataResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MEASUREMENT_DETAILS_FIELD_NUMBER: builtins.int
     MEASUREMENT_SIGNATURE_FIELD_NUMBER: builtins.int
     USER_INTERFACE_DETAILS_FIELD_NUMBER: builtins.int
     @property
     def measurement_details(self) -> global___MeasurementDetails:
         """Required. Specifies basic information about the measurement."""
+
     @property
     def measurement_signature(self) -> global___MeasurementSignature:
         """Required. Specifies the signature of the measurement."""
+
     @property
     def user_interface_details(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UserInterfaceDetails]:
         """Optional. Specifies the user interfaces available for use with the measurement, if any."""
+
     def __init__(
         self,
         *,
         measurement_details: global___MeasurementDetails | None = ...,
         measurement_signature: global___MeasurementSignature | None = ...,
         user_interface_details: collections.abc.Iterable[global___UserInterfaceDetails] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature", "user_interface_details", b"user_interface_details"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature", "user_interface_details", b"user_interface_details"]) -> None: ...
 
 global___GetMetadataResponse = GetMetadataResponse
 
-@typing_extensions.final
+@typing.final
 class MeasureRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONFIGURATION_PARAMETERS_FIELD_NUMBER: builtins.int
     PIN_MAP_CONTEXT_FIELD_NUMBER: builtins.int
     @property
     def configuration_parameters(self) -> google.protobuf.any_pb2.Any:
         """Required. Specifies the configuration to be used for the measurement. Each measurement will define its own set
         of required and optional parameters and generate errors as appropriate if the configuration does not conform
         to valid input ranges.
         """
+
     @property
     def pin_map_context(self) -> ni_measurementlink_pin_map_context_pb2.PinMapContext:
         """Optional. Specifies the pin map context for the measurement, if any. This field is optional in that callers
         may not always have a pin map context available to include in the request message. Each measurement will
         define if a valid pin map context is required in order to run or not and generate errors appropriately.
         """
+
     def __init__(
         self,
         *,
         configuration_parameters: google.protobuf.any_pb2.Any | None = ...,
         pin_map_context: ni_measurementlink_pin_map_context_pb2.PinMapContext | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> None: ...
 
 global___MeasureRequest = MeasureRequest
 
-@typing_extensions.final
+@typing.final
 class MeasureResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OUTPUTS_FIELD_NUMBER: builtins.int
     @property
     def outputs(self) -> google.protobuf.any_pb2.Any:
         """Required. Includes the output results from running the measurement. This field is required in that all measurements
         should return a valid output message even if it is just an empty message with no fields. Each measurement will define
         which of its output fields are required and which are optional based on the configuration for the measurement.
         """
+
     def __init__(
         self,
         *,
         outputs: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["outputs", b"outputs"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["outputs", b"outputs"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["outputs", b"outputs"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["outputs", b"outputs"]) -> None: ...
 
 global___MeasureResponse = MeasureResponse
 
-@typing_extensions.final
+@typing.final
 class MeasurementDetails(google.protobuf.message.Message):
     """Message that contains standard information reported by a measurement."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
@@ -123,102 +125,105 @@
     """Optional. The current version of the measurement."""
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         version: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["display_name", b"display_name", "version", b"version"]) -> None: ...
 
 global___MeasurementDetails = MeasurementDetails
 
-@typing_extensions.final
+@typing.final
 class MeasurementSignature(google.protobuf.message.Message):
     """Message that defines the signature of a measurement."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONFIGURATION_PARAMETERS_MESSAGE_TYPE_FIELD_NUMBER: builtins.int
     CONFIGURATION_PARAMETERS_FIELD_NUMBER: builtins.int
     CONFIGURATION_DEFAULTS_FIELD_NUMBER: builtins.int
     OUTPUTS_MESSAGE_TYPE_FIELD_NUMBER: builtins.int
     OUTPUTS_FIELD_NUMBER: builtins.int
     configuration_parameters_message_type: builtins.str
     """Required. The type name of the message used to define the measurement's configuration.
     This is the gRPC full name for the message.
     """
+    outputs_message_type: builtins.str
+    """Required. The type name of the message used to define the measurement's outputs.
+    This is the gRPC full name for the message.
+    """
     @property
     def configuration_parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ConfigurationParameter]:
         """Required. Defines the configuration parameters for the measurement."""
+
     @property
     def configuration_defaults(self) -> google.protobuf.any_pb2.Any:
         """Optional. The default values to use for the configuration parameters. Caller can use these default values
         rather than specifying their own. These values should be supplied using the message type defined by
         configuration_parameters_message_type.
         """
-    outputs_message_type: builtins.str
-    """Required. The type name of the message used to define the measurement's outputs.
-    This is the gRPC full name for the message.
-    """
+
     @property
     def outputs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Output]:
         """Required. Defines the outputs for the measurement."""
+
     def __init__(
         self,
         *,
         configuration_parameters_message_type: builtins.str = ...,
         configuration_parameters: collections.abc.Iterable[global___ConfigurationParameter] | None = ...,
         configuration_defaults: google.protobuf.any_pb2.Any | None = ...,
         outputs_message_type: builtins.str = ...,
         outputs: collections.abc.Iterable[global___Output] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["configuration_defaults", b"configuration_defaults"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["configuration_defaults", b"configuration_defaults", "configuration_parameters", b"configuration_parameters", "configuration_parameters_message_type", b"configuration_parameters_message_type", "outputs", b"outputs", "outputs_message_type", b"outputs_message_type"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["configuration_defaults", b"configuration_defaults"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["configuration_defaults", b"configuration_defaults", "configuration_parameters", b"configuration_parameters", "configuration_parameters_message_type", b"configuration_parameters_message_type", "outputs", b"outputs", "outputs_message_type", b"outputs_message_type"]) -> None: ...
 
 global___MeasurementSignature = MeasurementSignature
 
-@typing_extensions.final
+@typing.final
 class UserInterfaceDetails(google.protobuf.message.Message):
     """Contains measurement User Interface details."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FILE_URL_FIELD_NUMBER: builtins.int
     file_url: builtins.str
     """Optional. The URL to the file (such as .measui or .vi) providing a user interface for the measurement."""
     def __init__(
         self,
         *,
         file_url: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file_url", b"file_url"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["file_url", b"file_url"]) -> None: ...
 
 global___UserInterfaceDetails = UserInterfaceDetails
 
-@typing_extensions.final
+@typing.final
 class ConfigurationParameter(google.protobuf.message.Message):
     """Message that defines a configuration parameter for the measurement."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class AnnotationsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FIELD_NUMBER_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     REPEATED_FIELD_NUMBER: builtins.int
     ANNOTATIONS_FIELD_NUMBER: builtins.int
     MESSAGE_TYPE_FIELD_NUMBER: builtins.int
@@ -233,14 +238,18 @@
     """
     name: builtins.str
     """Required. The name of the configuration parameter. When defining a user interface for the measurement, a control
     that matches this name will be used to supply a value to this configuration parameter.
     """
     repeated: builtins.bool
     """Required. True if this configuration parameter represents repeated data and False if it represents a scalar value."""
+    message_type: builtins.str
+    """Required when 'type' is Kind.TypeMessage. Ignored for any other 'type'.
+    This is the gRPC full name of the message type.
+    """
     @property
     def annotations(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Optional. Represents a set of annotations on the type.
         Well-known annotations:
         - Type specialization. The keys to other annotations will be read based on the value of `ni/type_specialization` annotation.
           - Key: "ni/type_specialization"
           - Common Values: "pin", "path", "enum", ...
@@ -250,53 +259,50 @@
           - Key: "ni/pin.instrument_type"
           - Common Values: "niDCPower", "niScope"...
         - For enum parameter with ni/type_specialization annotation equals "enum"
           - Key: "ni/enum.values"
           - Expected format: JSON dictionary string"
           - Example: "{\\"RED\\":0, \\"GREEN\\":25, \\"BLUE\\":5}"
         """
-    message_type: builtins.str
-    """Required when 'type' is Kind.TypeMessage. Ignored for any other 'type'.
-    This is the gRPC full name of the message type.
-    """
+
     def __init__(
         self,
         *,
         field_number: builtins.int = ...,
         type: google.protobuf.type_pb2.Field.Kind.ValueType = ...,
         name: builtins.str = ...,
         repeated: builtins.bool = ...,
         annotations: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         message_type: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["annotations", b"annotations", "field_number", b"field_number", "message_type", b"message_type", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["annotations", b"annotations", "field_number", b"field_number", "message_type", b"message_type", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
 
 global___ConfigurationParameter = ConfigurationParameter
 
-@typing_extensions.final
+@typing.final
 class Output(google.protobuf.message.Message):
     """Message that defines an output of the measurement."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class AnnotationsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: builtins.str = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FIELD_NUMBER_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     REPEATED_FIELD_NUMBER: builtins.int
     ANNOTATIONS_FIELD_NUMBER: builtins.int
     MESSAGE_TYPE_FIELD_NUMBER: builtins.int
@@ -311,29 +317,30 @@
     """
     name: builtins.str
     """Required. The name of the output. When defining a user interface for the measurement, an indicator
     that matches this name will be used to display the value for this output.
     """
     repeated: builtins.bool
     """Required. True if this output represents repeated data and False if it represents a scalar value."""
+    message_type: builtins.str
+    """Required when 'type' is Kind.TypeMessage. Ignored for any other 'type'.
+    This is the gRPC full name of the message type.
+    """
     @property
     def annotations(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Optional. Represents a set of annotations on the type.
         See documentation for ConfigurationParameter annotations for more details and examples.
         """
-    message_type: builtins.str
-    """Required when 'type' is Kind.TypeMessage. Ignored for any other 'type'.
-    This is the gRPC full name of the message type.
-    """
+
     def __init__(
         self,
         *,
         field_number: builtins.int = ...,
         type: google.protobuf.type_pb2.Field.Kind.ValueType = ...,
         name: builtins.str = ...,
         repeated: builtins.bool = ...,
         annotations: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         message_type: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["annotations", b"annotations", "field_number", b"field_number", "message_type", b"message_type", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["annotations", b"annotations", "field_number", b"field_number", "message_type", b"message_type", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
 
 global___Output = Output
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 ---------------------------------------------------------------------
 ---------------------------------------------------------------------
 """
+
 import abc
 import collections.abc
 import grpc
 import grpc.aio
 import ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v2.measurement_service_pb2 as ni_measurementlink_measurement_v2_measurement_service_pb2
 import typing
 
-_T = typing.TypeVar('_T')
+_T = typing.TypeVar("_T")
 
-class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
-    ...
+class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta): ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore[misc, type-arg]
     ...
 
 class MeasurementServiceStub:
     """Service that implements a measurement. Unlike other services, a MeasurementService is designed to be a plugin
     where there can be multiple implementations of the service that provide different measurement capabilities.
     """
 
     def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None: ...
     GetMetadata: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_measurement_v2_measurement_service_pb2.GetMetadataRequest,
         ni_measurementlink_measurement_v2_measurement_service_pb2.GetMetadataResponse,
     ]
     """Returns information that describes the measurement."""
+
     Measure: grpc.UnaryStreamMultiCallable[
         ni_measurementlink_measurement_v2_measurement_service_pb2.MeasureRequest,
         ni_measurementlink_measurement_v2_measurement_service_pb2.MeasureResponse,
     ]
     """API used to perform a measurement."""
 
 class MeasurementServiceAsyncStub:
@@ -42,14 +43,15 @@
     """
 
     GetMetadata: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_measurement_v2_measurement_service_pb2.GetMetadataRequest,
         ni_measurementlink_measurement_v2_measurement_service_pb2.GetMetadataResponse,
     ]
     """Returns information that describes the measurement."""
+
     Measure: grpc.aio.UnaryStreamMultiCallable[
         ni_measurementlink_measurement_v2_measurement_service_pb2.MeasureRequest,
         ni_measurementlink_measurement_v2_measurement_service_pb2.MeasureResponse,
     ]
     """API used to perform a measurement."""
 
 class MeasurementServiceServicer(metaclass=abc.ABCMeta):
@@ -60,14 +62,15 @@
     @abc.abstractmethod
     def GetMetadata(
         self,
         request: ni_measurementlink_measurement_v2_measurement_service_pb2.GetMetadataRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_measurement_v2_measurement_service_pb2.GetMetadataResponse, collections.abc.Awaitable[ni_measurementlink_measurement_v2_measurement_service_pb2.GetMetadataResponse]]:
         """Returns information that describes the measurement."""
+
     @abc.abstractmethod
     def Measure(
         self,
         request: ni_measurementlink_measurement_v2_measurement_service_pb2.MeasureRequest,
         context: _ServicerContext,
     ) -> typing.Union[collections.abc.Iterator[ni_measurementlink_measurement_v2_measurement_service_pb2.MeasureResponse], collections.abc.AsyncIterator[ni_measurementlink_measurement_v2_measurement_service_pb2.MeasureResponse]]:
         """API used to perform a measurement."""
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class PinMapContext(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     SITES_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Required. The resource id of the pin map in the Pin Map service that should be used for the call."""
     @property
     def sites(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Optional. List of site numbers being used for the call. If unspecified, use all sites in the pin map."""
+
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
         sites: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id", "sites", b"sites"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pin_map_id", b"pin_map_id", "sites", b"sites"]) -> None: ...
 
 global___PinMapContext = PinMapContext
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class PinMap(google.protobuf.message.Message):
     """Pin map resource type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Output only. The resource id of the registered pin map resource."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pin_map_id", b"pin_map_id"]) -> None: ...
 
 global___PinMap = PinMap
 
-@typing_extensions.final
+@typing.final
 class CreatePinMapFromXmlRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     PIN_MAP_XML_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Required. The resource id of the pin map to register as a pin map resource."""
@@ -46,19 +42,19 @@
     """Required. A string representing contents of a pin map file."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
         pin_map_xml: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id", "pin_map_xml", b"pin_map_xml"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pin_map_id", b"pin_map_id", "pin_map_xml", b"pin_map_xml"]) -> None: ...
 
 global___CreatePinMapFromXmlRequest = CreatePinMapFromXmlRequest
 
-@typing_extensions.final
+@typing.final
 class UpdatePinMapFromXmlRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     PIN_MAP_XML_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Required. The resource id of the pin map to be updated."""
@@ -66,35 +62,35 @@
     """Required. New pin map file content."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
         pin_map_xml: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id", "pin_map_xml", b"pin_map_xml"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pin_map_id", b"pin_map_id", "pin_map_xml", b"pin_map_xml"]) -> None: ...
 
 global___UpdatePinMapFromXmlRequest = UpdatePinMapFromXmlRequest
 
-@typing_extensions.final
+@typing.final
 class GetPinMapRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Required. The resource id of the registered pin map resource."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pin_map_id", b"pin_map_id"]) -> None: ...
 
 global___GetPinMapRequest = GetPinMapRequest
 
-@typing_extensions.final
+@typing.final
 class QueryPinsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_ID_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Required. The resource id of the registered pin map resource."""
@@ -111,44 +107,46 @@
     """
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
         instrument_type_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["instrument_type_id", b"instrument_type_id", "pin_map_id", b"pin_map_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["instrument_type_id", b"instrument_type_id", "pin_map_id", b"pin_map_id"]) -> None: ...
 
 global___QueryPinsRequest = QueryPinsRequest
 
-@typing_extensions.final
+@typing.final
 class QueryPinsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PINS_FIELD_NUMBER: builtins.int
     PIN_GROUPS_FIELD_NUMBER: builtins.int
     @property
     def pins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___PinDefinition]:
         """List of pins on the registered pin map resource. This list includes both DUT and System pins."""
+
     @property
     def pin_groups(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___PinGroupDefinition]:
         """List of pin groups on the registered pin map resource.
         When an instrument type id filter is specified, a pin group will only be included
         in the response if all pins in the pin group match the instrument type.
         """
+
     def __init__(
         self,
         *,
         pins: collections.abc.Iterable[global___PinDefinition] | None = ...,
         pin_groups: collections.abc.Iterable[global___PinGroupDefinition] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pin_groups", b"pin_groups", "pins", b"pins"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pin_groups", b"pin_groups", "pins", b"pins"]) -> None: ...
 
 global___QueryPinsResponse = QueryPinsResponse
 
-@typing_extensions.final
+@typing.final
 class PinDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     IS_SYSTEM_PIN_FIELD_NUMBER: builtins.int
     display_name: builtins.str
     """Name of the dut pin."""
@@ -156,83 +154,87 @@
     """A boolean that indicates a System pin when 'true', or DUT pin when 'false'."""
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         is_system_pin: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "is_system_pin", b"is_system_pin"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["display_name", b"display_name", "is_system_pin", b"is_system_pin"]) -> None: ...
 
 global___PinDefinition = PinDefinition
 
-@typing_extensions.final
+@typing.final
 class PinGroupDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     PIN_OR_GROUP_REFERENCES_FIELD_NUMBER: builtins.int
     RESOLVED_PINS_FIELD_NUMBER: builtins.int
     display_name: builtins.str
     """Name of the pin group."""
     @property
     def pin_or_group_references(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """List of other pins or pin groups within this pin group."""
+
     @property
     def resolved_pins(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Distinct union of pins within this pin group, including those within nested pin groups."""
+
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         pin_or_group_references: collections.abc.Iterable[builtins.str] | None = ...,
         resolved_pins: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "pin_or_group_references", b"pin_or_group_references", "resolved_pins", b"resolved_pins"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["display_name", b"display_name", "pin_or_group_references", b"pin_or_group_references", "resolved_pins", b"resolved_pins"]) -> None: ...
 
 global___PinGroupDefinition = PinGroupDefinition
 
-@typing_extensions.final
+@typing.final
 class QueryRelaysRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Required. The resource id of the registered pin map resource."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pin_map_id", b"pin_map_id"]) -> None: ...
 
 global___QueryRelaysRequest = QueryRelaysRequest
 
-@typing_extensions.final
+@typing.final
 class QueryRelaysResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RELAYS_FIELD_NUMBER: builtins.int
     RELAY_GROUPS_FIELD_NUMBER: builtins.int
     @property
     def relays(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RelayDefinition]:
         """List of relays on the registered pin map resource. This list includes both Site relays and System relays."""
+
     @property
     def relay_groups(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RelayGroupDefinition]:
         """List of relay groups on the registered pin map resource."""
+
     def __init__(
         self,
         *,
         relays: collections.abc.Iterable[global___RelayDefinition] | None = ...,
         relay_groups: collections.abc.Iterable[global___RelayGroupDefinition] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["relay_groups", b"relay_groups", "relays", b"relays"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["relay_groups", b"relay_groups", "relays", b"relays"]) -> None: ...
 
 global___QueryRelaysResponse = QueryRelaysResponse
 
-@typing_extensions.final
+@typing.final
 class RelayDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     IS_SYSTEM_RELAY_FIELD_NUMBER: builtins.int
     display_name: builtins.str
     """Name of the relay."""
@@ -240,125 +242,131 @@
     """A boolean that indicates a System relay when 'true', or Site relay when 'false'."""
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         is_system_relay: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "is_system_relay", b"is_system_relay"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["display_name", b"display_name", "is_system_relay", b"is_system_relay"]) -> None: ...
 
 global___RelayDefinition = RelayDefinition
 
-@typing_extensions.final
+@typing.final
 class RelayGroupDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     RELAY_OR_GROUP_REFERENCES_FIELD_NUMBER: builtins.int
     RESOLVED_RELAYS_FIELD_NUMBER: builtins.int
     display_name: builtins.str
     """Name of the relay group."""
     @property
     def relay_or_group_references(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """List of other relays or relay groups within this relay group."""
+
     @property
     def resolved_relays(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Distinct union of relays within this relay group, including those within nested relay groups."""
+
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         relay_or_group_references: collections.abc.Iterable[builtins.str] | None = ...,
         resolved_relays: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "relay_or_group_references", b"relay_or_group_references", "resolved_relays", b"resolved_relays"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["display_name", b"display_name", "relay_or_group_references", b"relay_or_group_references", "resolved_relays", b"resolved_relays"]) -> None: ...
 
 global___RelayGroupDefinition = RelayGroupDefinition
 
-@typing_extensions.final
+@typing.final
 class QueryResourceAccessInformationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     SITES_FIELD_NUMBER: builtins.int
     PIN_OR_RELAY_NAMES_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_ID_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Required. The resource id of the registered pin map resource."""
-    @property
-    def sites(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-        """Optional. The list of sites for which to get instrument resource access information. If unspecified, get instrument resource information for all sites in the registered pin map resource."""
-    @property
-    def pin_or_relay_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """Optional. The list of pins, pin groups, relays, or relay groups for which to get instrument resource access information. If unspecified, get instrument resource information for all pins and relays in the registered pin map resource."""
     instrument_type_id: builtins.str
     """Optional. The instrument type for which to get instrument resource access information. If unspecified, get instrument resource information for all instrument types connected in the registered pin map resource.
     Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
          "niDCPower"
          "niDigitalPattern"
          "niScope"
          "niDMM"
          "niDAQmx"
          "niFGen"
          "niRelayDriver"
     For custom instruments the user defined instrument type id is defined in the pin map file.
     """
+    @property
+    def sites(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """Optional. The list of sites for which to get instrument resource access information. If unspecified, get instrument resource information for all sites in the registered pin map resource."""
+
+    @property
+    def pin_or_relay_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Optional. The list of pins, pin groups, relays, or relay groups for which to get instrument resource access information. If unspecified, get instrument resource information for all pins and relays in the registered pin map resource."""
+
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
         sites: collections.abc.Iterable[builtins.int] | None = ...,
         pin_or_relay_names: collections.abc.Iterable[builtins.str] | None = ...,
         instrument_type_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["instrument_type_id", b"instrument_type_id", "pin_map_id", b"pin_map_id", "pin_or_relay_names", b"pin_or_relay_names", "sites", b"sites"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["instrument_type_id", b"instrument_type_id", "pin_map_id", b"pin_map_id", "pin_or_relay_names", b"pin_or_relay_names", "sites", b"sites"]) -> None: ...
 
 global___QueryResourceAccessInformationRequest = QueryResourceAccessInformationRequest
 
-@typing_extensions.final
+@typing.final
 class QueryResourceAccessInformationResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class GroupMappingsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___ResolvedPinsOrRelays: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: global___ResolvedPinsOrRelays | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     RESOURCE_ACCESS_INFORMATION_FIELD_NUMBER: builtins.int
     GROUP_MAPPINGS_FIELD_NUMBER: builtins.int
     @property
     def resource_access_information(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResourceAccessInformation]:
         """List of ResourceAccessInformation objects with instrument resource names and channels."""
+
     @property
     def group_mappings(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___ResolvedPinsOrRelays]:
         """Represents the mapping between pin or relay groups and their respective pin or relay names."""
+
     def __init__(
         self,
         *,
         resource_access_information: collections.abc.Iterable[global___ResourceAccessInformation] | None = ...,
         group_mappings: collections.abc.Mapping[builtins.str, global___ResolvedPinsOrRelays] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["group_mappings", b"group_mappings", "resource_access_information", b"resource_access_information"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["group_mappings", b"group_mappings", "resource_access_information", b"resource_access_information"]) -> None: ...
 
 global___QueryResourceAccessInformationResponse = QueryResourceAccessInformationResponse
 
-@typing_extensions.final
+@typing.final
 class ResourceAccessInformation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESOURCE_NAME_FIELD_NUMBER: builtins.int
     CHANNEL_LIST_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_ID_FIELD_NUMBER: builtins.int
     CHANNEL_MAPPINGS_FIELD_NUMBER: builtins.int
@@ -387,27 +395,28 @@
     For custom instruments the user defined instrument type id is defined in the pin map file.
     """
     @property
     def channel_mappings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ChannelMapping]:
         """List of site and pin/relay mappings with optional multiplexer information for each channel in the channel_list.
         Each item represents a channel-to-pin connection for this instrument resource. In the case of shared pins, there is a separate item for each connection.
         """
+
     def __init__(
         self,
         *,
         resource_name: builtins.str = ...,
         channel_list: builtins.str = ...,
         instrument_type_id: builtins.str = ...,
         channel_mappings: collections.abc.Iterable[global___ChannelMapping] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_list", b"channel_list", "channel_mappings", b"channel_mappings", "instrument_type_id", b"instrument_type_id", "resource_name", b"resource_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["channel_list", b"channel_list", "channel_mappings", b"channel_mappings", "instrument_type_id", b"instrument_type_id", "resource_name", b"resource_name"]) -> None: ...
 
 global___ResourceAccessInformation = ResourceAccessInformation
 
-@typing_extensions.final
+@typing.final
 class ChannelMapping(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_OR_RELAY_NAME_FIELD_NUMBER: builtins.int
     SITE_FIELD_NUMBER: builtins.int
     CHANNEL_FIELD_NUMBER: builtins.int
     MULTIPLEXER_RESOURCE_NAME_FIELD_NUMBER: builtins.int
@@ -433,27 +442,28 @@
         pin_or_relay_name: builtins.str = ...,
         site: builtins.int = ...,
         channel: builtins.str = ...,
         multiplexer_resource_name: builtins.str = ...,
         multiplexer_route: builtins.str = ...,
         multiplexer_type_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel", b"channel", "multiplexer_resource_name", b"multiplexer_resource_name", "multiplexer_route", b"multiplexer_route", "multiplexer_type_id", b"multiplexer_type_id", "pin_or_relay_name", b"pin_or_relay_name", "site", b"site"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["channel", b"channel", "multiplexer_resource_name", b"multiplexer_resource_name", "multiplexer_route", b"multiplexer_route", "multiplexer_type_id", b"multiplexer_type_id", "pin_or_relay_name", b"pin_or_relay_name", "site", b"site"]) -> None: ...
 
 global___ChannelMapping = ChannelMapping
 
-@typing_extensions.final
+@typing.final
 class ResolvedPinsOrRelays(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_OR_RELAY_NAMES_FIELD_NUMBER: builtins.int
     @property
     def pin_or_relay_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """List of pin or relay names in the pin or relay group."""
+
     def __init__(
         self,
         *,
         pin_or_relay_names: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pin_or_relay_names", b"pin_or_relay_names"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pin_or_relay_names", b"pin_or_relay_names"]) -> None: ...
 
 global___ResolvedPinsOrRelays = ResolvedPinsOrRelays
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import abc
 import collections.abc
 import grpc
 import grpc.aio
 import ni_measurementlink_service._internal.stubs.ni.measurementlink.pinmap.v1.pin_map_service_pb2 as ni_measurementlink_pinmap_v1_pin_map_service_pb2
 import typing
 
-_T = typing.TypeVar('_T')
+_T = typing.TypeVar("_T")
 
-class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
-    ...
+class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta): ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore[misc, type-arg]
     ...
 
 class PinMapServiceStub:
     """Service to keep track of pin map resources."""
 
     def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None: ...
     CreatePinMapFromXml: grpc.UnaryUnaryMultiCallable[
@@ -26,47 +26,52 @@
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap,
     ]
     """Registers pin map with the PinMapService and returns a pin map resource.
     Status Codes for errors:
     - INVALID_ARGUMENT: Pin map id is empty or has whitespace, or pin map xml string is not valid
     - ALREADY_EXISTS: Pin map resource with the specified pin map id already exists
     """
+
     UpdatePinMapFromXml: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.UpdatePinMapFromXmlRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap,
     ]
     """Updates registered pin map contents and returns it.
     Creates and registers a pin map if a pin map resource for the specified pin map id is not found.
     Status Codes for errors:
     - INVALID_ARGUMENT: Pin map xml string is not valid
     """
+
     GetPinMap: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.GetPinMapRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap,
     ]
     """Get registered pin map resource.
     Status Codes for errors:
     - NOT_FOUND: Pin map resource for the specified pin map id is not found
     """
+
     QueryPins: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryPinsRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryPinsResponse,
     ]
     """Returns list of pins from the registered pin map resource.
     Status Codes for errors:
     - NOT_FOUND: Pin map resource for the specified pin map id is not found
     """
+
     QueryRelays: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryRelaysRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryRelaysResponse,
     ]
     """Returns list of relays from the registered pin map resource.
     Status Codes for errors:
     - NOT_FOUND: Pin map resource for the specified pin map id is not found
     """
+
     QueryResourceAccessInformation: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryResourceAccessInformationRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryResourceAccessInformationResponse,
     ]
     """Get instrument resource names, channels, and instrument type for the specified sites, pins or pin groups, relays or relay groups, instrument type in the registered pin map resource.
     Status Codes for errors:
     - NOT_FOUND:
@@ -85,47 +90,52 @@
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap,
     ]
     """Registers pin map with the PinMapService and returns a pin map resource.
     Status Codes for errors:
     - INVALID_ARGUMENT: Pin map id is empty or has whitespace, or pin map xml string is not valid
     - ALREADY_EXISTS: Pin map resource with the specified pin map id already exists
     """
+
     UpdatePinMapFromXml: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.UpdatePinMapFromXmlRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap,
     ]
     """Updates registered pin map contents and returns it.
     Creates and registers a pin map if a pin map resource for the specified pin map id is not found.
     Status Codes for errors:
     - INVALID_ARGUMENT: Pin map xml string is not valid
     """
+
     GetPinMap: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.GetPinMapRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap,
     ]
     """Get registered pin map resource.
     Status Codes for errors:
     - NOT_FOUND: Pin map resource for the specified pin map id is not found
     """
+
     QueryPins: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryPinsRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryPinsResponse,
     ]
     """Returns list of pins from the registered pin map resource.
     Status Codes for errors:
     - NOT_FOUND: Pin map resource for the specified pin map id is not found
     """
+
     QueryRelays: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryRelaysRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryRelaysResponse,
     ]
     """Returns list of relays from the registered pin map resource.
     Status Codes for errors:
     - NOT_FOUND: Pin map resource for the specified pin map id is not found
     """
+
     QueryResourceAccessInformation: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryResourceAccessInformationRequest,
         ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryResourceAccessInformationResponse,
     ]
     """Get instrument resource names, channels, and instrument type for the specified sites, pins or pin groups, relays or relay groups, instrument type in the registered pin map resource.
     Status Codes for errors:
     - NOT_FOUND:
@@ -146,55 +156,60 @@
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap, collections.abc.Awaitable[ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap]]:
         """Registers pin map with the PinMapService and returns a pin map resource.
         Status Codes for errors:
         - INVALID_ARGUMENT: Pin map id is empty or has whitespace, or pin map xml string is not valid
         - ALREADY_EXISTS: Pin map resource with the specified pin map id already exists
         """
+
     @abc.abstractmethod
     def UpdatePinMapFromXml(
         self,
         request: ni_measurementlink_pinmap_v1_pin_map_service_pb2.UpdatePinMapFromXmlRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap, collections.abc.Awaitable[ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap]]:
         """Updates registered pin map contents and returns it.
         Creates and registers a pin map if a pin map resource for the specified pin map id is not found.
         Status Codes for errors:
         - INVALID_ARGUMENT: Pin map xml string is not valid
         """
+
     @abc.abstractmethod
     def GetPinMap(
         self,
         request: ni_measurementlink_pinmap_v1_pin_map_service_pb2.GetPinMapRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap, collections.abc.Awaitable[ni_measurementlink_pinmap_v1_pin_map_service_pb2.PinMap]]:
         """Get registered pin map resource.
         Status Codes for errors:
         - NOT_FOUND: Pin map resource for the specified pin map id is not found
         """
+
     @abc.abstractmethod
     def QueryPins(
         self,
         request: ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryPinsRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryPinsResponse, collections.abc.Awaitable[ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryPinsResponse]]:
         """Returns list of pins from the registered pin map resource.
         Status Codes for errors:
         - NOT_FOUND: Pin map resource for the specified pin map id is not found
         """
+
     @abc.abstractmethod
     def QueryRelays(
         self,
         request: ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryRelaysRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryRelaysResponse, collections.abc.Awaitable[ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryRelaysResponse]]:
         """Returns list of relays from the registered pin map resource.
         Status Codes for errors:
         - NOT_FOUND: Pin map resource for the specified pin map id is not found
         """
+
     @abc.abstractmethod
     def QueryResourceAccessInformation(
         self,
         request: ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryResourceAccessInformationRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryResourceAccessInformationResponse, collections.abc.Awaitable[ni_measurementlink_pinmap_v1_pin_map_service_pb2.QueryResourceAccessInformationResponse]]:
         """Get instrument resource names, channels, and instrument type for the specified sites, pins or pin groups, relays or relay groups, instrument type in the registered pin map resource.
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import ni_measurementlink_service._internal.stubs.ni.measurementlink.pin_map_context_pb2 as ni_measurementlink_pin_map_context_pb2
 from ni_measurementlink_service._internal.stubs import session_pb2
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SessionInformation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSION_FIELD_NUMBER: builtins.int
     RESOURCE_NAME_FIELD_NUMBER: builtins.int
     CHANNEL_LIST_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_ID_FIELD_NUMBER: builtins.int
     SESSION_EXISTS_FIELD_NUMBER: builtins.int
     CHANNEL_MAPPINGS_FIELD_NUMBER: builtins.int
-    @property
-    def session(self) -> session_pb2.Session:
-        """Session identifier used to identify the session in the session management service, as well as in driver services such as grpc-device.
-        This field is readonly.
-        """
     resource_name: builtins.str
     """Resource name used to open this session in the driver.
     This field is readonly.
     """
     channel_list: builtins.str
     """Channel list used for driver initialization and measurement methods.
     This field is empty for any SessionInformation returned from ReserveAllRegisteredSessions.
@@ -56,36 +47,43 @@
     This field is readonly.
     """
     session_exists: builtins.bool
     """Indicates whether the session exists in the Session Manager. This indicates whether the session has been created.
     This field is readonly.
     """
     @property
+    def session(self) -> session_pb2.Session:
+        """Session identifier used to identify the session in the session management service, as well as in driver services such as grpc-device.
+        This field is readonly.
+        """
+
+    @property
     def channel_mappings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ChannelMapping]:
         """List of site and pin/relay mappings with optional multiplexer information for each channel in the channel_list.
         Each item represents a channel-to-pin connection for this instrument resource. In the case of shared pins, there is a separate item for each connection.
         This field is empty for any SessionInformation returned from ReserveAllRegisteredSessions.
         This field is readonly.
         """
+
     def __init__(
         self,
         *,
         session: session_pb2.Session | None = ...,
         resource_name: builtins.str = ...,
         channel_list: builtins.str = ...,
         instrument_type_id: builtins.str = ...,
         session_exists: builtins.bool = ...,
         channel_mappings: collections.abc.Iterable[global___ChannelMapping] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["session", b"session"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel_list", b"channel_list", "channel_mappings", b"channel_mappings", "instrument_type_id", b"instrument_type_id", "resource_name", b"resource_name", "session", b"session", "session_exists", b"session_exists"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["session", b"session"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["channel_list", b"channel_list", "channel_mappings", b"channel_mappings", "instrument_type_id", b"instrument_type_id", "resource_name", b"resource_name", "session", b"session", "session_exists", b"session_exists"]) -> None: ...
 
 global___SessionInformation = SessionInformation
 
-@typing_extensions.final
+@typing.final
 class ChannelMapping(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_OR_RELAY_NAME_FIELD_NUMBER: builtins.int
     SITE_FIELD_NUMBER: builtins.int
     CHANNEL_FIELD_NUMBER: builtins.int
     MULTIPLEXER_RESOURCE_NAME_FIELD_NUMBER: builtins.int
@@ -107,70 +105,65 @@
         *,
         pin_or_relay_name: builtins.str = ...,
         site: builtins.int = ...,
         channel: builtins.str = ...,
         multiplexer_resource_name: builtins.str = ...,
         multiplexer_route: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["channel", b"channel", "multiplexer_resource_name", b"multiplexer_resource_name", "multiplexer_route", b"multiplexer_route", "pin_or_relay_name", b"pin_or_relay_name", "site", b"site"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["channel", b"channel", "multiplexer_resource_name", b"multiplexer_resource_name", "multiplexer_route", b"multiplexer_route", "pin_or_relay_name", b"pin_or_relay_name", "site", b"site"]) -> None: ...
 
 global___ChannelMapping = ChannelMapping
 
-@typing_extensions.final
+@typing.final
 class MultiplexerSessionInformation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSION_FIELD_NUMBER: builtins.int
     RESOURCE_NAME_FIELD_NUMBER: builtins.int
     MULTIPLEXER_TYPE_ID_FIELD_NUMBER: builtins.int
     SESSION_EXISTS_FIELD_NUMBER: builtins.int
-    @property
-    def session(self) -> session_pb2.Session:
-        """Session identifier used to identify the session in the session management service, as well as in driver services such as grpc-device.
-        This field is readonly.
-        """
     resource_name: builtins.str
     """Resource name is used to open this session in the driver.
     This field is readonly.
     """
     multiplexer_type_id: builtins.str
     """User-defined identifier for the multiplexer type in the pin map editor.
     This field is readonly.
     """
     session_exists: builtins.bool
     """Indicates whether the session exists in the Session Manager. This indicates whether the session has been created.
     This field is readonly.
     """
+    @property
+    def session(self) -> session_pb2.Session:
+        """Session identifier used to identify the session in the session management service, as well as in driver services such as grpc-device.
+        This field is readonly.
+        """
+
     def __init__(
         self,
         *,
         session: session_pb2.Session | None = ...,
         resource_name: builtins.str = ...,
         multiplexer_type_id: builtins.str = ...,
         session_exists: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["session", b"session"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["multiplexer_type_id", b"multiplexer_type_id", "resource_name", b"resource_name", "session", b"session", "session_exists", b"session_exists"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["session", b"session"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["multiplexer_type_id", b"multiplexer_type_id", "resource_name", b"resource_name", "session", b"session", "session_exists", b"session_exists"]) -> None: ...
 
 global___MultiplexerSessionInformation = MultiplexerSessionInformation
 
-@typing_extensions.final
+@typing.final
 class ReserveSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_CONTEXT_FIELD_NUMBER: builtins.int
     PIN_OR_RELAY_NAMES_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_ID_FIELD_NUMBER: builtins.int
     TIMEOUT_IN_MILLISECONDS_FIELD_NUMBER: builtins.int
-    @property
-    def pin_map_context(self) -> ni_measurementlink_pin_map_context_pb2.PinMapContext:
-        """Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement."""
-    @property
-    def pin_or_relay_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """Optional. List of pins, pin groups, relays, or relay groups to use for the measurement. If unspecified, reserve sessions for all pins and relays in the registered pin map resource."""
     instrument_type_id: builtins.str
     """Optional. Instrument type ID for the measurement. If unspecified, reserve sessions for all instrument types connected in the registered pin map resource.
     Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
          "niDCPower"
          "niDigitalPattern"
          "niScope"
          "niDMM"
@@ -179,154 +172,168 @@
          "niRelayDriver"
     For custom instruments the user defined instrument type id is defined in the pin map file.
     """
     timeout_in_milliseconds: builtins.int
     """Optional. Timeout for the reservation request.
     Allowed values: 0 (non-blocking, fails immediately if resources cannot be reserved), -1 (infinite timeout), or any other positive numeric value (wait for that number of milliseconds)
     """
+    @property
+    def pin_map_context(self) -> ni_measurementlink_pin_map_context_pb2.PinMapContext:
+        """Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement."""
+
+    @property
+    def pin_or_relay_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Optional. List of pins, pin groups, relays, or relay groups to use for the measurement. If unspecified, reserve sessions for all pins and relays in the registered pin map resource."""
+
     def __init__(
         self,
         *,
         pin_map_context: ni_measurementlink_pin_map_context_pb2.PinMapContext | None = ...,
         pin_or_relay_names: collections.abc.Iterable[builtins.str] | None = ...,
         instrument_type_id: builtins.str = ...,
         timeout_in_milliseconds: builtins.int = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["instrument_type_id", b"instrument_type_id", "pin_map_context", b"pin_map_context", "pin_or_relay_names", b"pin_or_relay_names", "timeout_in_milliseconds", b"timeout_in_milliseconds"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["instrument_type_id", b"instrument_type_id", "pin_map_context", b"pin_map_context", "pin_or_relay_names", b"pin_or_relay_names", "timeout_in_milliseconds", b"timeout_in_milliseconds"]) -> None: ...
 
 global___ReserveSessionsRequest = ReserveSessionsRequest
 
-@typing_extensions.final
+@typing.final
 class ReserveSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class GroupMappingsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___ResolvedPinsOrRelays: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: global___ResolvedPinsOrRelays | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     SESSIONS_FIELD_NUMBER: builtins.int
     MULTIPLEXER_SESSIONS_FIELD_NUMBER: builtins.int
     GROUP_MAPPINGS_FIELD_NUMBER: builtins.int
     @property
     def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """List of information needed to create or use each session for the given pin, site, and instrument type ID."""
+
     @property
     def multiplexer_sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MultiplexerSessionInformation]:
         """List of information needed to create or use each multiplexer session for the given pin, site, and instrument type ID."""
+
     @property
     def group_mappings(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___ResolvedPinsOrRelays]:
         """Represents the mapping between pin or relay groups and their respective pin or relay names."""
+
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
         multiplexer_sessions: collections.abc.Iterable[global___MultiplexerSessionInformation] | None = ...,
         group_mappings: collections.abc.Mapping[builtins.str, global___ResolvedPinsOrRelays] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["group_mappings", b"group_mappings", "multiplexer_sessions", b"multiplexer_sessions", "sessions", b"sessions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["group_mappings", b"group_mappings", "multiplexer_sessions", b"multiplexer_sessions", "sessions", b"sessions"]) -> None: ...
 
 global___ReserveSessionsResponse = ReserveSessionsResponse
 
-@typing_extensions.final
+@typing.final
 class UnreserveSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSIONS_FIELD_NUMBER: builtins.int
     @property
     def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """Required. List of information of sessions to be unreserved in the session management service."""
+
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["sessions", b"sessions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["sessions", b"sessions"]) -> None: ...
 
 global___UnreserveSessionsRequest = UnreserveSessionsRequest
 
-@typing_extensions.final
+@typing.final
 class UnreserveSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___UnreserveSessionsResponse = UnreserveSessionsResponse
 
-@typing_extensions.final
+@typing.final
 class RegisterSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSIONS_FIELD_NUMBER: builtins.int
     @property
     def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """Required. List of sessions to register with the session management service to track as the sessions are open."""
+
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["sessions", b"sessions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["sessions", b"sessions"]) -> None: ...
 
 global___RegisterSessionsRequest = RegisterSessionsRequest
 
-@typing_extensions.final
+@typing.final
 class RegisterSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___RegisterSessionsResponse = RegisterSessionsResponse
 
-@typing_extensions.final
+@typing.final
 class UnregisterSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSIONS_FIELD_NUMBER: builtins.int
     @property
     def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """Required. List of sessions to unregister with the session management service to mark them as sessions were closed."""
+
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["sessions", b"sessions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["sessions", b"sessions"]) -> None: ...
 
 global___UnregisterSessionsRequest = UnregisterSessionsRequest
 
-@typing_extensions.final
+@typing.final
 class UnregisterSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___UnregisterSessionsResponse = UnregisterSessionsResponse
 
-@typing_extensions.final
+@typing.final
 class ReserveAllRegisteredSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIMEOUT_IN_MILLISECONDS_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_ID_FIELD_NUMBER: builtins.int
     timeout_in_milliseconds: builtins.int
     """Optional. Timeout for the reservation request.
@@ -346,174 +353,181 @@
     """
     def __init__(
         self,
         *,
         timeout_in_milliseconds: builtins.int = ...,
         instrument_type_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["instrument_type_id", b"instrument_type_id", "timeout_in_milliseconds", b"timeout_in_milliseconds"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["instrument_type_id", b"instrument_type_id", "timeout_in_milliseconds", b"timeout_in_milliseconds"]) -> None: ...
 
 global___ReserveAllRegisteredSessionsRequest = ReserveAllRegisteredSessionsRequest
 
-@typing_extensions.final
+@typing.final
 class ReserveAllRegisteredSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSIONS_FIELD_NUMBER: builtins.int
     @property
     def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """Sessions currently registered in the session management service."""
+
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["sessions", b"sessions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["sessions", b"sessions"]) -> None: ...
 
 global___ReserveAllRegisteredSessionsResponse = ReserveAllRegisteredSessionsResponse
 
-@typing_extensions.final
+@typing.final
 class RegisterMultiplexerSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MULTIPLEXER_SESSIONS_FIELD_NUMBER: builtins.int
     @property
     def multiplexer_sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MultiplexerSessionInformation]:
         """Required. List of multiplexer sessions to register with the session management service to track as the sessions are open."""
+
     def __init__(
         self,
         *,
         multiplexer_sessions: collections.abc.Iterable[global___MultiplexerSessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["multiplexer_sessions", b"multiplexer_sessions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["multiplexer_sessions", b"multiplexer_sessions"]) -> None: ...
 
 global___RegisterMultiplexerSessionsRequest = RegisterMultiplexerSessionsRequest
 
-@typing_extensions.final
+@typing.final
 class RegisterMultiplexerSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___RegisterMultiplexerSessionsResponse = RegisterMultiplexerSessionsResponse
 
-@typing_extensions.final
+@typing.final
 class UnregisterMultiplexerSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MULTIPLEXER_SESSIONS_FIELD_NUMBER: builtins.int
     @property
     def multiplexer_sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MultiplexerSessionInformation]:
         """Required. List of multiplexer sessions to unregister with the session management service to mark them as sessions were closed."""
+
     def __init__(
         self,
         *,
         multiplexer_sessions: collections.abc.Iterable[global___MultiplexerSessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["multiplexer_sessions", b"multiplexer_sessions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["multiplexer_sessions", b"multiplexer_sessions"]) -> None: ...
 
 global___UnregisterMultiplexerSessionsRequest = UnregisterMultiplexerSessionsRequest
 
-@typing_extensions.final
+@typing.final
 class UnregisterMultiplexerSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___UnregisterMultiplexerSessionsResponse = UnregisterMultiplexerSessionsResponse
 
-@typing_extensions.final
+@typing.final
 class GetMultiplexerSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_CONTEXT_FIELD_NUMBER: builtins.int
     MULTIPLEXER_TYPE_ID_FIELD_NUMBER: builtins.int
-    @property
-    def pin_map_context(self) -> ni_measurementlink_pin_map_context_pb2.PinMapContext:
-        """Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement."""
     multiplexer_type_id: builtins.str
     """Optional. User-defined identifier for the multiplexer type in the pin map editor.
     If unspecified, information for all multiplexer types is returned.
     """
+    @property
+    def pin_map_context(self) -> ni_measurementlink_pin_map_context_pb2.PinMapContext:
+        """Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement."""
+
     def __init__(
         self,
         *,
         pin_map_context: ni_measurementlink_pin_map_context_pb2.PinMapContext | None = ...,
         multiplexer_type_id: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["multiplexer_type_id", b"multiplexer_type_id", "pin_map_context", b"pin_map_context"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["multiplexer_type_id", b"multiplexer_type_id", "pin_map_context", b"pin_map_context"]) -> None: ...
 
 global___GetMultiplexerSessionsRequest = GetMultiplexerSessionsRequest
 
-@typing_extensions.final
+@typing.final
 class GetMultiplexerSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MULTIPLEXER_SESSIONS_FIELD_NUMBER: builtins.int
     @property
     def multiplexer_sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MultiplexerSessionInformation]:
         """List of information needed to create or use each multiplexer session for the given pin map context and multiplexer type ID."""
+
     def __init__(
         self,
         *,
         multiplexer_sessions: collections.abc.Iterable[global___MultiplexerSessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["multiplexer_sessions", b"multiplexer_sessions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["multiplexer_sessions", b"multiplexer_sessions"]) -> None: ...
 
 global___GetMultiplexerSessionsResponse = GetMultiplexerSessionsResponse
 
-@typing_extensions.final
+@typing.final
 class GetAllRegisteredMultiplexerSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MULTIPLEXER_TYPE_ID_FIELD_NUMBER: builtins.int
     multiplexer_type_id: builtins.str
     """Optional. User-defined identifier for the multiplexer type in the pin map editor.
     If unspecified, information for all registered multiplexer types is returned.
     """
     def __init__(
         self,
         *,
         multiplexer_type_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["multiplexer_type_id", b"multiplexer_type_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["multiplexer_type_id", b"multiplexer_type_id"]) -> None: ...
 
 global___GetAllRegisteredMultiplexerSessionsRequest = GetAllRegisteredMultiplexerSessionsRequest
 
-@typing_extensions.final
+@typing.final
 class GetAllRegisteredMultiplexerSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MULTIPLEXER_SESSIONS_FIELD_NUMBER: builtins.int
     @property
     def multiplexer_sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MultiplexerSessionInformation]:
         """Multiplexer sessions currently registered in the session management service."""
+
     def __init__(
         self,
         *,
         multiplexer_sessions: collections.abc.Iterable[global___MultiplexerSessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["multiplexer_sessions", b"multiplexer_sessions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["multiplexer_sessions", b"multiplexer_sessions"]) -> None: ...
 
 global___GetAllRegisteredMultiplexerSessionsResponse = GetAllRegisteredMultiplexerSessionsResponse
 
-@typing_extensions.final
+@typing.final
 class ResolvedPinsOrRelays(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_OR_RELAY_NAMES_FIELD_NUMBER: builtins.int
     @property
     def pin_or_relay_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """List of pin or relay names in the pin or relay group."""
+
     def __init__(
         self,
         *,
         pin_or_relay_names: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pin_or_relay_names", b"pin_or_relay_names"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["pin_or_relay_names", b"pin_or_relay_names"]) -> None: ...
 
 global___ResolvedPinsOrRelays = ResolvedPinsOrRelays
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import abc
 import collections.abc
 import grpc
 import grpc.aio
 import ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement.v1.session_management_service_pb2 as ni_measurementlink_sessionmanagement_v1_session_management_service_pb2
 import typing
 
-_T = typing.TypeVar('_T')
+_T = typing.TypeVar("_T")
 
-class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
-    ...
+class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta): ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore[misc, type-arg]
     ...
 
 class SessionManagementServiceStub:
     """Service to keep track of open sessions used by measurement services, and to allow measurement services to access sessions by pin and site."""
 
     def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None: ...
     ReserveSessions: grpc.UnaryUnaryMultiCallable[
@@ -33,75 +33,83 @@
         - Pin or relay name does not match any pin, pin group, relay, or relay group names in the pin map
         - Timeout specified is less than -1.
     - NOT_FOUND:
         - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
     - UNAVAILABLE:
         - Session(s) were already reserved and didn't become available before the specified timeout expired.
     """
+
     UnreserveSessions: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnreserveSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnreserveSessionsResponse,
     ]
     """Unreserves sessions so they can be accessed by other clients.
     - RESOURCE_EXHAUSTED:
         - Error occurred while unreserving sessions.
     """
+
     RegisterSessions: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterSessionsResponse,
     ]
     """Registers the sessions with this service. Indicates that the sessions are open and will need to be closed later.
     Status Codes for errors:
     - ALREADY_EXISTS:
         - Session by the same name is already registered.
     - INVALID_ARGUMENT:
         - Session names list has an empty string.
     """
+
     UnregisterSessions: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterSessionsResponse,
     ]
     """Unregisters the sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again."""
+
     ReserveAllRegisteredSessions: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.ReserveAllRegisteredSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.ReserveAllRegisteredSessionsResponse,
     ]
     """Reserves and gets all sessions currently registered with this service.
     - INVALID_ARGUMENT:
         - Timeout specified is less than -1.
     - UNAVAILABLE:
         - Session(s) were already reserved and didn't become available before the specified timeout expired.
     """
+
     RegisterMultiplexerSessions: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterMultiplexerSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterMultiplexerSessionsResponse,
     ]
     """Registers the multiplexer sessions with this service. Indicates that the sessions are open and will need to be closed later.
     Status Codes for errors:
     - ALREADY_EXISTS:
         - Session by the same name is already registered.
     - INVALID_ARGUMENT:
         - Session names list has an empty string.
     """
+
     UnregisterMultiplexerSessions: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterMultiplexerSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterMultiplexerSessionsResponse,
     ]
     """Unregisters the multiplexer sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again."""
+
     GetMultiplexerSessions: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetMultiplexerSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetMultiplexerSessionsResponse,
     ]
     """Gets all the connected multiplexer session(s) for the given pin map context and returns information needed to create or access the session.
     Status Codes for errors:
     - INVALID_ARGUMENT:
         - Pin Map Context references a site number that is not defined in the pin map.
     - NOT_FOUND:
         - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
     """
+
     GetAllRegisteredMultiplexerSessions: grpc.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetAllRegisteredMultiplexerSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetAllRegisteredMultiplexerSessionsResponse,
     ]
     """Gets all multiplexer sessions currently registered with this service."""
 
 class SessionManagementServiceAsyncStub:
@@ -119,75 +127,83 @@
         - Pin or relay name does not match any pin, pin group, relay, or relay group names in the pin map
         - Timeout specified is less than -1.
     - NOT_FOUND:
         - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
     - UNAVAILABLE:
         - Session(s) were already reserved and didn't become available before the specified timeout expired.
     """
+
     UnreserveSessions: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnreserveSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnreserveSessionsResponse,
     ]
     """Unreserves sessions so they can be accessed by other clients.
     - RESOURCE_EXHAUSTED:
         - Error occurred while unreserving sessions.
     """
+
     RegisterSessions: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterSessionsResponse,
     ]
     """Registers the sessions with this service. Indicates that the sessions are open and will need to be closed later.
     Status Codes for errors:
     - ALREADY_EXISTS:
         - Session by the same name is already registered.
     - INVALID_ARGUMENT:
         - Session names list has an empty string.
     """
+
     UnregisterSessions: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterSessionsResponse,
     ]
     """Unregisters the sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again."""
+
     ReserveAllRegisteredSessions: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.ReserveAllRegisteredSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.ReserveAllRegisteredSessionsResponse,
     ]
     """Reserves and gets all sessions currently registered with this service.
     - INVALID_ARGUMENT:
         - Timeout specified is less than -1.
     - UNAVAILABLE:
         - Session(s) were already reserved and didn't become available before the specified timeout expired.
     """
+
     RegisterMultiplexerSessions: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterMultiplexerSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterMultiplexerSessionsResponse,
     ]
     """Registers the multiplexer sessions with this service. Indicates that the sessions are open and will need to be closed later.
     Status Codes for errors:
     - ALREADY_EXISTS:
         - Session by the same name is already registered.
     - INVALID_ARGUMENT:
         - Session names list has an empty string.
     """
+
     UnregisterMultiplexerSessions: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterMultiplexerSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterMultiplexerSessionsResponse,
     ]
     """Unregisters the multiplexer sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again."""
+
     GetMultiplexerSessions: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetMultiplexerSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetMultiplexerSessionsResponse,
     ]
     """Gets all the connected multiplexer session(s) for the given pin map context and returns information needed to create or access the session.
     Status Codes for errors:
     - INVALID_ARGUMENT:
         - Pin Map Context references a site number that is not defined in the pin map.
     - NOT_FOUND:
         - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
     """
+
     GetAllRegisteredMultiplexerSessions: grpc.aio.UnaryUnaryMultiCallable[
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetAllRegisteredMultiplexerSessionsRequest,
         ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetAllRegisteredMultiplexerSessionsResponse,
     ]
     """Gets all multiplexer sessions currently registered with this service."""
 
 class SessionManagementServiceServicer(metaclass=abc.ABCMeta):
@@ -207,89 +223,97 @@
             - Pin or relay name does not match any pin, pin group, relay, or relay group names in the pin map
             - Timeout specified is less than -1.
         - NOT_FOUND:
             - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
         - UNAVAILABLE:
             - Session(s) were already reserved and didn't become available before the specified timeout expired.
         """
+
     @abc.abstractmethod
     def UnreserveSessions(
         self,
         request: ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnreserveSessionsRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnreserveSessionsResponse, collections.abc.Awaitable[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnreserveSessionsResponse]]:
         """Unreserves sessions so they can be accessed by other clients.
         - RESOURCE_EXHAUSTED:
             - Error occurred while unreserving sessions.
         """
+
     @abc.abstractmethod
     def RegisterSessions(
         self,
         request: ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterSessionsRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterSessionsResponse, collections.abc.Awaitable[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterSessionsResponse]]:
         """Registers the sessions with this service. Indicates that the sessions are open and will need to be closed later.
         Status Codes for errors:
         - ALREADY_EXISTS:
             - Session by the same name is already registered.
         - INVALID_ARGUMENT:
             - Session names list has an empty string.
         """
+
     @abc.abstractmethod
     def UnregisterSessions(
         self,
         request: ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterSessionsRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterSessionsResponse, collections.abc.Awaitable[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterSessionsResponse]]:
         """Unregisters the sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again."""
+
     @abc.abstractmethod
     def ReserveAllRegisteredSessions(
         self,
         request: ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.ReserveAllRegisteredSessionsRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.ReserveAllRegisteredSessionsResponse, collections.abc.Awaitable[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.ReserveAllRegisteredSessionsResponse]]:
         """Reserves and gets all sessions currently registered with this service.
         - INVALID_ARGUMENT:
             - Timeout specified is less than -1.
         - UNAVAILABLE:
             - Session(s) were already reserved and didn't become available before the specified timeout expired.
         """
+
     @abc.abstractmethod
     def RegisterMultiplexerSessions(
         self,
         request: ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterMultiplexerSessionsRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterMultiplexerSessionsResponse, collections.abc.Awaitable[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.RegisterMultiplexerSessionsResponse]]:
         """Registers the multiplexer sessions with this service. Indicates that the sessions are open and will need to be closed later.
         Status Codes for errors:
         - ALREADY_EXISTS:
             - Session by the same name is already registered.
         - INVALID_ARGUMENT:
             - Session names list has an empty string.
         """
+
     @abc.abstractmethod
     def UnregisterMultiplexerSessions(
         self,
         request: ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterMultiplexerSessionsRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterMultiplexerSessionsResponse, collections.abc.Awaitable[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.UnregisterMultiplexerSessionsResponse]]:
         """Unregisters the multiplexer sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again."""
+
     @abc.abstractmethod
     def GetMultiplexerSessions(
         self,
         request: ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetMultiplexerSessionsRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetMultiplexerSessionsResponse, collections.abc.Awaitable[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetMultiplexerSessionsResponse]]:
         """Gets all the connected multiplexer session(s) for the given pin map context and returns information needed to create or access the session.
         Status Codes for errors:
         - INVALID_ARGUMENT:
             - Pin Map Context references a site number that is not defined in the pin map.
         - NOT_FOUND:
             - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
         """
+
     @abc.abstractmethod
     def GetAllRegisteredMultiplexerSessions(
         self,
         request: ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetAllRegisteredMultiplexerSessionsRequest,
         context: _ServicerContext,
     ) -> typing.Union[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetAllRegisteredMultiplexerSessionsResponse, collections.abc.Awaitable[ni_measurementlink_sessionmanagement_v1_session_management_service_pb2.GetAllRegisteredMultiplexerSessionsResponse]]:
         """Gets all multiplexer sessions currently registered with this service."""
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 ---------------------------------------------------------------------
 ---------------------------------------------------------------------
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import sys
-
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
+import typing
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class DoubleXYData(google.protobuf.message.Message):
     """XYData for a cartesian graph.
     x_data and y_data should contain the same number of values.
     If they do not, the smaller-sized array will be used to determine
     the number of XY points.
     """
 
@@ -36,10 +32,10 @@
     def y_data(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
     def __init__(
         self,
         *,
         x_data: collections.abc.Iterable[builtins.float] | None = ...,
         y_data: collections.abc.Iterable[builtins.float] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["x_data", b"x_data", "y_data", b"y_data"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["x_data", b"x_data", "y_data", b"y_data"]) -> None: ...
 
 global___DoubleXYData = DoubleXYData
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2_grpc.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/ni/protobuf/types/xydata_pb2_grpc.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 ---------------------------------------------------------------------
 ---------------------------------------------------------------------
 """
+
 import abc
 import collections.abc
 import grpc
 import grpc.aio
 import typing
 
-_T = typing.TypeVar('_T')
+_T = typing.TypeVar("_T")
 
-class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
-    ...
+class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta): ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore[misc, type-arg]
     ...
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/README.md` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 option java_outer_classname = "PinMapContextProto";
 option java_package = "com.ni.measurementlink";
 option objc_class_prefix = "NIM";
 option php_namespace = "NI\\MeasurementLink";
 option ruby_package = "NI::MeasurementLink";
 
 message PinMapContext {
-    // Required. The resource id of the pin map in the Pin Map service that should be used for the call.
-    string pin_map_id = 1;
+  // Required. The resource id of the pin map in the Pin Map service that should be used for the call.
+  string pin_map_id = 1;
 
-    // Optional. List of site numbers being used for the call. If unspecified, use all sites in the pin map.
-    repeated int32 sites = 2;
+  // Optional. List of site numbers being used for the call. If unspecified, use all sites in the pin map.
+  repeated int32 sites = 2;
 }
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto`

 * *Files 12% similar despite different names*

```diff
@@ -9,235 +9,235 @@
 option java_package = "com.ni.measurementlink.pinmap.v1";
 option objc_class_prefix = "NIMP";
 option php_namespace = "NI\\MeasurementLink\\PinMap\\V1";
 option ruby_package = "NI::MeasurementLink::PinMap::V1";
 
 // Service to keep track of pin map resources.
 service PinMapService {
-    // Registers pin map with the PinMapService and returns a pin map resource.
-    // Status Codes for errors:
-    // - INVALID_ARGUMENT: Pin map id is empty or has whitespace, or pin map xml string is not valid
-    // - ALREADY_EXISTS: Pin map resource with the specified pin map id already exists
-    rpc CreatePinMapFromXml(CreatePinMapFromXmlRequest) returns(PinMap);
-
-    // Updates registered pin map contents and returns it.
-    // Creates and registers a pin map if a pin map resource for the specified pin map id is not found.
-    // Status Codes for errors:
-    // - INVALID_ARGUMENT: Pin map xml string is not valid
-    rpc UpdatePinMapFromXml(UpdatePinMapFromXmlRequest) returns (PinMap);
-
-    // Get registered pin map resource.
-    // Status Codes for errors:
-    // - NOT_FOUND: Pin map resource for the specified pin map id is not found
-    rpc GetPinMap(GetPinMapRequest) returns(PinMap);
-
-    // Returns list of pins from the registered pin map resource.
-    // Status Codes for errors:
-    // - NOT_FOUND: Pin map resource for the specified pin map id is not found
-    rpc QueryPins(QueryPinsRequest) returns (QueryPinsResponse);
-
-    // Returns list of relays from the registered pin map resource.
-    // Status Codes for errors:
-    // - NOT_FOUND: Pin map resource for the specified pin map id is not found
-    rpc QueryRelays(QueryRelaysRequest) returns (QueryRelaysResponse);
-
-    // Get instrument resource names, channels, and instrument type for the specified sites, pins or pin groups, relays or relay groups, instrument type in the registered pin map resource.
-    // Status Codes for errors:
-    // - NOT_FOUND:
-    //   - Pin map resource for the specified pin map id is not found.
-    //   - Specified site number is not in the valid range for the registered pin map.
-    // - INVALID_ARGUMENT:
-    //   - Specified pin or relay is not present in the registered pin map resource.
-    //   - Empty string specified for a pin or relay name.
-    rpc QueryResourceAccessInformation(QueryResourceAccessInformationRequest) returns (QueryResourceAccessInformationResponse);
+  // Registers pin map with the PinMapService and returns a pin map resource.
+  // Status Codes for errors:
+  // - INVALID_ARGUMENT: Pin map id is empty or has whitespace, or pin map xml string is not valid
+  // - ALREADY_EXISTS: Pin map resource with the specified pin map id already exists
+  rpc CreatePinMapFromXml(CreatePinMapFromXmlRequest) returns(PinMap);
+
+  // Updates registered pin map contents and returns it.
+  // Creates and registers a pin map if a pin map resource for the specified pin map id is not found.
+  // Status Codes for errors:
+  // - INVALID_ARGUMENT: Pin map xml string is not valid
+  rpc UpdatePinMapFromXml(UpdatePinMapFromXmlRequest) returns (PinMap);
+
+  // Get registered pin map resource.
+  // Status Codes for errors:
+  // - NOT_FOUND: Pin map resource for the specified pin map id is not found
+  rpc GetPinMap(GetPinMapRequest) returns(PinMap);
+
+  // Returns list of pins from the registered pin map resource.
+  // Status Codes for errors:
+  // - NOT_FOUND: Pin map resource for the specified pin map id is not found
+  rpc QueryPins(QueryPinsRequest) returns (QueryPinsResponse);
+
+  // Returns list of relays from the registered pin map resource.
+  // Status Codes for errors:
+  // - NOT_FOUND: Pin map resource for the specified pin map id is not found
+  rpc QueryRelays(QueryRelaysRequest) returns (QueryRelaysResponse);
+
+  // Get instrument resource names, channels, and instrument type for the specified sites, pins or pin groups, relays or relay groups, instrument type in the registered pin map resource.
+  // Status Codes for errors:
+  // - NOT_FOUND:
+  //   - Pin map resource for the specified pin map id is not found.
+  //   - Specified site number is not in the valid range for the registered pin map.
+  // - INVALID_ARGUMENT:
+  //   - Specified pin or relay is not present in the registered pin map resource.
+  //   - Empty string specified for a pin or relay name.
+  rpc QueryResourceAccessInformation(QueryResourceAccessInformationRequest) returns (QueryResourceAccessInformationResponse);
 }
 
 // Pin map resource type.
 message PinMap {
-    // Output only. The resource id of the registered pin map resource.
-    string pin_map_id = 1;
+  // Output only. The resource id of the registered pin map resource.
+  string pin_map_id = 1;
 }
 
 message CreatePinMapFromXmlRequest {
-    // Required. The resource id of the pin map to register as a pin map resource.
-    string pin_map_id = 1;
+  // Required. The resource id of the pin map to register as a pin map resource.
+  string pin_map_id = 1;
 
-    // Required. A string representing contents of a pin map file.
-    string pin_map_xml = 2;
+  // Required. A string representing contents of a pin map file.
+  string pin_map_xml = 2;
 }
 
 message UpdatePinMapFromXmlRequest {
-    // Required. The resource id of the pin map to be updated.
-    string pin_map_id = 1;
+  // Required. The resource id of the pin map to be updated.
+  string pin_map_id = 1;
 
-    // Required. New pin map file content.
-    string pin_map_xml = 2;
+  // Required. New pin map file content.
+  string pin_map_xml = 2;
 }
 
 message GetPinMapRequest {
-    // Required. The resource id of the registered pin map resource.
-    string pin_map_id = 1;
+  // Required. The resource id of the registered pin map resource.
+  string pin_map_id = 1;
 }
 
 message QueryPinsRequest {
-    // Required. The resource id of the registered pin map resource.
-    string pin_map_id = 1;
+  // Required. The resource id of the registered pin map resource.
+  string pin_map_id = 1;
 
-    // Optional. Filter pins by instrument type.
-    // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
-    //      "niDCPower"
-    //      "niDigitalPattern"
-    //      "niScope"
-    //      "niDMM"
-    //      "niDAQmx"
-    //      "niFGen"
-    // For custom instruments the user defined instrument type id is defined in the pin map file.
-    string instrument_type_id = 2;
+  // Optional. Filter pins by instrument type.
+  // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
+  //      "niDCPower"
+  //      "niDigitalPattern"
+  //      "niScope"
+  //      "niDMM"
+  //      "niDAQmx"
+  //      "niFGen"
+  // For custom instruments the user defined instrument type id is defined in the pin map file.
+  string instrument_type_id = 2;
 }
 
 message QueryPinsResponse {
-    // List of pins on the registered pin map resource. This list includes both DUT and System pins.
-    repeated PinDefinition pins = 1;
+  // List of pins on the registered pin map resource. This list includes both DUT and System pins.
+  repeated PinDefinition pins = 1;
 
-    // List of pin groups on the registered pin map resource.
-    // When an instrument type id filter is specified, a pin group will only be included
-    // in the response if all pins in the pin group match the instrument type.
-    repeated PinGroupDefinition pin_groups = 2;
+  // List of pin groups on the registered pin map resource.
+  // When an instrument type id filter is specified, a pin group will only be included
+  // in the response if all pins in the pin group match the instrument type.
+  repeated PinGroupDefinition pin_groups = 2;
 }
 
 message PinDefinition {
-    // Name of the dut pin.
-    string display_name = 1;
+  // Name of the dut pin.
+  string display_name = 1;
 
-    // A boolean that indicates a System pin when 'true', or DUT pin when 'false'.
-    bool is_system_pin = 2;
+  // A boolean that indicates a System pin when 'true', or DUT pin when 'false'.
+  bool is_system_pin = 2;
 }
 
 message PinGroupDefinition {
-    // Name of the pin group.
-    string display_name = 1;
+  // Name of the pin group.
+  string display_name = 1;
 
-    // List of other pins or pin groups within this pin group.
-    repeated string pin_or_group_references = 2;
+  // List of other pins or pin groups within this pin group.
+  repeated string pin_or_group_references = 2;
 
-    // Distinct union of pins within this pin group, including those within nested pin groups.
-    repeated string resolved_pins = 3;
+  // Distinct union of pins within this pin group, including those within nested pin groups.
+  repeated string resolved_pins = 3;
 }
 
 message QueryRelaysRequest {
-    // Required. The resource id of the registered pin map resource.
-    string pin_map_id = 1;
+  // Required. The resource id of the registered pin map resource.
+  string pin_map_id = 1;
 }
 
 message QueryRelaysResponse {
-    // List of relays on the registered pin map resource. This list includes both Site relays and System relays.
-    repeated RelayDefinition relays = 1;
+  // List of relays on the registered pin map resource. This list includes both Site relays and System relays.
+  repeated RelayDefinition relays = 1;
 
-    // List of relay groups on the registered pin map resource.
-    repeated RelayGroupDefinition relay_groups = 2;
+  // List of relay groups on the registered pin map resource.
+  repeated RelayGroupDefinition relay_groups = 2;
 }
 
 message RelayDefinition {
-    // Name of the relay.
-    string display_name = 1;
+  // Name of the relay.
+  string display_name = 1;
 
-    // A boolean that indicates a System relay when 'true', or Site relay when 'false'.
-    bool is_system_relay = 2;
+  // A boolean that indicates a System relay when 'true', or Site relay when 'false'.
+  bool is_system_relay = 2;
 }
 
 message RelayGroupDefinition {
-    // Name of the relay group.
-    string display_name = 1;
+  // Name of the relay group.
+  string display_name = 1;
 
-    // List of other relays or relay groups within this relay group.
-    repeated string relay_or_group_references = 2;
+  // List of other relays or relay groups within this relay group.
+  repeated string relay_or_group_references = 2;
 
-    // Distinct union of relays within this relay group, including those within nested relay groups.
-    repeated string resolved_relays = 3;
+  // Distinct union of relays within this relay group, including those within nested relay groups.
+  repeated string resolved_relays = 3;
 }
 
 message QueryResourceAccessInformationRequest {
-    // Required. The resource id of the registered pin map resource.
-    string pin_map_id = 1;
+  // Required. The resource id of the registered pin map resource.
+  string pin_map_id = 1;
 
-    // Optional. The list of sites for which to get instrument resource access information. If unspecified, get instrument resource information for all sites in the registered pin map resource.
-    repeated int32 sites = 2;
+  // Optional. The list of sites for which to get instrument resource access information. If unspecified, get instrument resource information for all sites in the registered pin map resource.
+  repeated int32 sites = 2;
 
-    // Optional. The list of pins, pin groups, relays, or relay groups for which to get instrument resource access information. If unspecified, get instrument resource information for all pins and relays in the registered pin map resource.
-    repeated string pin_or_relay_names = 3;
+  // Optional. The list of pins, pin groups, relays, or relay groups for which to get instrument resource access information. If unspecified, get instrument resource information for all pins and relays in the registered pin map resource.
+  repeated string pin_or_relay_names = 3;
 
-    // Optional. The instrument type for which to get instrument resource access information. If unspecified, get instrument resource information for all instrument types connected in the registered pin map resource.
-    // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
-    //      "niDCPower"
-    //      "niDigitalPattern"
-    //      "niScope"
-    //      "niDMM"
-    //      "niDAQmx"
-    //      "niFGen"
-    //      "niRelayDriver"
-    // For custom instruments the user defined instrument type id is defined in the pin map file.
-    string instrument_type_id = 4;
+  // Optional. The instrument type for which to get instrument resource access information. If unspecified, get instrument resource information for all instrument types connected in the registered pin map resource.
+  // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
+  //      "niDCPower"
+  //      "niDigitalPattern"
+  //      "niScope"
+  //      "niDMM"
+  //      "niDAQmx"
+  //      "niFGen"
+  //      "niRelayDriver"
+  // For custom instruments the user defined instrument type id is defined in the pin map file.
+  string instrument_type_id = 4;
 }
 
 message QueryResourceAccessInformationResponse {
-    // List of ResourceAccessInformation objects with instrument resource names and channels.
-    repeated ResourceAccessInformation resource_access_information = 1;
+  // List of ResourceAccessInformation objects with instrument resource names and channels.
+  repeated ResourceAccessInformation resource_access_information = 1;
 
-    // Represents the mapping between pin or relay groups and their respective pin or relay names.
-    map<string, ResolvedPinsOrRelays> group_mappings = 2;
+  // Represents the mapping between pin or relay groups and their respective pin or relay names.
+  map<string, ResolvedPinsOrRelays> group_mappings = 2;
 }
 
 message ResourceAccessInformation {
-    // Name of the instrument resource.
-    // This string is used for initializing the driver session.
-    string resource_name = 1;
-
-    // Channels on the instrument resource.
-    // This string is used by various driver API methods such as Read, Fetch etc., and driver initialization for some instruments.
-    // For a resource that represents a group of instruments or channels in the pin map, the channel list is a comma separated list of fully qualified channels in the format <instrument_name>/<channel>, e.g. "DCPower1/0, DCPower1/2, DCPower2/0".
-    // For a resource that represents a single instrument in the pin map that is not part of a group, the channel list is a comma separated list of channels, e.g. "0, 1, 2".
-    // For NI-Digital Pattern devices, the channel list is a comma separated list of pins in the format <site_number>/<pin>, e.g. "site0/PinA, site1/PinB".
-    // For a resource that represents a relay driver, the channel list is a comma separated list of NISwitch relay names, e.g. "K0, K1, K2".
-    string channel_list = 2;
-
-    // The instrument type of the instrument resource.
-    // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
-    //      "niDCPower"
-    //      "niDigitalPattern"
-    //      "niScope"
-    //      "niDMM"
-    //      "niDAQmx"
-    //      "niFGen"
-    //      "niRelayDriver"
-    // For custom instruments the user defined instrument type id is defined in the pin map file.
-    string instrument_type_id = 3;
-
-    // List of site and pin/relay mappings with optional multiplexer information for each channel in the channel_list.
-    // Each item represents a channel-to-pin connection for this instrument resource. In the case of shared pins, there is a separate item for each connection.
-    repeated ChannelMapping channel_mappings = 4;
+  // Name of the instrument resource.
+  // This string is used for initializing the driver session.
+  string resource_name = 1;
+
+  // Channels on the instrument resource.
+  // This string is used by various driver API methods such as Read, Fetch etc., and driver initialization for some instruments.
+  // For a resource that represents a group of instruments or channels in the pin map, the channel list is a comma separated list of fully qualified channels in the format <instrument_name>/<channel>, e.g. "DCPower1/0, DCPower1/2, DCPower2/0".
+  // For a resource that represents a single instrument in the pin map that is not part of a group, the channel list is a comma separated list of channels, e.g. "0, 1, 2".
+  // For NI-Digital Pattern devices, the channel list is a comma separated list of pins in the format <site_number>/<pin>, e.g. "site0/PinA, site1/PinB".
+  // For a resource that represents a relay driver, the channel list is a comma separated list of NISwitch relay names, e.g. "K0, K1, K2".
+  string channel_list = 2;
+
+  // The instrument type of the instrument resource.
+  // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
+  //      "niDCPower"
+  //      "niDigitalPattern"
+  //      "niScope"
+  //      "niDMM"
+  //      "niDAQmx"
+  //      "niFGen"
+  //      "niRelayDriver"
+  // For custom instruments the user defined instrument type id is defined in the pin map file.
+  string instrument_type_id = 3;
+
+  // List of site and pin/relay mappings with optional multiplexer information for each channel in the channel_list.
+  // Each item represents a channel-to-pin connection for this instrument resource. In the case of shared pins, there is a separate item for each connection.
+  repeated ChannelMapping channel_mappings = 4;
 }
 
 message ChannelMapping {
-    // The pin or relay that is mapped to a channel.
-    string pin_or_relay_name = 1;
+  // The pin or relay that is mapped to a channel.
+  string pin_or_relay_name = 1;
 
-    // The site on which the pin or relay is mapped to a channel.
-    // For system pins/relays the site number is -1 since they do not belong to a specific site.
-    int32 site = 2;
+  // The site on which the pin or relay is mapped to a channel.
+  // For system pins/relays the site number is -1 since they do not belong to a specific site.
+  int32 site = 2;
 
-    // The channel to which the pin or relay is mapped on this site.
-    string channel = 3;
+  // The channel to which the pin or relay is mapped on this site.
+  string channel = 3;
 
-    // The multiplexer resource name is used to open the multiplexer session in the driver.
-    string multiplexer_resource_name = 4;
+  // The multiplexer resource name is used to open the multiplexer session in the driver.
+  string multiplexer_resource_name = 4;
 
-    // The multiplexer route through which the pin is connected to an instrument's channel.
-    string multiplexer_route = 5;
+  // The multiplexer route through which the pin is connected to an instrument's channel.
+  string multiplexer_route = 5;
 
-    // User-defined identifier for the multiplexer type in the pin map editor.
-    string multiplexer_type_id = 6;
+  // User-defined identifier for the multiplexer type in the pin map editor.
+  string multiplexer_type_id = 6;
 }
 
 message ResolvedPinsOrRelays {
   // List of pin or relay names in the pin or relay group.
   repeated string pin_or_relay_names = 1;
 }
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto`

 * *Files 6% similar despite different names*

```diff
@@ -12,267 +12,267 @@
 option java_package = "com.ni.measurementlink.sessionmanagement.v1";
 option objc_class_prefix = "NIMS";
 option php_namespace = "NI\\MeasurementLink\\SessionManagement\\V1";
 option ruby_package = "NI::MeasurementLink::SessionManagement::V1";
 
 // Service to keep track of open sessions used by measurement services, and to allow measurement services to access sessions by pin and site.
 service SessionManagementService {
-    // Reserve session(s) for the given pins or relays, sites, and instrument type ID and returns the information needed to create or access the session.
-    // Also reserves the session so other processes cannot access it with a ReserveSessions() call.
-    // Status Codes for errors:
-    // - INVALID_ARGUMENT:
-    //     - Pin Map Context references a site number that is not defined in the pin map
-    //     - Pin or relay name does not match any pin, pin group, relay, or relay group names in the pin map
-    //     - Timeout specified is less than -1.
-    // - NOT_FOUND:
-    //     - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
-    // - UNAVAILABLE:
-    //     - Session(s) were already reserved and didn't become available before the specified timeout expired.
-    rpc ReserveSessions(ReserveSessionsRequest) returns (ReserveSessionsResponse);
-
-    // Unreserves sessions so they can be accessed by other clients.
-    // - RESOURCE_EXHAUSTED:
-    //     - Error occurred while unreserving sessions.
-    rpc UnreserveSessions(UnreserveSessionsRequest) returns (UnreserveSessionsResponse);
-
-    // Registers the sessions with this service. Indicates that the sessions are open and will need to be closed later.
-    // Status Codes for errors:
-    // - ALREADY_EXISTS:
-    //     - Session by the same name is already registered.
-    // - INVALID_ARGUMENT:
-    //     - Session names list has an empty string.
-    rpc RegisterSessions(RegisterSessionsRequest) returns (RegisterSessionsResponse);
-
-    // Unregisters the sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again.
-    rpc UnregisterSessions(UnregisterSessionsRequest) returns (UnregisterSessionsResponse);
-
-    // Reserves and gets all sessions currently registered with this service.
-    // - INVALID_ARGUMENT:
-    //     - Timeout specified is less than -1.
-    // - UNAVAILABLE:
-    //     - Session(s) were already reserved and didn't become available before the specified timeout expired.
-    rpc ReserveAllRegisteredSessions(ReserveAllRegisteredSessionsRequest) returns (ReserveAllRegisteredSessionsResponse);
-
-    // Registers the multiplexer sessions with this service. Indicates that the sessions are open and will need to be closed later.
-    // Status Codes for errors:
-    // - ALREADY_EXISTS:
-    //     - Session by the same name is already registered.
-    // - INVALID_ARGUMENT:
-    //     - Session names list has an empty string.
-    rpc RegisterMultiplexerSessions(RegisterMultiplexerSessionsRequest) returns (RegisterMultiplexerSessionsResponse);
-
-    // Unregisters the multiplexer sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again.
-    rpc UnregisterMultiplexerSessions(UnregisterMultiplexerSessionsRequest) returns (UnregisterMultiplexerSessionsResponse);
-
-    // Gets all the connected multiplexer session(s) for the given pin map context and returns information needed to create or access the session.
-    // Status Codes for errors:
-    // - INVALID_ARGUMENT:
-    //     - Pin Map Context references a site number that is not defined in the pin map.
-    // - NOT_FOUND:
-    //     - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
-    rpc GetMultiplexerSessions(GetMultiplexerSessionsRequest) returns (GetMultiplexerSessionsResponse);
+  // Reserve session(s) for the given pins or relays, sites, and instrument type ID and returns the information needed to create or access the session.
+  // Also reserves the session so other processes cannot access it with a ReserveSessions() call.
+  // Status Codes for errors:
+  // - INVALID_ARGUMENT:
+  //     - Pin Map Context references a site number that is not defined in the pin map
+  //     - Pin or relay name does not match any pin, pin group, relay, or relay group names in the pin map
+  //     - Timeout specified is less than -1.
+  // - NOT_FOUND:
+  //     - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
+  // - UNAVAILABLE:
+  //     - Session(s) were already reserved and didn't become available before the specified timeout expired.
+  rpc ReserveSessions(ReserveSessionsRequest) returns (ReserveSessionsResponse);
+
+  // Unreserves sessions so they can be accessed by other clients.
+  // - RESOURCE_EXHAUSTED:
+  //     - Error occurred while unreserving sessions.
+  rpc UnreserveSessions(UnreserveSessionsRequest) returns (UnreserveSessionsResponse);
+
+  // Registers the sessions with this service. Indicates that the sessions are open and will need to be closed later.
+  // Status Codes for errors:
+  // - ALREADY_EXISTS:
+  //     - Session by the same name is already registered.
+  // - INVALID_ARGUMENT:
+  //     - Session names list has an empty string.
+  rpc RegisterSessions(RegisterSessionsRequest) returns (RegisterSessionsResponse);
+
+  // Unregisters the sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again.
+  rpc UnregisterSessions(UnregisterSessionsRequest) returns (UnregisterSessionsResponse);
+
+  // Reserves and gets all sessions currently registered with this service.
+  // - INVALID_ARGUMENT:
+  //     - Timeout specified is less than -1.
+  // - UNAVAILABLE:
+  //     - Session(s) were already reserved and didn't become available before the specified timeout expired.
+  rpc ReserveAllRegisteredSessions(ReserveAllRegisteredSessionsRequest) returns (ReserveAllRegisteredSessionsResponse);
+
+  // Registers the multiplexer sessions with this service. Indicates that the sessions are open and will need to be closed later.
+  // Status Codes for errors:
+  // - ALREADY_EXISTS:
+  //     - Session by the same name is already registered.
+  // - INVALID_ARGUMENT:
+  //     - Session names list has an empty string.
+  rpc RegisterMultiplexerSessions(RegisterMultiplexerSessionsRequest) returns (RegisterMultiplexerSessionsResponse);
+
+  // Unregisters the multiplexer sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again.
+  rpc UnregisterMultiplexerSessions(UnregisterMultiplexerSessionsRequest) returns (UnregisterMultiplexerSessionsResponse);
+
+  // Gets all the connected multiplexer session(s) for the given pin map context and returns information needed to create or access the session.
+  // Status Codes for errors:
+  // - INVALID_ARGUMENT:
+  //     - Pin Map Context references a site number that is not defined in the pin map.
+  // - NOT_FOUND:
+  //     - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
+  rpc GetMultiplexerSessions(GetMultiplexerSessionsRequest) returns (GetMultiplexerSessionsResponse);
 
-    // Gets all multiplexer sessions currently registered with this service.
-    rpc GetAllRegisteredMultiplexerSessions(GetAllRegisteredMultiplexerSessionsRequest) returns (GetAllRegisteredMultiplexerSessionsResponse);
+  // Gets all multiplexer sessions currently registered with this service.
+  rpc GetAllRegisteredMultiplexerSessions(GetAllRegisteredMultiplexerSessionsRequest) returns (GetAllRegisteredMultiplexerSessionsResponse);
 }
 
 message SessionInformation{
-    // Session identifier used to identify the session in the session management service, as well as in driver services such as grpc-device.
-    // This field is readonly.
-    nidevice_grpc.Session session = 1;
-
-    // Resource name used to open this session in the driver.
-    // This field is readonly.
-    string resource_name = 2;
-
-    // Channel list used for driver initialization and measurement methods.
-    // This field is empty for any SessionInformation returned from ReserveAllRegisteredSessions.
-    // This field is readonly.
-    string channel_list = 3;
-
-    // Instrument type ID to identify which type of instrument the session represents.
-    // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
-    //      "niDCPower"
-    //      "niDigitalPattern"
-    //      "niScope"
-    //      "niDMM"
-    //      "niDAQmx"
-    //      "niFGen"
-    //      "niRelayDriver"
-    // For custom instruments the user defined instrument type id is defined in the pin map file.
-    // This field is readonly.
-    string instrument_type_id = 4;
-
-    // Indicates whether the session exists in the Session Manager. This indicates whether the session has been created.
-    // This field is readonly.
-    bool session_exists = 5;
-
-    // List of site and pin/relay mappings with optional multiplexer information for each channel in the channel_list.
-    // Each item represents a channel-to-pin connection for this instrument resource. In the case of shared pins, there is a separate item for each connection.
-    // This field is empty for any SessionInformation returned from ReserveAllRegisteredSessions.
-    // This field is readonly.
-    repeated ChannelMapping channel_mappings = 6;
+  // Session identifier used to identify the session in the session management service, as well as in driver services such as grpc-device.
+  // This field is readonly.
+  nidevice_grpc.Session session = 1;
+
+  // Resource name used to open this session in the driver.
+  // This field is readonly.
+  string resource_name = 2;
+
+  // Channel list used for driver initialization and measurement methods.
+  // This field is empty for any SessionInformation returned from ReserveAllRegisteredSessions.
+  // This field is readonly.
+  string channel_list = 3;
+
+  // Instrument type ID to identify which type of instrument the session represents.
+  // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
+  //      "niDCPower"
+  //      "niDigitalPattern"
+  //      "niScope"
+  //      "niDMM"
+  //      "niDAQmx"
+  //      "niFGen"
+  //      "niRelayDriver"
+  // For custom instruments the user defined instrument type id is defined in the pin map file.
+  // This field is readonly.
+  string instrument_type_id = 4;
+
+  // Indicates whether the session exists in the Session Manager. This indicates whether the session has been created.
+  // This field is readonly.
+  bool session_exists = 5;
+
+  // List of site and pin/relay mappings with optional multiplexer information for each channel in the channel_list.
+  // Each item represents a channel-to-pin connection for this instrument resource. In the case of shared pins, there is a separate item for each connection.
+  // This field is empty for any SessionInformation returned from ReserveAllRegisteredSessions.
+  // This field is readonly.
+  repeated ChannelMapping channel_mappings = 6;
 }
 
 message ChannelMapping {
-    // The pin or relay that is mapped to a channel.
-    string pin_or_relay_name = 1;
+  // The pin or relay that is mapped to a channel.
+  string pin_or_relay_name = 1;
 
-    // The site on which the pin or relay is mapped to a channel.
-    // For system pins/relays the site number is -1 since they do not belong to a specific site.
-    int32 site = 2;
+  // The site on which the pin or relay is mapped to a channel.
+  // For system pins/relays the site number is -1 since they do not belong to a specific site.
+  int32 site = 2;
 
-    // The channel to which the pin or relay is mapped on this site.
-    string channel = 3;
+  // The channel to which the pin or relay is mapped on this site.
+  string channel = 3;
 
-    // The multiplexer resource name is used to open the multiplexer session in the driver.
-    string multiplexer_resource_name = 4;
+  // The multiplexer resource name is used to open the multiplexer session in the driver.
+  string multiplexer_resource_name = 4;
 
-    // The multiplexer route through which the pin is connected to an instrument's channel.
-    string multiplexer_route = 5;
+  // The multiplexer route through which the pin is connected to an instrument's channel.
+  string multiplexer_route = 5;
 }
 
 message MultiplexerSessionInformation {
-    // Session identifier used to identify the session in the session management service, as well as in driver services such as grpc-device.
-    // This field is readonly.
-    nidevice_grpc.Session session = 1;
-
-    // Resource name is used to open this session in the driver.
-    // This field is readonly.
-    string resource_name = 2;
-
-    // User-defined identifier for the multiplexer type in the pin map editor.
-    // This field is readonly.
-    string multiplexer_type_id = 3;
-
-    // Indicates whether the session exists in the Session Manager. This indicates whether the session has been created.
-    // This field is readonly.
-    bool session_exists = 4;
+  // Session identifier used to identify the session in the session management service, as well as in driver services such as grpc-device.
+  // This field is readonly.
+  nidevice_grpc.Session session = 1;
+
+  // Resource name is used to open this session in the driver.
+  // This field is readonly.
+  string resource_name = 2;
+
+  // User-defined identifier for the multiplexer type in the pin map editor.
+  // This field is readonly.
+  string multiplexer_type_id = 3;
+
+  // Indicates whether the session exists in the Session Manager. This indicates whether the session has been created.
+  // This field is readonly.
+  bool session_exists = 4;
 }
 
 message ReserveSessionsRequest {
-    // Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement.
-    PinMapContext pin_map_context = 1;
+  // Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement.
+  PinMapContext pin_map_context = 1;
 
-    // Optional. List of pins, pin groups, relays, or relay groups to use for the measurement. If unspecified, reserve sessions for all pins and relays in the registered pin map resource.
-    repeated string pin_or_relay_names = 2;
+  // Optional. List of pins, pin groups, relays, or relay groups to use for the measurement. If unspecified, reserve sessions for all pins and relays in the registered pin map resource.
+  repeated string pin_or_relay_names = 2;
 
-    // Optional. Instrument type ID for the measurement. If unspecified, reserve sessions for all instrument types connected in the registered pin map resource.
-    // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
-    //      "niDCPower"
-    //      "niDigitalPattern"
-    //      "niScope"
-    //      "niDMM"
-    //      "niDAQmx"
-    //      "niFGen"
-    //      "niRelayDriver"
-    // For custom instruments the user defined instrument type id is defined in the pin map file.
-    string instrument_type_id = 3;
-
-    // Optional. Timeout for the reservation request.
-    // Allowed values: 0 (non-blocking, fails immediately if resources cannot be reserved), -1 (infinite timeout), or any other positive numeric value (wait for that number of milliseconds)
-    int32 timeout_in_milliseconds = 4;
+  // Optional. Instrument type ID for the measurement. If unspecified, reserve sessions for all instrument types connected in the registered pin map resource.
+  // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
+  //      "niDCPower"
+  //      "niDigitalPattern"
+  //      "niScope"
+  //      "niDMM"
+  //      "niDAQmx"
+  //      "niFGen"
+  //      "niRelayDriver"
+  // For custom instruments the user defined instrument type id is defined in the pin map file.
+  string instrument_type_id = 3;
+
+  // Optional. Timeout for the reservation request.
+  // Allowed values: 0 (non-blocking, fails immediately if resources cannot be reserved), -1 (infinite timeout), or any other positive numeric value (wait for that number of milliseconds)
+  int32 timeout_in_milliseconds = 4;
 }
 
 message ReserveSessionsResponse{
-    // List of information needed to create or use each session for the given pin, site, and instrument type ID.
-    repeated SessionInformation sessions = 1;
+  // List of information needed to create or use each session for the given pin, site, and instrument type ID.
+  repeated SessionInformation sessions = 1;
 
-    // List of information needed to create or use each multiplexer session for the given pin, site, and instrument type ID.
-    repeated MultiplexerSessionInformation multiplexer_sessions = 2;
-    
-    // Represents the mapping between pin or relay groups and their respective pin or relay names.
-    map<string, ResolvedPinsOrRelays> group_mappings = 3;
+  // List of information needed to create or use each multiplexer session for the given pin, site, and instrument type ID.
+  repeated MultiplexerSessionInformation multiplexer_sessions = 2;
+
+  // Represents the mapping between pin or relay groups and their respective pin or relay names.
+  map<string, ResolvedPinsOrRelays> group_mappings = 3;
 }
 
 message UnreserveSessionsRequest {
-    // Required. List of information of sessions to be unreserved in the session management service.
-    repeated SessionInformation sessions = 1;
+  // Required. List of information of sessions to be unreserved in the session management service.
+  repeated SessionInformation sessions = 1;
 }
 
 message UnreserveSessionsResponse {
 }
 
 message RegisterSessionsRequest{
-    // Required. List of sessions to register with the session management service to track as the sessions are open.
-    repeated SessionInformation sessions = 1;
+  // Required. List of sessions to register with the session management service to track as the sessions are open.
+  repeated SessionInformation sessions = 1;
 }
 
 message RegisterSessionsResponse{
 }
 
 message UnregisterSessionsRequest{
-    // Required. List of sessions to unregister with the session management service to mark them as sessions were closed.
-    repeated SessionInformation sessions = 1;
+  // Required. List of sessions to unregister with the session management service to mark them as sessions were closed.
+  repeated SessionInformation sessions = 1;
 }
 
 message UnregisterSessionsResponse{
 }
 
 message ReserveAllRegisteredSessionsRequest {
-    // Optional. Timeout for the reservation request.
-    // Allowed values: 0 (non-blocking, fails immediately if resources cannot be reserved), -1 (infinite timeout), or any other positive numeric value (wait for that number of milliseconds)
-    int32 timeout_in_milliseconds = 1;
-
-    // Optional. Instrument type ID of the registered sessions to reserve. If unspecified, reserve sessions for all instrument types connected in the registered pin map resource.
-    // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
-    //      "niDCPower"
-    //      "niDigitalPattern"
-    //      "niScope"
-    //      "niDMM"
-    //      "niDAQmx"
-    //      "niFGen"
-    //      "niRelayDriver"
-    // For custom instruments the user defined instrument type id is defined in the pin map file.
-    string instrument_type_id = 2;
+  // Optional. Timeout for the reservation request.
+  // Allowed values: 0 (non-blocking, fails immediately if resources cannot be reserved), -1 (infinite timeout), or any other positive numeric value (wait for that number of milliseconds)
+  int32 timeout_in_milliseconds = 1;
+
+  // Optional. Instrument type ID of the registered sessions to reserve. If unspecified, reserve sessions for all instrument types connected in the registered pin map resource.
+  // Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
+  //      "niDCPower"
+  //      "niDigitalPattern"
+  //      "niScope"
+  //      "niDMM"
+  //      "niDAQmx"
+  //      "niFGen"
+  //      "niRelayDriver"
+  // For custom instruments the user defined instrument type id is defined in the pin map file.
+  string instrument_type_id = 2;
 }
 
 message ReserveAllRegisteredSessionsResponse{
-    // Sessions currently registered in the session management service.
-    repeated SessionInformation sessions = 1;
+  // Sessions currently registered in the session management service.
+  repeated SessionInformation sessions = 1;
 }
 
 message RegisterMultiplexerSessionsRequest {
-    // Required. List of multiplexer sessions to register with the session management service to track as the sessions are open.
-    repeated MultiplexerSessionInformation multiplexer_sessions = 1;
+  // Required. List of multiplexer sessions to register with the session management service to track as the sessions are open.
+  repeated MultiplexerSessionInformation multiplexer_sessions = 1;
 }
 
 message RegisterMultiplexerSessionsResponse{
 }
 
 message UnregisterMultiplexerSessionsRequest {
-    // Required. List of multiplexer sessions to unregister with the session management service to mark them as sessions were closed.
-    repeated MultiplexerSessionInformation multiplexer_sessions = 1;
+  // Required. List of multiplexer sessions to unregister with the session management service to mark them as sessions were closed.
+  repeated MultiplexerSessionInformation multiplexer_sessions = 1;
 }
 
 message UnregisterMultiplexerSessionsResponse{
 }
 
 message GetMultiplexerSessionsRequest {
-    // Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement.
-    PinMapContext pin_map_context = 1;
+  // Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement.
+  PinMapContext pin_map_context = 1;
 
-    // Optional. User-defined identifier for the multiplexer type in the pin map editor.
-    // If unspecified, information for all multiplexer types is returned.
-    string multiplexer_type_id = 2;
+  // Optional. User-defined identifier for the multiplexer type in the pin map editor.
+  // If unspecified, information for all multiplexer types is returned.
+  string multiplexer_type_id = 2;
 }
 
 message GetMultiplexerSessionsResponse{
-    // List of information needed to create or use each multiplexer session for the given pin map context and multiplexer type ID.
-    repeated MultiplexerSessionInformation multiplexer_sessions = 1;
+  // List of information needed to create or use each multiplexer session for the given pin map context and multiplexer type ID.
+  repeated MultiplexerSessionInformation multiplexer_sessions = 1;
 }
 
 message GetAllRegisteredMultiplexerSessionsRequest{
-    // Optional. User-defined identifier for the multiplexer type in the pin map editor.
-    // If unspecified, information for all registered multiplexer types is returned.
-    string multiplexer_type_id = 1;
+  // Optional. User-defined identifier for the multiplexer type in the pin map editor.
+  // If unspecified, information for all registered multiplexer types is returned.
+  string multiplexer_type_id = 1;
 }
 
 message GetAllRegisteredMultiplexerSessionsResponse{
-    // Multiplexer sessions currently registered in the session management service.
-    repeated MultiplexerSessionInformation multiplexer_sessions = 1;
+  // Multiplexer sessions currently registered in the session management service.
+  repeated MultiplexerSessionInformation multiplexer_sessions = 1;
 }
 
 message ResolvedPinsOrRelays {
   // List of pin or relay names in the pin or relay group.
   repeated string pin_or_relay_names = 1;
 }
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/ni/protobuf/types/xydata.proto` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/protobuf/types/xydata.proto`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 
 // XYData for a cartesian graph.
 // x_data and y_data should contain the same number of values.
 // If they do not, the smaller-sized array will be used to determine
 // the number of XY points.
 message DoubleXYData
 {
-    repeated double x_data = 1;
-    repeated double y_data = 2;
+  repeated double x_data = 1;
+  repeated double y_data = 2;
 }
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/proto/session.proto` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/proto/session.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import sys
@@ -31,35 +32,35 @@
 class SessionInitializationBehavior(_SessionInitializationBehavior, metaclass=_SessionInitializationBehaviorEnumTypeWrapper): ...
 
 SESSION_INITIALIZATION_BEHAVIOR_UNSPECIFIED: SessionInitializationBehavior.ValueType  # 0
 SESSION_INITIALIZATION_BEHAVIOR_INITIALIZE_NEW: SessionInitializationBehavior.ValueType  # 1
 SESSION_INITIALIZATION_BEHAVIOR_ATTACH_TO_EXISTING: SessionInitializationBehavior.ValueType  # 2
 global___SessionInitializationBehavior = SessionInitializationBehavior
 
-@typing_extensions.final
+@typing.final
 class Session(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
     name: builtins.str
     id: builtins.int
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         id: builtins.int = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["id", b"id", "name", b"name", "session", b"session"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "name", b"name", "session", b"session"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["session", b"session"]) -> typing_extensions.Literal["name", "id"] | None: ...
+    def HasField(self, field_name: typing.Literal["id", b"id", "name", b"name", "session", b"session"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["id", b"id", "name", b"name", "session", b"session"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["session", b"session"]) -> typing.Literal["name", "id"] | None: ...
 
 global___Session = Session
 
-@typing_extensions.final
+@typing.final
 class DeviceProperties(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     MODEL_FIELD_NUMBER: builtins.int
     VENDOR_FIELD_NUMBER: builtins.int
     SERIAL_NUMBER_FIELD_NUMBER: builtins.int
@@ -74,45 +75,45 @@
         *,
         name: builtins.str = ...,
         model: builtins.str = ...,
         vendor: builtins.str = ...,
         serial_number: builtins.str = ...,
         product_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["model", b"model", "name", b"name", "product_id", b"product_id", "serial_number", b"serial_number", "vendor", b"vendor"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["model", b"model", "name", b"name", "product_id", b"product_id", "serial_number", b"serial_number", "vendor", b"vendor"]) -> None: ...
 
 global___DeviceProperties = DeviceProperties
 
-@typing_extensions.final
+@typing.final
 class EnumerateDevicesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___EnumerateDevicesRequest = EnumerateDevicesRequest
 
-@typing_extensions.final
+@typing.final
 class EnumerateDevicesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEVICES_FIELD_NUMBER: builtins.int
     @property
     def devices(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeviceProperties]: ...
     def __init__(
         self,
         *,
         devices: collections.abc.Iterable[global___DeviceProperties] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["devices", b"devices"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["devices", b"devices"]) -> None: ...
 
 global___EnumerateDevicesResponse = EnumerateDevicesResponse
 
-@typing_extensions.final
+@typing.final
 class ReserveRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESERVATION_ID_FIELD_NUMBER: builtins.int
     CLIENT_ID_FIELD_NUMBER: builtins.int
     reservation_id: builtins.str
     """client defined string representing a set of reservable resources"""
@@ -120,34 +121,34 @@
     """client defined identifier for a specific client"""
     def __init__(
         self,
         *,
         reservation_id: builtins.str = ...,
         client_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_id", b"client_id", "reservation_id", b"reservation_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["client_id", b"client_id", "reservation_id", b"reservation_id"]) -> None: ...
 
 global___ReserveRequest = ReserveRequest
 
-@typing_extensions.final
+@typing.final
 class ReserveResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IS_RESERVED_FIELD_NUMBER: builtins.int
     is_reserved: builtins.bool
     def __init__(
         self,
         *,
         is_reserved: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_reserved", b"is_reserved"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["is_reserved", b"is_reserved"]) -> None: ...
 
 global___ReserveResponse = ReserveResponse
 
-@typing_extensions.final
+@typing.final
 class IsReservedByClientRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESERVATION_ID_FIELD_NUMBER: builtins.int
     CLIENT_ID_FIELD_NUMBER: builtins.int
     reservation_id: builtins.str
     """client defined string representing a set of reservable resources"""
@@ -155,34 +156,34 @@
     """client defined identifier for a specific client"""
     def __init__(
         self,
         *,
         reservation_id: builtins.str = ...,
         client_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_id", b"client_id", "reservation_id", b"reservation_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["client_id", b"client_id", "reservation_id", b"reservation_id"]) -> None: ...
 
 global___IsReservedByClientRequest = IsReservedByClientRequest
 
-@typing_extensions.final
+@typing.final
 class IsReservedByClientResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IS_RESERVED_FIELD_NUMBER: builtins.int
     is_reserved: builtins.bool
     def __init__(
         self,
         *,
         is_reserved: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_reserved", b"is_reserved"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["is_reserved", b"is_reserved"]) -> None: ...
 
 global___IsReservedByClientResponse = IsReservedByClientResponse
 
-@typing_extensions.final
+@typing.final
 class UnreserveRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESERVATION_ID_FIELD_NUMBER: builtins.int
     CLIENT_ID_FIELD_NUMBER: builtins.int
     reservation_id: builtins.str
     """client defined string representing a set of reservable resources"""
@@ -190,50 +191,50 @@
     """client defined identifier for a specific client"""
     def __init__(
         self,
         *,
         reservation_id: builtins.str = ...,
         client_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_id", b"client_id", "reservation_id", b"reservation_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["client_id", b"client_id", "reservation_id", b"reservation_id"]) -> None: ...
 
 global___UnreserveRequest = UnreserveRequest
 
-@typing_extensions.final
+@typing.final
 class UnreserveResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IS_UNRESERVED_FIELD_NUMBER: builtins.int
     is_unreserved: builtins.bool
     def __init__(
         self,
         *,
         is_unreserved: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_unreserved", b"is_unreserved"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["is_unreserved", b"is_unreserved"]) -> None: ...
 
 global___UnreserveResponse = UnreserveResponse
 
-@typing_extensions.final
+@typing.final
 class ResetServerRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ResetServerRequest = ResetServerRequest
 
-@typing_extensions.final
+@typing.final
 class ResetServerResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IS_SERVER_RESET_FIELD_NUMBER: builtins.int
     is_server_reset: builtins.bool
     def __init__(
         self,
         *,
         is_server_reset: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_server_reset", b"is_server_reset"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["is_server_reset", b"is_server_reset"]) -> None: ...
 
 global___ResetServerResponse = ResetServerResponse
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.pyi` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,116 +1,128 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import abc
 import collections.abc
 import grpc
 import grpc.aio
 from ni_measurementlink_service._internal.stubs import session_pb2
 import typing
 
-_T = typing.TypeVar('_T')
+_T = typing.TypeVar("_T")
 
-class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
-    ...
+class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta): ...
 
-class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore[misc, type-arg]
     ...
 
 class SessionUtilitiesStub:
     def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None: ...
     EnumerateDevices: grpc.UnaryUnaryMultiCallable[
         session_pb2.EnumerateDevicesRequest,
         session_pb2.EnumerateDevicesResponse,
     ]
     """Provides a list of devices or chassis connected to server under localhost"""
+
     Reserve: grpc.UnaryUnaryMultiCallable[
         session_pb2.ReserveRequest,
         session_pb2.ReserveResponse,
     ]
     """Reserve a set of client defined resources for exclusive use"""
+
     IsReservedByClient: grpc.UnaryUnaryMultiCallable[
         session_pb2.IsReservedByClientRequest,
         session_pb2.IsReservedByClientResponse,
     ]
     """Determines if a set of client defined resources is currently reserved by a
     specific client
     """
+
     Unreserve: grpc.UnaryUnaryMultiCallable[
         session_pb2.UnreserveRequest,
         session_pb2.UnreserveResponse,
     ]
     """Unreserves a previously reserved resource"""
+
     ResetServer: grpc.UnaryUnaryMultiCallable[
         session_pb2.ResetServerRequest,
         session_pb2.ResetServerResponse,
     ]
     """Resets the server to a default state with no open sessions"""
 
 class SessionUtilitiesAsyncStub:
     EnumerateDevices: grpc.aio.UnaryUnaryMultiCallable[
         session_pb2.EnumerateDevicesRequest,
         session_pb2.EnumerateDevicesResponse,
     ]
     """Provides a list of devices or chassis connected to server under localhost"""
+
     Reserve: grpc.aio.UnaryUnaryMultiCallable[
         session_pb2.ReserveRequest,
         session_pb2.ReserveResponse,
     ]
     """Reserve a set of client defined resources for exclusive use"""
+
     IsReservedByClient: grpc.aio.UnaryUnaryMultiCallable[
         session_pb2.IsReservedByClientRequest,
         session_pb2.IsReservedByClientResponse,
     ]
     """Determines if a set of client defined resources is currently reserved by a
     specific client
     """
+
     Unreserve: grpc.aio.UnaryUnaryMultiCallable[
         session_pb2.UnreserveRequest,
         session_pb2.UnreserveResponse,
     ]
     """Unreserves a previously reserved resource"""
+
     ResetServer: grpc.aio.UnaryUnaryMultiCallable[
         session_pb2.ResetServerRequest,
         session_pb2.ResetServerResponse,
     ]
     """Resets the server to a default state with no open sessions"""
 
 class SessionUtilitiesServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def EnumerateDevices(
         self,
         request: session_pb2.EnumerateDevicesRequest,
         context: _ServicerContext,
     ) -> typing.Union[session_pb2.EnumerateDevicesResponse, collections.abc.Awaitable[session_pb2.EnumerateDevicesResponse]]:
         """Provides a list of devices or chassis connected to server under localhost"""
+
     @abc.abstractmethod
     def Reserve(
         self,
         request: session_pb2.ReserveRequest,
         context: _ServicerContext,
     ) -> typing.Union[session_pb2.ReserveResponse, collections.abc.Awaitable[session_pb2.ReserveResponse]]:
         """Reserve a set of client defined resources for exclusive use"""
+
     @abc.abstractmethod
     def IsReservedByClient(
         self,
         request: session_pb2.IsReservedByClientRequest,
         context: _ServicerContext,
     ) -> typing.Union[session_pb2.IsReservedByClientResponse, collections.abc.Awaitable[session_pb2.IsReservedByClientResponse]]:
         """Determines if a set of client defined resources is currently reserved by a
         specific client
         """
+
     @abc.abstractmethod
     def Unreserve(
         self,
         request: session_pb2.UnreserveRequest,
         context: _ServicerContext,
     ) -> typing.Union[session_pb2.UnreserveResponse, collections.abc.Awaitable[session_pb2.UnreserveResponse]]:
         """Unreserves a previously reserved resource"""
+
     @abc.abstractmethod
     def ResetServer(
         self,
         request: session_pb2.ResetServerRequest,
         context: _ServicerContext,
     ) -> typing.Union[session_pb2.ResetServerResponse, collections.abc.Awaitable[session_pb2.ResetServerResponse]]:
         """Resets the server to a default state with no open sessions"""
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/_tracelogging.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/_tracelogging.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/discovery/_client.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/discovery/_client.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/discovery/_support.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/discovery/_support.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/discovery/_types.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/discovery/_types.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/grpc/channelpool.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/grpc/channelpool.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/grpc/loggers.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/grpc/loggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,23 +145,21 @@
 
     def intercept_service(
         self,
         continuation: Callable[
             [grpc.HandlerCallDetails], grpc.RpcMethodHandler[grpc.TRequest, grpc.TResponse] | None
         ],
         handler_call_details: grpc.HandlerCallDetails,
-    ) -> grpc.RpcMethodHandler[grpc.TRequest, grpc.TResponse]:
+    ) -> Optional[grpc.RpcMethodHandler[grpc.TRequest, grpc.TResponse]]:
         """Intercept and log a server call."""
         if _ServerCallLogger.is_enabled():
             call_logger = _ServerCallLogger(handler_call_details.method)
             handler = continuation(handler_call_details)
             if handler is None:
-                # ServerInterceptor.intercept_service return type doesn't match continuation return
-                # type -- https://github.com/shabbyrobe/grpc-stubs/issues/48
-                return handler  # type: ignore[return-value]
+                return handler
             elif handler.unary_unary:
                 return grpc.unary_unary_rpc_method_handler(
                     functools.partial(self._log_unary_unary, call_logger, handler.unary_unary),
                     handler.request_deserializer,
                     handler.response_serializer,
                 )
             elif handler.unary_stream:
@@ -181,15 +179,15 @@
                     functools.partial(self._log_stream_stream, call_logger, handler.stream_stream),
                     handler.request_deserializer,
                     handler.response_serializer,
                 )
             else:
                 raise RuntimeError("Invalid RpcMethodHandler")
         else:
-            return continuation(handler_call_details)  # type: ignore[return-value]
+            return continuation(handler_call_details)
 
     def _log_unary_unary(
         self,
         call_logger: _CallLogger,
         handler_function: Callable[[grpc.TRequest, grpc.ServicerContext], grpc.TResponse],
         request: grpc.TRequest,
         context: grpc.ServicerContext,
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/measurement/info.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/measurement/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 class TypeSpecialization(enum.Enum):
     """Enum that represents the type specializations for measurement parameters."""
 
     NoType = ""
     Pin = "pin"
     Path = "path"
     Enum = "enum"
+    IOResource = "ioresource"
 
 
 class DataType(enum.Enum):
     """Enum that represents the supported data types."""
 
     Int32 = 0
     Int64 = 1
@@ -83,20 +84,22 @@
     Double = 5
     Boolean = 6
     String = 7
     Pin = 8
     Path = 9
     Enum = 10
     DoubleXYData = 11
+    IOResource = 12
 
     Int32Array1D = 100
     Int64Array1D = 101
     UInt32Array1D = 102
     UInt64Array1D = 103
     FloatArray1D = 104
     DoubleArray1D = 105
     BooleanArray1D = 106
     StringArray1D = 107
     PinArray1D = 108
     PathArray1D = 109
     EnumArray1D = 110
     DoubleXYDataArray1D = 111
+    IOResourceArray1D = 112
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/measurement/service.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/measurement/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Framework to host measurement service."""
 
 from __future__ import annotations
 
 import json
 import sys
 import threading
+import warnings
 from enum import Enum, EnumMeta
 from os import path
 from pathlib import Path
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -379,15 +380,15 @@
 
             type (DataType): Data type of the configuration.
 
             default_value (Any): Default value of the configuration.
 
             instrument_type (Optional[str]):
                 Filter pins by instrument type. This is only supported when configuration type
-                is DataType.Pin.
+                is DataType.IOResource or DataType.Pin (deprecated).
 
                 For NI instruments, use instrument type id constants defined by
                 :py:mod:`ni_measurementlink_service.session_management`, such as
                 :py:const:`~ni_measurementlink_service.session_management.INSTRUMENT_TYPE_NI_DCPOWER`
                 or
                 :py:const:`~ni_measurementlink_service.session_management.INSTRUMENT_TYPE_NI_DMM`.
 
@@ -397,14 +398,23 @@
                 Defines the enum type associated with this configuration parameter. This is only
                 supported when configuration type is DataType.Enum or DataType.EnumArray1D.
 
         Returns:
             Callable: Callable that takes in Any Python Function
             and returns the same python function.
         """
+        if type == DataType.Pin:
+            warnings.warn(
+                "DataType.Pin is deprecated. Use DataType.IOResource instead.", DeprecationWarning
+            )
+        if type == DataType.PinArray1D:
+            warnings.warn(
+                "DataType.PinArray1D is deprecated. Use DataType.IOResourceArray1D instead.",
+                DeprecationWarning,
+            )
         data_type_info = _datatypeinfo.get_type_info(type)
         annotations = self._make_annotations_dict(
             data_type_info.type_specialization, instrument_type=instrument_type, enum_type=enum_type
         )
         parameter = parameter_metadata.ParameterMetadata(
             display_name,
             data_type_info.grpc_field_type,
@@ -448,14 +458,23 @@
                 Defines the enum type associated with this configuration parameter. This is only
                 supported when configuration type is DataType.Enum or DataType.EnumArray1D.
 
         Returns:
             Callable: Callable that takes in Any Python Function and
             returns the same python function.
         """
+        if type == DataType.Pin:
+            warnings.warn(
+                "DataType.Pin is deprecated. Use DataType.IOResource instead.", DeprecationWarning
+            )
+        if type == DataType.PinArray1D:
+            warnings.warn(
+                "DataType.PinArray1D is deprecated. Use DataType.IOResourceArray1D instead.",
+                DeprecationWarning,
+            )
         data_type_info = _datatypeinfo.get_type_info(type)
         annotations = self._make_annotations_dict(
             data_type_info.type_specialization, enum_type=enum_type
         )
         parameter = parameter_metadata.ParameterMetadata(
             display_name,
             data_type_info.grpc_field_type,
@@ -509,14 +528,17 @@
         if type_specialization == TypeSpecialization.NoType:
             return annotations
 
         annotations[TYPE_SPECIALIZATION_KEY] = type_specialization.value
         if type_specialization == TypeSpecialization.Pin:
             if instrument_type != "" or instrument_type is not None:
                 annotations["ni/pin.instrument_type"] = instrument_type
+        if type_specialization == TypeSpecialization.IOResource:
+            if instrument_type != "" or instrument_type is not None:
+                annotations["ni/ioresource.instrument_type"] = instrument_type
         if type_specialization == TypeSpecialization.Enum:
             if enum_type is not None:
                 annotations[ENUM_VALUES_KEY] = self._enum_to_annotations_value(enum_type)
             else:
                 raise ValueError("enum_type is required for enum parameters.")
 
         return annotations
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/__init__.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/__init__.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/_client.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 import threading
 import warnings
 from typing import Dict, Iterable, Mapping, Optional, Union
 
 import google.protobuf.internal.containers
 import grpc
 
-from ni_measurementlink_service._featuretoggles import (
-    MULTIPLEXER_SUPPORT_2024Q2,
-    requires_feature,
-)
 from ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement.v1 import (
     session_management_service_pb2,
     session_management_service_pb2_grpc,
 )
 from ni_measurementlink_service.discovery import DiscoveryClient
 from ni_measurementlink_service.grpc.channelpool import GrpcChannelPool
 from ni_measurementlink_service.session_management._constants import (
@@ -255,15 +251,15 @@
         """
         request = session_management_service_pb2.UnregisterSessionsRequest(
             sessions=(info._to_grpc_v1() for info in session_info),
         )
         self._get_stub().UnregisterSessions(request)
 
     def reserve_all_registered_sessions(
-        self, instrument_type_id: Optional[str] = None, timeout: Optional[float] = 0.0
+        self, instrument_type_id: Optional[str] = None, timeout: Optional[float] = 10.0
     ) -> MultiSessionReservation:
         """Reserve all sessions currently registered with the session management service.
 
         Args:
             instrument_type_id: Instrument type ID for the measurement.
 
                 If unspecified, reserve sessions for all instrument types connected in the
@@ -272,14 +268,16 @@
                 For NI instruments, use instrument type id constants, such as
                 :py:const:`INSTRUMENT_TYPE_NI_DCPOWER` or :py:const:`INSTRUMENT_TYPE_NI_DMM`.
 
                 For custom instruments, use the instrument type id defined in the pin map file.
 
             timeout: Timeout in seconds.
 
+                An arbitrary timeout to wait for the measurement to complete or be canceled.
+
                 Allowed values: 0 (non-blocking, fails immediately if resources cannot be
                 reserved), -1 (infinite timeout), or any other positive numeric value (wait for
                 that number of seconds)
 
         Returns:
             A reservation object with which you can query information about the sessions and
             unreserve them.
@@ -291,15 +289,14 @@
             request.instrument_type_id = instrument_type_id
 
         response = self._get_stub().ReserveAllRegisteredSessions(request)
         return MultiSessionReservation(
             session_management_client=self, session_info=response.sessions
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def register_multiplexer_sessions(
         self, multiplexer_session_info: Iterable[MultiplexerSessionInformation]
     ) -> None:
         """Register multiplexer sessions with the session management service.
 
         Indicates that the sessions are open and will need to be closed later.
 
@@ -307,15 +304,14 @@
             multiplexer_session_info: Sessions to register.
         """
         request = session_management_service_pb2.RegisterMultiplexerSessionsRequest(
             multiplexer_sessions=(info._to_grpc_v1() for info in multiplexer_session_info),
         )
         self._get_stub().RegisterMultiplexerSessions(request)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def unregister_multiplexer_sessions(
         self, multiplexer_session_info: Iterable[MultiplexerSessionInformation]
     ) -> None:
         """Unregisters multiplexer sessions from the session management service.
 
         Indicates that the sessions have been closed and will need to be reopened before they can be
         used again.
@@ -324,15 +320,14 @@
             multiplexer_session_info: Sessions to unregister.
         """
         request = session_management_service_pb2.UnregisterMultiplexerSessionsRequest(
             multiplexer_sessions=(info._to_grpc_v1() for info in multiplexer_session_info),
         )
         self._get_stub().UnregisterMultiplexerSessions(request)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_multiplexer_sessions(
         self, pin_map_context: PinMapContext, multiplexer_type_id: Optional[str] = None
     ) -> MultiplexerSessionContainer:
         """Get all multiplexer session infos matching the specified criteria.
 
         Returns the information needed to create or access the multiplexer sessions
         without reserving the connected instruments.
@@ -354,15 +349,14 @@
         if multiplexer_type_id is not None:
             request.multiplexer_type_id = multiplexer_type_id
 
         response = self._get_stub().GetMultiplexerSessions(request)
         session_infos = [session for session in response.multiplexer_sessions]
         return MultiplexerSessionContainer(self, session_infos)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_all_registered_multiplexer_sessions(
         self, multiplexer_type_id: Optional[str] = None
     ) -> MultiplexerSessionContainer:
         """Get all multiplexer session infos registered with the session management service.
 
         Args:
             multiplexer_type_id: User-defined identifier for the multiplexer
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/_constants.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/_constants.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/_reservation.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/_reservation.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,14 @@
     cast,
 )
 
 from ni_measurementlink_service._drivers import (
     closing_session,
     closing_session_with_ts_code_module_support,
 )
-from ni_measurementlink_service._featuretoggles import (
-    MULTIPLEXER_SUPPORT_2024Q2,
-    requires_feature,
-)
 from ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement.v1 import (
     session_management_service_pb2,
 )
 from ni_measurementlink_service.discovery import DiscoveryClient
 from ni_measurementlink_service.grpc.channelpool import GrpcChannelPool
 from ni_measurementlink_service.session_management._constants import (
     INSTRUMENT_TYPE_NI_DAQMX,
@@ -225,15 +221,14 @@
     @cached_property
     def _multiplexer_type_ids(self) -> AbstractSet[str]:
         return _to_ordered_set(
             sorted(info.multiplexer_type_id for info in self._multiplexer_session_info)
         )
 
     @property
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def multiplexer_session_info(self) -> Sequence[MultiplexerSessionInformation]:
         """Multiplexer session information object."""
         if not self._multiplexer_session_cache:
             return self._multiplexer_session_info
 
         return [
             info._with_session(self._multiplexer_session_cache.get(info.session_name))
@@ -366,15 +361,14 @@
                 )
                 new_session_info = multiplexer_session_info._with_session(session)
                 typed_multiplexer_session_infos.append(
                     cast(TypedMultiplexerSessionInformation[TMultiplexerSession], new_session_info)
                 )
             yield typed_multiplexer_session_infos
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def initialize_multiplexer_session(
         self,
         session_constructor: Callable[[MultiplexerSessionInformation], TMultiplexerSession],
         multiplexer_type_id: Optional[str] = None,
     ) -> ContextManager[TypedMultiplexerSessionInformation[TMultiplexerSession]]:
         """Initialize a single multiplexer session.
 
@@ -396,15 +390,14 @@
             TypeError: If the argument types are incorrect.
 
             ValueError: If no multiplexer sessions are available or
                 too many multiplexer sessions are available.
         """
         return self._initialize_multiplexer_session_core(session_constructor, multiplexer_type_id)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def initialize_multiplexer_sessions(
         self,
         session_constructor: Callable[[MultiplexerSessionInformation], TMultiplexerSession],
         multiplexer_type_id: Optional[str] = None,
     ) -> ContextManager[Sequence[TypedMultiplexerSessionInformation[TMultiplexerSession]]]:
         """Initialize multiple multiplexer sessions.
 
@@ -425,15 +418,14 @@
         Raises:
             TypeError: If the argument types are incorrect.
 
             ValueError: If no multiplexer sessions are available.
         """
         return self._initialize_multiplexer_sessions_core(session_constructor, multiplexer_type_id)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def initialize_niswitch_multiplexer_session(
         self,
         topology: Optional[str] = None,
         simulate: Optional[bool] = None,
         reset_device: bool = False,
         initialization_behavior: SessionInitializationBehavior = SessionInitializationBehavior.AUTO,
         multiplexer_type_id: Optional[str] = None,
@@ -489,15 +481,14 @@
         closing_function = functools.partial(
             closing_session_with_ts_code_module_support, initialization_behavior
         )
         return self._initialize_multiplexer_session_core(
             session_constructor, multiplexer_type_id, closing_function
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def initialize_niswitch_multiplexer_sessions(
         self,
         topology: Optional[str] = None,
         simulate: Optional[bool] = None,
         reset_device: bool = False,
         initialization_behavior: SessionInitializationBehavior = SessionInitializationBehavior.AUTO,
         multiplexer_type_id: Optional[str] = None,
@@ -655,15 +646,14 @@
         return cache
 
     @property
     def _multiplexer_session_cache(self) -> Dict[str, object]:
         return self._multiplexer_session_container._multiplexer_session_cache
 
     @property
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def multiplexer_session_info(self) -> Sequence[MultiplexerSessionInformation]:
         """Multiplexer session information object."""
         return self._multiplexer_session_container.multiplexer_session_info
 
     def __enter__(self: Self) -> Self:
         """Context management protocol. Returns self."""
         return self
@@ -915,15 +905,14 @@
         Raises:
             ValueError: If the instrument type ID is empty, no reserved sessions
                 match the instrument type ID, or too many reserved sessions
                 match the instrument type ID.
         """
         return self._initialize_session_core(session_constructor, instrument_type_id)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def initialize_multiplexer_session(
         self,
         session_constructor: Callable[[MultiplexerSessionInformation], TMultiplexerSession],
         multiplexer_type_id: Optional[str] = None,
     ) -> ContextManager[TypedMultiplexerSessionInformation[TMultiplexerSession]]:
         """Initialize a single multiplexer session.
 
@@ -976,15 +965,14 @@
 
         Raises:
             ValueError: If the instrument type ID is empty or no reserved
                 sessions matched the instrument type ID.
         """
         return self._initialize_sessions_core(session_constructor, instrument_type_id)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def initialize_multiplexer_sessions(
         self,
         session_constructor: Callable[[MultiplexerSessionInformation], TMultiplexerSession],
         multiplexer_type_id: Optional[str] = None,
     ) -> ContextManager[Sequence[TypedMultiplexerSessionInformation[TMultiplexerSession]]]:
         """Initialize multiple multiplexer sessions.
 
@@ -1043,15 +1031,14 @@
             TypeError: If the argument types or session type are incorrect.
 
             ValueError: If no reserved connections match or too many reserved
                 connections match.
         """
         return self._get_connection_core(session_type, pin_or_relay_name, site, instrument_type_id)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_connection_with_multiplexer(
         self,
         session_type: Type[TSession],
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_or_relay_name: Optional[str] = None,
         site: Optional[int] = None,
         instrument_type_id: Optional[str] = None,
@@ -1123,15 +1110,14 @@
 
             ValueError: If no reserved connections match.
         """
         return self._get_connections_core(
             session_type, pin_or_relay_names, sites, instrument_type_id
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_connections_with_multiplexer(
         self,
         session_type: Type[TSession],
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_or_relay_names: Union[str, Iterable[str], None] = None,
         sites: Union[int, Iterable[int], None] = None,
         instrument_type_id: Optional[str] = None,
@@ -1268,15 +1254,14 @@
             ValueError: If no reserved connections match or too many reserved
                 connections match.
         """
         import nidaqmx
 
         return self._get_connection_core(nidaqmx.Task, pin_name, site, INSTRUMENT_TYPE_NI_DAQMX)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nidaqmx_connection_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_name: Optional[str] = None,
         site: Optional[int] = None,
     ) -> TypedConnectionWithMultiplexer[nidaqmx.Task, TMultiplexerSession]:
         """Get the NI-DAQmx connection matching the specified criteria.
@@ -1328,15 +1313,14 @@
 
             ValueError: If no reserved connections match.
         """
         import nidaqmx
 
         return self._get_connections_core(nidaqmx.Task, pin_names, sites, INSTRUMENT_TYPE_NI_DAQMX)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nidaqmx_connections_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_names: Union[str, Iterable[str], None] = None,
         sites: Union[int, Iterable[int], None] = None,
     ) -> Sequence[TypedConnectionWithMultiplexer[nidaqmx.Task, TMultiplexerSession]]:
         """Get all NI-DAQmx connections matching the specified criteria.
@@ -1481,15 +1465,14 @@
         """
         import nidcpower
 
         return self._get_connection_core(
             nidcpower.Session, pin_name, site, INSTRUMENT_TYPE_NI_DCPOWER
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nidcpower_connection_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_name: Optional[str] = None,
         site: Optional[int] = None,
     ) -> TypedConnectionWithMultiplexer[nidcpower.Session, TMultiplexerSession]:
         """Get the NI-DCPower connection matching the specified criteria.
@@ -1545,15 +1528,14 @@
         """
         import nidcpower
 
         return self._get_connections_core(
             nidcpower.Session, pin_names, sites, INSTRUMENT_TYPE_NI_DCPOWER
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nidcpower_connections_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_names: Union[str, Iterable[str], None] = None,
         sites: Union[int, Iterable[int], None] = None,
     ) -> Sequence[TypedConnectionWithMultiplexer[nidcpower.Session, TMultiplexerSession]]:
         """Get all NI-DCPower connections matching the specified criteria.
@@ -1710,15 +1692,14 @@
         """
         import nidigital
 
         return self._get_connection_core(
             nidigital.Session, pin_name, site, INSTRUMENT_TYPE_NI_DIGITAL_PATTERN
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nidigital_connection_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_name: Optional[str] = None,
         site: Optional[int] = None,
     ) -> TypedConnectionWithMultiplexer[nidigital.Session, TMultiplexerSession]:
         """Get the NI-Digital Pattern connection matching the specified criteria.
@@ -1778,15 +1759,14 @@
         """
         import nidigital
 
         return self._get_connections_core(
             nidigital.Session, pin_names, sites, INSTRUMENT_TYPE_NI_DIGITAL_PATTERN
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nidigital_connections_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_names: Union[str, Iterable[str], None] = None,
         sites: Union[int, Iterable[int], None] = None,
     ) -> Sequence[TypedConnectionWithMultiplexer[nidigital.Session, TMultiplexerSession]]:
         """Get all NI-Digital Pattern connections matching the specified criteria.
@@ -1941,15 +1921,14 @@
             ValueError: If no reserved connections match or too many reserved
                 connections match.
         """
         import nidmm
 
         return self._get_connection_core(nidmm.Session, pin_name, site, INSTRUMENT_TYPE_NI_DMM)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nidmm_connection_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_name: Optional[str] = None,
         site: Optional[int] = None,
     ) -> TypedConnectionWithMultiplexer[nidmm.Session, TMultiplexerSession]:
         """Get the NI-DMM connection matching the specified criteria.
@@ -2001,15 +1980,14 @@
 
             ValueError: If no reserved connections match.
         """
         import nidmm
 
         return self._get_connections_core(nidmm.Session, pin_names, sites, INSTRUMENT_TYPE_NI_DMM)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nidmm_connections_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_names: Union[str, Iterable[str], None] = None,
         sites: Union[int, Iterable[int], None] = None,
     ) -> Sequence[TypedConnectionWithMultiplexer[nidmm.Session, TMultiplexerSession]]:
         """Get all NI-DMM connections matching the specified criteria.
@@ -2160,15 +2138,14 @@
             ValueError: If no reserved connections match or too many reserved
                 connections match.
         """
         import nifgen
 
         return self._get_connection_core(nifgen.Session, pin_name, site, INSTRUMENT_TYPE_NI_FGEN)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nifgen_connection_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_name: Optional[str] = None,
         site: Optional[int] = None,
     ) -> TypedConnectionWithMultiplexer[nifgen.Session, TMultiplexerSession]:
         """Get the NI-FGEN connection matching the specified criteria.
@@ -2220,15 +2197,14 @@
 
             ValueError: If no reserved connections match.
         """
         import nifgen
 
         return self._get_connections_core(nifgen.Session, pin_names, sites, INSTRUMENT_TYPE_NI_FGEN)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_nifgen_connections_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_names: Union[str, Iterable[str], None] = None,
         sites: Union[int, Iterable[int], None] = None,
     ) -> Sequence[TypedConnectionWithMultiplexer[nifgen.Session, TMultiplexerSession]]:
         """Get all NI-FGEN connections matching the specified criteria.
@@ -2379,15 +2355,14 @@
             ValueError: If no reserved connections match or too many reserved
                 connections match.
         """
         import niscope
 
         return self._get_connection_core(niscope.Session, pin_name, site, INSTRUMENT_TYPE_NI_SCOPE)
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_niscope_connection_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_name: Optional[str] = None,
         site: Optional[int] = None,
     ) -> TypedConnectionWithMultiplexer[niscope.Session, TMultiplexerSession]:
         """Get the NI-SCOPE connection matching the specified criteria.
@@ -2443,15 +2418,14 @@
         """
         import niscope
 
         return self._get_connections_core(
             niscope.Session, pin_names, sites, INSTRUMENT_TYPE_NI_SCOPE
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def get_niscope_connections_with_multiplexer(
         self,
         multiplexer_session_type: Type[TMultiplexerSession],
         pin_names: Union[str, Iterable[str], None] = None,
         sites: Union[int, Iterable[int], None] = None,
     ) -> Sequence[TypedConnectionWithMultiplexer[niscope.Session, TMultiplexerSession]]:
         """Get all NI-SCOPE connections matching the specified criteria.
@@ -2646,15 +2620,14 @@
         """
         import niswitch
 
         return self._get_connections_core(
             niswitch.Session, relay_names, sites, INSTRUMENT_TYPE_NI_RELAY_DRIVER
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def initialize_niswitch_multiplexer_session(
         self,
         topology: Optional[str] = None,
         simulate: Optional[bool] = None,
         reset_device: bool = False,
         initialization_behavior: SessionInitializationBehavior = SessionInitializationBehavior.AUTO,
         multiplexer_type_id: Optional[str] = None,
@@ -2696,15 +2669,14 @@
         See Also:
             For more details, see :py:class:`niswitch.Session`.
         """
         return self._multiplexer_session_container.initialize_niswitch_multiplexer_session(
             topology, simulate, reset_device, initialization_behavior, multiplexer_type_id
         )
 
-    @requires_feature(MULTIPLEXER_SUPPORT_2024Q2)
     def initialize_niswitch_multiplexer_sessions(
         self,
         topology: Optional[str] = None,
         simulate: Optional[bool] = None,
         reset_device: bool = False,
         initialization_behavior: SessionInitializationBehavior = SessionInitializationBehavior.AUTO,
         multiplexer_type_id: Optional[str] = None,
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/ni_measurementlink_service/session_management/_types.py` & `ni_measurementlink_service-1.5.0.dev0/ni_measurementlink_service/session_management/_types.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.4.0.dev1/pyproject.toml` & `ni_measurementlink_service-1.5.0.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 line-length = 100
 
 [tool.ni-python-styleguide]
 extend_exclude = '.tox/,*_pb2_grpc.py,*_pb2_grpc.pyi,*_pb2.py,*_pb2.pyi,ni_measurementlink_generator/,examples/'
 
 [tool.poetry]
 name = "ni_measurementlink_service"
-version = "1.4.0-dev1"
+version = "1.5.0-dev0"
 description = "MeasurementLink Support for Python"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md" # apply the repo readme to the package as well
 repository = "https://github.com/ni/measurementlink-python/"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -140,11 +140,16 @@
   "nifgen",
   "niscope",
   "niswitch",
 ]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
+# mypy-protobuf codegen has some unused ignores.
+module = ["ni_measurementlink_service._internal.stubs.*","tests.utilities.stubs.*"]
+warn_unused_ignores = false
+
+[[tool.mypy.overrides]]
 # The tests are not yet ready for --disallow-untyped-defs (or even --disallow-incomplete-defs)
 module = ["tests.*"]
 check_untyped_defs = true
 disallow_untyped_defs = false
```

### Comparing `ni_measurementlink_service-1.4.0.dev1/setup.py` & `ni_measurementlink_service-1.5.0.dev0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,409 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ni_measurementlink_service
+Version: 1.5.0.dev0
+Summary: MeasurementLink Support for Python
+Home-page: https://github.com/ni/measurementlink-python/
+License: MIT
+Author: NI
+Author-email: opensource@ni.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Provides-Extra: drivers
+Provides-Extra: nidaqmx
+Provides-Extra: nidcpower
+Provides-Extra: nidigital
+Provides-Extra: nidmm
+Provides-Extra: nifgen
+Provides-Extra: niscope
+Provides-Extra: niswitch
+Requires-Dist: deprecation (>=2.1)
+Requires-Dist: grpcio (>=1.49.1,<2.0.0)
+Requires-Dist: nidaqmx[grpc] (>=0.8.0) ; extra == "drivers" or extra == "nidaqmx"
+Requires-Dist: nidcpower[grpc] (>=1.4.4) ; extra == "drivers" or extra == "nidcpower"
+Requires-Dist: nidigital[grpc] (>=1.4.4) ; extra == "drivers" or extra == "nidigital"
+Requires-Dist: nidmm[grpc] (>=1.4.4) ; extra == "drivers" or extra == "nidmm"
+Requires-Dist: nifgen[grpc] (>=1.4.4) ; extra == "drivers" or extra == "nifgen"
+Requires-Dist: niscope[grpc] (>=1.4.4) ; extra == "drivers" or extra == "niscope"
+Requires-Dist: niswitch[grpc] (>=1.4.4) ; extra == "drivers" or extra == "niswitch"
+Requires-Dist: protobuf (>=4.21,<5.0)
+Requires-Dist: python-decouple (>=3.8)
+Requires-Dist: pywin32 (>=303) ; sys_platform == "win32"
+Requires-Dist: traceloggingdynamic (>=1.0) ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32"
+Project-URL: Repository, https://github.com/ni/measurementlink-python/
+Description-Content-Type: text/markdown
 
-packages = \
-['ni_measurementlink_service',
- 'ni_measurementlink_service._drivers',
- 'ni_measurementlink_service._internal',
- 'ni_measurementlink_service._internal.parameter',
- 'ni_measurementlink_service._internal.stubs',
- 'ni_measurementlink_service._internal.stubs.ni',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink.discovery',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink.discovery.v1',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v1',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v2',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink.pinmap',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink.pinmap.v1',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement',
- 'ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement.v1',
- 'ni_measurementlink_service._internal.stubs.ni.protobuf',
- 'ni_measurementlink_service._internal.stubs.ni.protobuf.types',
- 'ni_measurementlink_service.discovery',
- 'ni_measurementlink_service.grpc',
- 'ni_measurementlink_service.measurement',
- 'ni_measurementlink_service.session_management']
-
-package_data = \
-{'': ['*'],
- 'ni_measurementlink_service._internal.stubs': ['proto/*',
-                                                'proto/ni/measurementlink/*',
-                                                'proto/ni/measurementlink/discovery/v1/*',
-                                                'proto/ni/measurementlink/measurement/v1/*',
-                                                'proto/ni/measurementlink/measurement/v2/*',
-                                                'proto/ni/measurementlink/pinmap/v1/*',
-                                                'proto/ni/measurementlink/sessionmanagement/v1/*',
-                                                'proto/ni/protobuf/types/*']}
-
-install_requires = \
-['deprecation>=2.1',
- 'grpcio>=1.49.1,<2.0.0',
- 'protobuf>=4.21,<5.0',
- 'python-decouple>=3.8']
-
-extras_require = \
-{':python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32"': ['traceloggingdynamic>=1.0'],
- ':sys_platform == "win32"': ['pywin32>=303'],
- 'drivers': ['nidaqmx[grpc]>=0.8.0',
-             'nidcpower[grpc]>=1.4.4',
-             'nidigital[grpc]>=1.4.4',
-             'nidmm[grpc]>=1.4.4',
-             'nifgen[grpc]>=1.4.4',
-             'niscope[grpc]>=1.4.4',
-             'niswitch[grpc]>=1.4.4'],
- 'nidaqmx': ['nidaqmx[grpc]>=0.8.0'],
- 'nidcpower': ['nidcpower[grpc]>=1.4.4'],
- 'nidigital': ['nidigital[grpc]>=1.4.4'],
- 'nidmm': ['nidmm[grpc]>=1.4.4'],
- 'nifgen': ['nifgen[grpc]>=1.4.4'],
- 'niscope': ['niscope[grpc]>=1.4.4'],
- 'niswitch': ['niswitch[grpc]>=1.4.4']}
-
-setup_kwargs = {
-    'name': 'ni-measurementlink-service',
-    'version': '1.4.0.dev1',
-    'description': 'MeasurementLink Support for Python',
-    'long_description': '# MeasurementLink™ Support for Python\n\n- [MeasurementLink™ Support for Python](#measurementlink--support-for-python)\n  - [Introduction](#introduction)\n  - [Dependencies](#dependencies)\n  - [Documentation](#documentation)\n  - [Examples](#examples)\n  - [Developing Measurements: Quick Start](#developing-measurements-quick-start)\n    - [Installation](#installation)\n    - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)\n  - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)\n  - [Static Registration of Python Measurements](#static-registration-of-python-measurements)\n    - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)\n    - [Create Executable for Python Scripts](#create-executable-for-python-scripts)\n  - [Appendix: Managing Measurement as Python Package (Project)](#appendix-managing-measurement-as-python-package-project)\n    - [Create and Manage Python Measurement Package using Poetry](#create-and-manage-python-measurement-package-using-poetry)\n    - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)\n    - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)\n\n---\n\n## Introduction\n\nMeasurementLink Support for Python (`ni-measurementlink-service`) is a Python\nframework that helps you create reusable measurement plug-ins using gRPC\nservices. Deploy your measurement plug-ins to perform interactive validation in\nInstrumentStudio and automated testing in TestStand.\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)\n- [protobuf >= 4.21, < 5.x](https://pypi.org/project/protobuf/4.21.0/)\n- [pywin32 >= 303 (Only for Windows)](https://pypi.org/project/pywin32/303/)\n\n---\n\n## Documentation\n\n- [MeasurementLink Manual](https://www.ni.com/docs/en-US/bundle/measurementlink)\n- [API Reference](https://ni.github.io/measurementlink-python/)\n\n---\n\n## System Configuration\n\n### Enable Win32 Long Paths\n\nBy default, Windows has a path length limit of 260 characters. NI recommends enabling support for long paths when developing and deploying Python measurement services. \n\nThere are three ways to do this:\n- When installing Python using the Python for Windows installer, click `Disable path length limit` at the end of the installation.\n- Set the `Enable Win32 long paths` group policy:\n  - Run `gpedit.msc`.\n  - Expand `Computer Configuration` » `Administrative Templates` » `All Settings`.\n  - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.\n- In the Windows registry, set `HKEY_LOCAL_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\FileSystem\\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).\n\n---\n\n## Examples\n\nThe `examples` directory contains example measurements for MeasurementLink 2024 Q2 or later. If\nyou are using a previous version of MeasurementLink, download the appropriate examples:\n\n- MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)\n- MeasurementLink 2023 Q3: [measurementlink-python-examples-1.1.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.1.0/measurementlink-python-examples-1.1.0.zip)\n- MeasurementLink 2023 Q4: [measurementlink-python-examples-1.2.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.2.0/measurementlink-python-examples-1.2.0.zip)\n- MeasurementLink 2024 Q1: [measurementlink-python-examples-1.3.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.3.0/measurementlink-python-examples-1.3.0.zip)\n\nFor more information on setting up and running the example measurements, see the included `README.md` file.\n\nFor best results, use the example measurements corresponding to the version of MeasurementLink\nthat you are using. Newer examples may demonstrate features that are not available in older\nversions of MeasurementLink.\n\n---\n\n## Developing Measurements: Quick Start\n\nThis section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.\n\n### Installation\n\nMake sure the system has the recommended Python version is installed. Install MeasurementLink Support for Python using [pip](https://pip.pypa.io/).\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-service\n```\n\nCheck if you have installed the expected version of MeasurementLink Support for Python installed by running the below command:\n\n```cmd\npip show ni-measurementlink-service\n```\n\n### Developing a minimal Python measurement\n\n1. Install the `ni-measurementlink-generator` package.\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-generator\n```\n\n2. Run the `ni-measurementlink-generator` tool. Use command line arguments to specify the `display-name` and optionally the `version`, `measurement-type`, and `product-type`.\n\n    1. Running `ni-measurementlink-generator` without optional arguments:\n\n    `ni-measurementlink-generator SampleMeasurement`\n\n    \'SampleMeasurement\' is the display name of your measurement service. Without the optional arguments,\n    the other arguments are generated for you based on the display name.\n\n    2. Running `ni-measurementlink-generator` with optional arguments for `measurement-version`, `ui-file`,\n    `service-class`, and `description-url`:\n\n    `ni-measurementlink-generator SampleMeasurement --measurement-version 0.1.0.0 --ui-file MeasurementUI.measui --service-class SampleMeasurement_Python --description-url https://www.example.com/SampleMeasurement.html`\n\n    3. Running `ni-measurementlink-generator` with optional argument for `directory-out`\n\n    `ni-measurementlink-generator SampleMeasurement --directory-out <new_path_for_created_files>`\n\n    If no output directory is specified, the files will\n    be placed in a new folder under the current directory\n    named after the display name without spaces.\n\n3. To customize the created measurement, provide metadata of the measurement\'s configuration (input parameters) and outputs (output parameters) in `measurement.py`.\n    1. Use the `configuration()` decorator to provide metadata about the configurations.**The order of the configuration decorator must match with the order of the parameters defined in the function signature.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        #Display Names can not contains backslash or front slash.\n        @foo_measurement_service.configuration("DisplayNameForInput1", DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", DataType.String, "DefaultValueForInput2")\n        def measure(input_1, input_2):\n            \'\'\' A simple Measurement method\'\'\'\n            return ["foo", "bar"]\n        ```\n\n    2. Use the `output()` decorator to provide metadata about the output.**The order of the output decorators from top to bottom must match the order of the values of the list returned by the function.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        @foo_measurement_service.configuration("DisplayNameForInput1", nims.DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", nims.DataType.String, "DefaultValueForInput2")\n        @foo_measurement_service.output("DisplayNameForOutput1", nims.DataType.String)\n        @foo_measurement_service.output("DisplayNameForOutput2", nims.DataType.String)\n        def measure(input_1, input_2):\n            return ["foo", "bar"]\n        ```\n\n4. Run/Debug the created measurement by following the steps discussed in the section ["Steps to run/debug the measurement service".](#steps-to-rundebug-the-measurement-service)\n\n---\n\n## Steps to run/debug the measurement service\n\n1. Start the discovery service if not already started.\n\n2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    .venv\\scripts\\activate\n    ```\n\n    - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.\n    - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:\n\n        ```cmd\n        Set-ExecutionPolicy RemoteSigned \n        ```\n\n3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.\n\n4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.\n\n5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    deactivate\n    ```\n\n---\n\n## Static Registration of Python Measurements\n\nThe MeasurementLink discovery service provides a registry of other services, and can discover and activate other services on the system. These features allow the discovery service to distinguish, manage, and describe measurement services on the system.\n\nTo statically register a measurement service with the MeasurementLink discovery service, do the following:\n\n1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.\n\n2. Edit the measurement service\'s `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.\n\n3. Copy the measurement service\'s directory (including the `.serviceconfig` file and startup batch file) to a subdirectory of `C:\\ProgramData\\National Instruments\\MeasurementLink\\Services`.\n> **Note**\n> If you are using a virtual environment, do not copy the `.venv` subdirectory&mdash;the virtual environment must be re-created in the new location.\n\nOnce your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.\n\n### Create a batch file that runs a Python measurement\n\nThe batch file used for static registration is responsible for starting the Python Scripts.\n\nTypical Batch File:\n\n``` cmd\n"<path_to_python_exe>" "<path_to_measurement_file>"\n```\n\nExamples to start the fictitious file named `foo_measurement.py`:\n\n1. Using the Python system distribution\n\n    ```cmd\n    python foo_measurement.py\n    ```\n\n2. Using the virtual environment\n\n    ```cmd\n    REM Windows\n    .\\.venv\\Scripts\\python.exe foo_measurement.py\n\n    REM Linux \n    .venv/bin/python foo_measurement.py\n    ```\n\n### Create Executable for Python Scripts\n\nTo create an executable from a measurement, you can use the [pyinstaller](https://www.pyinstaller.org/) tooling. If you are using a Poetry project, add `pyinstaller` to its `dev-dependencies`. When statically registering the service, install the EXE into a unique directory along with its .serviceconfig and UI files.\n\nTypical PyInstaller command to build executable:\n\n```cmd\npyinstaller --onefile --console --paths .venv\\Lib\\site-packages measurement.py\n```\n\n## Troubleshooting\n\n### "File not found" or "No such file or directory" errors when copying or running a measurement service\n\nIf copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.\n\n## Appendix: Managing Measurement as Python Package (Project)\n\nMeasurement and its related files can be maintained as a Python package. The basic components of any Python measurement package are:\n\n1. Measurement Python module (`.py` file)\n    - This file contains all the details related to the measurement and also contains the logic for the measurement execution.\n    - This file is run to start the measurement as a service.\n\n2. UI File\n    - UI file for the measurement. Types of supported UI files are:\n        - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.\n        - LabVIEW UI (`.vi`)\n    - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).\n\nPython communities have different ways of managing Python packages and their dependencies. It is up to the measurement developer to decide how to maintain the package and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.\n\n### Create and Manage Python Measurement Package using Poetry\n\n1. Install `poetry` (one-time setup)\n\n    1. Make sure the system has the recommended Python version installed.\n\n    2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.\n\n2. Create a new Python project and add `ni-measurementlink-service` as a dependency to the project.\n\n    1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.\n\n        ``` cmd\n        cd <path_of_directory_of_your_choice>\n        ```\n\n    2. Create a Python package (project) using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.\n\n        ``` cmd\n        poetry new <name_of_the_project>\n        ```\n\n    3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.\n\n        ``` cmd\n        cd <name_of_the_project>\n        poetry add ni-measurementlink-service\n        ```\n\n    4. The virtual environment will be auto-created by poetry.\n\n    5. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n        - Any additional dependencies required by measurement can be added using [add command](https://python-poetry.org/docs/cli/#add).\n\n            ``` cmd\n            poetry add <dependency_package_name>\n            ```\n\nFor detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).\n\n### Create and Manage Python Measurement Package using `venv`\n\n1. Make sure the system has the recommended Python version installed.\n\n2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.\n\n    ``` cmd\n    cd <path_of_directory_of_your_choice>\n    ```\n\n3. Create a virtual environment.\n\n    ``` cmd\n    REM This creates a virtual environment named .venv\n    python -m venv .venv\n    ```\n\n4. Activate the virtual environment. After successful activation\n\n    ``` cmd\n    .venv\\scripts\\activate\n    REM Optionally upgrade the pip within the venv by executing the command\n    python -m pip install -U pip\n    ```\n\n5. Install the `ni-measurementlink-service` package into the virtual environment.\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n6. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n    - Any additional dependencies required by measurement can be added pip install.\n\n        ``` cmd\n        pip install <dependency_package_name>\n        ```\n\nFor detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).\n\n### Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package\n\nMeasurement developers can also install `ni-measurementlink-service` as a system package if necessary.\n\n1. Install the `ni-measurementlink-service` package from the command prompt\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n2. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n\n---\n',
-    'author': 'NI',
-    'author_email': 'opensource@ni.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ni/measurementlink-python/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
+# MeasurementLink™ Support for Python
 
+- [MeasurementLink™ Support for Python](#measurementlink--support-for-python)
+  - [Introduction](#introduction)
+  - [Dependencies](#dependencies)
+  - [Documentation](#documentation)
+  - [Examples](#examples)
+  - [Developing Measurements: Quick Start](#developing-measurements-quick-start)
+    - [Installation](#installation)
+    - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)
+  - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)
+  - [Static Registration of Python Measurements](#static-registration-of-python-measurements)
+    - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)
+    - [Create Executable for Python Scripts](#create-executable-for-python-scripts)
+  - [Appendix: Managing Measurement with Python](#appendix-managing-measurement-with-python)
+    - [Create and Manage Python Measurement using Poetry](#create-and-manage-python-measurement-using-poetry)
+    - [Create and Manage Python Measurement using `venv`](#create-and-manage-python-measurement-using-venv)
+    - [Create and Manage Python Measurement by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)
+
+---
+
+## Introduction
+
+MeasurementLink Support for Python (`ni-measurementlink-service`) is a Python
+framework that helps you create reusable measurement plug-ins using gRPC
+services. Deploy your measurement plug-ins to perform interactive validation in
+InstrumentStudio and automated testing in TestStand.
+
+---
+
+## Dependencies
+
+- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)
+- [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)
+- [protobuf >= 4.21, < 5.x](https://pypi.org/project/protobuf/4.21.0/)
+- [pywin32 >= 303 (Only for Windows)](https://pypi.org/project/pywin32/303/)
+
+---
+
+## Documentation
+
+- [MeasurementLink Manual](https://www.ni.com/docs/en-US/bundle/measurementlink)
+- [API Reference](https://ni.github.io/measurementlink-python/)
+
+---
+
+## System Configuration
+
+### Enable Win32 Long Paths
+
+By default, Windows has a path length limit of 260 characters. NI recommends enabling support for long paths when developing and deploying Python measurement services. 
+
+There are three ways to do this:
+- When installing Python using the Python for Windows installer, click `Disable path length limit` at the end of the installation.
+- Set the `Enable Win32 long paths` group policy:
+  - Run `gpedit.msc`.
+  - Expand `Computer Configuration` » `Administrative Templates` » `All Settings`.
+  - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.
+- In the Windows registry, set `HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FileSystem\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).
+
+---
+
+## Examples
+
+The `examples` directory contains example measurements for MeasurementLink 2024 Q2 or later. If
+you are using a previous version of MeasurementLink, download the appropriate examples:
+
+- MeasurementLink 2023 Q1: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
+- MeasurementLink 2023 Q2: [measurementlink-python-examples-1.0.1.zip](https://github.com/ni/measurementlink-python/releases/download/1.0.1/measurementlink-python-examples-1.0.1.zip)
+- MeasurementLink 2023 Q3: [measurementlink-python-examples-1.1.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.1.0/measurementlink-python-examples-1.1.0.zip)
+- MeasurementLink 2023 Q4: [measurementlink-python-examples-1.2.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.2.0/measurementlink-python-examples-1.2.0.zip)
+- MeasurementLink 2024 Q1: [measurementlink-python-examples-1.3.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.3.0/measurementlink-python-examples-1.3.0.zip)
+- MeasurementLink 2024 Q2: [measurementlink-python-examples-1.4.0.zip](https://github.com/ni/measurementlink-python/releases/download/1.4.0/measurementlink-python-examples-1.4.0.zip)
+
+
+For more information on setting up and running the example measurements, see the included `README.md` file.
+
+For best results, use the example measurements corresponding to the version of MeasurementLink
+that you are using. Newer examples may demonstrate features that are not available in older
+versions of MeasurementLink.
+
+---
+
+## Developing Measurements: Quick Start
+
+This section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.
+
+### Installation
+
+Make sure the system has the recommended Python version is installed. Install MeasurementLink Support for Python using [pip](https://pip.pypa.io/).
+
+``` cmd
+REM Activate the required virtual environment if any.
+pip install ni-measurementlink-service
+```
+
+Check if you have installed the expected version of MeasurementLink Support for Python installed by running the below command:
+
+```cmd
+pip show ni-measurementlink-service
+```
+
+### Developing a minimal Python measurement
+
+1. Install the `ni-measurementlink-generator` package.
+
+``` cmd
+REM Activate the required virtual environment if any.
+pip install ni-measurementlink-generator
+```
+
+2. Run the `ni-measurementlink-generator` tool. Use command line arguments to specify the `display-name` and optionally the `version`, `measurement-type`, and `product-type`.
+
+    1. Running `ni-measurementlink-generator` without optional arguments:
+
+    `ni-measurementlink-generator SampleMeasurement`
+
+    'SampleMeasurement' is the display name of your measurement service. Without the optional arguments,
+    the other arguments are generated for you based on the display name.
+
+    2. Running `ni-measurementlink-generator` with optional arguments for `measurement-version`, `ui-file`,
+    `service-class`, and `description-url`:
+
+    `ni-measurementlink-generator SampleMeasurement --measurement-version 0.1.0.0 --ui-file MeasurementUI.measui --service-class SampleMeasurement_Python --description-url https://www.example.com/SampleMeasurement.html`
+
+    3. Running `ni-measurementlink-generator` with optional argument for `directory-out`
+
+    `ni-measurementlink-generator SampleMeasurement --directory-out <new_path_for_created_files>`
+
+    If no output directory is specified, the files will
+    be placed in a new folder under the current directory
+    named after the display name without spaces.
+
+3. To customize the created measurement, provide metadata of the measurement's configuration (input parameters) and outputs (output parameters) in `measurement.py`.
+    1. Use the `configuration()` decorator to provide metadata about the configurations.**The order of the configuration decorator must match with the order of the parameters defined in the function signature.**
+
+        ``` python
+        @foo_measurement_service.register_measurement
+        #Display Names can not contains backslash or front slash.
+        @foo_measurement_service.configuration("DisplayNameForInput1", DataType.String, "DefaultValueForInput1")
+        @foo_measurement_service.configuration("DisplayNameForInput2", DataType.String, "DefaultValueForInput2")
+        def measure(input_1, input_2):
+            ''' A simple Measurement method'''
+            return ["foo", "bar"]
+        ```
+
+    2. Use the `output()` decorator to provide metadata about the output.**The order of the output decorators from top to bottom must match the order of the values of the list returned by the function.**
+
+        ``` python
+        @foo_measurement_service.register_measurement
+        @foo_measurement_service.configuration("DisplayNameForInput1", nims.DataType.String, "DefaultValueForInput1")
+        @foo_measurement_service.configuration("DisplayNameForInput2", nims.DataType.String, "DefaultValueForInput2")
+        @foo_measurement_service.output("DisplayNameForOutput1", nims.DataType.String)
+        @foo_measurement_service.output("DisplayNameForOutput2", nims.DataType.String)
+        def measure(input_1, input_2):
+            return ["foo", "bar"]
+        ```
+
+4. Run/Debug the created measurement by following the steps discussed in the section ["Steps to run/debug the measurement service".](#steps-to-rundebug-the-measurement-service)
+
+---
+
+## Steps to run/debug the measurement service
+
+1. Start the discovery service if not already started.
+
+2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-using-poetry)
+
+    ```cmd
+    .venv\scripts\activate
+    ```
+
+    - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.
+    - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:
+
+        ```cmd
+        Set-ExecutionPolicy RemoteSigned 
+        ```
+
+3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.
+
+4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.
+
+5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-using-poetry)
+
+    ```cmd
+    deactivate
+    ```
+
+---
+
+## Static Registration of Python Measurements
+
+The MeasurementLink discovery service provides a registry of other services, and can discover and activate other services on the system. These features allow the discovery service to distinguish, manage, and describe measurement services on the system.
+
+To statically register a measurement service with the MeasurementLink discovery service, do the following:
+
+1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.
+
+2. Edit the measurement service's `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.
+
+3. Copy the measurement service's directory (including the `.serviceconfig` file and startup batch file) to a subdirectory of `C:\ProgramData\National Instruments\MeasurementLink\Services`.
+> **Note**
+> If you are using a virtual environment, do not copy the `.venv` subdirectory&mdash;the virtual environment must be re-created in the new location.
+
+Once your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.
+
+### Create a batch file that runs a Python measurement
+
+The batch file used for static registration is responsible for starting the Python Scripts.
+
+Typical Batch File:
+
+``` cmd
+"<path_to_python_exe>" "<path_to_measurement_file>"
+```
+
+Examples to start the fictitious file named `foo_measurement.py`:
+
+1. Using the Python system distribution
+
+    ```cmd
+    python foo_measurement.py
+    ```
+
+2. Using the virtual environment
+
+    ```cmd
+    REM Windows
+    .\.venv\Scripts\python.exe foo_measurement.py
+
+    REM Linux 
+    .venv/bin/python foo_measurement.py
+    ```
+
+### Create Executable for Python Scripts
+
+To create an executable from a measurement, you can use the [pyinstaller](https://www.pyinstaller.org/) tooling. If you are using a Poetry project, add `pyinstaller` to its `dev-dependencies`. When statically registering the service, install the EXE into a unique directory along with its .serviceconfig and UI files.
+
+Typical PyInstaller command to build executable:
+
+```cmd
+pyinstaller --onefile --console --paths .venv\Lib\site-packages measurement.py
+```
+
+## Troubleshooting
+
+### "File not found" or "No such file or directory" errors when copying or running a measurement service
+
+If copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.
+
+## Appendix: Managing Measurement with Python
+
+A measurement and its related files can be maintained in different ways in Python. The basic components of any Python measurement are:
+
+1. Measurement Python module (`.py` file)
+    - This file contains all the details related to the measurement and also contains the logic for the measurement execution.
+    - This file is run to start the measurement as a service.
+
+2. UI File
+    - UI file for the measurement. Types of supported UI files are:
+        - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.
+        - LabVIEW UI (`.vi`)
+    - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).
+
+Python communities have different ways of managing Python projects and their dependencies. It is up to the measurement developer to decide how to maintain the project and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.
+
+### Create and Manage Python Measurement using Poetry
+
+1. Install `poetry` (one-time setup)
+
+    1. Make sure the system has the recommended Python version installed.
+
+    2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.
+
+2. Create a new Python project and add `ni-measurementlink-service` as a dependency to the project.
+
+    1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.
+
+        ``` cmd
+        cd <path_of_directory_of_your_choice>
+        ```
+
+    2. Create a Poetry project using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.
+
+        ``` cmd
+        poetry new <name_of_the_project>
+        ```
+
+    3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.
+
+        ``` cmd
+        cd <name_of_the_project>
+        poetry add ni-measurementlink-service
+        ```
+
+    4. The virtual environment will be auto-created by poetry.
+
+    5. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)
+        - Any additional dependencies required by measurement can be added using [add command](https://python-poetry.org/docs/cli/#add).
+
+            ``` cmd
+            poetry add <dependency_package_name>
+            ```
+
+For detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).
+
+### Create and Manage Python Measurement using `venv`
+
+1. Make sure the system has the recommended Python version installed.
+
+2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.
+
+    ``` cmd
+    cd <path_of_directory_of_your_choice>
+    ```
+
+3. Create a virtual environment.
+
+    ``` cmd
+    REM This creates a virtual environment named .venv
+    python -m venv .venv
+    ```
+
+4. Activate the virtual environment. After successful activation
+
+    ``` cmd
+    .venv\scripts\activate
+    REM Optionally upgrade the pip within the venv by executing the command
+    python -m pip install -U pip
+    ```
+
+5. Install the `ni-measurementlink-service` package into the virtual environment.
+
+    ``` cmd
+    pip install ni-measurementlink-service
+    ```
+
+6. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)
+    - Any additional dependencies required by measurement can be added pip install.
+
+        ``` cmd
+        pip install <dependency_package_name>
+        ```
+
+For detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).
+
+### Create and Manage Python Measurement by directly installing `ni-measurementlink-service` as a system-level package
+
+Measurement developers can also install `ni-measurementlink-service` as a system package if necessary.
+
+1. Install the `ni-measurementlink-service` package from the command prompt
+
+    ``` cmd
+    pip install ni-measurementlink-service
+    ```
+
+2. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)
+
+---
 
-setup(**setup_kwargs)
```

