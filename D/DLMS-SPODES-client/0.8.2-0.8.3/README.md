# Comparing `tmp/DLMS_SPODES_client-0.8.2.tar.gz` & `tmp/DLMS_SPODES_client-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.8.2.tar", last modified: Thu Apr 18 10:33:29 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.8.3.tar", last modified: Thu Apr 18 10:44:44 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.8.2.tar` & `DLMS_SPODES_client-0.8.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.346743 DLMS_SPODES_client-0.8.2/
--rw-rw-rw-   0        0        0      526 2024-04-18 10:33:29.346743 DLMS_SPODES_client-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.8.2/README.md
--rw-rw-rw-   0        0        0      836 2024-04-18 10:32:20.000000 DLMS_SPODES_client-0.8.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 10:33:29.347743 DLMS_SPODES_client-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.200222 DLMS_SPODES_client-0.8.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.215263 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   115315 2024-04-18 10:32:20.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/client.py
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.189223 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.233225 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.276223 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.330743 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.333743 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1908 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     5575 2024-04-18 10:32:20.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0     3609 2024-04-15 10:18:59.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/services.py
--rw-rw-rw-   0        0        0    43781 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.229223 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-18 10:33:29.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3251 2024-04-18 10:33:29.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 10:33:29.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-18 10:33:29.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-18 10:33:29.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-18 10:33:29.000000 DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.8.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 10:33:29.343744 DLMS_SPODES_client-0.8.2/test/
--rw-rw-rw-   0        0        0       30 2024-04-15 07:35:51.000000 DLMS_SPODES_client-0.8.2/test/name2.csv
--rw-rw-rw-   0        0        0     8415 2024-04-18 07:59:03.000000 DLMS_SPODES_client-0.8.2/test/test_Client.py
--rw-rw-rw-   0        0        0      167 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.2/test/test_logger.py
--rw-rw-rw-   0        0        0      247 2024-04-15 08:13:39.000000 DLMS_SPODES_client-0.8.2/test/test_services.py
--rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.8.2/test/конфигурация GSM.csv
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.624550 DLMS_SPODES_client-0.8.3/
+-rw-rw-rw-   0        0        0      526 2024-04-18 10:44:44.624550 DLMS_SPODES_client-0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.8.3/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-18 10:42:01.000000 DLMS_SPODES_client-0.8.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 10:44:44.625554 DLMS_SPODES_client-0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.470548 DLMS_SPODES_client-0.8.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.487558 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   115315 2024-04-18 10:32:20.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.460548 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.506547 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.553548 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.608581 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.610550 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1908 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     5575 2024-04-18 10:32:20.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0     3609 2024-04-15 10:18:59.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/services.py
+-rw-rw-rw-   0        0        0    43921 2024-04-18 10:44:33.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.501547 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-18 10:44:44.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3251 2024-04-18 10:44:44.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 10:44:44.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-18 10:44:44.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-18 10:44:44.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-18 10:44:44.000000 DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.8.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:44:44.622550 DLMS_SPODES_client-0.8.3/test/
+-rw-rw-rw-   0        0        0       30 2024-04-15 07:35:51.000000 DLMS_SPODES_client-0.8.3/test/name2.csv
+-rw-rw-rw-   0        0        0     8415 2024-04-18 07:59:03.000000 DLMS_SPODES_client-0.8.3/test/test_Client.py
+-rw-rw-rw-   0        0        0      167 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.3/test/test_logger.py
+-rw-rw-rw-   0        0        0      247 2024-04-15 08:13:39.000000 DLMS_SPODES_client-0.8.3/test/test_services.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.8.3/test/конфигурация GSM.csv
```

### Comparing `DLMS_SPODES_client-0.8.2/PKG-INFO` & `DLMS_SPODES_client-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.8.2
+Version: 0.8.3
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.8.2/pyproject.toml` & `DLMS_SPODES_client-0.8.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.8.2"
+version = "0.8.3"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
     "DLMS-SPODES == 0.69.6",
     "DLMS-SPODES-communications >= 1.2.4",
     "pycryptodomex>=3.15"
```

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/client.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/logger.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/logger.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/servers.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/servers.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/services.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/services.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client/task.py` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -754,16 +754,15 @@
                 c.log(logL.INFO, "already INITIATED")
                 await ReadAttribute(
                     ln=obj.logical_name,
                     index=4
                 ).exchange(c)
                 try:
                     obj.set_block_for_transfer(int(obj.image_first_not_transferred_block_number))
-                except IndexError as e:
-                    """Skip set block"""
+                except IndexError as e:  # Skip set block
                     await c.execute_method(obj.get_meth_descriptor(3))
                     c.log(logL.INFO, "Start Verify Transfer")
             while True:
                 c.log(logL.INFO, F"{obj.image_transfer_status=}")
                 try:
                     match current_status:
                         case self.previous_status if self.previous_status == i_t_status.VERIFICATION_FAILED:
@@ -776,14 +775,15 @@
                         case i_t_status.TRANSFER_INITIATED:
                             while True:
                                 if c.is_stop_request:
                                     c.set_error(Transmit.ABORT, '')
                                     return False
                                 await c.execute_method(obj.get_meth_descriptor(2))  # start block: {obj.current_block_transfer} transferred
                                 try:
+                                    c.log(logL.STATE, Progress(obj.current_block_transfer, obj.get_n_blocks(), F"update {collection.get_name(obj.logical_name)}"))
                                     obj.set_next_block()
                                 except StopIteration:
                                     c.log(logL.INFO, "All blocks transferred")
                                     break
                             await c.execute_method(obj.get_meth_descriptor(3))  # Start Verify Transfer
                         case i_t_status.VERIFICATION_INITIATED:
                             c.log(logL.INFO, "read bitstring. It must grow")
```

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.8.2
+Version: 0.8.3
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.8.2/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.8.3/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.2/test/test_Client.py` & `DLMS_SPODES_client-0.8.3/test/test_Client.py`

 * *Files identical despite different names*

