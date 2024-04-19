# Comparing `tmp/inhandtest-0.0.85.tar.gz` & `tmp/inhandtest-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inhandtest-0.0.85.tar", last modified: Fri Feb 23 06:56:40 2024, max compression
+gzip compressed data, was "inhandtest-0.0.86.tar", last modified: Mon Mar 11 10:08:54 2024, max compression
```

## Comparing `inhandtest-0.0.85.tar` & `inhandtest-0.0.86.tar`

### file list

```diff
@@ -1,118 +1,119 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:40.175498 inhandtest-0.0.85/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.85/MANIFEST.in
--rw-rw-rw-   0        0        0     1114 2024-02-23 06:56:40.173529 inhandtest-0.0.85/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.85/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.446760 inhandtest-0.0.85/inhandtest/
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.456760 inhandtest-0.0.85/inhandtest/Task/
--rw-rw-rw-   0        0        0      134 2024-01-17 07:47:07.000000 inhandtest-0.0.85/inhandtest/Task/__init__.py
--rw-rw-rw-   0        0        0     9775 2024-02-23 06:50:22.000000 inhandtest-0.0.85/inhandtest/Task/task.py
--rw-rw-rw-   0        0        0      278 2024-02-01 08:41:59.000000 inhandtest-0.0.85/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.565096 inhandtest-0.0.85/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.85/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    65929 2024-02-22 03:55:42.000000 inhandtest-0.0.85/inhandtest/base_page/_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.85/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-09-27 08:02:56.000000 inhandtest-0.0.85/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    37381 2024-02-08 07:01:22.000000 inhandtest-0.0.85/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0     6036 2024-02-04 10:19:24.000000 inhandtest-0.0.85/inhandtest/base_page/contents_locale.yaml
--rw-rw-rw-   0        0        0     1432 2023-12-06 00:52:27.000000 inhandtest-0.0.85/inhandtest/base_page/login_config.yaml
--rw-rw-rw-   0        0        0    40295 2024-01-05 07:24:35.000000 inhandtest-0.0.85/inhandtest/base_page/page.py
--rw-rw-rw-   0        0        0    36524 2023-12-20 06:31:07.000000 inhandtest-0.0.85/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0     4815 2024-01-08 02:56:43.000000 inhandtest-0.0.85/inhandtest/er_events.yaml
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.85/inhandtest/exception.py
--rw-rw-rw-   0        0        0     9144 2024-02-06 10:30:52.000000 inhandtest-0.0.85/inhandtest/file.py
--rw-rw-rw-   0        0        0    30765 2024-02-07 05:17:36.000000 inhandtest-0.0.85/inhandtest/inexpect.py
--rw-rw-rw-   0        0        0    12257 2023-07-14 09:49:55.000000 inhandtest-0.0.85/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     7991 2023-11-27 01:29:51.000000 inhandtest-0.0.85/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.85/inhandtest/inmqtt.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.694392 inhandtest-0.0.85/inhandtest/inrequest/
--rw-rw-rw-   0        0        0      573 2023-07-13 10:11:38.000000 inhandtest-0.0.85/inhandtest/inrequest/__init__.py
--rw-rw-rw-   0        0        0    17104 2024-02-01 06:09:58.000000 inhandtest-0.0.85/inhandtest/inrequest/console.py
--rw-rw-rw-   0        0        0    29178 2024-02-06 10:30:52.000000 inhandtest-0.0.85/inhandtest/inrequest/dm.py
--rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.85/inhandtest/inrequest/dn.py
--rw-rw-rw-   0        0        0    15010 2024-02-22 03:55:42.000000 inhandtest-0.0.85/inhandtest/inrequest/er_default_config.py
--rw-rw-rw-   0        0        0    51318 2024-02-22 03:55:42.000000 inhandtest-0.0.85/inhandtest/inrequest/er_device.py
--rw-rw-rw-   0        0        0     3515 2024-02-01 06:09:58.000000 inhandtest-0.0.85/inhandtest/inrequest/execute_yaml_api.py
--rw-rw-rw-   0        0        0    10197 2024-02-06 10:30:52.000000 inhandtest-0.0.85/inhandtest/inrequest/ics.py
--rw-rw-rw-   0        0        0    15597 2024-02-21 08:50:24.000000 inhandtest-0.0.85/inhandtest/inrequest/inrequest.py
--rw-rw-rw-   0        0        0     5198 2023-11-30 02:56:51.000000 inhandtest-0.0.85/inhandtest/inrequest/link.py
--rw-rw-rw-   0        0        0   120807 2024-01-22 06:06:31.000000 inhandtest-0.0.85/inhandtest/inrequest/nezha.py
--rw-rw-rw-   0        0        0    11544 2023-11-30 09:31:34.000000 inhandtest-0.0.85/inhandtest/inrequest/oms.py
--rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.85/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    17053 2024-02-22 03:55:42.000000 inhandtest-0.0.85/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     8465 2024-02-08 07:01:22.000000 inhandtest-0.0.85/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     2042 2023-08-11 10:34:14.000000 inhandtest-0.0.85/inhandtest/ip.py
--rw-rw-rw-   0        0        0     1438 2023-12-06 09:20:18.000000 inhandtest-0.0.85/inhandtest/log.py
--rw-rw-rw-   0        0        0    18530 2024-02-23 06:50:22.000000 inhandtest-0.0.85/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.85/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.709899 inhandtest-0.0.85/inhandtest/openvpn_tools_in_windows/
--rw-rw-rw-   0        0        0      134 2023-10-09 06:21:40.000000 inhandtest-0.0.85/inhandtest/openvpn_tools_in_windows/__init__.py
--rw-rw-rw-   0        0        0     3344 2023-12-19 07:14:10.000000 inhandtest-0.0.85/inhandtest/openvpn_tools_in_windows/openvpn_tools.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.726868 inhandtest-0.0.85/inhandtest/pages/
--rw-rw-rw-   0        0        0      453 2023-11-30 09:30:52.000000 inhandtest-0.0.85/inhandtest/pages/__init__.py
--rw-rw-rw-   0        0        0    11124 2023-12-01 06:59:56.000000 inhandtest-0.0.85/inhandtest/pages/adapt_model_locator.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.741205 inhandtest-0.0.85/inhandtest/pages/er_device/
--rw-rw-rw-   0        0        0      263 2023-09-22 02:26:44.000000 inhandtest-0.0.85/inhandtest/pages/er_device/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.755405 inhandtest-0.0.85/inhandtest/pages/er_device/eap600/
--rw-rw-rw-   0        0        0      135 2023-11-30 08:36:07.000000 inhandtest-0.0.85/inhandtest/pages/er_device/eap600/__init__.py
--rw-rw-rw-   0        0        0      499 2023-11-30 10:19:55.000000 inhandtest-0.0.85/inhandtest/pages/er_device/eap600/config.py
--rw-rw-rw-   0        0        0     3578 2024-02-06 10:30:02.000000 inhandtest-0.0.85/inhandtest/pages/er_device/eap600/eap600.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.853212 inhandtest-0.0.85/inhandtest/pages/er_device/er2000/
--rw-rw-rw-   0        0        0      135 2023-11-30 09:22:31.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er2000/__init__.py
--rw-rw-rw-   0        0        0     5591 2024-02-06 10:30:02.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er2000/er2000.py
--rw-rw-rw-   0        0        0      658 2023-12-06 00:52:27.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er2000/local_network.py
--rw-rw-rw-   0        0        0     2098 2023-12-20 06:31:07.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er2000/security.py
--rw-rw-rw-   0        0        0     1637 2023-12-27 02:32:20.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er2000/services.py
--rw-rw-rw-   0        0        0     1783 2024-01-05 07:24:35.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er2000/status.py
--rw-rw-rw-   0        0        0     2139 2023-12-26 06:08:56.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er2000/system.py
--rw-rw-rw-   0        0        0     1302 2024-01-05 08:44:32.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er2000/vpn.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:39.988386 inhandtest-0.0.85/inhandtest/pages/er_device/er805/
--rw-rw-rw-   0        0        0      135 2023-11-30 08:55:33.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er805/__init__.py
--rw-rw-rw-   0        0        0     5249 2024-02-06 10:30:02.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er805/er805.py
--rw-rw-rw-   0        0        0      657 2023-11-30 08:55:33.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er805/local_network.py
--rw-rw-rw-   0        0        0     1911 2024-01-05 08:44:31.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er805/security.py
--rw-rw-rw-   0        0        0     1636 2023-12-27 02:32:20.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er805/services.py
--rw-rw-rw-   0        0        0     1779 2024-01-05 07:24:35.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er805/status.py
--rw-rw-rw-   0        0        0     2138 2023-12-27 02:32:20.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er805/system.py
--rw-rw-rw-   0        0        0     1300 2024-01-05 08:44:32.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er805/vpn.py
--rw-rw-rw-   0        0        0      557 2023-12-27 02:32:20.000000 inhandtest-0.0.85/inhandtest/pages/er_device/er805/wifi.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:40.015971 inhandtest-0.0.85/inhandtest/pages/er_device/functions/
--rw-rw-rw-   0        0        0      135 2023-11-30 08:17:38.000000 inhandtest-0.0.85/inhandtest/pages/er_device/functions/__init__.py
--rw-rw-rw-   0        0        0    94714 2024-02-08 07:01:22.000000 inhandtest-0.0.85/inhandtest/pages/er_device/functions/functions.py
--rw-rw-rw-   0        0        0   175033 2024-02-22 03:55:42.000000 inhandtest-0.0.85/inhandtest/pages/er_device/functions/functions_locators.py
--rw-rw-rw-   0        0        0    20107 2024-02-08 07:01:22.000000 inhandtest-0.0.85/inhandtest/pages/er_device/locale.yml
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:40.055870 inhandtest-0.0.85/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:40.077211 inhandtest-0.0.85/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0    79465 2024-01-04 02:35:00.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0    86358 2023-12-19 07:40:43.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     4176 2024-01-29 01:18:07.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0    12865 2023-11-15 09:10:00.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      994 2023-11-30 07:44:17.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:40.107711 inhandtest-0.0.85/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    69066 2023-11-30 07:44:17.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    87395 2023-12-04 09:24:03.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:40.135002 inhandtest-0.0.85/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6960 2023-11-30 07:44:17.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6459 2023-12-04 09:24:03.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:40.159499 inhandtest-0.0.85/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28577 2023-11-30 07:44:17.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    31662 2023-12-04 09:24:03.000000 inhandtest-0.0.85/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.85/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0     9102 2024-02-21 08:52:56.000000 inhandtest-0.0.85/inhandtest/sqlite.py
--rw-rw-rw-   0        0        0    36991 2024-02-02 07:33:44.000000 inhandtest-0.0.85/inhandtest/telnet.py
--rw-rw-rw-   0        0        0     2895 2024-02-22 03:55:42.000000 inhandtest-0.0.85/inhandtest/telnet.yaml
--rw-rw-rw-   0        0        0      829 2024-02-01 06:09:58.000000 inhandtest-0.0.85/inhandtest/tftp_server.py
--rw-rw-rw-   0        0        0    37376 2024-02-04 09:55:54.000000 inhandtest-0.0.85/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2024-02-23 06:56:40.172531 inhandtest-0.0.85/inhandtest.egg-info/
--rw-rw-rw-   0        0        0     1114 2024-02-23 06:56:38.000000 inhandtest-0.0.85/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3561 2024-02-23 06:56:39.000000 inhandtest-0.0.85/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 06:56:38.000000 inhandtest-0.0.85/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2024-02-23 06:56:38.000000 inhandtest-0.0.85/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-23 06:56:38.000000 inhandtest-0.0.85/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      230 2024-02-02 05:18:32.000000 inhandtest-0.0.85/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-23 06:56:40.175498 inhandtest-0.0.85/setup.cfg
--rw-rw-rw-   0        0        0     1586 2024-02-23 06:56:34.000000 inhandtest-0.0.85/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.605096 inhandtest-0.0.86/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.86/MANIFEST.in
+-rw-rw-rw-   0        0        0     1114 2024-03-11 10:08:54.604098 inhandtest-0.0.86/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.86/README.md
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:53.361481 inhandtest-0.0.86/inhandtest/
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:53.439673 inhandtest-0.0.86/inhandtest/Task/
+-rw-rw-rw-   0        0        0      134 2024-01-17 07:47:07.000000 inhandtest-0.0.86/inhandtest/Task/__init__.py
+-rw-rw-rw-   0        0        0    10045 2024-03-08 06:01:21.000000 inhandtest-0.0.86/inhandtest/Task/task.py
+-rw-rw-rw-   0        0        0      278 2024-02-01 08:41:59.000000 inhandtest-0.0.86/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:53.540059 inhandtest-0.0.86/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.86/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    65931 2024-03-11 06:28:08.000000 inhandtest-0.0.86/inhandtest/base_page/_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.86/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-09-27 08:02:56.000000 inhandtest-0.0.86/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    37434 2024-03-11 06:28:08.000000 inhandtest-0.0.86/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0     6036 2024-02-04 10:19:24.000000 inhandtest-0.0.86/inhandtest/base_page/contents_locale.yaml
+-rw-rw-rw-   0        0        0     1432 2023-12-06 00:52:27.000000 inhandtest-0.0.86/inhandtest/base_page/login_config.yaml
+-rw-rw-rw-   0        0        0    40627 2024-03-11 06:28:08.000000 inhandtest-0.0.86/inhandtest/base_page/page.py
+-rw-rw-rw-   0        0        0    36524 2024-03-11 06:28:08.000000 inhandtest-0.0.86/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0     4815 2024-01-08 02:56:43.000000 inhandtest-0.0.86/inhandtest/er_events.yaml
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.86/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     9692 2024-03-11 10:03:24.000000 inhandtest-0.0.86/inhandtest/file.py
+-rw-rw-rw-   0        0        0     5963 2024-03-11 06:28:09.000000 inhandtest-0.0.86/inhandtest/inconfig.py
+-rw-rw-rw-   0        0        0    30776 2024-03-11 06:28:08.000000 inhandtest-0.0.86/inhandtest/inexpect.py
+-rw-rw-rw-   0        0        0    12257 2023-07-14 09:49:55.000000 inhandtest-0.0.86/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     7584 2024-03-11 06:28:09.000000 inhandtest-0.0.86/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22542 2023-07-03 10:18:22.000000 inhandtest-0.0.86/inhandtest/inmqtt.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:53.836139 inhandtest-0.0.86/inhandtest/inrequest/
+-rw-rw-rw-   0        0        0      573 2023-07-13 10:11:38.000000 inhandtest-0.0.86/inhandtest/inrequest/__init__.py
+-rw-rw-rw-   0        0        0    17104 2024-02-01 06:09:58.000000 inhandtest-0.0.86/inhandtest/inrequest/console.py
+-rw-rw-rw-   0        0        0    29178 2024-02-06 10:30:52.000000 inhandtest-0.0.86/inhandtest/inrequest/dm.py
+-rw-rw-rw-   0        0        0     4043 2023-07-05 05:22:24.000000 inhandtest-0.0.86/inhandtest/inrequest/dn.py
+-rw-rw-rw-   0        0        0    15010 2024-02-22 03:55:42.000000 inhandtest-0.0.86/inhandtest/inrequest/er_default_config.py
+-rw-rw-rw-   0        0        0    52748 2024-03-11 06:28:08.000000 inhandtest-0.0.86/inhandtest/inrequest/er_device.py
+-rw-rw-rw-   0        0        0     3515 2024-02-01 06:09:58.000000 inhandtest-0.0.86/inhandtest/inrequest/execute_yaml_api.py
+-rw-rw-rw-   0        0        0    10197 2024-02-06 10:30:52.000000 inhandtest-0.0.86/inhandtest/inrequest/ics.py
+-rw-rw-rw-   0        0        0    15597 2024-02-21 08:50:24.000000 inhandtest-0.0.86/inhandtest/inrequest/inrequest.py
+-rw-rw-rw-   0        0        0     5198 2023-11-30 02:56:51.000000 inhandtest-0.0.86/inhandtest/inrequest/link.py
+-rw-rw-rw-   0        0        0   120807 2024-01-22 06:06:31.000000 inhandtest-0.0.86/inhandtest/inrequest/nezha.py
+-rw-rw-rw-   0        0        0    11544 2023-11-30 09:31:34.000000 inhandtest-0.0.86/inhandtest/inrequest/oms.py
+-rw-rw-rw-   0        0        0     8389 2023-07-03 08:50:33.000000 inhandtest-0.0.86/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    17053 2024-03-07 08:57:16.000000 inhandtest-0.0.86/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8465 2024-02-08 07:01:22.000000 inhandtest-0.0.86/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     2026 2024-03-11 10:07:09.000000 inhandtest-0.0.86/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1438 2023-12-06 09:20:18.000000 inhandtest-0.0.86/inhandtest/log.py
+-rw-rw-rw-   0        0        0    18530 2024-02-23 06:50:22.000000 inhandtest-0.0.86/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.86/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:53.874212 inhandtest-0.0.86/inhandtest/openvpn_tools_in_windows/
+-rw-rw-rw-   0        0        0      134 2023-10-09 06:21:40.000000 inhandtest-0.0.86/inhandtest/openvpn_tools_in_windows/__init__.py
+-rw-rw-rw-   0        0        0     3344 2024-03-04 01:37:32.000000 inhandtest-0.0.86/inhandtest/openvpn_tools_in_windows/openvpn_tools.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:53.908215 inhandtest-0.0.86/inhandtest/pages/
+-rw-rw-rw-   0        0        0      453 2023-11-30 09:30:52.000000 inhandtest-0.0.86/inhandtest/pages/__init__.py
+-rw-rw-rw-   0        0        0    11124 2023-12-01 06:59:56.000000 inhandtest-0.0.86/inhandtest/pages/adapt_model_locator.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:53.945183 inhandtest-0.0.86/inhandtest/pages/er_device/
+-rw-rw-rw-   0        0        0      263 2023-09-22 02:26:44.000000 inhandtest-0.0.86/inhandtest/pages/er_device/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:53.977798 inhandtest-0.0.86/inhandtest/pages/er_device/eap600/
+-rw-rw-rw-   0        0        0      135 2023-11-30 08:36:07.000000 inhandtest-0.0.86/inhandtest/pages/er_device/eap600/__init__.py
+-rw-rw-rw-   0        0        0      499 2023-11-30 10:19:55.000000 inhandtest-0.0.86/inhandtest/pages/er_device/eap600/config.py
+-rw-rw-rw-   0        0        0     3578 2024-02-06 10:30:02.000000 inhandtest-0.0.86/inhandtest/pages/er_device/eap600/eap600.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.121645 inhandtest-0.0.86/inhandtest/pages/er_device/er2000/
+-rw-rw-rw-   0        0        0      135 2023-11-30 09:22:31.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er2000/__init__.py
+-rw-rw-rw-   0        0        0     5591 2024-02-06 10:30:02.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er2000/er2000.py
+-rw-rw-rw-   0        0        0      658 2023-12-06 00:52:27.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er2000/local_network.py
+-rw-rw-rw-   0        0        0     2098 2023-12-20 06:31:07.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er2000/security.py
+-rw-rw-rw-   0        0        0     1637 2023-12-27 02:32:20.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er2000/services.py
+-rw-rw-rw-   0        0        0     1783 2024-01-05 07:24:35.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er2000/status.py
+-rw-rw-rw-   0        0        0     2139 2023-12-26 06:08:56.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er2000/system.py
+-rw-rw-rw-   0        0        0     1302 2024-01-05 08:44:32.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er2000/vpn.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.276294 inhandtest-0.0.86/inhandtest/pages/er_device/er805/
+-rw-rw-rw-   0        0        0      135 2023-11-30 08:55:33.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er805/__init__.py
+-rw-rw-rw-   0        0        0     5249 2024-02-06 10:30:02.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er805/er805.py
+-rw-rw-rw-   0        0        0      657 2023-11-30 08:55:33.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er805/local_network.py
+-rw-rw-rw-   0        0        0     1911 2024-01-05 08:44:31.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er805/security.py
+-rw-rw-rw-   0        0        0     1636 2023-12-27 02:32:20.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er805/services.py
+-rw-rw-rw-   0        0        0     1779 2024-01-05 07:24:35.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er805/status.py
+-rw-rw-rw-   0        0        0     2138 2023-12-27 02:32:20.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er805/system.py
+-rw-rw-rw-   0        0        0     1300 2024-01-05 08:44:32.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er805/vpn.py
+-rw-rw-rw-   0        0        0      557 2023-12-27 02:32:20.000000 inhandtest-0.0.86/inhandtest/pages/er_device/er805/wifi.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.315654 inhandtest-0.0.86/inhandtest/pages/er_device/functions/
+-rw-rw-rw-   0        0        0      135 2023-11-30 08:17:38.000000 inhandtest-0.0.86/inhandtest/pages/er_device/functions/__init__.py
+-rw-rw-rw-   0        0        0    94713 2024-03-11 06:28:08.000000 inhandtest-0.0.86/inhandtest/pages/er_device/functions/functions.py
+-rw-rw-rw-   0        0        0   175033 2024-02-22 03:55:42.000000 inhandtest-0.0.86/inhandtest/pages/er_device/functions/functions_locators.py
+-rw-rw-rw-   0        0        0    20107 2024-02-08 07:01:22.000000 inhandtest-0.0.86/inhandtest/pages/er_device/locale.yml
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.389683 inhandtest-0.0.86/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.457071 inhandtest-0.0.86/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0    79473 2024-03-05 06:30:17.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0    86358 2023-12-19 07:40:43.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     4176 2024-01-29 01:18:07.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0    12865 2023-11-15 09:10:00.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      994 2023-11-30 07:44:17.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.514455 inhandtest-0.0.86/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    69066 2023-11-30 07:44:17.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    87395 2023-12-04 09:24:03.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.552153 inhandtest-0.0.86/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6960 2023-11-30 07:44:17.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6459 2023-12-04 09:24:03.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.599115 inhandtest-0.0.86/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28577 2023-11-30 07:44:17.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    31662 2023-12-04 09:24:03.000000 inhandtest-0.0.86/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.86/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0     9125 2024-03-08 06:01:21.000000 inhandtest-0.0.86/inhandtest/sqlite.py
+-rw-rw-rw-   0        0        0    37736 2024-03-11 10:01:34.000000 inhandtest-0.0.86/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0     2895 2024-03-11 06:28:08.000000 inhandtest-0.0.86/inhandtest/telnet.yaml
+-rw-rw-rw-   0        0        0      829 2024-02-01 06:09:58.000000 inhandtest-0.0.86/inhandtest/tftp_server.py
+-rw-rw-rw-   0        0        0    37460 2024-03-08 06:01:21.000000 inhandtest-0.0.86/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2024-03-11 10:08:54.602096 inhandtest-0.0.86/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0     1114 2024-03-11 10:08:52.000000 inhandtest-0.0.86/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3584 2024-03-11 10:08:52.000000 inhandtest-0.0.86/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-11 10:08:52.000000 inhandtest-0.0.86/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      209 2024-03-11 10:08:52.000000 inhandtest-0.0.86/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-11 10:08:52.000000 inhandtest-0.0.86/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      230 2024-03-11 10:02:13.000000 inhandtest-0.0.86/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-03-11 10:08:54.605096 inhandtest-0.0.86/setup.cfg
+-rw-rw-rw-   0        0        0     1586 2024-03-11 10:08:26.000000 inhandtest-0.0.86/setup.py
```

### Comparing `inhandtest-0.0.85/PKG-INFO` & `inhandtest-0.0.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inhandtest
-Version: 0.0.85
+Version: 0.0.86
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `inhandtest-0.0.85/README.md` & `inhandtest-0.0.86/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/Task/task.py` & `inhandtest-0.0.86/inhandtest/Task/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         :param username: 轻流用户名
         :param password: 轻流密码
         :param kwargs: report_path| timeout
                         report_path: 报告路径
                         timeout: 任务超时时间, 默认48小时
                         enable_task_manager: 是否开启任务管理, 默认开启
                         model: 设备型号, 默认ER605
+                        todo_task_expired_time: todo任务过期时间, 默认30天
                         doing_task_expired_time: 任务过期时间, 默认7200秒
                         mail_to: str or list, 任务超时需要通知到的邮箱, 默认['liwei@inhand.com.cn', 'liangyy@inhand.com.cn', 'wangjiaw@inhand.com.cn',
                                               'taocan@inhand.com.cn', 'qinguoliang@inhand.com.cn']
                         mail_from: tuple (email, password), 发送邮件的邮箱, 默认('test@inhand.com.cn', ), 无需密码
                         test_host: str 测试主机地址, 会将主机地址发送到邮件中，
         """
         CiTaskDb.__init__(self, data_file)
@@ -110,14 +111,17 @@
         expires_at = get_time_stamp(delta=8 + self.doing_task_expired_time, delta_type='h',
                                     time_format=self._time_format)
         try:
             if set_args.get('status') == 'doing':
                 if self._get_task_from_qing_flow(status='cancel', _id=_id):
                     self.update({'status': 'cancel', "updated_at": updated_at}, **{"id": _id})
                     return False
+                elif set_args.get('status') == 'timeout':
+                    self.update({**set_args, **{"updated_at": updated_at}}, **{"id": _id})
+                    return False
             self.update({**set_args, **{"updated_at": updated_at, "expires_at": expires_at}}, **{"id": _id})
         except Exception as e:
             logging.debug(f'update task {_id} failed for error:{e}')
         return True
 
     def health_check(self):
         """健康检查"""
```

### Comparing `inhandtest-0.0.85/inhandtest/base_page/_contents_locators.py` & `inhandtest-0.0.86/inhandtest/base_page/_contents_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,16 +421,16 @@
                                 'aria-selected': 'true'}}
                         },
                     },
                     'policy_based_routing': {
                         'menu': self.page.locator(
                             f'div[role="tab"]:text-is("{self.locale.get("policy_based_routing")}")'),
                         'visible_locator': [
-                            self.page.locator('//div[@class="ant-table-container"]').first],
-                        'wait_locator': [self.page.locator('//div[@class="ant-table-container"]').first],
+                            self.page.locator('//div[@class="ant-pro-grid-content"]').first],
+                        'wait_locator': [self.page.locator('//div[@class="ant-pro-grid-content"]').first],
                         'attributes': {self.page.locator(
                             f'div[role="tab"]:text-is("{self.locale.get("policy_based_routing")}")'): {
                             'aria-selected': 'true'}}
                     },
                     'traffic_shaping': {
                         'menu': self.page.locator(
                             f'div[role="tab"]:text-is("{self.locale.get("traffic_shaping")}")'),
```

### Comparing `inhandtest-0.0.85/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.86/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.86/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/base_page/base_page.py` & `inhandtest-0.0.86/inhandtest/base_page/base_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 import os
 import time
 import allure
 import logging
 import base64
 import re
+from playwright._impl._errors import Error
 from inhandtest.base_page._contents_locators import ContentsLocators
 from inhandtest.exception import ModelError
 from inhandtest.base_page.page import Page_
 from inhandtest.inrequest import ErDevice
 from inhandtest.tools import replace_str
 from playwright.sync_api import Page, Locator, TimeoutError, sync_playwright
 from inhandtest.file import read_yaml_file
@@ -162,15 +163,15 @@
                 self.__login_.get('wait_locator')).is_hidden():
                 auth_login()
             elif self.page.locator(self.__login_.get('wait_locator')).is_visible():
                 pass
             else:
                 self.page.reload()
             self.page.locator(self.__login_.get('wait_locator')).wait_for(state='visible', timeout=10 * 1000)
-        except TimeoutError:
+        except (TimeoutError, Error):
             logging.error(f"Device {self.host} page is error")
             goto_router()
             auth_login()
 
     @allure.step('进入菜单')
     def access_menu(self, menu: str, wait_time=None) -> None:
         """进入菜单，多个菜单使用点号隔开，不限多少层级   menu_locator 存放在 base_locators 里面，
```

### Comparing `inhandtest-0.0.85/inhandtest/base_page/contents_locale.yaml` & `inhandtest-0.0.86/inhandtest/base_page/contents_locale.yaml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/base_page/login_config.yaml` & `inhandtest-0.0.86/inhandtest/base_page/login_config.yaml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/base_page/page.py` & `inhandtest-0.0.86/inhandtest/base_page/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,18 @@
                         f'//ul[@role="listbox"]/li').get_by_text(value, exact=True)
                 if now_option != value:
                     locator.scroll_into_view_if_needed()
                     if not locator.is_editable():
                         locator.click(force=True)
                     else:
                         locator.click()
+                    if locator.get_attribute("aria-controls"):  # ER 设备
+                        option = option_p.locator(f'//div[@title="{value}"]') if option_p.locator(
+                            f'//div[@title="{value}"]').count() > 0 else option_p.locator(
+                            f'div:has-text("{value}")').first
                     self.__scroll_into_view_action(all_option, option)
             else:  # IR300 等设备的下拉选择
                 locator.select_option(value)  # value 可以为label 或者value
                 if locator.locator(f'//option[@value="{value}"]').count() == 1:
                     value = locator.locator(f'//option[@value="{value}"]').inner_text()
             if log_desc:
                 logging.info(f"Device {self.host} select {log_desc} of {value}")
```

### Comparing `inhandtest-0.0.85/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.86/inhandtest/base_page/table_tr.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,15 +618,15 @@
                 find_elements[0].locator('.anticon.anticon-edit').click()
                 if ('save' not in list(kwargs.keys())) and ('cancel' not in list(kwargs.keys())):
                     kwargs['save'] = True
                 self.agg_in(self.columns, kwargs)
                 logging.debug(f'locator resource {old_value} to {kwargs} edit success')
                 break
             else:
-                logging.debug(f'tr resource {old_value} not exist in page_number {page_number}')
+                logging.error(f'tr resource {old_value} not exist in page_number {page_number}')
             if not self.turn_page(page_number + 1):
                 break
 
     def delete(self, value: str or re.Pattern) -> None:
         """
         :param value str, 待删除列 及对应值 每列值可按顺序直接连接在一起传入，当然也可以传一列的值 自己国际化
         :return:
```

### Comparing `inhandtest-0.0.85/inhandtest/er_events.yaml` & `inhandtest-0.0.86/inhandtest/er_events.yaml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/exception.py` & `inhandtest-0.0.86/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/file.py` & `inhandtest-0.0.86/inhandtest/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,11 +246,27 @@
             raise ResourceNotFoundError('sheet_names is None')
         sheets_dict = pd.read_excel(file_path, sheet_names)
         for sheet_name, df in sheets_dict.items():
             all_result.extend(df.to_dict('records'))
         return all_result
 
 
+def set_yaml_file(file_path, value: dict):
+    """
+    设置yaml文件中的值
+    :param file_path: 文件路径
+    :param value: 要更改的项和值(不支持嵌套字典)
+    :return: None
+    """
+    with open(file_path, 'r', encoding='utf-8') as file:
+        yaml_info = yaml.safe_load(file)
+    for k, v in value.items():
+        yaml_info[k] = v
+    with open(file_path, 'w', encoding='utf-8') as file:
+        yaml.dump(yaml_info, file, allow_unicode=True)
+
+
 if __name__ == '__main__':
+    pass
     # create_yaml_file({'a': 1, 'b': '中過人'}, './test.yaml')
-    read_csv_file('./EAP600.csv', )
-    print(read_yaml_file('./test.yaml'))
+    # set_yaml_file('G:\ER805_AUTO\conf\er805_setting.yaml', {'local_first': True})
+    # print(read_yaml_file('./test.yaml'))
```

### Comparing `inhandtest-0.0.85/inhandtest/inexpect.py` & `inhandtest-0.0.86/inhandtest/inexpect.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 in_expect
 
 """
 import datetime
 import os
 import typing
+import re
 
 
 class expect:
     def __init__(self, value, args=None, kwargs=None):
         self._value = value
         self._args = args
         self._kwargs = kwargs
```

### Comparing `inhandtest-0.0.85/inhandtest/inmodbus.py` & `inhandtest-0.0.86/inhandtest/inmodbus.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inmongodb.py` & `inhandtest-0.0.86/inhandtest/inmongodb.py`

 * *Files 20% similar despite different names*

```diff
@@ -140,52 +140,54 @@
         :param db: 数据库
         :param collection: 集合
         :param data: 数据     [{'$match': {'name': 'liwei'}}, {$group : {_id : "$iccid", total : {$sum : "$bytesUsed"}}}]
         :return:
         """
         return list(self.client[db][collection].aggregate(data))
 
+    def copy_collection(self, db: str, collection: str):
+        """ 备份某张表，表名为 表名+_backup
+
+        :param db: 数据库
+        :param collection: 集合
+        :return:
+        """
+
+        # 复制集合内容
+        pipeline = [
+            {'$match': {}},  # 可以根据需要添加筛选条件
+            {'$out': f'{collection}_backup'}
+        ]
+        self.client[db][collection].aggregate(pipeline)
+
+    def drop_collection(self, db: str, collection: str):
+        """ 删除某张表格
+
+        :param db: 数据库
+        :param collection: 集合
+        :return:
+        """
+        self.client[db].drop_collection(collection)
+
 
 if __name__ == '__main__':
     from inhandtest.ip import create_ip, create_mac
     from inhandtest.tools import dict_merge
     from bson.objectid import ObjectId
     from dateutil import parser
     import random
 
-
-    def create_one_client() -> dict:
-        type_ = random.choice(['WIRELESS', 'WIRED'])
-        online = False
-        one = {'name': 'test', 'mac': create_mac(),
-               'ip': create_ip(),
-               'type': type_, 'ssid': 'ssid',
-               'wireless': {'rssi': random.randint(-120, -38), 'sinr': random.randint(-23, 40),
-                            'generation': random.choice(['WiFi4', 'WiFi5']),
-                            'band': random.choice(['2.4GHz', '5GHz']),
-                            'mimo': random.choice(['1x1', '2x2', '3x3', '4x4']),
-                            'channel': random.randint(1, 13),
-                            'bandWidth': random.choice(['20MHz', '40MHz', '80MHz', '160MHz'])},
-               'throughput': {'up': random.randint(1 * 1024, 1 * 1024 * 1024 * 10),
-                              'down': random.randint(1 * 1024, 1 * 1024 * 1024 * 10)},
-               'offline': online, "createdAt": parser.parse("2023-08-28T03:06:31.961Z"),
-               "connectedAt": parser.parse("2023-08-28T03:06:31.961Z"),
-               "disconnectedAt": parser.parse("2023-07-25T00:39:31.961Z"),
-               "updatedAt": parser.parse("2023-08-28T03:06:31.961Z"),
-               "lastMessageAt": parser.parse("2023-08-28T03:06:31.961Z"), }
-        if type_ == 'WIRED':
-            one['wireless'] = None
-            one['ssid'] = None
-            one['vlan'] = random.randint(1, 4000)
-            one['networkName'] = f'vlan{one["vlan"]}'
-        return one
-
-
-    beta_mo = mongo = Mongodb('10.5.17.102', 27017, 'root', 'admin')
-    for i in range(0, 100):
-        result = []
-        for x in range(0, 1000):
-            y = dict_merge(create_one_client(),
-                           {"tid": ObjectId("64ab693fd8bbbd7b9820fca0"), "oid": ObjectId("64ab693fd8bbbd7b9820fca0"),
-                            "deviceId": ObjectId("64b73f11d6034e5b52d58807"), })
-            result.append(y)
-        beta_mo.insert_many('nezha_network', 'clients', result)
+    sss = {"network_manager": ["networks"], "nezha_billing": ["license.types"],
+           "nezha_device_manager": ["device.firmware", "firmwares", "ota.modules"],
+           "nezha_iot": ['device.ota.modules', 'device.properties', 'devicegroups', 'devices', 'license.trials',
+                         'product.events',
+                         'product.features', 'product.methods', 'product.models', 'product.properties',
+                         'product.serialNumber.patterns', 'product.topic.jobs', 'product.topics',
+                         'products', 'serialNumber.strategies'],
+           'nezha_network': ["network.devices"]}
+    beta_mo = Mongodb('10.5.17.102', 27017, 'root', 'admin')
+    # for k, v in sss.items():
+    #     for value in v:
+    #         beta_mo.copy_collection(k, value)
+    for k, v in sss.items():
+        for value in v:
+            beta_mo.drop_collection(k, f'{value}_backup')
```

### Comparing `inhandtest-0.0.85/inhandtest/inmqtt.py` & `inhandtest-0.0.86/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/__init__.py` & `inhandtest-0.0.86/inhandtest/inrequest/__init__.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/console.py` & `inhandtest-0.0.86/inhandtest/inrequest/console.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/dm.py` & `inhandtest-0.0.86/inhandtest/inrequest/dm.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/dn.py` & `inhandtest-0.0.86/inhandtest/inrequest/dn.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/er_default_config.py` & `inhandtest-0.0.86/inhandtest/inrequest/er_default_config.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/er_device.py` & `inhandtest-0.0.86/inhandtest/inrequest/er_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -981,14 +981,41 @@
         except (AssertionError, ValueError):
             result = False
         if contain == result:
             return True
         else:
             return False
 
+    def config_rule_priority(self, priority: str, rule_type='inbound'):
+        """
+
+        :param rule_type: 'inbound'|'outbound'|'policy_routing'|'shaping'
+        :param priority: 传入预期优先级排序，eg: 'rule_A>rule_B>rule_C'
+        :return:
+        """
+        sequence = []
+        priority_rule_names = priority.split('>')
+        if rule_type in ("inbound", "outbound"):
+            fields, rule_name, function = 'firewall', rule_type + '_rules', f'firewall.{rule_type}_rules'
+        elif rule_type == 'policy_routing':
+            fields, rule_name, function = 'policy_route', 'ip_rules', f'policy_based_routing'
+        else:
+            fields, rule_name, function = 'qos', 'user_rules', f'traffic_shaping'
+        rule_list = self.get_config(fields=fields).get(fields).get(rule_name)
+        for priority_rule_name in priority_rule_names:
+            for rule in rule_list:
+                if priority_rule_name == rule.get('name'):
+                    sequence.append(rule.get('sequence'))
+                    break
+        sequence.sort()
+        [rule.update({'sequence': sequence[priority_rule_names.index(rule.get('name'))]}) for rule in rule_list if
+         rule.get('name') in priority_rule_names]
+        self.api.send_request(self.path_url.get('config_url'), method='put', body={fields: {rule_name: rule_list}},
+                              expect={'result': 'ok'})
+
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
 
     enable_log(console_level='debug')
     # device = ErDevice('adm', '123456', '10.5.34.184')
     # # device.config_l2tp(character='server', enabled=True, ip='2.2.2.2', start_ip='2.2.2.1', end_ip='2.2.2.254',
```

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/execute_yaml_api.py` & `inhandtest-0.0.86/inhandtest/inrequest/execute_yaml_api.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/ics.py` & `inhandtest-0.0.86/inhandtest/inrequest/ics.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/inrequest.py` & `inhandtest-0.0.86/inhandtest/inrequest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/link.py` & `inhandtest-0.0.86/inhandtest/inrequest/link.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/nezha.py` & `inhandtest-0.0.86/inhandtest/inrequest/nezha.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inrequest/oms.py` & `inhandtest-0.0.86/inhandtest/inrequest/oms.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inserial.py` & `inhandtest-0.0.86/inhandtest/inserial.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/insocket.py` & `inhandtest-0.0.86/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/inssh.py` & `inhandtest-0.0.86/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/ip.py` & `inhandtest-0.0.86/inhandtest/ip.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 """
 import ipaddress
 import random
 import re
 import socket
 
-import xeger
-
 
 def ip_range(ip: str = '192.168.2.3', start_ip: str = '192.168.2.1', end_ip: str = '192.168.2.254',
              assertion=True) -> bool:
     """验证IP地址是否在约定的范围
 
     :param ip: 验证的IP地址
     :param start_ip: IP地址起始
```

### Comparing `inhandtest-0.0.85/inhandtest/log.py` & `inhandtest-0.0.86/inhandtest/log.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/mail.py` & `inhandtest-0.0.86/inhandtest/mail.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/openvpn_tools_in_windows/openvpn_tools.py` & `inhandtest-0.0.86/inhandtest/openvpn_tools_in_windows/openvpn_tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/adapt_model_locator.py` & `inhandtest-0.0.86/inhandtest/pages/adapt_model_locator.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/eap600/eap600.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/eap600/eap600.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er2000/er2000.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er2000/er2000.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er2000/local_network.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er2000/local_network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er2000/security.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er2000/security.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er2000/services.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er2000/services.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er2000/status.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er2000/status.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er2000/system.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er2000/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er2000/vpn.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er2000/vpn.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er805/er805.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er805/er805.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er805/local_network.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er805/local_network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er805/security.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er805/security.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er805/services.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er805/services.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er805/status.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er805/status.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er805/system.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er805/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er805/vpn.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er805/vpn.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/er805/wifi.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/er805/wifi.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/functions/functions.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/functions/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
 
 
 class TrafficShaping(BasePage):
     @allure.step('配置流量整形')
     def config(self, **kwargs):
         """
         :param kwargs:
-            uplinlk_bandwidth:
+            uplink_bandwidth:
                 [('edit', $interface, $new)]
                 action: edit
                     edit parameters:
                         up_bandwidth: int
                         up_bandwidth_unit: 'Kbps'|'Mbps'
                         down_bandwidth: int
                         down_bandwidth_unit: 'Kbps'|'Mbps'
```

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/functions/functions_locators.py` & `inhandtest-0.0.86/inhandtest/pages/er_device/functions/functions_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/er_device/locale.yml` & `inhandtest-0.0.86/inhandtest/pages/er_device/locale.yml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,16 +396,16 @@
     def measure_card_status(self, name) -> list:
         measure_name = f'//div[@class="ant-table-body"]//div[text()="{name}"]'
         measures = [
             ('online_', {'locator': self.page.locator(f'{measure_name}/../../span/span[1]'), 'type': 'class'}),
             ('group', {'locator': self.page.locator(f'{measure_name}/../../../../td[3]'), 'type': 'text'}),
             ('datatype', {'locator': self.page.locator(f'{measure_name}/../../../../td[4]'), 'type': 'text'}),
             ('address', {'locator': self.page.locator(f'{measure_name}/../../../../td[5]'), 'type': 'text'}),
-            ('value', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]/span[1]'), 'type': 'text'}),
-            ('unit', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]/span[2]'), 'type': 'text'}),
+            ('value', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]'), 'type': 'text', 'index': 0}),
+            ('unit', {'locator': self.page.locator(f'{measure_name}/../../../../td[6]'), 'type': 'text', 'index': 1}),
             ('description', {'locator': self.page.locator(f'{measure_name}/../../../../td[7]'), 'type': 'text'}),
             ('time', {'locator': self.page.locator(f'{measure_name}/../../../../td[8]'), 'type': 'text'}),
         ]
         return measures
 
     @property
     def add_measure_all(self):
```

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/ingateway.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.86/inhandtest/pages/ingateway/locale.yml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.86/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/pytest_email.html` & `inhandtest-0.0.86/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/sqlite.py` & `inhandtest-0.0.86/inhandtest/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 class CiTaskDb(Table):
 
     def __init__(self, data_file):
         table_type = ['id TEXT PRIMARY KEY', 'model TEXT', 'firmware_name TEXT', 'svn_path TEXT',
                       'last_firmware_name TEXT', 'last_svn_path TEXT', 'language TEXT',
                       'priority INTEGER', 'status TEXT', 'total_case INTEGER', 'done_case INTEGER',
                       'pass_case INTEGER', 'report_path TEXT', 'reported INTEGER', 'expires_at TEXT',
-                      'created_at TEXT', 'updated_at TEXT']
+                      'created_at TEXT', 'updated_at TEXT', 'test_functions TEXT']
         self.keys = [i.split(' ')[0] for i in table_type]
         super(CiTaskDb, self).__init__(data_file, 'ci_task', table_type)
 
     def select(self, **kwargs) -> typing.List[dict]:
         """ 根据条件查询 返回任务列表里面所有字段
 
         :param kwargs: 查询条件 id='123333'
```

### Comparing `inhandtest-0.0.85/inhandtest/telnet.py` & `inhandtest-0.0.86/inhandtest/telnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -595,15 +595,15 @@
             logging.exception('TcpdumpTimeOutError')
             raise Exception('TcpdumpTimeOutError')
 
     @__auto_login
     @loop_inspector('Telnet regular match content')
     def re_match(self, command: str or list, regular: str or list, type_='super',
                  key_replace=None, key_replace_type='last_read', timeout=20, interval=5,
-                 read_until_time=1) -> str or List[str]:
+                 read_until_time=1, **kwargs) -> str or List[str]:
         """根据表达式获取最后一次执行命令的匹配值
 
         :param command: 发送命令，可以是一条或多条
         :param regular: 正则表达式，对执行的最后一次命令返回内容进行正则查询，必须要查询到，
                         如果查不到，直至查询超时并报错
                         如果查到不止一个，返回每个正则表达式的第一个
                         列子：硬件地址 r'HWaddr(.*)inet6'， '(([0-9a-fA-F]{2}[:]){5}([0-9a-fA-F]{2})|([0-9a-fA-F]{2}[-]){5}([0-9a-fA-F]{2}))'
@@ -612,18 +612,22 @@
         :param key_replace_type: 'cli'|'last_read'|'cli_last_read'，仅在key_replace 有值时生效，默认last_read
                                  'cli': 仅替换发出去的命令
                                  'last_read': 仅替换最后读取到的内容
                                  'cli_last_read': 既要替换cli 也要替换最后读取到的内容
         :param timeout: 超时时间 s
         :param interval: 检测间隔时间 s
         :param read_until_time: 每次读取的间隔时间 s
-        :return: str or list ，根据正则表达式的个数返回值
+        :param kwargs
+                    match_result_model:  only_one | all   每个正则表达式匹配的结果返回值， 默认only_one
+        :return: match_result_model='only_one'  返回str or List[str] ，根据正则表达式的个数返回值
+                 match_result_model='all'  返回List[str] or List[List] ，根据正则表达式的个数返回值
         """
         key_replace = {'\r\n': '', ' ': ''} if key_replace is None else key_replace
         key_replace_type = 'last_read' if key_replace_type is None else key_replace_type
+        match_result_model = kwargs.get('match_result_model', 'only_one')
         result = self.send_cli(command, type_=type_, key_replace=key_replace, key_replace_type=key_replace_type,
                                read_until_time=read_until_time)
         if isinstance(regular, str):
             re_list = re.findall(regular, result)
             if re_list:
                 for i in re_list:
                     if isinstance(i, str):
@@ -635,18 +639,24 @@
                 return False
         elif isinstance(regular, list):
             result_ = []
             for regular_ in regular:
                 re_list = re.findall(regular_, result)
                 if re_list:
                     for i in re_list:
-                        if isinstance(i, str):
-                            result_.append(re.findall(regular_, result)[0])
+                        if match_result_model == 'only_one':
+                            if isinstance(i, str):
+                                result_.append(re.findall(regular_, result)[0])
+                            else:
+                                result_.append(re.findall(regular_, result)[0][0])
                         else:
-                            result_.append(re.findall(regular_, result)[0][0])
+                            if isinstance(i, str):
+                                result_.append(re.findall(regular_, result))
+                            else:
+                                result_.append(re.findall(regular_, result)[0])
                 else:
                     logging.debug(f'regular {regular_} match content None')
                     return False
             else:
                 return result_
 
     # intools 实现获取信息更改信息
```

### Comparing `inhandtest-0.0.85/inhandtest/telnet.yaml` & `inhandtest-0.0.86/inhandtest/telnet.yaml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/tftp_server.py` & `inhandtest-0.0.86/inhandtest/tftp_server.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.85/inhandtest/tools.py` & `inhandtest-0.0.86/inhandtest/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,30 +631,30 @@
     """
 
     def report_expired(file_name: str) -> bool:
         expired = False
         try:
             if report_file_start_with in file_name and file_name != report_file_start_with:
                 report_time = file_name.replace(report_file_start_with + '_', '')
-                report_time = datetime.datetime.strptime(report_time, '%Y-%m-%d-%H')
+                report_time = datetime.datetime.strptime(report_time, '%Y-%m-%d-%H-%M')
                 if (datetime.datetime.now() - report_time).days >= days:
                     expired = True
         except Exception:
             pass
         finally:
             return expired
 
     if os.path.isdir(file_path):
         for i in os.listdir(file_path):
             if report_expired(i):
                 import shutil
                 shutil.rmtree(os.path.join(file_path, i))
                 logging.debug(f'{i} has expired days {days}, auto remove')
 
-    return '_'.join([report_file_start_with, get_time_stamp(delta=+8, time_format='%Y-%m-%d-%H')])
+    return '_'.join([report_file_start_with, get_time_stamp(delta=+8, time_format='%Y-%m-%d-%H-%M')])
 
 
 def stop_thread(thread):
     """某些线程会在后台一直运行，当在外界满足一定条件时，是可以停掉的
 
     :param thread: 定义的线程
     :return:
@@ -861,17 +861,18 @@
         self[key] = value
 
 
 if __name__ == '__main__':
     from inhandtest.log import enable_log
     from inhandtest.file import read_csv_file, file_to_csv
     enable_log(console_level='debug')
-    result = read_csv_file('./iccid.csv', has_header=False)[0]
-    result = ["'" + iccid for iccid in result]
-    file_to_csv({"iccid": result}, './iccid1.csv')
+    # result = read_csv_file('./iccid.csv', has_header=False)[0]
+    # result = ["'" + iccid for iccid in result]
+    # file_to_csv({"iccid": result}, './iccid1.csv')
+    print(pytest_report_save(file_path='G:/ER805_AUTO/Report',days=7))
     # print(calculate_iccid_checksum('89860619110020726049'))
     # print(len('89860619110020718731'))
     # pc_ping('1.2.3.4', lost_packets=True, assert_result=True, timeout=10, interval=5)
     # a = {"key": {"value": 1, "value2": 2}}
     # s = update_dict_by_path(a, 'key/value', 3)
     # print(a)
     # print(s)
```

### Comparing `inhandtest-0.0.85/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.86/inhandtest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inhandtest
-Version: 0.0.85
+Version: 0.0.86
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `inhandtest-0.0.85/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.86/inhandtest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 requirements.txt
 setup.py
 inhandtest/__init__.py
 inhandtest/er_events.yaml
 inhandtest/exception.py
 inhandtest/file.py
+inhandtest/inconfig.py
 inhandtest/inexpect.py
 inhandtest/inmodbus.py
 inhandtest/inmongodb.py
 inhandtest/inmqtt.py
 inhandtest/inserial.py
 inhandtest/insocket.py
 inhandtest/inssh.py
```

### Comparing `inhandtest-0.0.85/setup.py` & `inhandtest-0.0.86/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # 读取requirements 文件中的库，并生成一个列表
 require_list = open('requirements.txt', 'r', encoding='utf-8').readlines()
 require_list = [i.strip() for i in require_list]
 
 setup(
     name='inhandtest',
-    version='0.0.85',
+    version='0.0.86',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

