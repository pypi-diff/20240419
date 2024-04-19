# Comparing `tmp/biotech-1.0.3.tar.gz` & `tmp/biotech-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotech-1.0.3.tar", max compression
+gzip compressed data, was "biotech-1.1.0.tar", max compression
```

## Comparing `biotech-1.0.3.tar` & `biotech-1.1.0.tar`

### file list

```diff
@@ -1,709 +1,785 @@
--rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.0.3/license.S.HTML
--rwxr-xr-x   0        0        0     1147 2024-04-16 20:54:31.597863 biotech-1.0.3/pyproject.toml
--rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.0.3/readme.md
--rwxr-xr-x   0        0        0     2106 2024-04-16 20:48:35.047380 biotech-1.0.3/venue.S.HTML
--rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.0.3/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
--rwxr-xr-x   0        0        0      845 2024-04-15 23:43:38.033889 biotech-1.0.3/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.0.3/venues/stages/biotech/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.0.3/venues/stages/biotech/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.0.3/venues/stages/biotech/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.0.3/venues/stages/biotech/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.0.3/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.0.3/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.0.3/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.0.3/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0        0 2024-04-11 23:18:49.717845 biotech-1.0.3/venues/stages/biotech/__bin/biotech_1
--rwxr-xr-x   0        0        0       78 2024-04-16 20:48:34.595388 biotech-1.0.3/venues/stages/biotech/__init__.py
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.0.3/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.0.3/venues/stages/biotech/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.0.3/venues/stages/biotech/_book/book.s.HTML
--rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.0.3/venues/stages/biotech/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2099 2024-04-16 20:48:34.547389 biotech-1.0.3/venues/stages/biotech/_clique/__init__.py
--rw-r--r--   0        0        0     2543 2024-04-16 20:49:26.966517 biotech-1.0.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.0.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.0.3/venues/stages/biotech/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.0.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.0.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0   653990 2024-04-16 20:50:06.189880 biotech-1.0.3/venues/stages/biotech/_status/DB/records.json
--rw-r--r--   0        0        0     1158 2024-04-16 20:49:27.238512 biotech-1.0.3/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.0.3/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.0.3/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1466 2024-04-16 20:48:34.915382 biotech-1.0.3/venues/stages/biotech/_status/establish.py
--rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416143 biotech-1.0.3/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.0.3/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.0.3/venues/stages/biotech/_status/monitors/-1_start/status_1.py
--rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.0.3/venues/stages/biotech/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.0.3/venues/stages/biotech/_status/monitors/0_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.0.3/venues/stages/biotech/_status/monitors/0_start/status_1.py
--rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708149 biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.0.3/venues/stages/biotech/_status/monitors/1/status_1.py
--rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.0.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.0.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.0.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.0.3/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1045 2024-04-16 20:48:34.915382 biotech-1.0.3/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
--rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.0.3/venues/stages/biotech/_status/monitors/2/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.0.3/venues/stages/biotech/_status/monitors/2/stasis/2_health.py
--rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.0.3/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.0.3/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.0.3/venues/stages/biotech/_status/monitors/2/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.0.3/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.0.3/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.0.3/venues/stages/biotech/_status/monitors/2/status_1.py
--rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.0.3/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py
--rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.0.3/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.0.3/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.0.3/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.0.3/venues/stages/biotech/_status/monitors/4_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.0.3/venues/stages/biotech/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.0.3/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/stasis/3_health.py
--rwxr-xr-x   0        0        0      150 2023-10-13 03:39:00.591139 biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      547 2023-10-13 03:39:26.199864 biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1032 2024-04-13 23:09:41.284112 biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      179 2024-04-13 23:09:41.284112 biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      165 2024-04-13 23:09:41.284112 biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      900 2024-04-16 20:48:34.895383 biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/status_1.py
--rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.0.3/venues/stages/biotech/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.0.3/venues/stages/biotech/_status/monitors/7/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.0.3/venues/stages/biotech/_status/monitors/7/status_1.py
--rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.0.3/venues/stages/biotech/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.0.3/venues/stages/biotech/_status/monitors/8_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1471 2024-04-16 20:48:34.907383 biotech-1.0.3/venues/stages/biotech/_status/monitors/8_DB/status_1.py
--rwxr-xr-x   0        0        0    65524 2024-04-16 20:49:58.426005 biotech-1.0.3/venues/stages/biotech/_status/monitors/8_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.0.3/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.0.3/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.0.3/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.0.3/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.0.3/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.0.3/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1039 2024-04-16 20:48:34.879383 biotech-1.0.3/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/status_1.py
--rwxr-xr-x   0        0        0      919 2024-04-16 20:48:34.955382 biotech-1.0.3/venues/stages/biotech/_status/status.proc.py
--rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.0.3/venues/stages/biotech/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.0.3/venues/stages/biotech/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.0.3/venues/stages/biotech/architecture.s.HTML
--rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.0.3/venues/stages/biotech/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.0.3/venues/stages/biotech/license.S.HTML
--rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.0.3/venues/stages/biotech/module.s.HTML
--rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.0.3/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
--rw-r--r--   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.0.3/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      479 2024-04-16 20:49:28.130498 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rw-r--r--   0        0        0     1861 2024-04-16 20:49:28.130498 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      347 2024-04-16 20:48:34.555389 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2121 2024-04-16 20:48:34.555389 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     1584 2024-04-16 20:48:34.555389 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      537 2024-04-16 04:35:00.446216 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      976 2024-04-16 04:43:10.970009 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      570 2024-04-16 04:32:47.783248 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__coms/done_with_scan.py
--rwxr-xr-x   0        0        0      834 2024-04-16 04:42:59.962108 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__coms/send_patch.py
--rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     2004 2024-04-16 04:42:27.398399 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py
--rwxr-xr-x   0        0        0     1970 2024-04-16 04:42:32.314355 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__keg/__init__.py
--rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      542 2024-04-14 03:40:33.432138 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__mixes/format_rel_path.py
--rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
--rw-r--r--   0        0        0     1466 2024-04-16 20:49:27.010516 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      626 2024-04-15 21:44:04.889606 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc
--rwxr-xr-x   0        0        0       77 2024-04-16 00:57:52.151598 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/implicit_procedure.S.HTML
--rwxr-xr-x   0        0        0     1447 2024-04-16 20:48:34.575388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/on.py
--rwxr-xr-x   0        0        0      359 2024-04-15 21:41:08.268047 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/paths.py
--rwxr-xr-x   0        0        0      554 2024-04-14 01:25:11.648020 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/clique/__init__.py
--rwxr-xr-x   0        0        0     1147 2024-04-15 21:44:21.713379 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      351 2024-04-16 20:48:34.567388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/implicit_procedure.process.py
--rwxr-xr-x   0        0        0      783 2024-04-16 00:52:47.863029 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/keg/__init__.py
--rwxr-xr-x   0        0        0     1223 2024-04-16 00:52:52.470976 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      903 2024-04-16 20:49:28.070499 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2349 2024-04-16 20:49:28.126498 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      515 2024-04-16 20:48:34.563388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py
--rwxr-xr-x   0        0        0     3005 2024-04-16 20:48:34.563388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/keg/spaces/paths_patch.py
--rw-r--r--   0        0        0     1714 2024-04-16 20:49:28.126498 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0     1217 2024-04-16 20:49:28.126498 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rwxr-xr-x   0        0        0      395 2024-04-15 23:17:17.483301 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
--rw-r--r--   0        0        0     2531 2024-04-16 20:49:28.130498 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
--rwxr-xr-x   0        0        0      630 2024-04-15 20:31:31.342880 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rw-r--r--   0        0        0      845 2024-04-16 20:49:28.130498 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
--rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
--rwxr-xr-x   0        0        0     2942 2024-04-16 20:48:34.571388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     1673 2024-04-16 20:48:34.567388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/done_with_scan.py
--rwxr-xr-x   0        0        0      182 2024-04-15 23:17:12.503322 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/format_path.py
--rwxr-xr-x   0        0        0     3792 2024-04-16 20:48:34.567388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py
--rwxr-xr-x   0        0        0      384 2024-04-15 20:28:52.255899 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/send_done.py
--rwxr-xr-x   0        0        0     1072 2024-04-16 20:48:34.571388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/stop_process.py
--rwxr-xr-x   0        0        0     1215 2024-04-16 20:48:34.571388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/venture_finish.py
--rwxr-xr-x   0        0        0     1208 2024-04-16 20:48:34.567388 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     1055 2024-04-16 20:49:28.126498 biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     6649 2024-04-16 20:48:34.559388 biotech-1.0.3/venues/stages/biotech/procedures/intro/__init__.py
--rw-r--r--   0        0        0     3169 2024-04-16 20:49:26.998516 biotech-1.0.3/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1199 2024-04-16 20:49:27.098514 biotech-1.0.3/venues/stages/biotech/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      920 2024-04-16 20:49:27.238512 biotech-1.0.3/venues/stages/biotech/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      872 2024-04-16 20:48:34.559388 biotech-1.0.3/venues/stages/biotech/procedures/intro/coms/implicit_procedure/on.py
--rwxr-xr-x   0        0        0      634 2024-04-16 20:48:34.559388 biotech-1.0.3/venues/stages/biotech/procedures/intro/coms/implicit_procedure/send_paths.py
--rwxr-xr-x   0        0        0     1541 2024-04-15 20:59:54.302740 biotech-1.0.3/venues/stages/biotech/procedures/intro/keg/__init__.py
--rwxr-xr-x   0        0        0     1396 2024-04-16 20:48:34.559388 biotech-1.0.3/venues/stages/biotech/procedures/intro/keg/__init__v1.py
--rwxr-xr-x   0        0        0     2587 2024-04-15 20:59:57.206699 biotech-1.0.3/venues/stages/biotech/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1447 2024-04-16 20:48:34.559388 biotech-1.0.3/venues/stages/biotech/procedures/intro/keg/quart__init__.py
--rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.0.3/venues/stages/biotech/procedures/processes.S.HTML
--rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.0.3/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.0.3/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.0.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.0.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.0.3/venues/stages/biotech/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.0.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.0.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.0.3/venues/stages/biotech/topics/alarm_parser/__init__.py
--rw-r--r--   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.0.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.0.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.0.3/venues/stages/biotech/topics/exceptions.py
--rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.0.3/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2024-04-15 19:19:22.749400 biotech-1.0.3/venues/stages/biotech/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1154 2024-04-16 20:48:34.579388 biotech-1.0.3/venues/stages/biotech/topics/implicit/thread/__init__.py
--rw-r--r--   0        0        0      855 2024-04-16 20:49:28.130498 biotech-1.0.3/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.0.3/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.0.3/venues/stages/biotech/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.0.3/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1879 2024-04-16 20:48:34.579388 biotech-1.0.3/venues/stages/biotech/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1842 2024-04-16 20:49:27.062515 biotech-1.0.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.0.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     1483 2024-04-16 20:49:27.078515 biotech-1.0.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0     1461 2024-04-16 20:48:34.579388 biotech-1.0.3/venues/stages/biotech/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0       75 2024-04-13 23:45:41.546277 biotech-1.0.3/venues/stages/biotech/topics/process_on/process_on.S.HTML
--rwxr-xr-x   0        0        0     1442 2024-04-16 20:48:34.591388 biotech-1.0.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
--rw-r--r--   0        0        0     1464 2024-04-16 20:49:28.126498 biotech-1.0.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.0.3/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
--rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.0.3/venues/stages/biotech/topics/start--/one.py
--rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.0.3/venues/stages/biotech/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.0.3/venues/stages/biotech/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.0.3/venues/stages/biotech/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.0.3/venues/stages/biotech/variables/__init__.py
--rw-r--r--   0        0        0     5155 1970-01-01 00:00:00.000000 biotech-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 biotech-1.1.0/license.S.HTML
+-rwxr-xr-x   0        0        0     1145 2024-04-19 20:06:30.613524 biotech-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0     3866 2024-04-16 20:53:30.034757 biotech-1.1.0/readme.md
+-rwxr-xr-x   0        0        0     2331 2024-04-19 15:34:34.407444 biotech-1.1.0/venue.S.HTML
+-rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 biotech-1.1.0/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rwxr-xr-x   0        0        0     1270 2024-04-17 22:22:59.944800 biotech-1.1.0/venues/stages/biotech/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4079 2024-04-16 20:48:34.871383 biotech-1.1.0/venues/stages/biotech/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      645 2024-04-16 20:48:34.875383 biotech-1.1.0/venues/stages/biotech/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0      385 2024-04-17 18:49:44.656786 biotech-1.1.0/venues/stages/biotech/__glossary/biotech_1
+-rwxr-xr-x   0        0        0      114 2024-04-17 18:45:06.744254 biotech-1.1.0/venues/stages/biotech/__glossary/glossary.S.HTML
+-rwxr-xr-x   0        0        0      130 2024-04-19 16:49:02.311131 biotech-1.1.0/venues/stages/biotech/__init__.py
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 biotech-1.1.0/venues/stages/biotech/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1252 2024-04-16 20:48:34.867383 biotech-1.1.0/venues/stages/biotech/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1786 2024-04-16 20:48:34.867383 biotech-1.1.0/venues/stages/biotech/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      542 2024-04-16 20:48:34.867383 biotech-1.1.0/venues/stages/biotech/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2129 2024-04-17 19:24:51.191926 biotech-1.1.0/venues/stages/biotech/_clique/__init__.py
+-rwxr-xr-x   0        0        0     2493 2024-04-17 19:24:52.839918 biotech-1.1.0/venues/stages/biotech/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 biotech-1.1.0/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 biotech-1.1.0/venues/stages/biotech/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 biotech-1.1.0/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 biotech-1.1.0/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0  1328100 2024-04-19 20:05:41.074199 biotech-1.1.0/venues/stages/biotech/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1156 2024-04-19 17:06:33.102985 biotech-1.1.0/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 biotech-1.1.0/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 biotech-1.1.0/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1463 2024-04-19 17:05:25.115746 biotech-1.1.0/venues/stages/biotech/_status/establish.py
+-rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416142 biotech-1.1.0/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 biotech-1.1.0/venues/stages/biotech/_status/monitors/-1_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      720 2024-04-16 20:48:34.887383 biotech-1.1.0/venues/stages/biotech/_status/monitors/-1_start/status_1.py
+-rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 biotech-1.1.0/venues/stages/biotech/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 biotech-1.1.0/venues/stages/biotech/_status/monitors/0_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      793 2024-04-16 20:48:34.883383 biotech-1.1.0/venues/stages/biotech/_status/monitors/0_start/status_1.py
+-rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708148 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1161 2024-04-16 20:48:34.903383 biotech-1.1.0/venues/stages/biotech/_status/monitors/1/status_1.py
+-rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1147 2024-04-19 19:06:56.036882 biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py
+-rw-r--r--   0        0        0      316 2024-04-19 18:57:32.516036 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       77 2024-04-19 18:57:24.196146 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1208 2024-04-19 17:04:46.812176 biotech-1.1.0/venues/stages/biotech/_status/monitors/11/status_1.py
+-rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/2_health.py
+-rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1214 2024-04-16 20:48:34.899383 biotech-1.1.0/venues/stages/biotech/_status/monitors/2/status_1.py
+-rwxr-xr-x   0        0        0      794 2024-04-16 20:48:34.891383 biotech-1.1.0/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py
+-rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      942 2024-04-16 20:48:34.883383 biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 biotech-1.1.0/venues/stages/biotech/_status/monitors/4_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 biotech-1.1.0/venues/stages/biotech/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      939 2024-04-16 20:48:34.887383 biotech-1.1.0/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      867 2024-04-16 20:48:34.891383 biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/3_health.py
+-rw-r--r--   0        0        0     1036 2024-04-19 19:54:47.501752 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
+-rw-r--r--   0        0        0      183 2024-04-19 19:54:47.501752 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
+-rw-r--r--   0        0        0      169 2024-04-19 19:54:47.505751 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      926 2024-04-19 19:53:38.302512 biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/status_1.py
+-rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 biotech-1.1.0/venues/stages/biotech/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 biotech-1.1.0/venues/stages/biotech/_status/monitors/7/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      809 2024-04-16 20:48:34.907383 biotech-1.1.0/venues/stages/biotech/_status/monitors/7/status_1.py
+-rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1561 2024-04-19 19:13:07.956368 biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/status_1.py
+-rwxr-xr-x   0        0        0    82190 2024-04-19 20:05:31.254334 biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1402 2024-04-19 19:21:30.822364 biotech-1.1.0/venues/stages/biotech/_status/monitors/9_aggregation_format_and_exit/status_1.py
+-rwxr-xr-x   0        0        0      984 2024-04-18 03:32:30.971629 biotech-1.1.0/venues/stages/biotech/_status/status.proc.py
+-rwxr-xr-x   0        0        0      256 2024-04-16 20:48:34.875383 biotech-1.1.0/venues/stages/biotech/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1483 2024-04-16 20:48:34.851384 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 biotech-1.1.0/venues/stages/biotech/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1779 2024-04-16 20:48:34.575388 biotech-1.1.0/venues/stages/biotech/architecture.s.HTML
+-rwxr-xr-x   0        0        0      241 2024-04-16 20:53:18.546926 biotech-1.1.0/venues/stages/biotech/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 biotech-1.1.0/venues/stages/biotech/license.S.HTML
+-rwxr-xr-x   0        0        0     3068 2024-04-16 20:48:34.543389 biotech-1.1.0/venues/stages/biotech/module.s.HTML
+-rwxr-xr-x   0        0        0     1615 2024-04-19 16:31:12.412493 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      640 2024-04-19 16:26:52.595637 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/__pycache__/paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      259 2024-04-19 16:20:24.028904 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/aggregator.S.HTML
+-rwxr-xr-x   0        0        0     1461 2024-04-19 16:31:10.152519 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.648116 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/paths.py
+-rwxr-xr-x   0        0        0      366 2024-04-19 16:26:14.660116 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/aggregator_procedure.process.py
+-rwxr-xr-x   0        0        0      562 2024-04-17 21:48:05.111704 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py
+-rwxr-xr-x   0        0        0     1163 2024-04-17 21:49:49.362841 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1734 2024-04-19 16:26:14.672115 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__init__.py
+-rwxr-xr-x   0        0        0     2173 2024-04-19 16:27:13.567375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      965 2024-04-19 16:27:13.567375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2744 2024-04-19 19:39:17.347586 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1137 2024-04-19 16:27:13.567375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      643 2024-04-19 16:26:14.684115 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/done_with_scan.py
+-rwxr-xr-x   0        0        0     3672 2024-04-19 19:29:49.876463 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/paths_patch.py
+-rwxr-xr-x   0        0        0      789 2024-04-19 16:26:14.712115 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/the_health_scan_started.py
+-rwxr-xr-x   0        0        0     2031 2024-04-19 16:27:13.563375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0     1743 2024-04-19 18:03:45.582807 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      418 2024-04-17 20:03:55.692458 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3455 2024-04-17 21:41:59.150872 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
+-rwxr-xr-x   0        0        0      746 2024-04-17 23:09:52.928659 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0      849 2024-04-17 20:12:15.035804 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
+-rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3451 2024-04-19 16:26:14.724115 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     2705 2024-04-19 18:03:38.578879 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py
+-rwxr-xr-x   0        0        0      193 2024-04-17 20:02:37.661229 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/format_path.py
+-rwxr-xr-x   0        0        0      566 2024-04-17 23:09:07.804988 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/send_done.py
+-rwxr-xr-x   0        0        0     1834 2024-04-19 18:55:07.129933 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-19 18:55:11.397883 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      799 2024-04-19 16:27:13.563375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/send_done_if_finished.cpython-310.pyc
+-rw-r--r--   0        0        0     4038 2024-04-19 19:39:17.347586 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/__pycache__/the_physical.cpython-310.pyc
+-rwxr-xr-x   0        0        0      754 2024-04-18 00:33:41.120405 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/monitor.S.HTML
+-rw-r--r--   0        0        0     1826 2024-04-19 18:56:22.468973 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-19 18:56:27.160910 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/records/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      996 2024-04-19 16:26:14.764114 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py
+-rwxr-xr-x   0        0        0     8610 2024-04-19 19:38:19.764145 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/the_physical.py
+-rwxr-xr-x   0        0        0     1223 2024-04-19 16:26:14.792114 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/venture_finish--.py
+-rwxr-xr-x   0        0        0     2910 2024-04-19 16:26:14.804114 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__init__.py
+-rwxr-xr-x   0        0        0     1684 2024-04-19 16:27:13.563375 biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      834 2024-04-16 20:48:34.547389 biotech-1.1.0/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py
+-rwxr-xr-x   0        0        0      951 2024-04-16 20:49:56.266040 biotech-1.1.0/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      479 2024-04-16 20:49:28.130498 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1838 2024-04-19 16:27:13.567375 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      347 2024-04-16 20:48:34.555389 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2105 2024-04-19 16:26:14.612116 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     2201 2024-04-18 02:31:19.570492 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1441 2024-04-18 02:04:22.961501 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__harbor/__init__.py
+-rwxr-xr-x   0        0        0      774 2024-04-16 20:48:34.555389 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py
+-rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      309 2024-04-17 23:41:26.722721 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      562 2024-04-17 23:41:26.734721 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      525 2024-04-17 23:09:55.764639 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2024-04-19 20:05:11.362609 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      636 2024-04-18 01:15:59.039315 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/the_health_scan_started.cpython-310.pyc
+-rwxr-xr-x   0        0        0      289 2024-04-17 23:05:28.138584 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      803 2024-04-19 20:05:09.858629 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/send_patch.py
+-rwxr-xr-x   0        0        0      378 2024-04-18 01:13:51.928249 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/the_health_scan_started.py
+-rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/format_rel_path.py
+-rwxr-xr-x   0        0        0     2182 2024-04-18 01:57:52.896535 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py
+-rwxr-xr-x   0        0        0     2125 2024-04-18 01:58:34.052216 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1027 2024-04-17 23:41:26.738721 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1368 2024-04-17 23:38:58.631806 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/show/variable.py
+-rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules_pip.UTF8
+-rwxr-xr-x   0        0        0      152 2024-04-19 16:48:50.419277 biotech-1.1.0/venues/stages/biotech/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3443 2024-04-19 20:02:47.664429 biotech-1.1.0/venues/stages/biotech/procedures/intro/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.0/venues/stages/biotech/procedures/intro/intro.S.HTML
+-rwxr-xr-x   0        0        0     5074 2024-04-19 20:02:38.772528 biotech-1.1.0/venues/stages/biotech/procedures/intro/on.py
+-rw-r--r--   0        0        0     2887 2024-04-19 19:04:05.278996 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/__pycache__/adventure.cpython-310.pyc
+-rw-r--r--   0        0        0     3989 2024-04-19 19:03:05.467745 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/adventure.py
+-rwxr-xr-x   0        0        0     1267 2024-04-19 16:26:52.599637 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      905 2024-04-19 16:56:52.013564 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      901 2024-04-19 16:26:14.840113 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      614 2024-04-19 16:56:41.273688 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      138 2024-04-19 17:33:23.717242 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/intro.proc.py
+-rwxr-xr-x   0        0        0     3047 2024-04-19 19:04:01.875038 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/keg/__init__.py
+-rw-r--r--   0        0        0     3044 2024-04-19 19:04:05.278996 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/variables/__init__.py
+-rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321766 biotech-1.1.0/venues/stages/biotech/procedures/intro/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       33 2024-04-17 22:47:27.362384 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/__init__.py
+-rwxr-xr-x   0        0        0      192 2024-04-17 22:47:29.166371 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1930 2024-04-19 16:45:15.609992 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3212 2024-04-19 16:26:52.583637 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/_ops/__pycache__/start.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4487 2024-04-19 16:26:14.828113 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/_ops/start.py
+-rwxr-xr-x   0        0        0     1267 2024-04-19 16:26:52.599637 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      855 2024-04-19 16:26:52.631636 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      901 2024-04-19 16:26:14.840113 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/on.py
+-rwxr-xr-x   0        0        0      572 2024-04-19 16:26:14.856113 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/send_paths.py
+-rwxr-xr-x   0        0        0      374 2024-04-18 06:14:11.069403 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/intro.S.HTML
+-rwxr-xr-x   0        0        0     1991 2024-04-18 03:48:25.192521 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__init__.py
+-rwxr-xr-x   0        0        0     1394 2024-04-18 06:18:52.492292 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__init__v1.py
+-rwxr-xr-x   0        0        0     2895 2024-04-18 05:23:09.408255 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1447 2024-04-16 20:48:34.559388 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/quart__init__.py
+-rwxr-xr-x   0        0        0     2039 2024-04-19 16:45:13.398021 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/on.py
+-rwxr-xr-x   0        0        0     4069 2024-04-19 16:41:30.225039 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/intro.proc.py
+-rwxr-xr-x   0        0        0     2819 2024-04-19 16:40:32.337866 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/keg/__init__.py
+-rwxr-xr-x   0        0        0     3015 2024-04-19 16:40:36.437807 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3062 2024-04-19 16:26:53.431626 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/moves/__pycache__/adventure.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4716 2024-04-19 16:26:14.896113 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/moves/adventure.py
+-rwxr-xr-x   0        0        0       89 2024-04-18 06:36:12.314122 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/variables/__init__.py
+-rwxr-xr-x   0        0        0      245 2024-04-18 06:37:06.321765 biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      172 2024-04-16 20:48:34.551389 biotech-1.1.0/venues/stages/biotech/procedures/procedures.S.HTML
+-rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 biotech-1.1.0/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 biotech-1.1.0/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 biotech-1.1.0/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 biotech-1.1.0/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 biotech-1.1.0/venues/stages/biotech/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 biotech-1.1.0/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 biotech-1.1.0/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      708 2024-04-16 20:48:34.591388 biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__init__.py
+-rwxr-xr-x   0        0        0      673 2024-04-16 20:49:28.126498 biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      405 2024-04-16 20:48:34.579388 biotech-1.1.0/venues/stages/biotech/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1190 2024-01-27 05:31:08.525189 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/$ company/company.s.HTML
+-rwxr-xr-x   0        0        0     2446 2024-04-17 19:24:25.140060 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__init__.py
+-rwxr-xr-x   0        0        0     2491 2024-04-17 19:24:52.839918 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4471 2024-02-01 06:11:56.801715 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1050 2024-04-16 06:10:03.111579 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1920 2024-01-31 18:50:23.812071 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/__pycache__/_clique.cpython-311.pyc
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:56.558087 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 1.s.HTML
+-rwxr-xr-x   0        0        0       24 2024-01-26 17:38:52.854129 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/_status/1/shares/shares 2.s.HTML
+-rwxr-xr-x   0        0        0      751 2024-04-17 19:16:04.226583 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/_status/1/ztatus_1.py
+-rwxr-xr-x   0        0        0     1981 2024-04-17 19:25:47.591625 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__init__.py
+-rwxr-xr-x   0        0        0     2283 2024-04-17 19:25:53.011595 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4019 2024-01-31 18:51:47.652157 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3843 2024-04-17 19:25:53.099595 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4426 2024-01-27 06:34:32.979965 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/__pycache__/treasury.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3559 2024-04-17 19:25:22.227762 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/basin/treasury.py
+-rwxr-xr-x   0        0        0     1727 2024-04-17 19:15:19.882965 biotech-1.1.0/venues/stages/biotech/topics/help_documentation/shares.s.HTML
+-rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 biotech-1.1.0/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1558 2024-04-18 05:22:02.832642 biotech-1.1.0/venues/stages/biotech/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1155 2024-04-18 05:46:33.436738 biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/__init__.py
+-rwxr-xr-x   0        0        0      855 2024-04-18 06:05:23.346518 biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0       90 2024-04-17 22:51:08.968798 biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/thread.S.HTML
+-rwxr-xr-x   0        0        0      598 2024-04-17 22:33:48.860256 biotech-1.1.0/venues/stages/biotech/topics/printout/__pycache__/bracket.cpython-310.pyc
+-rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 biotech-1.1.0/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      470 2024-04-17 23:02:14.419990 biotech-1.1.0/venues/stages/biotech/topics/printout/bracket.py
+-rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 biotech-1.1.0/venues/stages/biotech/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 biotech-1.1.0/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2163 2024-04-19 18:50:11.157390 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1997 2024-04-19 18:52:58.595432 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     1818 2024-04-19 18:54:33.250328 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0      919 2024-04-18 01:45:27.254200 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/parse_records.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1766 2024-04-19 18:53:11.523281 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0      320 2024-04-18 01:48:34.504806 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/p_expect.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-04-18 01:45:24.082223 biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/parse_records.py
+-rwxr-xr-x   0        0        0      195 2024-04-16 22:50:54.515336 biotech-1.1.0/venues/stages/biotech/topics/process_on/process_on.S.HTML
+-rwxr-xr-x   0        0        0     1470 2024-04-18 04:12:56.845888 biotech-1.1.0/venues/stages/biotech/topics/quay/garage.py
+-rwxr-xr-x   0        0        0     2546 2024-04-18 04:38:41.478278 biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_1.py
+-rwxr-xr-x   0        0        0     1612 2024-04-18 04:54:58.414971 biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_2.py
+-rwxr-xr-x   0        0        0      551 2024-04-18 05:20:40.701113 biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_3.py
+-rwxr-xr-x   0        0        0     1083 2024-04-18 05:19:11.645613 biotech-1.1.0/venues/stages/biotech/topics/quay/implicit_process_test_4.py
+-rwxr-xr-x   0        0        0     1442 2024-04-16 20:48:34.591388 biotech-1.1.0/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py
+-rwxr-xr-x   0        0        0     1464 2024-04-16 20:49:28.126498 biotech-1.1.0/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 biotech-1.1.0/venues/stages/biotech/topics/queues/unlimited_capacity/__init__.py
+-rw-r--r--   0        0        0     1776 2024-04-19 19:50:41.332444 biotech-1.1.0/venues/stages/biotech/topics/show/__pycache__/variable.cpython-310.pyc
+-rwxr-xr-x   0        0        0      461 2024-04-17 23:59:06.614967 biotech-1.1.0/venues/stages/biotech/topics/show/show.S.HTML
+-rwxr-xr-x   0        0        0     2305 2024-04-19 19:50:39.412465 biotech-1.1.0/venues/stages/biotech/topics/show/variable.py
+-rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      273 2024-04-16 20:48:34.583388 biotech-1.1.0/venues/stages/biotech/topics/start--/one.py
+-rwxr-xr-x   0        0        0      406 2024-04-16 20:48:34.587388 biotech-1.1.0/venues/stages/biotech/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      532 2024-04-16 20:48:34.587388 biotech-1.1.0/venues/stages/biotech/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 biotech-1.1.0/venues/stages/biotech/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 biotech-1.1.0/venues/stages/biotech/variables/__init__.py
+-rw-r--r--   0        0        0     5153 1970-01-01 00:00:00.000000 biotech-1.1.0/PKG-INFO
```

### Comparing `biotech-1.0.3/pyproject.toml` & `biotech-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "biotech"
-version = "1.0.3"
+version = "1.1.0"
 description = "A health monitoring stack"
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "biotech", from = "venues/stages" }
 ]
@@ -54,25 +54,25 @@
 
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 body-scan = "^1.1.1"
 botanist = "^1.0.0"
-shares = "^3.1.9"
 click = "^8.1.7"
 coverage = "^7.4.4"
 flask = "^3.0.3"
 pexpect = "^4.9.0"
 redis = "^5.0.3"
 requests = "^2.31.0"
 tinydb = "^4.8.0"
 rich = "^13.7.1"
 sanic = "^23.12.1"
 pymongo = "^4.6.3"
+mako = "^1.3.3"
 
 
 [tool.poetry.scripts]
 biotech = 'biotech:clique'
 
 [tool.poetry.urls]
 GitLab = "https://gitlab.com/status600/climates/biotech"
```

### Comparing `biotech-1.0.3/readme.md` & `biotech-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venue.S.HTML` & `biotech-1.1.0/venue.S.HTML`

 * *Files 18% similar despite different names*

```diff
@@ -5,48 +5,64 @@
 
 	<h1>biotech</h1>
 		# neurons
 	
 	<h2>docker</h2>
 		docker network create --subnet=192.168.0.0/24 container_network
 		docker run --network container_network --ip 192.168.0.102 -v .:/biotech -it jumps:v2.1.0
-		docker exec -it 389597d6510a bash
+		docker exec -it a6599081a9fb bash 
 
-	<h2>link the readme</h2>
-		ln -s venues/stages/biotech/room.md readme.MD
+	<h2>install</h2>
+		#
+		#	⚠️ ⚠️ ⚠️ ⚠️
+		#
+		#		Make sure that none of the stages that "biotech"
+		#		utilizes rely on "biotech".
+		#
+		#		For the sake of sanity, please keep the "reliability, testing, etc."
+		#		structure as a "tree, hierarchy, etc." etc. with no coodependencies.
+		#
+	
+		python3 moves/install.py
+		
+		<h3>remove</h3>
+			python3 moves/stage_remove.py
+			
+		<h3>add</h3>
+			python3 moves/stage_add.py
+		
+		<h3>upgrade</h3>
+			# poetry update sanic
+		
+	<h2>source</h2>
+		source source.sh
+
+	<h2>git</h2>
+		git push --set-upstream git@gitlab.com:status600/climates/biotech.git performance
+	
 
 	<h2>poetry</h2>
 		pip install poetry poetry-plugin-export
 	
 		<h3>add</h3>
-			#
-			#	⚠️
-			#		Make sure that none of these depend on this module!
-			#
-			#		For the sake of sanity, please keep the "reliability, testing, etc."
-			#		structure as a "tree, hierarchy, etc." etc. with no coodependencies
-			#		that almost definitely cause chaos.
-			#
-						
-			poetry add sanic
 			
+			poetry add sanic
 			
 			#
 			#	if dev dependencies
 			#
 			# poetry export --with dev --format requirements.txt --output requirements.txt
 			
 			
 			rm -rf /biotech/venues/stages_pip && poetry export --format requirements.txt --output requirements.txt && pip install -r requirements.txt -t /biotech/venues/stages_pip
 			
 			# /root/.cache/pypoetry/virtualenvs/biotech-p2eJTVsK-py3.10/lib/python3.10/site-packages/
 			# cp -R /root/.cache/pypoetry/virtualenvs/biotech-p2eJTVsK-py3.10/lib/python3.10/site-packages/ /biotech/venues/stages_pip
 		
-		<h3>upgrade</h3>
-			poetry update sanic
+		
 		
 		<h3>installations venv</h3>
 			poetry config virtualenvs.path /path/to/your/directory
 			poetry env use python3
 			poetry shell
```

### Comparing `biotech-1.0.3/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg` & `biotech-1.1.0/venues/stages/biotech/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/___itinerary/itinerary.S.HTML` & `biotech-1.1.0/venues/stages/biotech/___itinerary/itinerary.S.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/___itinerary/maybes.s.HTML` & `biotech-1.1.0/venues/stages/biotech/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/___itinerary/processes/errout/start.py` & `biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/___itinerary/processes/errout_v2/start.py` & `biotech-1.1.0/venues/stages/biotech/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/__license/options/gpl-3.0-standalone.html` & `biotech-1.1.0/venues/stages/biotech/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_book/advanced tutorial.s.HTML` & `biotech-1.1.0/venues/stages/biotech/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_book/book.s.HTML` & `biotech-1.1.0/venues/stages/biotech/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_book/relevant.s.HTML` & `biotech-1.1.0/venues/stages/biotech/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_clique/__init__.py` & `biotech-1.1.0/venues/stages/biotech/_clique/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 
 
+print ('biotech')
 
-import click
-
+import biotech.topics.help_documentation as help_documentation
+	
+import click	
+	
+import pathlib
 import time
+from os.path import dirname, join, normpath
 
-
-from .group import clique as clique_group
-
-
-def the_help_procedure ():
-	import pathlib
-	from os.path import dirname, join, normpath
+def the_help_procedure (
+	port = ""
+):
 	this_directory = pathlib.Path (__file__).parent.resolve ()
 	this_module = str (normpath (join (this_directory, "..")))
 
-	import shares
-	shares.start ({
+	print ("port:", port)
+
+	help_documentation.start ({
 		"directory": this_module,
 		"extension": ".s.HTML",
-		"relative path": this_module
+		"relative path": this_module,
+		
+		"port": int (port)
 	})
 	
 	while True:
 		time.sleep (1)
 
 def clique ():
-	print ("clique")
-
-	
 	@click.group ()
 	def group ():
 		pass
-
-	@click.command ("shares")
-	def shares ():
-		the_help_procedure ()
 		
 	@click.command ("help")
-	def help ():
-		the_help_procedure ()
+	@click.option ('--port', default = "20000")
+	def help (port):
+		the_help_procedure (port)
 		
 	@click.command ("internal-status")
 	@click.option ('--glob-string', default = "")
 	def biotech_biotech (glob_string):
 
 		if (len (glob_string) >= 1):
 			import pathlib
@@ -85,21 +83,19 @@
 		import biotech
 		biotech.start (
 			glob_string = CWD + glob_string,
 			simultaneous = simultaneous
 		)
 
 
-	group.add_command (shares)	
 	group.add_command (help)	
 	
-	
 	group.add_command (biotech_biotech)	
 	group.add_command (status)
 	
-	group.add_command (clique_group ())
+	#group.add_command (clique_group ())
 	group ()
 
 
 
 
 #
```

### Comparing `biotech-1.0.3/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/__pycache__/establish.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 20:48:34 2024 UTC, .py size: 1466 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-00000000: 6f0d 0d0a 0000 0000 22e4 1e66 ba05 0000  o......."..f....
+00000000: 6f0d 0d0a 0000 0000 55a4 2266 b705 0000  o.......U."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6402  Z...d.d.l.Z.d.d.
 00000040: 6c02 5a02 6401 6403 6c03 6d04 5a04 6d05  l.Z.d.d.l.m.Z.m.
 00000050: 5a05 6d06 5a06 0100 6401 6402 6c07 5a07  Z.m.Z...d.d.l.Z.
 00000060: 6401 6402 6c08 5a08 6401 6402 6c09 5a09  d.d.l.Z.d.d.l.Z.
 00000070: 0904 6407 6405 6406 8401 5a0a 6402 5300  ..d.d.d...Z.d.S.
 00000080: 2908 7a3e 0a09 5468 6973 206f 6e65 2069  ).z>..This one i
 00000090: 7320 666f 7220 6361 6c6c 696e 670a 090a  s for calling...
 000000a0: 0909 5b78 6f6e 7368 5d20 6269 6f74 6563  ..[xonsh] biotec
 000000b0: 6820 7374 6174 7573 2d69 6e74 6572 6e61  h status-interna
 000000c0: 6c0a e900 0000 004e 2903 da07 6469 726e  l......N)...dirn
 000000d0: 616d 65da 046a 6f69 6eda 086e 6f72 6d70  ame..join..normp
 000000e0: 6174 68da 0063 0100 0000 0000 0000 0000  ath..c..........
-000000f0: 0000 0700 0000 0800 0000 4300 0000 7304  ..........C...s.
+000000f0: 0000 0700 0000 0800 0000 4300 0000 7300  ..........C...s.
 00000100: 0100 0074 00a0 0174 02a1 016a 03a0 04a1  ...t...t...j....
 00000110: 007d 0174 0574 067c 0164 0183 0283 017d  .}.t.t.|.d.....}
 00000120: 0274 0774 0574 067c 0164 0283 0283 0183  .t.t.t.|.d......
 00000130: 017d 0374 0774 0574 067c 0164 0383 0283  .}.t.t.t.|.d....
 00000140: 0183 017d 0474 086a 087c 0064 0464 058d  ...}.t.j.|.d.d..
 00000150: 027d 0574 096a 0a7c 0564 068d 0101 0074  .}.t.j.|.d.....t
 00000160: 0b6a 0c7c 0564 0774 0574 067c 0264 0883  .j.|.d.t.t.|.d..
 00000170: 0283 0174 0574 067c 0264 0983 0283 0167  ...t.t.|.d.....g
-00000180: 027c 037c 0464 0a8d 057d 0674 0d64 0b83  .|.|.d...}.t.d..
-00000190: 0101 0074 096a 0a7c 0664 0c19 0064 068d  ...t.j.|.d...d..
-000001a0: 0101 007c 0664 0c19 0064 0d19 0064 0e6b  ...|.d...d...d.k
-000001b0: 0273 5e4a 007c 0664 0c19 0083 0182 017c  .s^J.|.d.......|
-000001c0: 0664 0c19 0064 0f19 0064 0e6b 0273 6c4a  .d...d...d.k.slJ
-000001d0: 007c 0664 0c19 0083 0182 017c 0664 0c19  .|.d.......|.d..
-000001e0: 0064 1019 0064 0d19 0064 0e6b 0273 7c4a  .d...d...d.k.s|J
-000001f0: 007c 0664 0c19 0083 0182 0174 0d64 1183  .|.d.......t.d..
-00000200: 0101 007c 0653 0029 124e 7a08 2e2e 2f2e  ...|.S.).Nz.../.
-00000210: 2e2f 2e2e 7a02 2e2e da02 4442 5429 01da  ./..z.....DBT)..
-00000220: 0972 6563 7572 7369 7665 2901 da04 6461  .recursive)...da
-00000230: 7461 46da 0673 7461 6765 73da 0a73 7461  taF..stages..sta
-00000240: 6765 735f 7069 7029 05da 0570 6174 6873  ges_pip)...paths
-00000250: da0c 7369 6d75 6c74 616e 656f 7573 da0c  ..simultaneous..
-00000260: 6d6f 6475 6c65 5f70 6174 6873 da0d 7265  module_paths..re
-00000270: 6c61 7469 7665 5f70 6174 68da 0c64 625f  lative_path..db_
-00000280: 6469 7265 6374 6f72 797a 0e62 6f64 7920  directoryz.body 
-00000290: 7363 616e 2064 6f6e 65da 0573 7461 7473  scan done..stats
-000002a0: da06 616c 6172 6d73 7201 0000 00da 0565  ..alarmsr......e
-000002b0: 6d70 7479 da06 6368 6563 6b73 7a0f 626f  mpty..checksz.bo
-000002c0: 6479 2073 6361 6e20 646f 6e65 3f29 0eda  dy scan done?)..
-000002d0: 0770 6174 686c 6962 da04 5061 7468 da08  .pathlib..Path..
-000002e0: 5f5f 6669 6c65 5f5f da06 7061 7265 6e74  __file__..parent
-000002f0: da07 7265 736f 6c76 6572 0400 0000 7203  ..resolver....r.
-00000300: 0000 00da 0373 7472 da04 676c 6f62 da04  .....str..glob..
-00000310: 7269 6368 da0a 7072 696e 745f 6a73 6f6e  rich..print_json
-00000320: da09 626f 6479 5f73 6361 6eda 0573 7461  ..body_scan..sta
-00000330: 7274 da05 7072 696e 7429 07da 0b67 6c6f  rt..print)...glo
-00000340: 625f 7374 7269 6e67 da0b 7468 6973 5f66  b_string..this_f
-00000350: 6f6c 6465 72da 0a73 7472 7563 7475 7265  older..structure
-00000360: 73da 0974 6865 5f73 7461 6765 7206 0000  s..the_stager...
-00000370: 00da 0c73 7461 7475 735f 7061 7468 73da  ...status_paths.
-00000380: 0473 6361 6ea9 0072 2600 0000 fa33 2f62  .scan..r&....3/b
-00000390: 696f 7465 6368 2f76 656e 7565 732f 7374  iotech/venues/st
-000003a0: 6167 6573 2f62 696f 7465 6368 2f5f 7374  ages/biotech/_st
-000003b0: 6174 7573 2f65 7374 6162 6c69 7368 2e70  atus/establish.p
-000003c0: 7972 1e00 0000 1b00 0000 7330 0000 0010  yr........s0....
-000003d0: 040e 0212 0112 010e 0504 0702 0106 ff04  ................
-000003e0: 0402 0102 020c 030c 0102 fe02 0502 0206  ................
-000003f0: f408 0f10 021c 021c 0120 0108 0204 0372  ......... .....r
-00000400: 1e00 0000 2901 7205 0000 0029 0bda 075f  ....).r....)..._
-00000410: 5f64 6f63 5f5f 721a 0000 0072 1400 0000  _doc__r....r....
-00000420: da07 6f73 2e70 6174 6872 0200 0000 7203  ..os.pathr....r.
-00000430: 0000 0072 0400 0000 da02 6f73 721b 0000  ...r......osr...
-00000440: 0072 1d00 0000 721e 0000 0072 2600 0000  .r....r....r&...
-00000450: 7226 0000 0072 2600 0000 7227 0000 00da  r&...r&...r'....
-00000460: 083c 6d6f 6475 6c65 3e01 0000 0073 1400  .<module>....s..
-00000470: 0000 0402 0206 0807 0801 1401 0801 0802  ................
-00000480: 0802 0205 0eff                           ......
+00000180: 027c 037c 0464 0a8d 057d 0674 096a 0a64  .|.|.d...}.t.j.d
+00000190: 0b7c 0664 0c19 0069 0164 068d 0101 007c  .|.d...i.d.....|
+000001a0: 0664 0c19 0064 0d19 0064 0e6b 0273 5c4a  .d...d...d.k.s\J
+000001b0: 007c 0664 0c19 0083 0182 017c 0664 0c19  .|.d.......|.d..
+000001c0: 0064 0f19 0064 0e6b 0273 6a4a 007c 0664  .d...d.k.sjJ.|.d
+000001d0: 0c19 0083 0182 017c 0664 0c19 0064 1019  .......|.d...d..
+000001e0: 0064 0d19 0064 0e6b 0273 7a4a 007c 0664  .d...d.k.szJ.|.d
+000001f0: 0c19 0083 0182 0174 0d64 1183 0101 007c  .......t.d.....|
+00000200: 0653 0029 124e 7a08 2e2e 2f2e 2e2f 2e2e  .S.).Nz.../../..
+00000210: 7a02 2e2e da02 4442 5429 01da 0972 6563  z.....DBT)...rec
+00000220: 7572 7369 7665 2901 da04 6461 7461 46da  ursive)...dataF.
+00000230: 0673 7461 6765 73da 0a73 7461 6765 735f  .stages..stages_
+00000240: 7069 7029 05da 0570 6174 6873 da0c 7369  pip)...paths..si
+00000250: 6d75 6c74 616e 656f 7573 da0c 6d6f 6475  multaneous..modu
+00000260: 6c65 5f70 6174 6873 da0d 7265 6c61 7469  le_paths..relati
+00000270: 7665 5f70 6174 68da 0c64 625f 6469 7265  ve_path..db_dire
+00000280: 6374 6f72 797a 0e62 6f64 7920 7363 616e  ctoryz.body scan
+00000290: 2064 6f6e 65da 0573 7461 7473 da06 616c   done..stats..al
+000002a0: 6172 6d73 7201 0000 00da 0565 6d70 7479  armsr......empty
+000002b0: da06 6368 6563 6b73 7a0f 626f 6479 2073  ..checksz.body s
+000002c0: 6361 6e20 646f 6e65 3f29 0eda 0770 6174  can done?)...pat
+000002d0: 686c 6962 da04 5061 7468 da08 5f5f 6669  hlib..Path..__fi
+000002e0: 6c65 5f5f da06 7061 7265 6e74 da07 7265  le__..parent..re
+000002f0: 736f 6c76 6572 0400 0000 7203 0000 00da  solver....r.....
+00000300: 0373 7472 da04 676c 6f62 da04 7269 6368  .str..glob..rich
+00000310: da0a 7072 696e 745f 6a73 6f6e da09 626f  ..print_json..bo
+00000320: 6479 5f73 6361 6eda 0573 7461 7274 da05  dy_scan..start..
+00000330: 7072 696e 7429 07da 0b67 6c6f 625f 7374  print)...glob_st
+00000340: 7269 6e67 da0b 7468 6973 5f66 6f6c 6465  ring..this_folde
+00000350: 72da 0a73 7472 7563 7475 7265 73da 0974  r..structures..t
+00000360: 6865 5f73 7461 6765 7206 0000 00da 0c73  he_stager......s
+00000370: 7461 7475 735f 7061 7468 73da 0473 6361  tatus_paths..sca
+00000380: 6ea9 0072 2600 0000 fa33 2f62 696f 7465  n..r&....3/biote
+00000390: 6368 2f76 656e 7565 732f 7374 6167 6573  ch/venues/stages
+000003a0: 2f62 696f 7465 6368 2f5f 7374 6174 7573  /biotech/_status
+000003b0: 2f65 7374 6162 6c69 7368 2e70 7972 1e00  /establish.pyr..
+000003c0: 0000 1b00 0000 7332 0000 0010 040e 0212  ......s2........
+000003d0: 0112 010e 0504 0702 0106 ff04 0402 0102  ................
+000003e0: 020c 030c 0102 fe02 0502 0206 f404 0f08  ................
+000003f0: 0108 ff1c 041c 0120 0108 0204 0372 1e00  ....... .....r..
+00000400: 0000 2901 7205 0000 0029 0bda 075f 5f64  ..).r....)...__d
+00000410: 6f63 5f5f 721a 0000 0072 1400 0000 da07  oc__r....r......
+00000420: 6f73 2e70 6174 6872 0200 0000 7203 0000  os.pathr....r...
+00000430: 0072 0400 0000 da02 6f73 721b 0000 0072  .r......osr....r
+00000440: 1d00 0000 721e 0000 0072 2600 0000 7226  ....r....r&...r&
+00000450: 0000 0072 2600 0000 7227 0000 00da 083c  ...r&...r'.....<
+00000460: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
+00000470: 0402 0206 0807 0801 1401 0801 0802 0802  ................
+00000480: 0205 0eff                                ....
```

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/establish.py` & `biotech-1.1.0/venues/stages/biotech/_status/establish.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,17 +59,17 @@
 		],
 		
 		relative_path = the_stage,
 		
 		db_directory = DB
 	)
 	
-	print ("body scan done")
-	
-	rich.print_json (data = scan ["stats"])
+	rich.print_json (data = {
+		"body scan done": scan ["stats"]
+	})
 	
 	assert (scan ["stats"] ["alarms"] == 0), scan ["stats"]
 	assert (scan ["stats"] ["empty"] == 0), scan ["stats"]
 	assert (scan ["stats"] ["checks"] ["alarms"] == 0), scan ["stats"]
 	
 	print ("body scan done?")
```

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/-1_start/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/-1_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/0_start/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/0_start/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/1/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/1/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/10_time_limits/status_1.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,37 +3,44 @@
 	python3 /biotech/venues/stages/biotech/_status/status.proc.py "_status/monitors/10_time_limits/status_1.py"
 '''
 
 import pathlib
 from os.path import dirname, join, normpath
 import biotech
 
+import time
+
 def check_1 ():
+
 	
 	this_directory = pathlib.Path (__file__).parent.resolve ()
 	this_module = str (this_directory)
 	the_guarantees = str (normpath (join (this_directory, f"guarantees")))
 	
-	scan = biotech.start (
-		glob_string = the_guarantees + "/**/guarantee_*.py",
+
+	
+	scan = biotech.on ({
+		"glob_string": this_module + "/**/guarantee_*.py",
 		
-		time_limit = 5,
+		"time_limit": 5,
 		
-		simultaneous = True,
-		simultaneous_capacity = 10,
+		"simultaneous": True,
+		"simultaneous_capacity": 10,
 
-		module_paths = [
+		"module_paths": [
 			normpath (join (this_module, "modules")),
 			normpath (join (this_module, "modules_pip"))
 		],
 
-		relative_path = this_module,
+		"relative_path": this_module,
 		
-		aggregation_format = 2
-	)
+		"aggregation_format": 2
+	})
+	
+	assert (scan ["paths"] [0] ["alarm"] == "time limit exceeded"), scan ["paths"]
 
 	assert (scan ["stats"] ["paths"] ["alarms"] == 1), scan ["stats"]
 	assert (scan ["stats"] ["paths"] ["empty"] == 0), scan ["stats"]
 
 	assert (scan ["stats"] ["checks"] ["passes"] == 0), scan ["stats"]
 	assert (scan ["stats"] ["checks"] ["alarms"] == 0), scan ["stats"]
```

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/2/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/2/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/3_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/4.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/4_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/5__file__/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/5__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Oct 28 18:23:15 2023 UTC, .py size: 311 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -5,61 +5,61 @@
 00000040: 6501 6404 6405 8400 6406 6405 8400 6407  e.d.d...d.d...d.
 00000050: 6405 8400 6408 6405 8400 6409 6405 8400  d...d.d...d.d...
 00000060: 640a 6405 8400 640b 9c08 5a02 640c 5300  d.d...d...Z.d.S.
 00000070: 290d 6300 0000 0000 0000 0000 0000 0000  ).c.............
 00000080: 0000 0002 0000 0043 0000 0073 0c00 0000  .......C...s....
 00000090: 7400 6401 8301 0100 6400 5300 2902 4efa  t.d.....d.S.).N.
 000000a0: 0763 6865 636b 2031 2901 da05 7072 696e  .check 1)...prin
-000000b0: 74a9 0072 0300 0000 7203 0000 00fa 482f  t..r....r.....H/
-000000c0: 766f 6c74 732f 7665 6e75 6573 2f73 7461  volts/venues/sta
-000000d0: 6765 732f 766f 6c74 732f 5f73 7461 7475  ges/volts/_statu
-000000e0: 732f 6d6f 6e69 746f 7273 2f36 5f76 6172  s/monitors/6_var
-000000f0: 696f 7573 2f73 7461 7369 732f 315f 6865  ious/stasis/1_he
-00000100: 616c 7468 2e70 79da 0763 6865 636b 5f31  alth.py..check_1
-00000110: 0500 0000 7302 0000 000c 0172 0500 0000  ....s......r....
-00000120: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000130: 0002 0000 0043 0000 0073 1000 0000 7400  .....C...s....t.
-00000140: 6401 8301 0100 7401 6402 8301 8201 2903  d.....t.d.....).
-00000150: 4efa 0763 6865 636b 2032 7a08 4e4f 5420  N..check 2z.NOT 
-00000160: 3130 3025 2902 7202 0000 00da 0945 7863  100%).r......Exc
-00000170: 6570 7469 6f6e 7203 0000 0072 0300 0000  eptionr....r....
-00000180: 7203 0000 0072 0400 0000 da07 6368 6563  r....r......chec
-00000190: 6b5f 3209 0000 0073 0400 0000 0801 0801  k_2....s........
-000001a0: 7208 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000001b0: 0000 0000 0000 0100 0000 4300 0000 f304  ..........C.....
-000001c0: 0000 0064 0153 00a9 024e 7203 0000 0072  ...d.S...Nr....r
-000001d0: 0300 0000 7203 0000 0072 0300 0000 7203  ....r....r....r.
-000001e0: 0000 0072 0400 0000 da08 3c6c 616d 6264  ...r......<lambd
-000001f0: 613e 1100 0000 f302 0000 0004 0072 0b00  a>...........r..
-00000200: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000210: 0000 0001 0000 0043 0000 0072 0900 0000  .......C...r....
-00000220: 720a 0000 0072 0300 0000 7203 0000 0072  r....r....r....r
-00000230: 0300 0000 7203 0000 0072 0400 0000 720b  ....r....r....r.
-00000240: 0000 0012 0000 0072 0c00 0000 6300 0000  .......r....c...
-00000250: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00000260: 0043 0000 0072 0900 0000 720a 0000 0072  .C...r....r....r
-00000270: 0300 0000 7203 0000 0072 0300 0000 7203  ....r....r....r.
-00000280: 0000 0072 0400 0000 720b 0000 0013 0000  ...r....r.......
-00000290: 0072 0c00 0000 6300 0000 0000 0000 0000  .r....c.........
-000002a0: 0000 0000 0000 0001 0000 0043 0000 0072  ...........C...r
-000002b0: 0900 0000 720a 0000 0072 0300 0000 7203  ....r....r....r.
-000002c0: 0000 0072 0300 0000 7203 0000 0072 0400  ...r....r....r..
-000002d0: 0000 720b 0000 0014 0000 0072 0c00 0000  ..r........r....
-000002e0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000002f0: 0001 0000 0043 0000 0072 0900 0000 720a  .....C...r....r.
-00000300: 0000 0072 0300 0000 7203 0000 0072 0300  ...r....r....r..
-00000310: 0000 7203 0000 0072 0400 0000 720b 0000  ..r....r....r...
-00000320: 0015 0000 0072 0c00 0000 6300 0000 0000  .....r....c.....
-00000330: 0000 0000 0000 0000 0000 0001 0000 0043  ...............C
-00000340: 0000 0072 0900 0000 720a 0000 0072 0300  ...r....r....r..
-00000350: 0000 7203 0000 0072 0300 0000 7203 0000  ..r....r....r...
-00000360: 0072 0400 0000 720b 0000 0016 0000 0072  .r....r........r
-00000370: 0c00 0000 2908 7201 0000 0072 0600 0000  ....).r....r....
-00000380: 7a07 6368 6563 6b20 337a 0763 6865 636b  z.check 3z.check
-00000390: 2034 7a07 6368 6563 6b20 357a 0763 6865   4z.check 5z.che
-000003a0: 636b 2036 7a07 6368 6563 6b20 377a 0763  ck 6z.check 7z.c
-000003b0: 6865 636b 2038 4e29 0372 0500 0000 7208  heck 8N).r....r.
-000003c0: 0000 00da 0663 6865 636b 7372 0300 0000  .....checksr....
-000003d0: 7203 0000 0072 0300 0000 7204 0000 00da  r....r....r.....
-000003e0: 083c 6d6f 6475 6c65 3e01 0000 0073 1600  .<module>....s..
-000003f0: 0000 0804 0804 0206 0201 0601 0601 0601  ................
-00000400: 0601 0601 0601 0af8                      ........
+000000b0: 74a9 0072 0300 0000 7203 0000 00fa 4c2f  t..r....r.....L/
+000000c0: 6269 6f74 6563 682f 7665 6e75 6573 2f73  biotech/venues/s
+000000d0: 7461 6765 732f 6269 6f74 6563 682f 5f73  tages/biotech/_s
+000000e0: 7461 7475 732f 6d6f 6e69 746f 7273 2f36  tatus/monitors/6
+000000f0: 5f76 6172 696f 7573 2f73 7461 7369 732f  _various/stasis/
+00000100: 315f 6865 616c 7468 2e70 79da 0763 6865  1_health.py..che
+00000110: 636b 5f31 0500 0000 7302 0000 000c 0172  ck_1....s......r
+00000120: 0500 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00000130: 0000 0000 0002 0000 0043 0000 0073 1000  .........C...s..
+00000140: 0000 7400 6401 8301 0100 7401 6402 8301  ..t.d.....t.d...
+00000150: 8201 2903 4efa 0763 6865 636b 2032 7a08  ..).N..check 2z.
+00000160: 4e4f 5420 3130 3025 2902 7202 0000 00da  NOT 100%).r.....
+00000170: 0945 7863 6570 7469 6f6e 7203 0000 0072  .Exceptionr....r
+00000180: 0300 0000 7203 0000 0072 0400 0000 da07  ....r....r......
+00000190: 6368 6563 6b5f 3209 0000 0073 0400 0000  check_2....s....
+000001a0: 0801 0801 7208 0000 0063 0000 0000 0000  ....r....c......
+000001b0: 0000 0000 0000 0000 0000 0100 0000 4300  ..............C.
+000001c0: 0000 f304 0000 0064 0153 00a9 024e 7203  .......d.S...Nr.
+000001d0: 0000 0072 0300 0000 7203 0000 0072 0300  ...r....r....r..
+000001e0: 0000 7203 0000 0072 0400 0000 da08 3c6c  ..r....r......<l
+000001f0: 616d 6264 613e 1100 0000 f302 0000 0004  ambda>..........
+00000200: 0072 0b00 0000 6300 0000 0000 0000 0000  .r....c.........
+00000210: 0000 0000 0000 0001 0000 0043 0000 0072  ...........C...r
+00000220: 0900 0000 720a 0000 0072 0300 0000 7203  ....r....r....r.
+00000230: 0000 0072 0300 0000 7203 0000 0072 0400  ...r....r....r..
+00000240: 0000 720b 0000 0012 0000 0072 0c00 0000  ..r........r....
+00000250: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000260: 0001 0000 0043 0000 0072 0900 0000 720a  .....C...r....r.
+00000270: 0000 0072 0300 0000 7203 0000 0072 0300  ...r....r....r..
+00000280: 0000 7203 0000 0072 0400 0000 720b 0000  ..r....r....r...
+00000290: 0013 0000 0072 0c00 0000 6300 0000 0000  .....r....c.....
+000002a0: 0000 0000 0000 0000 0000 0001 0000 0043  ...............C
+000002b0: 0000 0072 0900 0000 720a 0000 0072 0300  ...r....r....r..
+000002c0: 0000 7203 0000 0072 0300 0000 7203 0000  ..r....r....r...
+000002d0: 0072 0400 0000 720b 0000 0014 0000 0072  .r....r........r
+000002e0: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000002f0: 0000 0000 0001 0000 0043 0000 0072 0900  .........C...r..
+00000300: 0000 720a 0000 0072 0300 0000 7203 0000  ..r....r....r...
+00000310: 0072 0300 0000 7203 0000 0072 0400 0000  .r....r....r....
+00000320: 720b 0000 0015 0000 0072 0c00 0000 6300  r........r....c.
+00000330: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00000340: 0000 0043 0000 0072 0900 0000 720a 0000  ...C...r....r...
+00000350: 0072 0300 0000 7203 0000 0072 0300 0000  .r....r....r....
+00000360: 7203 0000 0072 0400 0000 720b 0000 0016  r....r....r.....
+00000370: 0000 0072 0c00 0000 2908 7201 0000 0072  ...r....).r....r
+00000380: 0600 0000 7a07 6368 6563 6b20 337a 0763  ....z.check 3z.c
+00000390: 6865 636b 2034 7a07 6368 6563 6b20 357a  heck 4z.check 5z
+000003a0: 0763 6865 636b 2036 7a07 6368 6563 6b20  .check 6z.check 
+000003b0: 377a 0763 6865 636b 2038 4e29 0372 0500  7z.check 8N).r..
+000003c0: 0000 7208 0000 00da 0663 6865 636b 7372  ..r......checksr
+000003d0: 0300 0000 7203 0000 0072 0300 0000 7204  ....r....r....r.
+000003e0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000003f0: 0073 1600 0000 0804 0804 0206 0201 0601  .s..............
+00000400: 0601 0601 0601 0601 0601 0af8            ............
```

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/6_various/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/7/status_1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 
-
 '''
-	python3 status.proc.py '_status/monitors/UT/6/status_1.py'
+
 '''
 
 def check_1 ():
 	import pathlib
 	from os.path import dirname, join, normpath
 
 	THIS_FOLDER = pathlib.Path (__file__).parent.resolve ()
-	stasis = normpath (join (THIS_FOLDER, "stasis"))
+	stasis = normpath (join (THIS_FOLDER, f"stasis"))
 
 	import biotech
-	SCAN = biotech.start (
-		glob_string = stasis + '/**/*_health.py',
+	scan = biotech.start (
+		glob_string = stasis + '/**/guarantee_*.py',
 		
 		simultaneous = True,
 		
 		relative_path = stasis,
 		module_paths = [
-			#* FIND_STRUCTURE_paths (),			
-			normpath (join (stasis, "MODULES"))
+			normpath (join (stasis, "modules"))
 		]
 	)
-	status = SCAN ['status']
+	status = scan ['status']
 	paths = status ["paths"]
 	
 	import json
-	print ("Unit test suite 6 status found:", json.dumps (status ["stats"], indent = 4))
-	assert (len (paths) == 3)
+	print (f"Unit test suite status found:", json.dumps (status ["stats"], indent = 4))
+	assert (len (paths) == 1)
 			
-	assert (status ["stats"]["alarms"] == 1)
-	assert (status ["stats"]["empty"] == 1)
-	assert (status ["stats"]["checks"]["passes"] == 7)
+	assert (status ["stats"]["alarms"] == 0)
+	assert (status ["stats"]["empty"] == 0)
+	assert (status ["stats"]["checks"]["passes"] == 1)
 	assert (status ["stats"]["checks"]["alarms"] == 1)
 	
 checks = {
 	'check 1': check_1
 }
```

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/monitors/8_DB/status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status/monitors/8_DB/status_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 
 '''
 
 '''
 
+import rich
+
+import pathlib
+from os.path import dirname, join, normpath
+
 def check_1 ():
-	import pathlib
-	from os.path import dirname, join, normpath
+	
 
 	this_folder = pathlib.Path (__file__).parent.resolve ()
 	stasis = normpath (join (this_folder, f"stasis"))
 	variable = normpath (join (this_folder, f"variable"))
 
 	import biotech.procedures.data_nodes.tiny as biotech_db
 	records_1 = biotech_db.records (
@@ -25,14 +29,16 @@
 			normpath (join (stasis, "modules"))
 		],
 		db_directory = normpath (join (variable, f"status_db"))
 	)
 	status = scan ["status"]
 	paths = status ["paths"]
 	
+	rich.print_json (data = scan)
+	
 	'''
 	import json
 	print (
 		f"Unit test suite { ut_number } status found:", 
 		json.dumps (status ["stats"], indent = 4)
 	)
 	'''
@@ -47,15 +53,18 @@
 
 	
 	check_status (scan ["status"])
 
 	records_2 = biotech_db.records (
 		db_directory = normpath (join (variable, f"status_db"))
 	)
-	assert (len (records_2) == (len (records_1) + 1))
+	assert (len (records_2) == (len (records_1) + 1)), [
+		len (records_2),
+		len (records_1)
+	]
 	
 	last_record = biotech_db.last_record (
 		db_directory = normpath (join (variable, f"status_db"))
 	)
 	check_status (last_record)
 	
 checks = {
```

### Comparing `biotech-1.0.3/venues/stages/biotech/_status/status.proc.py` & `biotech-1.1.0/venues/stages/biotech/_status/status.proc.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 import pathlib
 from os.path import dirname, join, normpath
 this_folder = pathlib.Path (__file__).parent.resolve ()
 
 structures = normpath (join (this_folder, "../../.."))
 biotech_path = str (normpath (join (this_folder, "..")))
 
+biotech_path = str (normpath (join (this_folder, "monitors")))
+
+
 print ("biotech_path:", biotech_path)
 
 import sys
 if (len (sys.argv) >= 2):
 	glob_string = biotech_path + '/' + sys.argv [1]
 else:
 	glob_string = biotech_path + '/**/status_*.py'
```

### Comparing `biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py` & `biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json` & `biotech-1.1.0/venues/stages/biotech/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/_status_advanced/status.proc.py` & `biotech-1.1.0/venues/stages/biotech/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/architecture.s.HTML` & `biotech-1.1.0/venues/stages/biotech/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/module.s.HTML` & `biotech-1.1.0/venues/stages/biotech/module.s.HTML`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py` & `biotech-1.1.0/venues/stages/biotech/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 20:48:34 2024 UTC, .py size: 2121 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,117 +1,115 @@
-00000000: 6f0d 0d0a 0000 0000 22e4 1e66 4908 0000  o......."..fI...
+00000000: 6f0d 0d0a 0000 0000 269b 2266 3908 0000  o.......&."f9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
-00000050: 6d06 5a06 0100 6401 6402 6c07 5a07 6404  m.Z...d.d.l.Z.d.
-00000060: 6405 6c08 6d08 5a08 0100 6401 6402 6c09  d.l.m.Z...d.d.l.
+00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6403  Z.d.d.l.m.Z...d.
+00000040: 6404 6c02 5a02 6403 6404 6c03 5a03 6403  d.l.Z.d.d.l.Z.d.
+00000050: 6404 6c04 5a04 6403 6405 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
+00000060: 6d07 5a07 6d08 5a08 0100 6403 6404 6c09  m.Z.m.Z...d.d.l.
 00000070: 5a09 6406 6407 8400 5a0a 6408 6409 8400  Z.d.d...Z.d.d...
 00000080: 5a0b 0900 6900 6601 640a 640b 8401 5a0c  Z...i.f.d.d...Z.
-00000090: 6402 5300 290c 614e 0100 000a 0966 726f  d.S.).aN.....fro
+00000090: 6404 5300 290c 6150 0100 000a 0966 726f  d.S.).aP.....fro
 000000a0: 6d20 6269 6f74 6563 682e 7072 6f63 6564  m biotech.proced
 000000b0: 7572 6573 2e68 6561 6c74 685f 7363 616e  ures.health_scan
 000000c0: 2e6f 6e20 696d 706f 7274 2074 7572 6e5f  .on import turn_
 000000d0: 6f6e 5f68 6561 6c74 685f 6368 6563 6b0a  on_health_check.
 000000e0: 0974 6865 5f68 6561 6c74 685f 6368 6563  .the_health_chec
 000000f0: 6b20 3d20 7475 726e 5f6f 6e5f 6865 616c  k = turn_on_heal
 00000100: 7468 5f63 6865 636b 2028 0a09 0974 6865  th_check (...the
 00000110: 5f70 6174 682c 0a09 090a 0909 7468 655f  _path,......the_
 00000120: 6d6f 6475 6c65 5f64 6972 6563 746f 7269  module_directori
 00000130: 6573 203d 205b 5d2c 0a09 0972 656c 6174  es = [],...relat
 00000140: 6976 655f 7061 7468 203d 2022 222c 0a09  ive_path = "",..
-00000150: 090a 0909 696d 706c 6963 6974 5f70 726f  ....implicit_pro
-00000160: 6365 6475 7265 203d 207b 0a09 0909 2270  cedure = {...."p
-00000170: 6f72 7422 3a20 2222 2c0a 0909 0922 686f  ort": "",...."ho
-00000180: 7374 223a 2022 220a 0909 7d0a 0929 0a09  st": ""...}..)..
-00000190: 0a09 7468 655f 6865 616c 7468 5f63 6865  ..the_health_che
-000001a0: 636b 205b 2270 726f 6365 7373 225d 2e74  ck ["process"].t
-000001b0: 6572 6d69 6e61 7465 2028 290a 090a 0974  erminate ()....t
-000001c0: 6865 5f72 6570 6f72 7420 3d20 7468 655f  he_report = the_
-000001d0: 6865 616c 7468 5f63 6865 636b 205b 2272  health_check ["r
-000001e0: 6570 6f72 7422 5d09 0ae9 0000 0000 4e29  eport"].......N)
-000001f0: 03da 0764 6972 6e61 6d65 da04 6a6f 696e  ...dirname..join
-00000200: da08 6e6f 726d 7061 7468 e901 0000 0029  ..normpath.....)
-00000210: 01da 0c64 796e 616d 6963 5f70 6f72 7463  ...dynamic_portc
-00000220: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00000230: 0500 0000 4300 0000 7322 0000 0074 00a0  ....C...s"...t..
-00000240: 0174 02a1 016a 03a0 04a1 007d 0074 0574  .t...j.....}.t.t
-00000250: 0674 077c 0064 0183 0283 0183 0153 0029  .t.|.d.......S.)
-00000260: 024e 7a1b 7072 6f63 6573 732f 6865 616c  .Nz.process/heal
-00000270: 7468 5f73 6361 6e2e 7072 6f63 2e70 79a9  th_scan.proc.py.
-00000280: 08da 0770 6174 686c 6962 da04 5061 7468  ...pathlib..Path
-00000290: da08 5f5f 6669 6c65 5f5f da06 7061 7265  ..__file__..pare
-000002a0: 6e74 da07 7265 736f 6c76 65da 0373 7472  nt..resolve..str
-000002b0: 7204 0000 0072 0300 0000 a901 da0b 7468  r....r........th
-000002c0: 6973 5f66 6f6c 6465 72a9 0072 1000 0000  is_folder..r....
-000002d0: fa3b 2f62 696f 7465 6368 2f76 656e 7565  .;/biotech/venue
-000002e0: 732f 7374 6167 6573 2f62 696f 7465 6368  s/stages/biotech
-000002f0: 2f70 726f 6365 6475 7265 732f 6865 616c  /procedures/heal
-00000300: 7468 5f73 6361 6e2f 6f6e 2e70 79da 1c74  th_scan/on.py..t
-00000310: 6865 5f68 6561 6c74 685f 7363 616e 5f70  he_health_scan_p
-00000320: 726f 6365 7373 5f70 6174 6821 0000 0073  rocess_path!...s
-00000330: 0400 0000 1001 1201 7212 0000 0063 0000  ........r....c..
-00000340: 0000 0000 0000 0000 0000 0100 0000 0500  ................
-00000350: 0000 4300 0000 7324 0000 0074 00a0 0174  ..C...s$...t...t
-00000360: 02a1 016a 03a0 04a1 007d 0074 0574 0674  ...j.....}.t.t.t
-00000370: 077c 0064 0183 0283 0183 0167 0153 0029  .|.d.......g.S.)
-00000380: 024e 7a0f 7072 6f63 6573 732f 6d6f 6475  .Nz.process/modu
-00000390: 6c65 7372 0700 0000 720e 0000 0072 1000  lesr....r....r..
-000003a0: 0000 7210 0000 0072 1100 0000 da14 6669  ..r....r......fi
-000003b0: 6e64 5f62 7569 6c74 696e 5f6d 6f64 756c  nd_builtin_modul
-000003c0: 6573 2500 0000 7306 0000 0010 0110 0204  es%...s.........
-000003d0: ff72 1300 0000 6301 0000 0000 0000 0000  .r....c.........
-000003e0: 0000 0008 0000 0005 0000 0043 0000 0073  ...........C...s
-000003f0: c000 0000 7400 6401 8301 0100 7c00 6402  ....t.d.....|.d.
-00000400: 1900 7d01 7c00 6403 1900 7d02 7c00 6404  ..}.|.d...}.|.d.
-00000410: 1900 7d03 7c00 6405 1900 7d04 7401 6a02  ..}.|.d...}.t.j.
-00000420: a003 a100 7d05 6406 a004 6700 7c02 a201  ....}.d...g.|...
-00000430: 7405 8300 a201 a101 7c05 6407 3c00 7c01  t.......|.d.<.|.
-00000440: 7c05 6408 3c00 6409 7c05 640a 3c00 7406  |.d.<.d.|.d.<.t.
-00000450: 7c04 640b 1900 8301 7c05 640c 3c00 7407  |.d.....|.d.<.t.
-00000460: 7c03 8301 7406 6b02 724d 7408 7c03 8301  |...t.k.rMt.|...
-00000470: 640d 6b05 724d 7401 6a09 a00a 7c01 7c03  d.k.rMt.j...|.|.
-00000480: a102 7d06 7c03 7c05 640e 3c00 6e08 640f  ..}.|.|.d.<.n.d.
-00000490: 7c01 1700 7d06 6410 7c05 640e 3c00 0900  |...}.d.|.d.<...
-000004a0: 740b 740c 8300 7c05 7c06 6411 8d03 7d07  t.t...|.|.d...}.
-000004b0: 7c07 5300 2912 4e7a 0874 6865 2070 6174  |.S.).Nz.the pat
-000004c0: 68da 1173 7461 7475 735f 6368 6563 6b5f  h..status_check_
-000004d0: 7061 7468 da0c 6d6f 6475 6c65 5f70 6174  path..module_pat
-000004e0: 6873 da0d 7265 6c61 7469 7665 5f70 6174  hs..relative_pat
-000004f0: 68da 1269 6d70 6c69 6369 745f 7072 6f63  h..implicit_proc
-00000500: 6564 7572 65fa 013a da0a 5059 5448 4f4e  edure..:..PYTHON
-00000510: 5041 5448 da15 6269 6f74 6563 685f 5f5f  PATH..biotech___
-00000520: 7374 6174 7573 5f70 6174 687a 0730 2e30  status_pathz.0.0
-00000530: 2e30 2e30 da15 6269 6f74 6563 685f 5f5f  .0.0..biotech___
-00000540: 6861 7262 6f72 5f68 6f73 74da 0470 6f72  harbor_host..por
-00000550: 74da 1562 696f 7465 6368 5f5f 5f68 6172  t..biotech___har
-00000560: 626f 725f 706f 7274 7205 0000 00da 1e62  bor_portr......b
-00000570: 696f 7465 6368 5f5f 5f73 7461 7475 735f  iotech___status_
-00000580: 7265 6c61 7469 7665 5f70 6174 687a 0573  relative_pathz.s
-00000590: 6361 6e20 da00 2903 da0c 7072 6f63 6573  can ..)...proces
-000005a0: 735f 7061 7468 da03 656e 76da 046e 616d  s_path..env..nam
-000005b0: 6529 0dda 0570 7269 6e74 da02 6f73 da07  e)...print..os..
-000005c0: 656e 7669 726f 6eda 0463 6f70 7972 0300  environ..copyr..
-000005d0: 0000 7213 0000 0072 0d00 0000 da04 7479  ..r....r......ty
-000005e0: 7065 da03 6c65 6eda 0470 6174 68da 0772  pe..len..path..r
-000005f0: 656c 7061 7468 7206 0000 0072 1200 0000  elpathr....r....
-00000600: 2908 da06 7061 636b 6574 da08 7468 655f  )...packet..the_
-00000610: 7061 7468 da16 7468 655f 6d6f 6475 6c65  path..the_module
-00000620: 5f64 6972 6563 746f 7269 6573 7216 0000  _directoriesr...
-00000630: 0072 1700 0000 7221 0000 0072 2200 0000  .r....r!...r"...
-00000640: da10 7468 655f 6865 616c 7468 5f63 6865  ..the_health_che
-00000650: 636b 7210 0000 0072 1000 0000 7211 0000  ckr....r....r...
-00000660: 00da 1474 7572 6e5f 6f6e 5f68 6561 6c74  ...turn_on_healt
-00000670: 685f 6368 6563 6b39 0000 0073 3400 0000  h_check9...s4...
-00000680: 0803 0802 0802 0801 0801 0a02 0601 0201  ................
-00000690: 02ff 0402 0afe 0809 0802 1001 1803 0e01  ................
-000006a0: 0a01 0802 0801 0203 0204 0401 0202 0201  ................
-000006b0: 06fc 040b 722f 0000 0029 0dda 075f 5f64  ....r/...)...__d
-000006c0: 6f63 5f5f 7224 0000 0072 0800 0000 da07  oc__r$...r......
-000006d0: 6f73 2e70 6174 6872 0200 0000 7203 0000  os.pathr....r...
-000006e0: 0072 0400 0000 da03 7379 7372 0600 0000  .r......sysr....
-000006f0: da05 666c 6173 6b72 1200 0000 7213 0000  ..flaskr....r...
-00000700: 0072 2f00 0000 7210 0000 0072 1000 0000  .r/...r....r....
-00000710: 7210 0000 0072 1100 0000 da08 3c6d 6f64  r....r......<mod
-00000720: 756c 653e 0100 0000 7318 0000 0004 0108  ule>....s.......
-00000730: 1508 0214 0108 010c 0208 0208 0208 0402  ................
-00000740: 0802 0d0e ff                             .....
+00000150: 090a 0909 6167 6772 6567 6174 6f72 5f70  ....aggregator_p
+00000160: 726f 6365 6475 7265 203d 207b 0a09 0909  rocedure = {....
+00000170: 2270 6f72 7422 3a20 2222 2c0a 0909 0922  "port": "",...."
+00000180: 686f 7374 223a 2022 220a 0909 7d0a 0929  host": ""...}..)
+00000190: 0a09 0a09 7468 655f 6865 616c 7468 5f63  ....the_health_c
+000001a0: 6865 636b 205b 2270 726f 6365 7373 225d  heck ["process"]
+000001b0: 2e74 6572 6d69 6e61 7465 2028 290a 090a  .terminate ()...
+000001c0: 0974 6865 5f72 6570 6f72 7420 3d20 7468  .the_report = th
+000001d0: 655f 6865 616c 7468 5f63 6865 636b 205b  e_health_check [
+000001e0: 2272 6570 6f72 7422 5d09 0ae9 0100 0000  "report"].......
+000001f0: 2901 da0c 6479 6e61 6d69 635f 706f 7274  )...dynamic_port
+00000200: e900 0000 004e 2903 da07 6469 726e 616d  .....N)...dirnam
+00000210: 65da 046a 6f69 6eda 086e 6f72 6d70 6174  e..join..normpat
+00000220: 6863 0000 0000 0000 0000 0000 0000 0100  hc..............
+00000230: 0000 0500 0000 4300 0000 7322 0000 0074  ......C...s"...t
+00000240: 00a0 0174 02a1 016a 03a0 04a1 007d 0074  ...t...j.....}.t
+00000250: 0574 0674 077c 0064 0183 0283 0183 0153  .t.t.|.d.......S
+00000260: 0029 024e 7a1b 7072 6f63 6573 732f 6865  .).Nz.process/he
+00000270: 616c 7468 5f73 6361 6e2e 7072 6f63 2e70  alth_scan.proc.p
+00000280: 79a9 08da 0770 6174 686c 6962 da04 5061  y....pathlib..Pa
+00000290: 7468 da08 5f5f 6669 6c65 5f5f da06 7061  th..__file__..pa
+000002a0: 7265 6e74 da07 7265 736f 6c76 65da 0373  rent..resolve..s
+000002b0: 7472 7206 0000 0072 0500 0000 a901 da0b  trr....r........
+000002c0: 7468 6973 5f66 6f6c 6465 72a9 0072 1000  this_folder..r..
+000002d0: 0000 fa3b 2f62 696f 7465 6368 2f76 656e  ...;/biotech/ven
+000002e0: 7565 732f 7374 6167 6573 2f62 696f 7465  ues/stages/biote
+000002f0: 6368 2f70 726f 6365 6475 7265 732f 6865  ch/procedures/he
+00000300: 616c 7468 5f73 6361 6e2f 6f6e 2e70 79da  alth_scan/on.py.
+00000310: 1c74 6865 5f68 6561 6c74 685f 7363 616e  .the_health_scan
+00000320: 5f70 726f 6365 7373 5f70 6174 6825 0000  _process_path%..
+00000330: 0073 0400 0000 1001 1201 7212 0000 0063  .s........r....c
+00000340: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000350: 0500 0000 4300 0000 7324 0000 0074 00a0  ....C...s$...t..
+00000360: 0174 02a1 016a 03a0 04a1 007d 0074 0574  .t...j.....}.t.t
+00000370: 0674 077c 0064 0183 0283 0183 0167 0153  .t.|.d.......g.S
+00000380: 0029 024e 7a0f 7072 6f63 6573 732f 6d6f  .).Nz.process/mo
+00000390: 6475 6c65 7372 0700 0000 720e 0000 0072  dulesr....r....r
+000003a0: 1000 0000 7210 0000 0072 1100 0000 da14  ....r....r......
+000003b0: 6669 6e64 5f62 7569 6c74 696e 5f6d 6f64  find_builtin_mod
+000003c0: 756c 6573 2900 0000 7306 0000 0010 0110  ules)...s.......
+000003d0: 0204 ff72 1300 0000 6301 0000 0000 0000  ...r....c.......
+000003e0: 0000 0000 0008 0000 0005 0000 0043 0000  .............C..
+000003f0: 0073 b800 0000 7c00 6401 1900 7d01 7c00  .s....|.d...}.|.
+00000400: 6402 1900 7d02 7c00 6403 1900 7d03 7c00  d...}.|.d...}.|.
+00000410: 6404 1900 7d04 7400 6a01 a002 a100 7d05  d...}.t.j.....}.
+00000420: 6405 a003 6700 7c02 a201 7404 8300 a201  d...g.|...t.....
+00000430: a101 7c05 6406 3c00 7c01 7c05 6407 3c00  ..|.d.<.|.|.d.<.
+00000440: 6408 7c05 6409 3c00 7405 7c04 640a 1900  d.|.d.<.t.|.d...
+00000450: 8301 7c05 640b 3c00 7406 7c03 8301 7405  ..|.d.<.t.|...t.
+00000460: 6b02 7249 7407 7c03 8301 640c 6b05 7249  k.rIt.|...d.k.rI
+00000470: 7400 6a08 a009 7c01 7c03 a102 7d06 7c03  t.j...|.|...}.|.
+00000480: 7c05 640d 3c00 6e08 640e 7c01 1700 7d06  |.d.<.n.d.|...}.
+00000490: 640f 7c05 640d 3c00 0900 740a 740b 8300  d.|.d.<...t.t...
+000004a0: 7c05 7c06 6410 8d03 7d07 7c07 5300 2911  |.|.d...}.|.S.).
+000004b0: 4eda 1173 7461 7475 735f 6368 6563 6b5f  N..status_check_
+000004c0: 7061 7468 da0c 6d6f 6475 6c65 5f70 6174  path..module_pat
+000004d0: 6873 da0d 7265 6c61 7469 7665 5f70 6174  hs..relative_pat
+000004e0: 68da 1461 6767 7265 6761 746f 725f 7072  h..aggregator_pr
+000004f0: 6f63 6564 7572 65fa 013a da0a 5059 5448  ocedure..:..PYTH
+00000500: 4f4e 5041 5448 da15 6269 6f74 6563 685f  ONPATH..biotech_
+00000510: 5f5f 7374 6174 7573 5f70 6174 687a 0730  __status_pathz.0
+00000520: 2e30 2e30 2e30 da15 6269 6f74 6563 685f  .0.0.0..biotech_
+00000530: 5f5f 6861 7262 6f72 5f68 6f73 74da 0470  __harbor_host..p
+00000540: 6f72 74da 1562 696f 7465 6368 5f5f 5f68  ort..biotech___h
+00000550: 6172 626f 725f 706f 7274 7201 0000 00da  arbor_portr.....
+00000560: 1e62 696f 7465 6368 5f5f 5f73 7461 7475  .biotech___statu
+00000570: 735f 7265 6c61 7469 7665 5f70 6174 687a  s_relative_pathz
+00000580: 0573 6361 6e20 da00 2903 da0c 7072 6f63  .scan ..)...proc
+00000590: 6573 735f 7061 7468 da03 656e 76da 046e  ess_path..env..n
+000005a0: 616d 6529 0cda 026f 73da 0765 6e76 6972  ame)...os..envir
+000005b0: 6f6e da04 636f 7079 7205 0000 0072 1300  on..copyr....r..
+000005c0: 0000 720d 0000 00da 0474 7970 65da 036c  ..r......type..l
+000005d0: 656e da04 7061 7468 da07 7265 6c70 6174  en..path..relpat
+000005e0: 6872 0200 0000 7212 0000 0029 08da 0670  hr....r....)...p
+000005f0: 6163 6b65 74da 0874 6865 5f70 6174 68da  acket..the_path.
+00000600: 1674 6865 5f6d 6f64 756c 655f 6469 7265  .the_module_dire
+00000610: 6374 6f72 6965 7372 1600 0000 7217 0000  ctoriesr....r...
+00000620: 0072 2100 0000 7222 0000 00da 1074 6865  .r!...r".....the
+00000630: 5f68 6561 6c74 685f 6368 6563 6b72 1000  _health_checkr..
+00000640: 0000 7210 0000 0072 1100 0000 da14 7475  ..r....r......tu
+00000650: 726e 5f6f 6e5f 6865 616c 7468 5f63 6865  rn_on_health_che
+00000660: 636b 3d00 0000 7332 0000 0008 0308 0208  ck=...s2........
+00000670: 0108 010a 0206 0102 0102 ff04 060a fa08  ................
+00000680: 0a08 0210 0118 030e 010a 0108 0208 0102  ................
+00000690: 0302 0404 0102 0202 0106 fc04 0872 2e00  .............r..
+000006a0: 0000 290d da07 5f5f 646f 635f 5f72 0200  ..)...__doc__r..
+000006b0: 0000 da05 666c 6173 6b72 2300 0000 7208  ....flaskr#...r.
+000006c0: 0000 00da 076f 732e 7061 7468 7204 0000  .....os.pathr...
+000006d0: 0072 0500 0000 7206 0000 00da 0373 7973  .r....r......sys
+000006e0: 7212 0000 0072 1300 0000 722e 0000 0072  r....r....r....r
+000006f0: 1000 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
+00000700: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000710: 0073 1800 0000 0401 0c15 0803 0803 0801  .s..............
+00000720: 1401 0801 0805 0804 0208 020d 0eff       ..............
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/on.py` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/on.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,36 +3,40 @@
 	from biotech.procedures.health_scan.on import turn_on_health_check
 	the_health_check = turn_on_health_check (
 		the_path,
 		
 		the_module_directories = [],
 		relative_path = "",
 		
-		implicit_procedure = {
+		aggregator_procedure = {
 			"port": "",
 			"host": ""
 		}
 	)
 	
 	the_health_check ["process"].terminate ()
 	
 	the_report = the_health_check ["report"]	
 '''
 
-
-
+#----
+#
+from .dynamic_port import dynamic_port
+#
+#
+import flask
+#
+#
 import os
-
 import pathlib
 from os.path import dirname, join, normpath
 import sys
+#
+#----
 
-from .dynamic_port import dynamic_port
-
-import flask
 
 def the_health_scan_process_path ():
 	this_folder = pathlib.Path (__file__).parent.resolve ()
 	return str (normpath (join (this_folder, "process/health_scan.proc.py")))
 
 def find_builtin_modules ():
 	this_folder = pathlib.Path (__file__).parent.resolve ()
@@ -45,44 +49,43 @@
 '''
 	packet = {
 		"status_check_path": status_check_path,
 		
 		"module_paths": module_paths,
 		"relative_path": relative_path,
 		
-		"implicit_procedure": {
+		"aggregator_procedure": {
 			"port": port
 		}
 	}
 '''
 def turn_on_health_check (
 	packet = {}
 ):
-	print ("the path")
-
 	the_path = packet ["status_check_path"]
 	
 	the_module_directories = packet ["module_paths"]
 	relative_path = packet ["relative_path"]
-	implicit_procedure = packet ["implicit_procedure"]
+	aggregator_procedure = packet ["aggregator_procedure"]
 
 	env = os.environ.copy ()
 	env ["PYTHONPATH"] = ":".join ([
 		* the_module_directories,
+		
+		#
+		#	These should actually be reduced... to one module...
+		#
 		* find_builtin_modules ()		
 	])
-	
-	#print ()
-	#print ("PYTHONPATH:", env ["PYTHONPATH"])
-	#print ()
+
 	
 	env ["biotech___status_path"] = the_path
 		
 	env ["biotech___harbor_host"] = "0.0.0.0"
-	env ["biotech___harbor_port"] = str (implicit_procedure ["port"])	
+	env ["biotech___harbor_port"] = str (aggregator_procedure ["port"])	
 	
 	
 	if (type (relative_path) == str and len (relative_path) >= 1):
 		name = os.path.relpath (the_path, relative_path)
 		env ["biotech___status_relative_path"] = relative_path
 	else:
 		name = "scan " + the_path
@@ -96,12 +99,9 @@
 	the_health_check = dynamic_port (
 		process_path = the_health_scan_process_path (),
 		
 		env = env,
 		name = name
 	)
 	
-	
-	
-	#print (the_venture)
 
 	return the_health_check
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/health_scan.proc.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,63 +5,90 @@
 		process is started
 		
 		
 '''
 
 
 
-
-#from __keg import open_scan_harbor
-
-from __import_from_path import import_from_path
-
-from __coms.done_with_scan import done_with_scan
-from __mixes.format_rel_path import format_rel_path
-
+#
+#
+from __health_scan_utilities.coms.done_with_scan import done_with_scan
+from __health_scan_utilities.coms.the_health_scan_started import the_health_scan_started
+from __health_scan_utilities.format_rel_path import format_rel_path
+from __health_scan_utilities.import_from_path import import_from_path
+from __health_scan_utilities.show.variable import show_variable
+#
+#
+import io
+import json
 import os
-import time
 from pprint import pprint
-
-
 import sys
-for path in sys.path:
-	print ("health scan, sys path:", path)
-
+import time
 import traceback
-import io
+#
+#
+
+#
+#	objective, make the sys path 100% declarative
+#
+# sys.path = os.environ.get ("PYTHONPATH").split (":")
+# print ("health scan, sys path:", json.dumps (sys.path, indent = 4))
+#
+
 def find_trace (exception : Exception) -> str:
 	try:
 		file = io.StringIO ()
 		traceback.print_exception (exception, file = file)
 		
 		return file.getvalue ().rstrip ().split ("\n")
 	except Exception:
 		pass;
 		
 	return 'An exception occurred while calculating trace.'
 
 def main ():
 	#raise Exception ("An exception occurred")
+	status_path = os.environ.get ("biotech___status_path")
+	status_relative_path = os.environ.get ("biotech___status_relative_path")
+	host = os.environ.get ("biotech___harbor_host")
+	port = int (os.environ.get ("biotech___harbor_port"))
+	
+	the_health_scan_started (
+		host = host,
+		port = port,
+		proceeds = {
+			"path": format_rel_path (status_path, status_relative_path),
+			"status_path": status_path,
+			"relative_path": status_relative_path
+		}
+	)
+	
+	#
+	#	elapsed check
+	#
+	time.sleep (1)
+	
 	try:
-		status_path = os.environ.get ("biotech___status_path")
-		status_relative_path = os.environ.get ("biotech___status_relative_path")
-
-		host = os.environ.get ("biotech___harbor_host")
-		port = int (os.environ.get ("biotech___harbor_port"))
+		#----
+		#
+		
+		#
+		#----
 
 		proceeds = import_from_path (status_path)
 
-		pprint ({
+		show_variable ({
 			"pid": os.getpid (),
 			"proceeds": proceeds,
 			"harbor": {
 				"host": host,
 				"port": port
 			}
-		})
+		}, mode = "show")
 	except Exception as E:
 		proceeds = {
 			"parsed": False,
 			"alarm": "An exception occurred while running the scan.",
 			"exception": repr (E),
 			"exception trace": find_trace (E)
 		}
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 04:32:47 2024 UTC, .py size: 570 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6fff 1d66 3a02 0000  o.......o..f:...
+00000000: 6f0d 0d0a 0000 0000 b855 2066 2101 0000  o........U f!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6403  Z.d.d.l.m.Z...d.
 00000040: 6404 6405 6405 6900 6605 6406 6407 8401  d.d.d.i.f.d.d...
 00000050: 5a02 6408 5300 2909 7a46 0a09 6672 6f6d  Z.d.S.).zF..from
 00000060: 205f 5f63 6f6d 732e 646f 6e65 5f77 6974   __coms.done_wit
 00000070: 685f 7363 616e 2069 6d70 6f72 7420 646f  h_scan import do
@@ -14,21 +14,20 @@
 000000d0: 0500 0000 0000 0000 0000 0000 0500 0000  ................
 000000e0: 0500 0000 4300 0000 7312 0000 0074 0064  ....C...s....t.d
 000000f0: 017c 0264 027c 0483 0401 0064 0053 0029  .|.d.|.....d.S.)
 00000100: 034e 7204 0000 0072 0500 0000 7202 0000  .Nr....r....r...
 00000110: 0029 05da 0468 6f73 74da 0855 524c 5f70  .)...host..URL_p
 00000120: 6174 68da 0470 6f72 74da 0470 6174 68da  ath..port..path.
 00000130: 0870 726f 6365 6564 73a9 0072 0c00 0000  .proceeds..r....
-00000140: fa68 2f66 6163 746f 7279 5f66 6172 6d2f  .h/factory_farm/
-00000150: 7665 6e75 6573 2f73 7461 6765 732f 6661  venues/stages/fa
-00000160: 6374 6f72 795f 6661 726d 2f70 726f 6365  ctory_farm/proce
-00000170: 6475 7265 732f 6865 616c 7468 5f73 6361  dures/health_sca
-00000180: 6e2f 7072 6f63 6573 732f 6d6f 6475 6c65  n/process/module
-00000190: 732f 5f5f 636f 6d73 2f64 6f6e 655f 7769  s/__coms/done_wi
-000001a0: 7468 5f73 6361 6e2e 7079 da0e 646f 6e65  th_scan.py..done
-000001b0: 5f77 6974 685f 7363 616e 0a00 0000 7304  _with_scan....s.
-000001c0: 0000 000e 0804 0272 0e00 0000 4e29 03da  .......r....N)..
-000001d0: 075f 5f64 6f63 5f5f 7203 0000 0072 0e00  .__doc__r....r..
-000001e0: 0000 720c 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-000001f0: 0072 0d00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000200: 0100 0000 7310 0000 0004 020c 0502 0302  ....s...........
-00000210: 0102 0102 0202 010e fa                   .........
+00000140: fa5e 2f62 696f 7465 6368 2f76 656e 7565  .^/biotech/venue
+00000150: 732f 7374 6167 6573 2f62 696f 7465 6368  s/stages/biotech
+00000160: 2f70 726f 6365 6475 7265 732f 6865 616c  /procedures/heal
+00000170: 7468 5f73 6361 6e2f 7072 6f63 6573 732f  th_scan/process/
+00000180: 6d6f 6475 6c65 732f 5f5f 636f 6d73 2f64  modules/__coms/d
+00000190: 6f6e 655f 7769 7468 5f73 6361 6e2e 7079  one_with_scan.py
+000001a0: da0e 646f 6e65 5f77 6974 685f 7363 616e  ..done_with_scan
+000001b0: 0a00 0000 7302 0000 0012 0872 0e00 0000  ....s......r....
+000001c0: 4e29 03da 075f 5f64 6f63 5f5f 7203 0000  N)...__doc__r...
+000001d0: 0072 0e00 0000 720c 0000 0072 0c00 0000  .r....r....r....
+000001e0: 720c 0000 0072 0d00 0000 da08 3c6d 6f64  r....r......<mod
+000001f0: 756c 653e 0100 0000 7310 0000 0004 020c  ule>....s.......
+00000200: 0502 0302 0102 0102 0202 010e fa         .............
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/coms/__pycache__/send_patch.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 04:42:59 2024 UTC, .py size: 834 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,57 @@
-00000000: 6f0d 0d0a 0000 0000 d301 1e66 4203 0000  o..........fB...
+00000000: 6f0d 0d0a 0000 0000 75ce 2266 2303 0000  o.......u."f#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6403 6404 8400  Z.d.d.l.Z.d.d...
 00000050: 5a04 6402 5300 2905 7a5a 0a09 6672 6f6d  Z.d.S.).zZ..from
 00000060: 202e 7365 6e64 5f70 6174 6368 2069 6d70   .send_patch imp
 00000070: 6f72 7420 7365 6e64 5f70 6174 6368 0a09  ort send_patch..
 00000080: 7365 6e64 5f70 6174 6368 2028 2230 2e30  send_patch ("0.0
 00000090: 2e30 2e30 222c 2070 6f72 742c 2022 2f64  .0.0", port, "/d
 000000a0: 6f6e 655f 7769 7468 5f73 6361 6e22 2c20  one_with_scan", 
 000000b0: 7b7d 290a e900 0000 004e 6304 0000 0000  {})......Nc.....
-000000c0: 0000 0000 0000 0009 0000 0009 0000 0043  ...............C
-000000d0: 0000 0073 c400 0000 7400 8300 0100 7400  ...s....t.....t.
-000000e0: 6401 7401 a002 a100 7c03 8303 0100 7400  d.t.....|.....t.
-000000f0: 8300 0100 7403 a004 7c03 a101 7d04 7405  ....t...|...}.t.
-00000100: a005 7405 6a06 7405 6a07 a102 8f36 7d05  ..t.j.t.j....6}.
-00000110: 7c05 a008 7c00 7c01 6602 a101 0100 6402  |...|.|.f.....d.
-00000120: 7c02 9b00 6403 7c00 9b00 6404 7409 7c04  |...d.|...d.t.|.
-00000130: 8301 9b00 6405 7c04 9b00 9d08 7d06 7c05  ....d.|.....}.|.
-00000140: a00a 7c06 a00b a100 a101 0100 6406 7d07  ..|.........d.}.
-00000150: 0900 7c05 a00c 6408 a101 7d08 7c08 7345  ..|...d...}.|.sE
-00000160: 6e05 7c07 7c08 3700 7d07 713d 5700 6400  n.|.|.7.}.q=W.d.
-00000170: 0400 0400 8303 0100 6e08 3100 7354 7701  ........n.1.sTw.
-00000180: 0100 0100 0100 5900 0100 7400 6409 7c07  ......Y...t.d.|.
-00000190: a00d a100 8302 0100 6400 5300 290a 4e7a  ........d.S.).Nz
-000001a0: 1773 656e 6469 6e67 202f 646f 6e65 5f77  .sending /done_w
-000001b0: 6974 685f 7363 616e 7a06 5041 5443 4820  ith_scanz.PATCH 
-000001c0: 7a11 2048 5454 502f 312e 310d 0a48 6f73  z. HTTP/1.1..Hos
-000001d0: 743a 207a 320d 0a43 6f6e 7465 6e74 2d54  t: z2..Content-T
-000001e0: 7970 653a 2061 7070 6c69 6361 7469 6f6e  ype: application
-000001f0: 2f6a 736f 6e0d 0a43 6f6e 7465 6e74 2d4c  /json..Content-L
-00000200: 656e 6774 683a 207a 040d 0a0d 0af3 0000  ength: z........
-00000210: 0000 5469 0004 0000 7a09 7265 7370 6f6e  ..Ti....z.respon
-00000220: 7365 3a29 0eda 0570 7269 6e74 da02 6f73  se:)...print..os
-00000230: da06 6765 7470 6964 da04 6a73 6f6e da05  ..getpid..json..
-00000240: 6475 6d70 73da 0673 6f63 6b65 74da 0741  dumps..socket..A
-00000250: 465f 494e 4554 da0b 534f 434b 5f53 5452  F_INET..SOCK_STR
-00000260: 4541 4dda 0763 6f6e 6e65 6374 da03 6c65  EAM..connect..le
-00000270: 6eda 0773 656e 6461 6c6c da06 656e 636f  n..sendall..enco
-00000280: 6465 da04 7265 6376 da06 6465 636f 6465  de..recv..decode
-00000290: 2909 da04 686f 7374 da04 706f 7274 da04  )...host..port..
-000002a0: 7061 7468 da09 6a73 6f6e 5f64 6174 61da  path..json_data.
-000002b0: 086a 736f 6e5f 7374 72da 0173 da07 7265  .json_str..s..re
-000002c0: 7175 6573 74da 0872 6573 706f 6e73 65da  quest..response.
-000002d0: 0464 6174 61a9 0072 1a00 0000 fa64 2f66  .data..r.....d/f
-000002e0: 6163 746f 7279 5f66 6172 6d2f 7665 6e75  actory_farm/venu
-000002f0: 6573 2f73 7461 6765 732f 6661 6374 6f72  es/stages/factor
-00000300: 795f 6661 726d 2f70 726f 6365 6475 7265  y_farm/procedure
-00000310: 732f 6865 616c 7468 5f73 6361 6e2f 7072  s/health_scan/pr
-00000320: 6f63 6573 732f 6d6f 6475 6c65 732f 5f5f  ocess/modules/__
-00000330: 636f 6d73 2f73 656e 645f 7061 7463 682e  coms/send_patch.
-00000340: 7079 da0a 7365 6e64 5f70 6174 6368 0b00  py..send_patch..
-00000350: 0000 7324 0000 0006 0110 0106 010a 0312  ..s$............
-00000360: 030e 0120 030e 0104 0302 010a 0104 0102  ... ............
-00000370: 0108 0102 fc02 031c f412 1072 1c00 0000  ...........r....
-00000380: 2905 da07 5f5f 646f 635f 5f72 0800 0000  )...__doc__r....
-00000390: 7206 0000 0072 0400 0000 721c 0000 0072  r....r....r....r
-000003a0: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
-000003b0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000003c0: 0073 0a00 0000 0401 0805 0801 0801 0c02  .s..............
+000000c0: 0000 0000 0000 000a 0000 0009 0000 0043  ...............C
+000000d0: 0000 0073 a600 0000 7400 a001 a100 7d04  ...s....t.....}.
+000000e0: 0900 7402 a003 7c03 a101 7d05 7404 a004  ..t...|...}.t...
+000000f0: 7404 6a05 7404 6a06 a102 8f37 7d06 7c06  t.j.t.j....7}.|.
+00000100: a007 7c00 7c01 6602 a101 0100 6401 7c02  ..|.|.f.....d.|.
+00000110: 9b00 6402 7c00 9b00 6403 7408 7c05 8301  ..d.|...d.t.|...
+00000120: 9b00 6404 7c05 9b00 9d08 7d07 7c06 a009  ..d.|.....}.|...
+00000130: 7c07 a00a a100 a101 0100 6405 7d08 0900  |.........d.}...
+00000140: 7c06 a00b 6407 a101 7d09 7c09 733c 6e05  |...d...}.|.s<n.
+00000150: 7c08 7c09 3700 7d08 7134 5700 6400 0400  |.|.7.}.q4W.d...
+00000160: 0400 8303 0100 6400 5300 3100 734c 7701  ......d.S.1.sLw.
+00000170: 0100 0100 0100 5900 0100 6400 5300 2908  ......Y...d.S.).
+00000180: 4e7a 0650 4154 4348 207a 1120 4854 5450  Nz.PATCH z. HTTP
+00000190: 2f31 2e31 0d0a 486f 7374 3a20 7a32 0d0a  /1.1..Host: z2..
+000001a0: 436f 6e74 656e 742d 5479 7065 3a20 6170  Content-Type: ap
+000001b0: 706c 6963 6174 696f 6e2f 6a73 6f6e 0d0a  plication/json..
+000001c0: 436f 6e74 656e 742d 4c65 6e67 7468 3a20  Content-Length: 
+000001d0: 7a04 0d0a 0d0a f300 0000 0054 6900 0400  z..........Ti...
+000001e0: 0029 0cda 026f 73da 0667 6574 7069 64da  .)...os..getpid.
+000001f0: 046a 736f 6eda 0564 756d 7073 da06 736f  .json..dumps..so
+00000200: 636b 6574 da07 4146 5f49 4e45 54da 0b53  cket..AF_INET..S
+00000210: 4f43 4b5f 5354 5245 414d da07 636f 6e6e  OCK_STREAM..conn
+00000220: 6563 74da 036c 656e da07 7365 6e64 616c  ect..len..sendal
+00000230: 6cda 0665 6e63 6f64 65da 0472 6563 7629  l..encode..recv)
+00000240: 0ada 0468 6f73 74da 0470 6f72 74da 0470  ...host..port..p
+00000250: 6174 68da 096a 736f 6e5f 6461 7461 da03  ath..json_data..
+00000260: 7069 64da 086a 736f 6e5f 7374 72da 0173  pid..json_str..s
+00000270: da07 7265 7175 6573 74da 0872 6573 706f  ..request..respo
+00000280: 6e73 65da 0464 6174 61a9 0072 1900 0000  nse..data..r....
+00000290: fa70 2f62 696f 7465 6368 2f76 656e 7565  .p/biotech/venue
+000002a0: 732f 7374 6167 6573 2f62 696f 7465 6368  s/stages/biotech
+000002b0: 2f70 726f 6365 6475 7265 732f 6865 616c  /procedures/heal
+000002c0: 7468 5f73 6361 6e2f 7072 6f63 6573 732f  th_scan/process/
+000002d0: 6d6f 6475 6c65 732f 5f5f 6865 616c 7468  modules/__health
+000002e0: 5f73 6361 6e5f 7574 696c 6974 6965 732f  _scan_utilities/
+000002f0: 636f 6d73 2f73 656e 645f 7061 7463 682e  coms/send_patch.
+00000300: 7079 da0a 7365 6e64 5f70 6174 6368 0b00  py..send_patch..
+00000310: 0000 7320 0000 0008 0202 020a 0812 030e  ..s ............
+00000320: 0120 030e 0104 0302 010a 0104 0202 0108  . ..............
+00000330: 0202 fa02 0422 f372 1b00 0000 2905 da07  .....".r....)...
+00000340: 5f5f 646f 635f 5f72 0700 0000 7205 0000  __doc__r....r...
+00000350: 0072 0300 0000 721b 0000 0072 1900 0000  .r....r....r....
+00000360: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00000370: 083c 6d6f 6475 6c65 3e01 0000 0073 0a00  .<module>....s..
+00000380: 0000 0401 0805 0801 0801 0c02            ............
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__exec_from_path/__init__.py` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__import_from_path/__init__.py` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 	
 		spec = importlib.util.spec_from_file_location (module_name, module_path)
 		the_module = importlib.util.module_from_spec (spec)
 		proceeds = spec.loader.exec_module (the_module)
 		
 		print ("proceeds", proceeds)
 		print ("checks in module", hasattr (the_module, 'checks'))
+		
+		
 		if (hasattr (the_module, 'checks')):
 			checks = the_module.checks
 			
 			for check in checks:
 				try:
 					time_start = perf_counter ()
 					
@@ -87,13 +89,21 @@
 				"empty": True,
 				"parsed": True
 			}
 			
 	except Exception as E:
 		path_exception = E;
 		
+	try:	
+		return {
+			"parsed": False,
+			"alarm": "An exception occurred while importing the path.",
+			"exception": repr (path_exception),
+			"exception trace": find_trace (path_exception)
+		}
+	except Exception:
+		pass;
+		
 	return {
 		"parsed": False,
-		"alarm": "An exception occurred while importing the path.",
-		"exception": repr (path_exception),
-		"exception trace": find_trace (path_exception)
+		"alarm": "An exception occurred while importing the path.  The exception could not be parsed."
 	}
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 04:42:27 2024 UTC, .py size: 2004 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b301 1e66 d407 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 207e 2066 8608 0000  o....... ~ f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6403 6c05 5a05 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c06 5a06 6401 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6403 6c09 5a09 6401 6403 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0a 6401 6405 6c0a 6d0b 5a0b 0100 6401  Z.d.d.l.m.Z...d.
@@ -28,97 +28,106 @@
 000001b0: 7768 696c 6520 6361 6c63 756c 6174 696e  while calculatin
 000001c0: 6720 7472 6163 652e 2908 da02 696f da08  g trace.)...io..
 000001d0: 5374 7269 6e67 494f da09 7472 6163 6562  StringIO..traceb
 000001e0: 6163 6bda 0f70 7269 6e74 5f65 7863 6570  ack..print_excep
 000001f0: 7469 6f6e da08 6765 7476 616c 7565 da06  tion..getvalue..
 00000200: 7273 7472 6970 da05 7370 6c69 74da 0945  rstrip..split..E
 00000210: 7863 6570 7469 6f6e 2902 7206 0000 0072  xception).r....r
-00000220: 0800 0000 a900 7212 0000 00fa 6e2f 6661  ......r.....n/fa
-00000230: 6374 6f72 795f 6661 726d 2f76 656e 7565  ctory_farm/venue
-00000240: 732f 7374 6167 6573 2f66 6163 746f 7279  s/stages/factory
-00000250: 5f66 6172 6d2f 7072 6f63 6564 7572 6573  _farm/procedures
-00000260: 2f68 6561 6c74 685f 7363 616e 2f70 726f  /health_scan/pro
-00000270: 6365 7373 2f6d 6f64 756c 6573 2f5f 5f69  cess/modules/__i
-00000280: 6d70 6f72 745f 6672 6f6d 5f70 6174 682f  mport_from_path/
-00000290: 5f5f 696e 6974 5f5f 2e70 79da 0a66 696e  __init__.py..fin
-000002a0: 645f 7472 6163 6512 0000 0073 1000 0000  d_trace....s....
-000002b0: 0201 0801 0e01 1402 0c01 0201 0402 02fd  ................
-000002c0: 7214 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000002d0: 0000 0e00 0000 0b00 0000 4300 0000 7364  ..........C...sd
-000002e0: 0100 0064 017d 017a 9067 007d 0264 0264  ...d.}.z.g.}.d.d
-000002f0: 0264 039c 027d 0364 047d 0474 006a 01a0  .d...}.d.}.t.j..
-00000300: 027c 047c 00a1 027d 0574 006a 01a0 037c  .|.|...}.t.j...|
-00000310: 05a1 017d 067c 056a 04a0 057c 06a1 017d  ...}.|.j...|...}
-00000320: 0774 0664 057c 0783 0201 0074 0664 0674  .t.d.|.....t.d.t
-00000330: 077c 0664 0783 0283 0201 0074 077c 0664  .|.d.......t.|.d
-00000340: 0783 0272 8d7c 066a 087d 087c 0844 005d  ...r.|.j.}.|.D.]
-00000350: 4e7d 097a 2474 0983 007d 0a7c 087c 0919  N}.z$t...}.|.|..
-00000360: 0083 0001 0074 0983 007d 0b7c 0b7c 0a18  .....t...}.|.|..
-00000370: 007d 0c7c 02a0 0a7c 0964 087c 0c64 0967  .}.|...|.d.|.d.g
-00000380: 0264 0a9c 03a1 0101 007c 0364 0b05 0019  .d.......|.d....
-00000390: 0064 0c37 0003 003c 0057 0071 3604 0074  .d.7...<.W.q6..t
-000003a0: 0b79 8401 007d 0d01 007a 1c7c 02a0 0a7c  .y...}...z.|...|
-000003b0: 0964 0d74 0c7c 0d83 0174 0d7c 0d83 0164  .d.t.|...t.|...d
-000003c0: 0e9c 04a1 0101 007c 0364 0f05 0019 0064  .......|.d.....d
-000003d0: 0c37 0003 003c 0057 0059 0064 007d 0d7e  .7...<.W.Y.d.}.~
-000003e0: 0d71 3664 007d 0d7e 0d77 0177 0064 0d64  .q6d.}.~.w.w.d.d
-000003f0: 087c 037c 0264 109c 0457 0053 0064 0864  .|.|.d...W.S.d.d
-00000400: 0864 119c 0257 0053 0004 0074 0b79 a601  .d...W.S...t.y..
-00000410: 007d 0d01 007a 087c 0d7d 0157 0059 0064  .}...z.|.}.W.Y.d
-00000420: 007d 0d7e 0d6e 0564 007d 0d7e 0d77 0177  .}.~.n.d.}.~.w.w
-00000430: 0064 0d64 1274 0c7c 0183 0174 0d7c 0183  .d.d.t.|...t.|..
-00000440: 0164 139c 0453 0029 144e da00 7201 0000  .d...S.).N..r...
-00000450: 0029 02da 0670 6173 7365 73da 0661 6c61  .)...passes..ala
-00000460: 726d 73da 085f 5f6d 6169 6e5f 5fda 0870  rms..__main__..p
-00000470: 726f 6365 6564 737a 1063 6865 636b 7320  roceedsz.checks 
-00000480: 696e 206d 6f64 756c 65da 0663 6865 636b  in module..check
-00000490: 7354 da07 7365 636f 6e64 7329 03da 0563  sT..seconds)...c
-000004a0: 6865 636b da06 7061 7373 6564 da07 656c  heck..passed..el
-000004b0: 6170 7365 6472 1600 0000 e901 0000 0046  apsedr.........F
-000004c0: 2904 721c 0000 0072 1d00 0000 7206 0000  ).r....r....r...
-000004d0: 00fa 0f65 7863 6570 7469 6f6e 2074 7261  ...exception tra
-000004e0: 6365 7217 0000 0029 04da 0565 6d70 7479  cer....)...empty
-000004f0: da06 7061 7273 6564 da05 7374 6174 7372  ..parsed..statsr
-00000500: 1a00 0000 2902 7221 0000 0072 2200 0000  ....).r!...r"...
-00000510: 7a2f 416e 2065 7863 6570 7469 6f6e 206f  z/An exception o
-00000520: 6363 7572 7265 6420 7768 696c 6520 696d  ccurred while im
-00000530: 706f 7274 696e 6720 7468 6520 7061 7468  porting the path
-00000540: 2e29 0472 2200 0000 da05 616c 6172 6d72  .).r".....alarmr
-00000550: 0600 0000 7220 0000 0029 0eda 0969 6d70  ....r ...)...imp
-00000560: 6f72 746c 6962 da04 7574 696c da17 7370  ortlib..util..sp
-00000570: 6563 5f66 726f 6d5f 6669 6c65 5f6c 6f63  ec_from_file_loc
-00000580: 6174 696f 6eda 106d 6f64 756c 655f 6672  ation..module_fr
-00000590: 6f6d 5f73 7065 63da 066c 6f61 6465 72da  om_spec..loader.
-000005a0: 0b65 7865 635f 6d6f 6475 6c65 da05 7072  .exec_module..pr
-000005b0: 696e 74da 0768 6173 6174 7472 721a 0000  int..hasattrr...
-000005c0: 0072 0500 0000 da06 6170 7065 6e64 7211  .r......appendr.
-000005d0: 0000 00da 0472 6570 7272 1400 0000 290e  .....reprr....).
-000005e0: da0b 6d6f 6475 6c65 5f70 6174 68da 0e70  ..module_path..p
-000005f0: 6174 685f 6578 6365 7074 696f 6eda 0866  ath_exception..f
-00000600: 696e 6469 6e67 7372 2300 0000 da0b 6d6f  indingsr#.....mo
-00000610: 6475 6c65 5f6e 616d 65da 0473 7065 63da  dule_name..spec.
-00000620: 0a74 6865 5f6d 6f64 756c 6572 1900 0000  .the_moduler....
-00000630: 721a 0000 0072 1c00 0000 da0a 7469 6d65  r....r......time
-00000640: 5f73 7461 7274 da08 7469 6d65 5f65 6e64  _start..time_end
-00000650: da0c 7469 6d65 5f65 6c61 7073 6564 da01  ..time_elapsed..
-00000660: 4572 1200 0000 7212 0000 0072 1300 0000  Er....r....r....
-00000670: da10 696d 706f 7274 5f66 726f 6d5f 7061  ..import_from_pa
-00000680: 7468 1d00 0000 736a 0000 0004 0102 0204  th....sj........
-00000690: 0102 0202 0106 fe04 050e 020c 010c 010a  ................
-000006a0: 0210 010a 0106 0108 0202 0106 010a 0206  ................
-000006b0: 0208 0104 0202 0102 0106 0108 fd14 060e  ................
-000006c0: 0204 0102 0102 0106 0106 0108 fc1c 0708  ................
-000006d0: 8002 f802 0b02 0102 0202 0108 fb02 0a02  ................
-000006e0: 0108 fe0e 0510 0108 8002 ff02 0402 0106  ................
-000006f0: 0106 0106 fc72 3900 0000 2912 da07 5f5f  .....r9...)...__
-00000700: 646f 635f 5fda 0966 7261 6374 696f 6e73  doc__..fractions
-00000710: 7202 0000 00da 0e69 6d70 6f72 746c 6962  r......importlib
-00000720: 2e75 7469 6c72 2500 0000 720a 0000 00da  .utilr%...r.....
-00000730: 046a 736f 6eda 0770 6174 686c 6962 7203  .json..pathlibr.
-00000740: 0000 00da 0373 7973 da04 7469 6d65 7204  .....sys..timer.
-00000750: 0000 0072 0500 0000 720c 0000 0072 1100  ...r....r....r..
-00000760: 0000 da03 7374 7272 1400 0000 7239 0000  ....strr....r9..
-00000770: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00000780: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000790: 0000 0073 1a00 0000 0401 0c05 0801 0801  ...s............
-000007a0: 0801 0c01 0801 0801 0c01 0c01 0801 1202  ................
-000007b0: 0c0b                                     ..
+00000220: 0800 0000 a900 7212 0000 00fa 7a2f 6269  ......r.....z/bi
+00000230: 6f74 6563 682f 7665 6e75 6573 2f73 7461  otech/venues/sta
+00000240: 6765 732f 6269 6f74 6563 682f 7072 6f63  ges/biotech/proc
+00000250: 6564 7572 6573 2f68 6561 6c74 685f 7363  edures/health_sc
+00000260: 616e 2f70 726f 6365 7373 2f6d 6f64 756c  an/process/modul
+00000270: 6573 2f5f 5f68 6561 6c74 685f 7363 616e  es/__health_scan
+00000280: 5f75 7469 6c69 7469 6573 2f69 6d70 6f72  _utilities/impor
+00000290: 745f 6672 6f6d 5f70 6174 682f 5f5f 696e  t_from_path/__in
+000002a0: 6974 5f5f 2e70 79da 0a66 696e 645f 7472  it__.py..find_tr
+000002b0: 6163 6512 0000 0073 1000 0000 0201 0801  ace....s........
+000002c0: 0e01 1402 0c01 0201 0402 02fd 7214 0000  ............r...
+000002d0: 0063 0100 0000 0000 0000 0000 0000 0e00  .c..............
+000002e0: 0000 0b00 0000 4300 0000 7384 0100 0064  ......C...s....d
+000002f0: 017d 017a 9067 007d 0264 0264 0264 039c  .}.z.g.}.d.d.d..
+00000300: 027d 0364 047d 0474 006a 01a0 027c 047c  .}.d.}.t.j...|.|
+00000310: 00a1 027d 0574 006a 01a0 037c 05a1 017d  ...}.t.j...|...}
+00000320: 067c 056a 04a0 057c 06a1 017d 0774 0664  .|.j...|...}.t.d
+00000330: 057c 0783 0201 0074 0664 0674 077c 0664  .|.....t.d.t.|.d
+00000340: 0783 0283 0201 0074 077c 0664 0783 0272  .......t.|.d...r
+00000350: 8d7c 066a 087d 087c 0844 005d 4e7d 097a  .|.j.}.|.D.]N}.z
+00000360: 2474 0983 007d 0a7c 087c 0919 0083 0001  $t...}.|.|......
+00000370: 0074 0983 007d 0b7c 0b7c 0a18 007d 0c7c  .t...}.|.|...}.|
+00000380: 02a0 0a7c 0964 087c 0c64 0967 0264 0a9c  ...|.d.|.d.g.d..
+00000390: 03a1 0101 007c 0364 0b05 0019 0064 0c37  .....|.d.....d.7
+000003a0: 0003 003c 0057 0071 3604 0074 0b79 8401  ...<.W.q6..t.y..
+000003b0: 007d 0d01 007a 1c7c 02a0 0a7c 0964 0d74  .}...z.|...|.d.t
+000003c0: 0c7c 0d83 0174 0d7c 0d83 0164 0e9c 04a1  .|...t.|...d....
+000003d0: 0101 007c 0364 0f05 0019 0064 0c37 0003  ...|.d.....d.7..
+000003e0: 003c 0057 0059 0064 007d 0d7e 0d71 3664  .<.W.Y.d.}.~.q6d
+000003f0: 007d 0d7e 0d77 0177 0064 0d64 087c 037c  .}.~.w.w.d.d.|.|
+00000400: 0264 109c 0457 0053 0064 0864 0864 119c  .d...W.S.d.d.d..
+00000410: 0257 0053 0004 0074 0b79 a601 007d 0d01  .W.S...t.y...}..
+00000420: 007a 087c 0d7d 0157 0059 0064 007d 0d7e  .z.|.}.W.Y.d.}.~
+00000430: 0d6e 0564 007d 0d7e 0d77 0177 007a 0c64  .n.d.}.~.w.w.z.d
+00000440: 0d64 1274 0c7c 0183 0174 0d7c 0183 0164  .d.t.|...t.|...d
+00000450: 139c 0457 0053 0004 0074 0b79 bc01 0001  ...W.S...t.y....
+00000460: 0001 0059 006e 0177 0064 0d64 1464 159c  ...Y.n.w.d.d.d..
+00000470: 0253 0029 164e da00 7201 0000 0029 02da  .S.).N..r....)..
+00000480: 0670 6173 7365 73da 0661 6c61 726d 73da  .passes..alarms.
+00000490: 085f 5f6d 6169 6e5f 5fda 0870 726f 6365  .__main__..proce
+000004a0: 6564 737a 1063 6865 636b 7320 696e 206d  edsz.checks in m
+000004b0: 6f64 756c 65da 0663 6865 636b 7354 da07  odule..checksT..
+000004c0: 7365 636f 6e64 7329 03da 0563 6865 636b  seconds)...check
+000004d0: da06 7061 7373 6564 da07 656c 6170 7365  ..passed..elapse
+000004e0: 6472 1600 0000 e901 0000 0046 2904 721c  dr.........F).r.
+000004f0: 0000 0072 1d00 0000 7206 0000 00fa 0f65  ...r....r......e
+00000500: 7863 6570 7469 6f6e 2074 7261 6365 7217  xception tracer.
+00000510: 0000 0029 04da 0565 6d70 7479 da06 7061  ...)...empty..pa
+00000520: 7273 6564 da05 7374 6174 7372 1a00 0000  rsed..statsr....
+00000530: 2902 7221 0000 0072 2200 0000 7a2f 416e  ).r!...r"...z/An
+00000540: 2065 7863 6570 7469 6f6e 206f 6363 7572   exception occur
+00000550: 7265 6420 7768 696c 6520 696d 706f 7274  red while import
+00000560: 696e 6720 7468 6520 7061 7468 2e29 0472  ing the path.).r
+00000570: 2200 0000 da05 616c 6172 6d72 0600 0000  ".....alarmr....
+00000580: 7220 0000 007a 5341 6e20 6578 6365 7074  r ...zSAn except
+00000590: 696f 6e20 6f63 6375 7272 6564 2077 6869  ion occurred whi
+000005a0: 6c65 2069 6d70 6f72 7469 6e67 2074 6865  le importing the
+000005b0: 2070 6174 682e 2020 5468 6520 6578 6365   path.  The exce
+000005c0: 7074 696f 6e20 636f 756c 6420 6e6f 7420  ption could not 
+000005d0: 6265 2070 6172 7365 642e 2902 7222 0000  be parsed.).r"..
+000005e0: 0072 2400 0000 290e da09 696d 706f 7274  .r$...)...import
+000005f0: 6c69 62da 0475 7469 6cda 1773 7065 635f  lib..util..spec_
+00000600: 6672 6f6d 5f66 696c 655f 6c6f 6361 7469  from_file_locati
+00000610: 6f6e da10 6d6f 6475 6c65 5f66 726f 6d5f  on..module_from_
+00000620: 7370 6563 da06 6c6f 6164 6572 da0b 6578  spec..loader..ex
+00000630: 6563 5f6d 6f64 756c 65da 0570 7269 6e74  ec_module..print
+00000640: da07 6861 7361 7474 7272 1a00 0000 7205  ..hasattrr....r.
+00000650: 0000 00da 0661 7070 656e 6472 1100 0000  .....appendr....
+00000660: da04 7265 7072 7214 0000 0029 0eda 0b6d  ..reprr....)...m
+00000670: 6f64 756c 655f 7061 7468 da0e 7061 7468  odule_path..path
+00000680: 5f65 7863 6570 7469 6f6e da08 6669 6e64  _exception..find
+00000690: 696e 6773 7223 0000 00da 0b6d 6f64 756c  ingsr#.....modul
+000006a0: 655f 6e61 6d65 da04 7370 6563 da0a 7468  e_name..spec..th
+000006b0: 655f 6d6f 6475 6c65 7219 0000 0072 1a00  e_moduler....r..
+000006c0: 0000 721c 0000 00da 0a74 696d 655f 7374  ..r......time_st
+000006d0: 6172 74da 0874 696d 655f 656e 64da 0c74  art..time_end..t
+000006e0: 696d 655f 656c 6170 7365 64da 0145 7212  ime_elapsed..Er.
+000006f0: 0000 0072 1200 0000 7213 0000 00da 1069  ...r....r......i
+00000700: 6d70 6f72 745f 6672 6f6d 5f70 6174 681d  mport_from_path.
+00000710: 0000 0073 7800 0000 0401 0202 0401 0202  ...sx...........
+00000720: 0201 06fe 0405 0e02 0c01 0c01 0a02 1001  ................
+00000730: 0a03 0601 0802 0201 0601 0a02 0602 0801  ................
+00000740: 0402 0201 0201 0601 08fd 1406 0e02 0401  ................
+00000750: 0201 0201 0601 0601 08fc 1c07 0880 02f8  ................
+00000760: 020b 0201 0202 0201 08fb 020a 0201 08fe  ................
+00000770: 0e05 1001 0880 02ff 0203 0202 0201 0601  ................
+00000780: 0601 08fc 0c06 0401 02ff 0204 0201 06fe  ................
+00000790: 7239 0000 0029 12da 075f 5f64 6f63 5f5f  r9...)...__doc__
+000007a0: da09 6672 6163 7469 6f6e 7372 0200 0000  ..fractionsr....
+000007b0: da0e 696d 706f 7274 6c69 622e 7574 696c  ..importlib.util
+000007c0: 7225 0000 0072 0a00 0000 da04 6a73 6f6e  r%...r......json
+000007d0: da07 7061 7468 6c69 6272 0300 0000 da03  ..pathlibr......
+000007e0: 7379 73da 0474 696d 6572 0400 0000 7205  sys..timer....r.
+000007f0: 0000 0072 0c00 0000 7211 0000 00da 0373  ...r....r......s
+00000800: 7472 7214 0000 0072 3900 0000 7212 0000  trr....r9...r...
+00000810: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000820: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
+00000830: 0000 0004 010c 0508 0108 0108 010c 0108  ................
+00000840: 0108 010c 010c 0108 0112 020c 0b         .............
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__keg/__init__.py` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/health_scan/process/modules/__health_scan_utilities/__pycache__/format_rel_path.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 14 03:40:28 2024 UTC, .py size: 321 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 000000e0: 0164 016b 0572 1574 036a 04a0 057c 007c  .d.k.r.t.j...|.|
 000000f0: 01a1 027d 027c 0253 007c 007d 027c 0253  ...}.|.S.|.}.|.S
 00000100: 0029 024e e901 0000 0029 06da 0474 7970  .).N.....)...typ
 00000110: 65da 0373 7472 da03 6c65 6eda 026f 73da  e..str..len..os.
 00000120: 0470 6174 68da 0772 656c 7061 7468 2903  .path..relpath).
 00000130: da08 7375 625f 7061 7468 da0d 7265 6c61  ..sub_path..rela
 00000140: 7469 7665 5f70 6174 6872 0700 0000 a900  tive_pathr......
-00000150: 720b 0000 00fa 5c2f 766f 6c74 732f 7665  r.....\/volts/ve
-00000160: 6e75 6573 2f73 7461 6765 732f 766f 6c74  nues/stages/volt
-00000170: 732f 7072 6f63 6564 7572 6573 2f68 6561  s/procedures/hea
-00000180: 6c74 685f 7363 616e 2f70 726f 6365 7373  lth_scan/process
-00000190: 2f6d 6f64 756c 6573 2f5f 5f6d 6978 6573  /modules/__mixes
-000001a0: 2f66 6f72 6d61 745f 7265 6c5f 7061 7468  /format_rel_path
-000001b0: 2e70 79da 0f66 6f72 6d61 745f 7265 6c5f  .py..format_rel_
-000001c0: 7061 7468 0a00 0000 730a 0000 0018 010e  path....s.......
-000001d0: 0104 0404 fe04 0272 0d00 0000 2903 da07  .......r....)...
-000001e0: 5f5f 646f 635f 5f72 0600 0000 720d 0000  __doc__r....r...
-000001f0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00000200: 720c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000210: 0000 0073 0600 0000 0402 0805 0c02       ...s..........
+00000150: 720b 0000 00fa 702f 6269 6f74 6563 682f  r.....p/biotech/
+00000160: 7665 6e75 6573 2f73 7461 6765 732f 6269  venues/stages/bi
+00000170: 6f74 6563 682f 7072 6f63 6564 7572 6573  otech/procedures
+00000180: 2f68 6561 6c74 685f 7363 616e 2f70 726f  /health_scan/pro
+00000190: 6365 7373 2f6d 6f64 756c 6573 2f5f 5f68  cess/modules/__h
+000001a0: 6561 6c74 685f 7363 616e 5f75 7469 6c69  ealth_scan_utili
+000001b0: 7469 6573 2f66 6f72 6d61 745f 7265 6c5f  ties/format_rel_
+000001c0: 7061 7468 2e70 79da 0f66 6f72 6d61 745f  path.py..format_
+000001d0: 7265 6c5f 7061 7468 0a00 0000 730a 0000  rel_path....s...
+000001e0: 0018 010e 0104 0404 fe04 0272 0d00 0000  ...........r....
+000001f0: 2903 da07 5f5f 646f 635f 5f72 0600 0000  )...__doc__r....
+00000200: 720d 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
+00000210: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
+00000220: 6c65 3e01 0000 0073 0600 0000 0402 0805  le>....s........
+00000230: 0c02                                     ..
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/on.py` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/on.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 '''
-	from biotech.procedures.implicit_procedure.on import implicit_procedure_on
-	implicit_procedure_on ()
+	from biotech.procedures.aggregator_procedure.on import aggregator_procedure_on
+	aggregator_procedure_on ()
 '''
 
 '''
 	picks:
 		( ) sequentially
 		( ) simultaneously
 		( ) one
@@ -13,46 +13,53 @@
 
 
 
 '''
 	This script starts the keg process.
 '''
 
+#----
+#
 from botanist.cycle.presents import presents as cycle_presents
 import botanist.processes.multiple as multi_proc
 import botanist.cycle.loops as cycle_loops
 import botanist.ports_v2.available as available_port
-
+#
 from biotech.topics.process_on.p_expect import process_on
 from biotech.topics.process_on.p_expect.implicit import process_on_implicit
-
-from .paths import find_implicit_procedure_paths
-		
-# ----
-
+from biotech.topics.show.variable import show_variable
+#
+from .paths import find_aggregator_procedure_paths
+#
+#
 import pexpect
 import rich
-
-# ----
-
+#
+#
 import sys
 import json
 import os
 from fractions import Fraction
 import time
+#
+#----
 
-# ----
-
-def implicit_procedure_on (
+def aggregator_procedure_on (
 	port,
 	packet
 ):
+	show_variable ("""
+	
+	aggregator_procedure_on
+	
+	""")
+
 	limit_start = 25000
 		
-	path_of_the_scan_process = find_implicit_procedure_paths ()
+	path_of_the_scan_process = find_aggregator_procedure_paths ()
 	process_string = (
 		f'''python3 { path_of_the_scan_process } keg open --port { port }'''
 	)
 	
 	process_environment = os.environ.copy ()
 	process_environment ["PYTHONPATH"] = ":".join ([
 		* sys.path
@@ -63,24 +70,16 @@
 		
 		CWD = None,
 		env = process_environment,
 		name = "aggregator"
 	)
 	
 	time.sleep (1)
-	print ('the implicit procedure:', the_venture)
+	show_variable ({
+		'the aggregator procedure:': the_venture
+	}, mode = "show")
 
 	return the_venture
 
-	'''
-	procs = multi_proc.start (
-		processes = [{
-			"string": process_string,
-			"CWD": None,
-			"ENV": process_environment
-		}]
-	)
-	'''
-
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/clique/__init__.py` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pathlib
 import sys
 
 import click
 
 from keg import open_harbor
 
-def clique ():
+def keg_clique ():
 	@click.group ("keg")
 	def group ():
 		pass
 
 	'''
 		./status_check keg open --port 10000
 	'''
@@ -33,14 +33,14 @@
 	return group
 	
 def start_clique ():
 	@click.group ()
 	def group ():
 		pass
 		
-	group.add_command (clique ())
+	group.add_command (keg_clique ())
 	group ()
 
 
 
 
 #
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 14 01:25:11 2024 UTC, .py size: 554 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7730 1b66 2a02 0000  o.......w0.f*...
+00000000: 6f0d 0d0a 0000 0000 9543 2066 3202 0000  o........C f2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6402 6c06 5a06 6401 6402 6c07 5a07 6401  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c08 5a08 6401 6402 6c09 5a09 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0a 6d0b 5a0b 0100 6405 6406 8400  d.l.m.Z...d.d...
@@ -17,56 +17,57 @@
 00000100: 00a0 0164 01a1 0164 0264 0384 0083 017d  ...d...d.d.....}
 00000110: 0009 007c 00a0 0264 04a1 0174 006a 0364  ...|...d...t.j.d
 00000120: 0564 0664 078d 0264 0864 0984 0083 0183  .d.d...d.d......
 00000130: 017d 017c 0053 0029 0a4e da03 6b65 6763  .}.|.S.).N..kegc
 00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000150: 0100 0000 5300 0000 f304 0000 0064 0053  ....S........d.S
 00000160: 00a9 014e a900 720a 0000 0072 0a00 0000  ...N..r....r....
-00000170: 720a 0000 00fa 532f 766f 6c74 732f 7665  r.....S/volts/ve
-00000180: 6e75 6573 2f73 7461 6765 732f 766f 6c74  nues/stages/volt
-00000190: 732f 7072 6f63 6564 7572 6573 2f69 6d70  s/procedures/imp
-000001a0: 6c69 6369 745f 7072 6f63 6564 7572 652f  licit_procedure/
-000001b0: 7072 6f63 6573 732f 636c 6971 7565 2f5f  process/clique/_
-000001c0: 5f69 6e69 745f 5f2e 7079 da05 6772 6f75  _init__.py..grou
-000001d0: 7012 0000 00f3 0200 0000 0402 7a15 636c  p...........z.cl
-000001e0: 6971 7565 2e3c 6c6f 6361 6c73 3e2e 6772  ique.<locals>.gr
-000001f0: 6f75 70da 046f 7065 6e7a 062d 2d70 6f72  oup..openz.--por
-00000200: 7454 2901 da08 7265 7175 6972 6564 6301  tT)...requiredc.
-00000210: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000220: 0000 0053 0000 0073 0e00 0000 7400 7c00  ...S...s....t.|.
-00000230: 6401 8d01 0100 6400 5300 2902 4ea9 01da  d.....d.S.).N...
-00000240: 0470 6f72 7472 0500 0000 7210 0000 0072  .portr....r....r
-00000250: 0a00 0000 720a 0000 0072 0b00 0000 720e  ....r....r....r.
-00000260: 0000 0019 0000 0073 0600 0000 0203 0201  .......s........
-00000270: 0aff 7a14 636c 6971 7565 2e3c 6c6f 6361  ..z.clique.<loca
-00000280: 6c73 3e2e 6f70 656e 2904 da05 636c 6963  ls>.open)...clic
-00000290: 6b72 0c00 0000 da07 636f 6d6d 616e 64da  kr......command.
-000002a0: 066f 7074 696f 6e29 0272 0c00 0000 720e  .option).r....r.
-000002b0: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
-000002c0: 0000 da06 636c 6971 7565 1100 0000 730e  ....clique....s.
-000002d0: 0000 0008 010a 0102 0308 030c 010c 0104  ................
-000002e0: 0672 1500 0000 6300 0000 0000 0000 0000  .r....c.........
-000002f0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00000300: 2600 0000 7400 a001 a100 6401 6402 8400  &...t.....d.d...
-00000310: 8301 7d00 7c00 a002 7403 8300 a101 0100  ..}.|...t.......
-00000320: 7c00 8300 0100 6400 5300 2903 4e63 0000  |.....d.S.).Nc..
-00000330: 0000 0000 0000 0000 0000 0000 0000 0100  ................
-00000340: 0000 5300 0000 7208 0000 0072 0900 0000  ..S...r....r....
-00000350: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00000360: 0a00 0000 720b 0000 0072 0c00 0000 2400  ....r....r....$.
-00000370: 0000 720d 0000 007a 1b73 7461 7274 5f63  ..r....z.start_c
-00000380: 6c69 7175 652e 3c6c 6f63 616c 733e 2e67  lique.<locals>.g
-00000390: 726f 7570 2904 7212 0000 0072 0c00 0000  roup).r....r....
-000003a0: da0b 6164 645f 636f 6d6d 616e 6472 1500  ..add_commandr..
-000003b0: 0000 2901 720c 0000 0072 0a00 0000 720a  ..).r....r....r.
-000003c0: 0000 0072 0b00 0000 da0c 7374 6172 745f  ...r......start_
-000003d0: 636c 6971 7565 2300 0000 7308 0000 0006  clique#...s.....
-000003e0: 010a 010c 030a 0172 1700 0000 290e da07  .......r....)...
-000003f0: 5f5f 646f 635f 5fda 046a 736f 6eda 076f  __doc__..json..o
-00000400: 732e 7061 7468 7202 0000 0072 0300 0000  s.pathr....r....
-00000410: 7204 0000 00da 026f 73da 0770 6174 686c  r......os..pathl
-00000420: 6962 da03 7379 7372 1200 0000 7207 0000  ib..sysr....r...
-00000430: 0072 0600 0000 7215 0000 0072 1700 0000  .r....r....r....
-00000440: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
-00000450: 0b00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000460: 0000 7314 0000 0004 0308 0314 0108 0108  ..s.............
-00000470: 0108 0108 020c 0208 020c 12              ...........
+00000170: 720a 0000 00fa 572f 6269 6f74 6563 682f  r.....W/biotech/
+00000180: 7665 6e75 6573 2f73 7461 6765 732f 6269  venues/stages/bi
+00000190: 6f74 6563 682f 7072 6f63 6564 7572 6573  otech/procedures
+000001a0: 2f69 6d70 6c69 6369 745f 7072 6f63 6564  /implicit_proced
+000001b0: 7572 652f 7072 6f63 6573 732f 636c 6971  ure/process/cliq
+000001c0: 7565 2f5f 5f69 6e69 745f 5f2e 7079 da05  ue/__init__.py..
+000001d0: 6772 6f75 7012 0000 00f3 0200 0000 0402  group...........
+000001e0: 7a19 6b65 675f 636c 6971 7565 2e3c 6c6f  z.keg_clique.<lo
+000001f0: 6361 6c73 3e2e 6772 6f75 70da 046f 7065  cals>.group..ope
+00000200: 6e7a 062d 2d70 6f72 7454 2901 da08 7265  nz.--portT)...re
+00000210: 7175 6972 6564 6301 0000 0000 0000 0000  quiredc.........
+00000220: 0000 0001 0000 0003 0000 0053 0000 0073  ...........S...s
+00000230: 0e00 0000 7400 7c00 6401 8d01 0100 6400  ....t.|.d.....d.
+00000240: 5300 2902 4ea9 01da 0470 6f72 7472 0500  S.).N....portr..
+00000250: 0000 7210 0000 0072 0a00 0000 720a 0000  ..r....r....r...
+00000260: 0072 0b00 0000 720e 0000 0019 0000 0073  .r....r........s
+00000270: 0600 0000 0203 0201 0aff 7a18 6b65 675f  ..........z.keg_
+00000280: 636c 6971 7565 2e3c 6c6f 6361 6c73 3e2e  clique.<locals>.
+00000290: 6f70 656e 2904 da05 636c 6963 6b72 0c00  open)...clickr..
+000002a0: 0000 da07 636f 6d6d 616e 64da 066f 7074  ....command..opt
+000002b0: 696f 6e29 0272 0c00 0000 720e 0000 0072  ion).r....r....r
+000002c0: 0a00 0000 720a 0000 0072 0b00 0000 da0a  ....r....r......
+000002d0: 6b65 675f 636c 6971 7565 1100 0000 730e  keg_clique....s.
+000002e0: 0000 0008 010a 0102 0308 030c 010c 0104  ................
+000002f0: 0672 1500 0000 6300 0000 0000 0000 0000  .r....c.........
+00000300: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+00000310: 2600 0000 7400 a001 a100 6401 6402 8400  &...t.....d.d...
+00000320: 8301 7d00 7c00 a002 7403 8300 a101 0100  ..}.|...t.......
+00000330: 7c00 8300 0100 6400 5300 2903 4e63 0000  |.....d.S.).Nc..
+00000340: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00000350: 0000 5300 0000 7208 0000 0072 0900 0000  ..S...r....r....
+00000360: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
+00000370: 0a00 0000 720b 0000 0072 0c00 0000 2400  ....r....r....$.
+00000380: 0000 720d 0000 007a 1b73 7461 7274 5f63  ..r....z.start_c
+00000390: 6c69 7175 652e 3c6c 6f63 616c 733e 2e67  lique.<locals>.g
+000003a0: 726f 7570 2904 7212 0000 0072 0c00 0000  roup).r....r....
+000003b0: da0b 6164 645f 636f 6d6d 616e 6472 1500  ..add_commandr..
+000003c0: 0000 2901 720c 0000 0072 0a00 0000 720a  ..).r....r....r.
+000003d0: 0000 0072 0b00 0000 da0c 7374 6172 745f  ...r......start_
+000003e0: 636c 6971 7565 2300 0000 7308 0000 0006  clique#...s.....
+000003f0: 010a 010c 030a 0172 1700 0000 290e da07  .......r....)...
+00000400: 5f5f 646f 635f 5fda 046a 736f 6eda 076f  __doc__..json..o
+00000410: 732e 7061 7468 7202 0000 0072 0300 0000  s.pathr....r....
+00000420: 7204 0000 00da 026f 73da 0770 6174 686c  r......os..pathl
+00000430: 6962 da03 7379 7372 1200 0000 7207 0000  ib..sysr....r...
+00000440: 0072 0600 0000 7215 0000 0072 1700 0000  .r....r....r....
+00000450: 720a 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
+00000460: 0b00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000470: 0000 7314 0000 0004 0308 0314 0108 0108  ..s.............
+00000480: 0108 0108 020c 0208 020c 12              ...........
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 20:48:34 2024 UTC, .py size: 3005 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,147 +1,172 @@
-00000000: 6f0d 0d0a 0000 0000 22e4 1e66 bd0b 0000  o......."..f....
+00000000: 6f0d 0d0a 0000 0000 2dc6 2266 580e 0000  o.......-."fX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
-00000060: 5a07 6400 6401 6c08 5a08 6400 6401 6c09  Z.d.d.l.Z.d.d.l.
-00000070: 5a09 6400 6403 6c0a 6d0b 5a0b 6d0c 5a0c  Z.d.d.l.m.Z.m.Z.
-00000080: 0100 6400 6401 6c0d 5a0d 6400 6404 6c0e  ..d.d.l.Z.d.d.l.
-00000090: 6d0f 5a0f 0100 6400 6405 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
-000000a0: 0100 6400 6406 6c12 6d13 5a13 6d14 5a14  ..d.d.l.m.Z.m.Z.
-000000b0: 0100 6400 6407 6c15 6d16 5a16 0100 0901  ..d.d.l.m.Z.....
-000000c0: 640a 6408 6409 8401 5a17 6401 5300 290b  d.d.d...Z.d.S.).
-000000d0: e900 0000 004e 2903 da07 6469 726e 616d  .....N)...dirnam
-000000e0: 65da 046a 6f69 6eda 086e 6f72 6d70 6174  e..join..normpat
-000000f0: 6829 02da 0546 6c61 736b da07 7265 7175  h)...Flask..requ
-00000100: 6573 7429 01da 1671 7565 7565 5f63 6170  est)...queue_cap
-00000110: 6163 6974 795f 6c69 6d69 7465 7229 01da  acity_limiter)..
-00000120: 1474 7572 6e5f 6f6e 5f68 6561 6c74 685f  .turn_on_health_
-00000130: 6368 6563 6b29 02da 1c69 6d70 6c69 6369  check)...implici
-00000140: 745f 7072 6f63 6564 7572 655f 7661 7269  t_procedure_vari
-00000150: 6162 6c65 73da 1773 6574 7570 5f69 6e74  ables..setup_int
-00000160: 6572 6e61 6c5f 7374 6174 7573 6573 2901  ernal_statuses).
-00000170: da0b 666f 726d 6174 5f70 6174 6863 0200  ..format_pathc..
-00000180: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000190: 0000 0300 0000 7320 0000 007c 006a 0064  ......s ...|.j.d
-000001a0: 0164 0267 0164 038d 0287 0066 0164 0464  .d.g.d.....f.d.d
-000001b0: 0584 0883 017d 0264 0053 0029 064e 7a06  .....}.d.S.).Nz.
-000001c0: 2f70 6174 6873 da05 5041 5443 4829 01da  /paths..PATCH)..
-000001d0: 076d 6574 686f 6473 6300 0000 0000 0000  .methodsc.......
-000001e0: 0000 0000 0009 0000 0005 0000 0013 0000  ................
-000001f0: 0073 d600 0000 7400 6401 8301 0100 0900  .s....t.d.......
-00000200: 7401 a002 7403 6a04 a005 6402 a101 a101  t...t.j...d.....
-00000210: 7d00 7406 6a07 6403 7c00 6901 6404 8d01  }.t.j.d.|.i.d...
-00000220: 0100 7c00 6405 1900 7d01 7c00 6406 1900  ..|.d...}.|.d...
-00000230: 8900 7c00 6407 1900 8901 7c00 6408 1900  ..|.d.....|.d...
-00000240: 7d02 7c00 6409 1900 7d03 7c00 640a 1900  }.|.d...}.|.d...
-00000250: 7d04 7c00 640b 1900 7d05 7c00 7408 640c  }.|.d...}.|.t.d.
-00000260: 3c00 7c00 640d 1900 7408 640e 3c00 0900  <.|.d...t.d.<...
-00000270: 7409 7c01 8801 8302 0100 640f 7408 6410  t.|.......d.t.d.
-00000280: 3c00 8702 8700 8701 6603 6411 6412 8408  <.......f.d.d...
-00000290: 7d06 7c02 725f 740a 7c03 7c01 7c06 6413  }.|.r_t.|.|.|.d.
-000002a0: 8d03 7d07 7400 6414 7c07 8302 0100 0900  ..}.t.d.|.......
-000002b0: 6415 5300 7c01 4400 5d06 7d08 7c06 7c08  d.S.|.D.].}.|.|.
-000002c0: 8301 0100 7161 0900 6415 5300 2916 4e7a  ....qa..d.S.).Nz
-000002d0: 1040 205b 7061 7463 685d 202f 7061 7468  .@ [patch] /path
-000002e0: 73da 0475 7466 387a 1070 6174 6873 2074  s..utf8z.paths t
-000002f0: 6865 5f70 6163 6b65 7429 01da 0464 6174  he_packet)...dat
-00000300: 61da 1273 7461 7475 735f 6368 6563 6b5f  a..status_check_
-00000310: 7061 7468 73da 0c6d 6f64 756c 655f 7061  paths..module_pa
-00000320: 7468 73da 0d72 656c 6174 6976 655f 7061  ths..relative_pa
-00000330: 7468 da0c 7369 6d75 6c74 616e 656f 7573  th..simultaneous
-00000340: da15 7369 6d75 6c74 616e 656f 7573 5f63  ..simultaneous_c
-00000350: 6170 6163 6974 79da 0662 6566 6f72 65da  apacity..before.
-00000360: 0561 6674 6572 da0f 696e 7472 6f5f 7661  .after..intro_va
-00000370: 7269 6162 6c65 73da 1074 6865 5f69 6e74  riables..the_int
-00000380: 726f 5f68 6172 626f 72da 0c69 6e74 726f  ro_harbor..intro
-00000390: 5f68 6172 626f 72da 0379 6573 da17 696e  _harbor..yes..in
-000003a0: 7465 726e 616c 5f73 7461 7475 7365 735f  ternal_statuses_
-000003b0: 6275 696c 7463 0100 0000 0000 0000 0000  builtc..........
-000003c0: 0000 0300 0000 0600 0000 1300 0000 736e  ..............sn
-000003d0: 0000 0074 0074 01a0 01a1 0083 017d 0174  ...t.t.......}.t
-000003e0: 027c 0088 0188 0264 0188 0069 0164 029c  .|.....d...i.d..
-000003f0: 0464 038d 017d 0274 0383 0001 0074 0364  .d...}.t.....t.d
-00000400: 047c 0283 0201 0074 0383 0001 007c 0274  .|.....t.....|.t
-00000410: 0464 0519 0074 057c 0088 0283 0219 0064  .d...t.|.......d
-00000420: 063c 007c 0174 0464 0519 0074 057c 0088  .<.|.t.d...t.|..
-00000430: 0283 0219 0064 0719 0064 083c 007c 0253  .....d...d.<.|.S
-00000440: 0029 094e da04 706f 7274 2904 da11 7374  .).N..port)...st
-00000450: 6174 7573 5f63 6865 636b 5f70 6174 6872  atus_check_pathr
-00000460: 1100 0000 7212 0000 00da 1269 6d70 6c69  ....r......impli
-00000470: 6369 745f 7072 6f63 6564 7572 6529 01da  cit_procedure)..
-00000480: 0670 6163 6b65 747a 0974 6865 5f73 6361  .packetz.the_sca
-00000490: 6e3a da11 696e 7465 726e 616c 5f73 7461  n:..internal_sta
-000004a0: 7475 7365 73da 0770 726f 6365 7373 da05  tuses..process..
-000004b0: 7469 6d65 73da 0773 7461 7274 6564 2906  times..started).
-000004c0: da03 7374 72da 0474 696d 6572 0800 0000  ..str..timer....
-000004d0: da05 7072 696e 7472 0900 0000 720b 0000  ..printr....r...
-000004e0: 0029 0372 1d00 0000 da0a 7374 6172 745f  .).r......start_
-000004f0: 7469 6d65 da08 7468 655f 7363 616e 2903  time..the_scan).
-00000500: da17 696d 706c 6963 6974 5f70 726f 6365  ..implicit_proce
-00000510: 6475 7265 5f70 6f72 7472 1100 0000 7212  dure_portr....r.
-00000520: 0000 00a9 00fa 5e2f 6269 6f74 6563 682f  ......^/biotech/
-00000530: 7665 6e75 6573 2f73 7461 6765 732f 6269  venues/stages/bi
-00000540: 6f74 6563 682f 7072 6f63 6564 7572 6573  otech/procedures
-00000550: 2f69 6d70 6c69 6369 745f 7072 6f63 6564  /implicit_proced
-00000560: 7572 652f 7072 6f63 6573 732f 6b65 672f  ure/process/keg/
-00000570: 7370 6163 6573 2f70 6174 6873 5f70 6174  spaces/paths_pat
-00000580: 6368 2e70 79da 0776 656e 7475 7265 5800  ch.py..ventureX.
-00000590: 0000 733e 0000 000c 0102 0202 0202 0202  ..s>............
-000005a0: 0104 0302 ff04 fa06 ff06 0d0a 0106 0102  ................
-000005b0: 0902 fa02 0102 ff08 0302 fd02 0502 fb02  ................
-000005c0: 1102 f802 0102 ff08 0302 fd02 0502 fb02  ................
-000005d0: 0702 f904 0a7a 3170 6174 6873 5f70 6174  .....z1paths_pat
-000005e0: 6368 2e3c 6c6f 6361 6c73 3e2e 7061 7468  ch.<locals>.path
-000005f0: 735f 7061 7463 682e 3c6c 6f63 616c 733e  s_patch.<locals>
-00000600: 2e76 656e 7475 7265 2903 da08 6361 7061  .venture)...capa
-00000610: 6369 7479 da05 6974 656d 73da 046d 6f76  city..items..mov
-00000620: 657a 2071 7565 7565 5f63 6170 6163 6974  ez queue_capacit
-00000630: 795f 6c69 6d69 7465 7220 7072 6f63 6565  y_limiter procee
-00000640: 6473 3ada 0872 6563 6569 7665 6429 0b72  ds:..received).r
-00000650: 2600 0000 da04 6a73 6f6e da05 6c6f 6164  &.....json..load
-00000660: 7372 0600 0000 720f 0000 00da 0664 6563  sr....r......dec
-00000670: 6f64 65da 0472 6963 68da 0a70 7269 6e74  ode..rich..print
-00000680: 5f6a 736f 6e72 0900 0000 720a 0000 0072  _jsonr....r....r
-00000690: 0700 0000 2909 da0a 7468 655f 7061 636b  ....)...the_pack
-000006a0: 6574 7210 0000 0072 1300 0000 7214 0000  etr....r....r...
-000006b0: 0072 1500 0000 7216 0000 0072 2c00 0000  .r....r....r,...
-000006c0: da08 7072 6f63 6565 6473 721d 0000 00a9  ..proceedsr.....
-000006d0: 0172 2900 0000 2902 7211 0000 0072 1200  .r)...).r....r..
-000006e0: 0000 722b 0000 00da 0b70 6174 6873 5f70  ..r+.....paths_p
-000006f0: 6174 6368 1d00 0000 7346 0000 0008 0202  atch....sF......
-00000700: 0312 1004 0104 0108 ff08 0608 0208 0108  ................
-00000710: 0208 0108 0208 0108 040c 0102 0402 0302  ................
-00000720: 0102 0104 fe08 0410 0604 2c02 0102 0102  ..........,.....
-00000730: 0102 0106 fd0a 0602 0604 0408 f90a 0102  ................
-00000740: 0204 047a 2070 6174 6873 5f70 6174 6368  ...z paths_patch
-00000750: 2e3c 6c6f 6361 6c73 3e2e 7061 7468 735f  .<locals>.paths_
-00000760: 7061 7463 6829 01da 0572 6f75 7465 2903  patch)...route).
-00000770: da03 6170 7072 2900 0000 7239 0000 0072  ..appr)...r9...r
-00000780: 2a00 0000 7238 0000 0072 2b00 0000 7239  *...r8...r+...r9
-00000790: 0000 0018 0000 0073 0400 0000 0e05 1201  .......s........
-000007a0: 7239 0000 0029 014e 2918 7231 0000 00da  r9...).N).r1....
-000007b0: 0770 6174 686c 6962 da02 6f73 da07 6f73  .pathlib..os..os
-000007c0: 2e70 6174 6872 0200 0000 7203 0000 0072  .pathr....r....r
-000007d0: 0400 0000 da03 7379 73da 0974 6872 6561  ......sys..threa
-000007e0: 6469 6e67 7225 0000 00da 0566 6c61 736b  dingr%.....flask
-000007f0: 7205 0000 0072 0600 0000 7234 0000 00da  r....r....r4....
-00000800: 2c62 696f 7465 6368 2e74 6f70 6963 732e  ,biotech.topics.
-00000810: 7175 6575 6573 2e71 7565 7565 5f63 6170  queues.queue_cap
-00000820: 6163 6974 795f 6c69 6d69 7465 7272 0700  acity_limiterr..
-00000830: 0000 da21 6269 6f74 6563 682e 7072 6f63  ...!biotech.proc
-00000840: 6564 7572 6573 2e68 6561 6c74 685f 7363  edures.health_sc
-00000850: 616e 2e6f 6e72 0800 0000 da37 6269 6f74  an.onr.....7biot
-00000860: 6563 682e 7072 6f63 6564 7572 6573 2e69  ech.procedures.i
-00000870: 6d70 6c69 6369 745f 7072 6f63 6564 7572  mplicit_procedur
-00000880: 652e 7072 6f63 6573 732e 7661 7269 6162  e.process.variab
-00000890: 6c65 7372 0900 0000 720a 0000 00da 3f62  lesr....r.....?b
-000008a0: 696f 7465 6368 2e70 726f 6365 6475 7265  iotech.procedure
-000008b0: 732e 696d 706c 6963 6974 5f70 726f 6365  s.implicit_proce
-000008c0: 6475 7265 2e70 726f 6365 7373 2e6d 6f76  dure.process.mov
-000008d0: 6573 2e66 6f72 6d61 745f 7061 7468 720b  es.format_pathr.
-000008e0: 0000 0072 3900 0000 722a 0000 0072 2a00  ...r9...r*...r*.
-000008f0: 0000 722a 0000 0072 2b00 0000 da08 3c6d  ..r*...r+.....<m
-00000900: 6f64 756c 653e 0100 0000 731e 0000 0008  odule>....s.....
-00000910: 0308 0108 0114 0108 0108 0108 0110 0308  ................
-00000920: 010c 020c 0110 020c 0102 070e fd         .............
+00000020: 0003 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
+00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
+00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
+00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 0100 6401 6407 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
+00000080: 0100 6401 6408 6c0f 5a0f 6401 6408 6c10  ..d.d.l.Z.d.d.l.
+00000090: 5a10 6401 6408 6c11 5a11 6401 6408 6c12  Z.d.d.l.Z.d.d.l.
+000000a0: 5a12 6401 6409 6c13 6d14 5a14 6d15 5a15  Z.d.d.l.m.Z.m.Z.
+000000b0: 6d16 5a16 0100 6401 6408 6c17 5a17 6401  m.Z...d.d.l.Z.d.
+000000c0: 6408 6c18 5a18 6401 6408 6c19 5a19 0908  d.l.Z.d.d.l.Z...
+000000d0: 640c 640a 640b 8401 5a1a 6408 5300 290d  d.d.d...Z.d.S.).
+000000e0: 7a34 0a09 6465 7363 7269 7074 696f 6e3a  z4..description:
+000000f0: 0a09 0954 6869 7320 6973 2077 6861 7420  ...This is what 
+00000100: 7374 6172 7473 2074 6865 2061 6767 7265  starts the aggre
+00000110: 6761 746f 720a e900 0000 0029 02da 1461  gator......)...a
+00000120: 6767 7265 6761 746f 725f 7661 7269 6162  ggregator_variab
+00000130: 6c65 73da 1773 6574 7570 5f69 6e74 6572  les..setup_inter
+00000140: 6e61 6c5f 7374 6174 7573 6573 2901 da0b  nal_statuses)...
+00000150: 666f 726d 6174 5f70 6174 6829 01da 0d73  format_path)...s
+00000160: 686f 775f 7661 7269 6162 6c65 2901 da16  how_variable)...
+00000170: 7175 6575 655f 6361 7061 6369 7479 5f6c  queue_capacity_l
+00000180: 696d 6974 6572 2901 da14 7475 726e 5f6f  imiter)...turn_o
+00000190: 6e5f 6865 616c 7468 5f63 6865 636b 2902  n_health_check).
+000001a0: da05 466c 6173 6bda 0772 6571 7565 7374  ..Flask..request
+000001b0: 4e29 03da 0764 6972 6e61 6d65 da04 6a6f  N)...dirname..jo
+000001c0: 696e da08 6e6f 726d 7061 7468 6302 0000  in..normpathc...
+000001d0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+000001e0: 0003 0000 0073 2000 0000 7c00 6a00 6401  .....s ...|.j.d.
+000001f0: 6402 6701 6403 8d02 8700 6601 6404 6405  d.g.d.....f.d.d.
+00000200: 8408 8301 7d02 6400 5300 2906 4e7a 062f  ....}.d.S.).Nz./
+00000210: 7061 7468 73da 0550 4154 4348 2901 da07  paths..PATCH)...
+00000220: 6d65 7468 6f64 7363 0000 0000 0000 0000  methodsc........
+00000230: 0000 0000 0700 0000 0500 0000 1300 0000  ................
+00000240: 73d0 0000 0009 0074 00a0 0174 026a 03a0  s......t...t.j..
+00000250: 0464 01a1 01a1 017d 0074 0564 027c 0069  .d.....}.t.d.|.i
+00000260: 0183 0101 007c 0064 0319 007d 017c 0064  .....|.d...}.|.d
+00000270: 0419 0089 007c 0064 0519 0089 017c 0064  .....|.d.....|.d
+00000280: 0619 007d 027c 0064 0719 007d 037c 0074  ...}.|.d...}.|.t
+00000290: 0664 083c 007c 0064 0919 0074 0664 0a3c  .d.<.|.d...t.d.<
+000002a0: 0064 0b7c 0076 0072 387c 0064 0b19 0074  .d.|.v.r8|.d...t
+000002b0: 0664 0b3c 0009 0074 077c 0188 0183 0201  .d.<...t.|......
+000002c0: 0064 0c74 0664 0d3c 0087 0287 0087 0166  .d.t.d.<.......f
+000002d0: 0364 0e64 0f84 087d 047c 0272 5d74 087c  .d.d...}.|.r]t.|
+000002e0: 037c 017c 0464 108d 037d 0574 0564 117c  .|.|.d...}.t.d.|
+000002f0: 0569 0164 1264 138d 0201 0064 1453 007c  .i.d.d.....d.S.|
+00000300: 0144 005d 067d 067c 047c 0683 0101 0071  .D.].}.|.|.....q
+00000310: 5f64 1453 0029 157a 570a 0909 7368 6f77  _d.S.).zW...show
+00000320: 5f76 6172 6961 626c 6520 287b 0a09 0909  _variable ({....
+00000330: 2264 6f63 6b22 3a20 7b0a 0909 0909 2276  "dock": {....."v
+00000340: 6572 6222 3a20 2270 6174 6368 222c 0a09  erb": "patch",..
+00000350: 0909 0922 7061 7468 223a 2022 2f70 6174  ..."path": "/pat
+00000360: 6873 220a 0909 097d 0a09 097d 290a 0909  hs"....}...})...
+00000370: da04 7574 6638 7a11 2f70 6174 6873 2074  ..utf8z./paths t
+00000380: 6865 5f70 6163 6b65 74da 1273 7461 7475  he_packet..statu
+00000390: 735f 6368 6563 6b5f 7061 7468 73da 0c6d  s_check_paths..m
+000003a0: 6f64 756c 655f 7061 7468 73da 0d72 656c  odule_paths..rel
+000003b0: 6174 6976 655f 7061 7468 da0c 7369 6d75  ative_path..simu
+000003c0: 6c74 616e 656f 7573 da15 7369 6d75 6c74  ltaneous..simult
+000003d0: 616e 656f 7573 5f63 6170 6163 6974 79da  aneous_capacity.
+000003e0: 0f69 6e74 726f 5f76 6172 6961 626c 6573  .intro_variables
+000003f0: da10 7468 655f 696e 7472 6f5f 6861 7262  ..the_intro_harb
+00000400: 6f72 da0c 696e 7472 6f5f 6861 7262 6f72  or..intro_harbor
+00000410: da0d 7265 636f 7264 735f 6c65 7665 6cda  ..records_level.
+00000420: 0379 6573 da17 696e 7465 726e 616c 5f73  .yes..internal_s
+00000430: 7461 7475 7365 735f 6275 696c 7463 0100  tatuses_builtc..
+00000440: 0000 0000 0000 0000 0000 0400 0000 0600  ................
+00000450: 0000 1300 0000 73be 0000 0074 007c 0088  ......s....t.|..
+00000460: 0283 027d 0164 0174 0164 0219 007c 0119  ...}.d.t.d...|..
+00000470: 0064 0319 0064 043c 0074 0274 03a0 03a1  .d...d.<.t.t....
+00000480: 0083 0174 0164 0219 007c 0119 0064 0519  ...t.d...|...d..
+00000490: 0064 063c 0074 0274 03a0 03a1 0083 017d  .d.<.t.t.......}
+000004a0: 0274 0464 077c 0088 0188 0264 089c 0369  .t.d.|.....d...i
+000004b0: 0183 0101 0074 057c 0088 0188 0264 0988  .....t.|.....d..
+000004c0: 0069 0164 0a9c 0464 0b8d 017d 0374 0464  .i.d...d...}.t.d
+000004d0: 0c7c 0369 0164 0d64 0e8d 0201 007c 0374  .|.i.d.d.....|.t
+000004e0: 0164 0219 007c 0119 0064 0f3c 007c 0274  .d...|...d.<.|.t
+000004f0: 0164 0219 007c 0119 0064 0519 0064 103c  .d...|...d...d.<
+00000500: 0064 0174 0164 0219 007c 0119 0064 0319  .d.t.d...|...d..
+00000510: 0064 113c 007c 0353 0029 124e 7219 0000  .d.<.|.S.).Nr...
+00000520: 00da 1169 6e74 6572 6e61 6c5f 7374 6174  ...internal_stat
+00000530: 7573 6573 da0b 6f63 6375 7272 656e 6365  uses..occurrence
+00000540: 737a 1c73 6361 6e20 7072 6f63 6573 7320  sz.scan process 
+00000550: 7665 6e74 7572 6520 7374 6172 7465 64da  venture started.
+00000560: 0574 696d 6573 7a0f 7665 6e74 7572 6520  .timesz.venture 
+00000570: 7374 6172 7465 647a 0e73 7461 7274 696e  startedz.startin
+00000580: 6720 7363 616e 3a29 03da 1173 7461 7475  g scan:)...statu
+00000590: 735f 6368 6563 6b5f 7061 7468 7211 0000  s_check_pathr...
+000005a0: 0072 1200 0000 da04 706f 7274 2904 721e  .r......port).r.
+000005b0: 0000 0072 1100 0000 7212 0000 00da 1461  ...r....r......a
+000005c0: 6767 7265 6761 746f 725f 7072 6f63 6564  ggregator_proced
+000005d0: 7572 6529 01da 0670 6163 6b65 747a 0974  ure)...packetz.t
+000005e0: 6865 5f73 6361 6e3a da04 7368 6f77 a901  he_scan:..show..
+000005f0: da04 6d6f 6465 da07 7072 6f63 6573 73da  ..mode..process.
+00000600: 0773 7461 7274 6564 7a14 7363 616e 2070  .startedz.scan p
+00000610: 726f 6365 7373 2073 7461 7274 6564 2906  rocess started).
+00000620: 7204 0000 0072 0200 0000 da03 7374 72da  r....r......str.
+00000630: 0474 696d 6572 0500 0000 7207 0000 0029  .timer....r....)
+00000640: 0472 1e00 0000 da08 7265 6c5f 7061 7468  .r......rel_path
+00000650: da0a 7374 6172 745f 7469 6d65 da08 7468  ..start_time..th
+00000660: 655f 7363 616e 2903 da19 6167 6772 6567  e_scan)...aggreg
+00000670: 6174 6f72 5f70 726f 6365 6475 7265 5f70  ator_procedure_p
+00000680: 6f72 7472 1100 0000 7212 0000 00a9 00fa  ortr....r.......
+00000690: 602f 6269 6f74 6563 682f 7665 6e75 6573  `/biotech/venues
+000006a0: 2f73 7461 6765 732f 6269 6f74 6563 682f  /stages/biotech/
+000006b0: 7072 6f63 6564 7572 6573 2f61 6767 7265  procedures/aggre
+000006c0: 6761 746f 725f 7072 6f63 6564 7572 652f  gator_procedure/
+000006d0: 7072 6f63 6573 732f 6b65 672f 7370 6163  process/keg/spac
+000006e0: 6573 2f70 6174 6873 5f70 6174 6368 2e70  es/paths_patch.p
+000006f0: 79da 0776 656e 7475 7265 6a00 0000 7338  y..venturej...s8
+00000700: 0000 000a 0114 021c 010c 0202 0202 0102  ................
+00000710: 0102 0102 0104 fd06 ff02 0802 0202 0202  ................
+00000720: 0104 0302 ff04 fa06 ff02 0d04 0102 ff02  ................
+00000730: 0206 fe10 0414 0114 0104 027a 3170 6174  ...........z1pat
+00000740: 6873 5f70 6174 6368 2e3c 6c6f 6361 6c73  hs_patch.<locals
+00000750: 3e2e 7061 7468 735f 7061 7463 682e 3c6c  >.paths_patch.<l
+00000760: 6f63 616c 733e 2e76 656e 7475 7265 2903  ocals>.venture).
+00000770: da08 6361 7061 6369 7479 da05 6974 656d  ..capacity..item
+00000780: 73da 046d 6f76 657a 1f71 7565 7565 5f63  s..movez.queue_c
+00000790: 6170 6163 6974 795f 6c69 6d69 7465 7220  apacity_limiter 
+000007a0: 7072 6f63 6565 6473 7222 0000 0072 2300  proceedsr"...r#.
+000007b0: 0000 da08 7265 6365 6976 6564 2909 da04  ....received)...
+000007c0: 6a73 6f6e da05 6c6f 6164 7372 0900 0000  json..loadsr....
+000007d0: da04 6461 7461 da06 6465 636f 6465 7205  ..data..decoder.
+000007e0: 0000 0072 0200 0000 7203 0000 0072 0600  ...r....r....r..
+000007f0: 0000 2907 da0a 7468 655f 7061 636b 6574  ..)...the_packet
+00000800: 7210 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000810: 2f00 0000 da08 7072 6f63 6565 6473 721e  /.....proceedsr.
+00000820: 0000 00a9 0172 2c00 0000 2902 7211 0000  .....r,...).r...
+00000830: 0072 1200 0000 722e 0000 00da 0b70 6174  .r....r......pat
+00000840: 6873 5f70 6174 6368 2400 0000 7348 0000  hs_patch$...sH..
+00000850: 0002 0b12 1002 0104 0106 ff08 0608 0208  ................
+00000860: 0108 0208 0108 070c 0108 030c 0102 0202  ................
+00000870: 0302 0102 0104 fe08 0710 0604 2902 0102  ............)...
+00000880: 0102 0102 0106 fd02 0604 0102 ff02 0206  ................
+00000890: fe04 0908 fc0a 0104 037a 2070 6174 6873  .........z paths
+000008a0: 5f70 6174 6368 2e3c 6c6f 6361 6c73 3e2e  _patch.<locals>.
+000008b0: 7061 7468 735f 7061 7463 6829 01da 0572  paths_patch)...r
+000008c0: 6f75 7465 2903 da03 6170 7072 2c00 0000  oute)...appr,...
+000008d0: 723b 0000 0072 2d00 0000 723a 0000 0072  r;...r-...r:...r
+000008e0: 2e00 0000 723b 0000 001f 0000 0073 0400  ....r;.......s..
+000008f0: 0000 0e05 1201 723b 0000 0029 014e 291b  ......r;...).N).
+00000900: da07 5f5f 646f 635f 5fda 3962 696f 7465  ..__doc__.9biote
+00000910: 6368 2e70 726f 6365 6475 7265 732e 6167  ch.procedures.ag
+00000920: 6772 6567 6174 6f72 5f70 726f 6365 6475  gregator_procedu
+00000930: 7265 2e70 726f 6365 7373 2e76 6172 6961  re.process.varia
+00000940: 626c 6573 7202 0000 0072 0300 0000 da41  blesr....r.....A
+00000950: 6269 6f74 6563 682e 7072 6f63 6564 7572  biotech.procedur
+00000960: 6573 2e61 6767 7265 6761 746f 725f 7072  es.aggregator_pr
+00000970: 6f63 6564 7572 652e 7072 6f63 6573 732e  ocedure.process.
+00000980: 6d6f 7665 732e 666f 726d 6174 5f70 6174  moves.format_pat
+00000990: 6872 0400 0000 da1c 6269 6f74 6563 682e  hr......biotech.
+000009a0: 746f 7069 6373 2e73 686f 772e 7661 7269  topics.show.vari
+000009b0: 6162 6c65 7205 0000 00da 2c62 696f 7465  abler.....,biote
+000009c0: 6368 2e74 6f70 6963 732e 7175 6575 6573  ch.topics.queues
+000009d0: 2e71 7565 7565 5f63 6170 6163 6974 795f  .queue_capacity_
+000009e0: 6c69 6d69 7465 7272 0600 0000 da21 6269  limiterr.....!bi
+000009f0: 6f74 6563 682e 7072 6f63 6564 7572 6573  otech.procedures
+00000a00: 2e68 6561 6c74 685f 7363 616e 2e6f 6e72  .health_scan.onr
+00000a10: 0700 0000 da05 666c 6173 6b72 0800 0000  ......flaskr....
+00000a20: 7209 0000 00da 0472 6963 6872 3400 0000  r......richr4...
+00000a30: da07 7061 7468 6c69 62da 026f 73da 076f  ..pathlib..os..o
+00000a40: 732e 7061 7468 720a 0000 0072 0b00 0000  s.pathr....r....
+00000a50: 720c 0000 00da 0373 7973 da09 7468 7265  r......sys..thre
+00000a60: 6164 696e 6772 2800 0000 723b 0000 0072  adingr(...r;...r
+00000a70: 2d00 0000 722d 0000 0072 2d00 0000 722e  -...r-...r-...r.
+00000a80: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000a90: 0073 2200 0000 0401 1007 0c01 0c02 0c01  .s".............
+00000aa0: 0c01 1003 0801 0803 0801 0801 1401 0801  ................
+00000ab0: 0801 0801 0207 0efd                      ........
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 20:48:34 2024 UTC, .py size: 2942 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,127 @@
-00000000: 6f0d 0d0a 0000 0000 22e4 1e66 7e0b 0000  o......."..f~...
+00000000: 6f0d 0d0a 0000 0000 269b 2266 7b0d 0000  o.......&."f{...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
-00000030: 5a00 0900 6401 6402 6c01 6d02 5a02 0100  Z...d.d.l.m.Z...
-00000040: 6401 6403 6c03 6d04 0200 0100 6d05 5a05  d.d.l.m.....m.Z.
-00000050: 0100 0900 0900 6404 6405 8400 5a06 0900  ......d.d...Z...
-00000060: 6406 6407 8400 5a07 6403 5300 2908 7a27  d.d...Z.d.S.).z'
-00000070: 0a09 6167 6772 6567 6174 655f 7374 6174  ..aggregate_stat
-00000080: 7320 280a 0909 7061 7468 5f73 7461 7475  s (...path_statu
-00000090: 7365 730a 0929 0ae9 0000 0000 2901 da1c  ses..)......)...
-000000a0: 696d 706c 6963 6974 5f70 726f 6365 6475  implicit_procedu
-000000b0: 7265 5f76 6172 6961 626c 6573 4e63 0000  re_variablesNc..
-000000c0: 0000 0000 0000 0000 0000 0400 0000 0800  ................
-000000d0: 0000 4300 0000 734e 0000 0067 007d 0074  ..C...sN...g.}.t
-000000e0: 0064 0119 007d 017c 0144 005d 1c7d 027c  .d...}.|.D.].}.|
-000000f0: 017c 0219 0064 0219 007d 037c 0364 006b  .|...d...}.|.d.k
-00000100: 0272 1f7c 00a0 017c 0264 0364 0464 0564  .r.|...|.d.d.d.d
-00000110: 069c 04a1 0101 0071 087c 00a0 017c 03a1  .......q.|...|..
-00000120: 0101 0071 087c 0053 0029 074e da11 696e  ...q.|.S.).N..in
-00000130: 7465 726e 616c 5f73 7461 7475 7365 73da  ternal_statuses.
-00000140: 0f72 6573 756c 7473 5f6f 665f 7363 616e  .results_of_scan
-00000150: da07 6578 6974 7465 647a 3154 6865 2070  ..exittedz1The p
-00000160: 726f 6365 7373 2065 7869 7474 6564 2062  rocess exitted b
-00000170: 6566 6f72 6520 7265 7375 6c74 7320 636f  efore results co
-00000180: 756c 6420 6265 2073 656e 742e 5429 04da  uld be sent.T)..
-00000190: 0470 6174 68da 0561 6c61 726d 7a0a 616c  .path..alarmz.al
-000001a0: 6172 6d20 6e6f 7465 da06 6578 6974 6564  arm note..exited
-000001b0: 2902 7202 0000 00da 0661 7070 656e 6429  ).r......append)
-000001c0: 04da 0d70 6174 685f 7374 6174 7573 6573  ...path_statuses
-000001d0: 7203 0000 00da 0973 6361 6e5f 7061 7468  r......scan_path
-000001e0: 7204 0000 00a9 0072 0c00 0000 fa5d 2f62  r......r.....]/b
-000001f0: 696f 7465 6368 2f76 656e 7565 732f 7374  iotech/venues/st
-00000200: 6167 6573 2f62 696f 7465 6368 2f70 726f  ages/biotech/pro
-00000210: 6365 6475 7265 732f 696d 706c 6963 6974  cedures/implicit
-00000220: 5f70 726f 6365 6475 7265 2f70 726f 6365  _procedure/proce
-00000230: 7373 2f6d 6f76 6573 2f61 6767 7265 6761  ss/moves/aggrega
-00000240: 7465 5f73 7461 7473 2e70 79da 1370 6172  te_stats.py..par
-00000250: 7365 5f70 6174 685f 7374 6174 7573 6573  se_path_statuses
-00000260: 4300 0000 731a 0000 0004 0108 0208 010c  C...s...........
-00000270: 0108 0104 0102 0102 0202 0102 020a fa0c  ................
-00000280: 0a04 0272 0e00 0000 6300 0000 0000 0000  ...r....c.......
-00000290: 0000 0000 0005 0000 0007 0000 0043 0000  .............C..
-000002a0: 0073 a801 0000 7400 8300 7d00 7401 a002  .s....t...}.t...
-000002b0: 7c00 a101 7d01 7403 6401 1900 6402 1900  |...}.t.d...d...
-000002c0: 7d02 7c02 6403 6b02 726a 7c00 7c01 6404  }.|.d.k.rj|.|.d.
-000002d0: 6404 6404 6404 6405 9c02 6406 9c03 6407  d.d.d.d...d...d.
-000002e0: 9c03 7d03 7c00 4400 5d46 7d04 6408 7c04  ..}.|.D.]F}.d.|.
-000002f0: 7600 7238 7c04 6408 1900 6409 6b02 7238  v.r8|.d...d.k.r8
-00000300: 7c03 640a 1900 6408 0500 1900 6403 3700  |.d...d.....d.7.
-00000310: 0300 3c00 7121 640b 7c04 7600 7247 7c03  ..<.q!d.|.v.rG|.
-00000320: 640a 1900 640c 0500 1900 6403 3700 0300  d...d.....d.7...
-00000330: 3c00 7121 7c03 640a 1900 640d 1900 640e  <.q!|.d...d...d.
-00000340: 0500 1900 7c04 640a 1900 640e 1900 3700  ....|.d...d...7.
-00000350: 0300 3c00 7c03 640a 1900 640d 1900 640c  ..<.|.d...d...d.
-00000360: 0500 1900 7c04 640a 1900 640c 1900 3700  ....|.d...d...7.
-00000370: 0300 3c00 7121 7c03 5300 7c02 640f 6b02  ..<.q!|.S.|.d.k.
-00000380: 72cc 7c00 7c01 6404 6404 6410 9c02 6404  r.|.|.d.d.d...d.
-00000390: 6404 6405 9c02 6411 9c02 6407 9c03 7d03  d.d...d...d...}.
-000003a0: 7c00 4400 5d4a 7d04 6408 7c04 7600 7298  |.D.]J}.d.|.v.r.
-000003b0: 7c04 6408 1900 6409 6b02 7298 7c03 640a  |.d...d.k.r.|.d.
-000003c0: 1900 6412 1900 6408 0500 1900 6403 3700  ..d...d.....d.7.
-000003d0: 0300 3c00 717f 640b 7c04 7600 72a9 7c03  ..<.q.d.|.v.r.|.
-000003e0: 640a 1900 6412 1900 640c 0500 1900 6403  d...d...d.....d.
-000003f0: 3700 0300 3c00 717f 7c03 640a 1900 640d  7...<.q.|.d...d.
-00000400: 1900 640e 0500 1900 7c04 640a 1900 640e  ..d.....|.d...d.
-00000410: 1900 3700 0300 3c00 7c03 640a 1900 640d  ..7...<.|.d...d.
-00000420: 1900 640c 0500 1900 7c04 640a 1900 640c  ..d.....|.d...d.
-00000430: 1900 3700 0300 3c00 717f 7c03 5300 7404  ..7...<.q.|.S.t.
-00000440: 6413 7c02 9b00 6414 9d03 8301 8201 2915  d.|...d.......).
-00000450: 4eda 0f69 6e74 726f 5f76 6172 6961 626c  N..intro_variabl
-00000460: 6573 da12 6167 6772 6567 6174 696f 6e5f  es..aggregation_
-00000470: 666f 726d 6174 e901 0000 0072 0100 0000  format.....r....
-00000480: 2902 da06 7061 7373 6573 da06 616c 6172  )...passes..alar
-00000490: 6d73 2903 7213 0000 00da 0565 6d70 7479  ms).r......empty
-000004a0: da06 6368 6563 6b73 2903 da05 7061 7468  ..checks)...path
-000004b0: 7372 1300 0000 da05 7374 6174 7372 1400  sr......statsr..
-000004c0: 0000 5472 1700 0000 7207 0000 0072 1300  ..Tr....r....r..
-000004d0: 0000 7215 0000 0072 1200 0000 e902 0000  ..r....r........
-000004e0: 0029 0272 1300 0000 7214 0000 0029 0272  .).r....r....).r
-000004f0: 1600 0000 7215 0000 0072 1600 0000 7a14  ....r....r....z.
-00000500: 6167 6772 6567 6174 696f 6e20 666f 726d  aggregation form
-00000510: 6174 2027 7a14 2720 6e6f 7420 6163 636f  at 'z.' not acco
-00000520: 756e 7465 6420 666f 722e 2905 720e 0000  unted for.).r...
-00000530: 00da 0c61 6c61 726d 5f70 6172 7365 72da  ...alarm_parser.
-00000540: 0573 7461 7274 7202 0000 00da 0945 7863  .startr......Exc
-00000550: 6570 7469 6f6e 2905 720a 0000 0072 1300  eption).r....r..
-00000560: 0000 7210 0000 00da 0673 7461 7475 7372  ..r......statusr
-00000570: 0600 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000580: 0000 00da 0f61 6767 7265 6761 7465 5f73  .....aggregate_s
-00000590: 7461 7473 5c00 0000 735a 0000 0006 010a  tats\...sZ......
-000005a0: 010c 0208 0202 0202 0102 0202 0102 0202  ................
-000005b0: 0104 fe04 fd06 fd08 0d14 0114 0102 0108  ................
-000005c0: 0214 0102 0120 0222 0104 0308 0202 0202  ..... ."........
-000005d0: 0102 0302 0104 fe02 0502 0104 fe04 fb06  ................
-000005e0: fd08 0f14 0118 0102 0108 0218 0102 0120  ............... 
-000005f0: 0222 0104 0310 0372 1d00 0000 2908 da07  .".....r....)...
-00000600: 5f5f 646f 635f 5fda 3762 696f 7465 6368  __doc__.7biotech
-00000610: 2e70 726f 6365 6475 7265 732e 696d 706c  .procedures.impl
-00000620: 6963 6974 5f70 726f 6365 6475 7265 2e70  icit_procedure.p
-00000630: 726f 6365 7373 2e76 6172 6961 626c 6573  rocess.variables
-00000640: 7202 0000 00da 1b62 696f 7465 6368 2e74  r......biotech.t
-00000650: 6f70 6963 732e 616c 6172 6d5f 7061 7273  opics.alarm_pars
-00000660: 6572 da06 746f 7069 6373 7219 0000 0072  er..topicsr....r
-00000670: 0e00 0000 721d 0000 0072 0c00 0000 720c  ....r....r....r.
-00000680: 0000 0072 0c00 0000 720d 0000 00da 083c  ...r....r......<
-00000690: 6d6f 6475 6c65 3e01 0000 0073 1200 0000  module>....s....
-000006a0: 0404 0206 0c1e 1201 0203 020c 080a 0215  ................
-000006b0: 0c04                                     ..
+00000020: 0002 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
+00000030: 5a00 0900 0900 6401 6402 6c01 6d02 5a02  Z.....d.d.l.m.Z.
+00000040: 0100 6401 6403 6c03 6d04 0200 0100 6d05  ..d.d.l.m.....m.
+00000050: 5a05 0100 6401 6404 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
+00000060: 0900 0900 6405 6406 8400 5a08 0900 6407  ....d.d...Z...d.
+00000070: 6408 8400 5a09 6403 5300 2909 7a27 0a09  d...Z.d.S.).z'..
+00000080: 6167 6772 6567 6174 655f 7374 6174 7320  aggregate_stats 
+00000090: 280a 0909 7061 7468 5f73 7461 7475 7365  (...path_statuse
+000000a0: 730a 0929 0ae9 0000 0000 2901 da14 6167  s..)......)...ag
+000000b0: 6772 6567 6174 6f72 5f76 6172 6961 626c  gregator_variabl
+000000c0: 6573 4e29 01da 0d73 686f 775f 7661 7269  esN)...show_vari
+000000d0: 6162 6c65 6300 0000 0000 0000 0000 0000  ablec...........
+000000e0: 0006 0000 000b 0000 0043 0000 0073 f600  .........C...s..
+000000f0: 0000 6700 7d00 7400 6401 1900 7d01 7c01  ..g.}.t.d...}.|.
+00000100: 4400 5d70 7d02 7c01 7c02 1900 6402 1900  D.]p}.|.|...d...
+00000110: 7d03 7c03 6400 6b02 7273 7c02 6403 6404  }.|.d.k.rs|.d.d.
+00000120: 9c02 7d04 7a0a 7c01 7c02 1900 6405 1900  ..}.z.|.|...d...
+00000130: 7c04 6405 3c00 5700 6e1f 0400 7401 7942  |.d.<.W.n...t.yB
+00000140: 0100 7d05 0100 7a13 7402 6406 7c05 8302  ..}...z.t.d.|...
+00000150: 0100 7403 7c01 7c02 1900 6407 6408 8d02  ..t.|.|...d.d...
+00000160: 0100 5700 5900 6400 7d05 7e05 6e05 6400  ..W.Y.d.}.~.n.d.
+00000170: 7d05 7e05 7701 7700 7a0a 7c01 7c02 1900  }.~.w.w.z.|.|...
+00000180: 6409 1900 7c04 6409 3c00 5700 6e1f 0400  d...|.d.<.W.n...
+00000190: 7401 796c 0100 7d05 0100 7a13 7402 640a  t.yl..}...z.t.d.
+000001a0: 7c05 8302 0100 7403 7c01 7c02 1900 6407  |.....t.|.|...d.
+000001b0: 6408 8d02 0100 5700 5900 6400 7d05 7e05  d.....W.Y.d.}.~.
+000001c0: 6e05 6400 7d05 7e05 7701 7700 7c00 a004  n.d.}.~.w.w.|...
+000001d0: 7c04 a101 0100 7108 7c00 a004 7c03 a101  |.....q.|...|...
+000001e0: 0100 7108 7c00 5300 290b 4eda 1169 6e74  ..q.|.S.).N..int
+000001f0: 6572 6e61 6c5f 7374 6174 7573 6573 da0f  ernal_statuses..
+00000200: 7265 7375 6c74 735f 6f66 5f73 6361 6e7a  results_of_scanz
+00000210: 0a6e 6f20 7265 7375 6c74 7329 02da 0470  .no results)...p
+00000220: 6174 68da 0561 6c61 726d da0b 6f63 6375  ath..alarm..occu
+00000230: 7272 656e 6365 737a 1c72 6573 756c 7473  rrencesz.results
+00000240: 206f 6620 7363 616e 2065 7863 6570 7469   of scan excepti
+00000250: 6f6e 2031 3ada 0473 686f 7729 01da 046d  on 1:..show)...m
+00000260: 6f64 65da 0772 6563 6f72 6473 7a1c 7265  ode..recordsz.re
+00000270: 7375 6c74 7320 6f66 2073 6361 6e20 6578  sults of scan ex
+00000280: 6365 7074 696f 6e20 323a 2905 7202 0000  ception 2:).r...
+00000290: 00da 0945 7863 6570 7469 6f6e da05 7072  ...Exception..pr
+000002a0: 696e 7472 0300 0000 da06 6170 7065 6e64  intr......append
+000002b0: 2906 da0d 7061 7468 5f73 7461 7475 7365  )...path_statuse
+000002c0: 7372 0400 0000 da09 7363 616e 5f70 6174  sr......scan_pat
+000002d0: 6872 0500 0000 da0a 7468 655f 7061 636b  hr......the_pack
+000002e0: 6574 da01 45a9 0072 1300 0000 fa5f 2f62  et..E..r....._/b
+000002f0: 696f 7465 6368 2f76 656e 7565 732f 7374  iotech/venues/st
+00000300: 6167 6573 2f62 696f 7465 6368 2f70 726f  ages/biotech/pro
+00000310: 6365 6475 7265 732f 6167 6772 6567 6174  cedures/aggregat
+00000320: 6f72 5f70 726f 6365 6475 7265 2f70 726f  or_procedure/pro
+00000330: 6365 7373 2f6d 6f76 6573 2f61 6767 7265  cess/moves/aggre
+00000340: 6761 7465 5f73 7461 7473 2e70 79da 1370  gate_stats.py..p
+00000350: 6172 7365 5f70 6174 685f 7374 6174 7573  arse_path_status
+00000360: 6573 4900 0000 7332 0000 0004 0108 0208  esI...s2........
+00000370: 010c 0108 0102 0302 0106 fe02 0514 010e  ................
+00000380: 010a 011c 0108 8002 fe02 0414 010e 010a  ................
+00000390: 011c 0108 8002 fe0c 040c 0504 0272 1500  .............r..
+000003a0: 0000 6300 0000 0000 0000 0000 0000 0005  ..c.............
+000003b0: 0000 0007 0000 0043 0000 0073 a801 0000  .......C...s....
+000003c0: 7400 8300 7d00 7401 a002 7c00 a101 7d01  t...}.t...|...}.
+000003d0: 7403 6401 1900 6402 1900 7d02 7c02 6403  t.d...d...}.|.d.
+000003e0: 6b02 726a 7c00 7c01 6404 6404 6404 6404  k.rj|.|.d.d.d.d.
+000003f0: 6405 9c02 6406 9c03 6407 9c03 7d03 7c00  d...d...d...}.|.
+00000400: 4400 5d46 7d04 6408 7c04 7600 7238 7c04  D.]F}.d.|.v.r8|.
+00000410: 6408 1900 6409 6b02 7238 7c03 640a 1900  d...d.k.r8|.d...
+00000420: 6408 0500 1900 6403 3700 0300 3c00 7121  d.....d.7...<.q!
+00000430: 640b 7c04 7600 7247 7c03 640a 1900 640c  d.|.v.rG|.d...d.
+00000440: 0500 1900 6403 3700 0300 3c00 7121 7c03  ....d.7...<.q!|.
+00000450: 640a 1900 640d 1900 640e 0500 1900 7c04  d...d...d.....|.
+00000460: 640a 1900 640e 1900 3700 0300 3c00 7c03  d...d...7...<.|.
+00000470: 640a 1900 640d 1900 640c 0500 1900 7c04  d...d...d.....|.
+00000480: 640a 1900 640c 1900 3700 0300 3c00 7121  d...d...7...<.q!
+00000490: 7c03 5300 7c02 640f 6b02 72cc 7c00 7c01  |.S.|.d.k.r.|.|.
+000004a0: 6404 6404 6410 9c02 6404 6404 6405 9c02  d.d.d...d.d.d...
+000004b0: 6411 9c02 6407 9c03 7d03 7c00 4400 5d4a  d...d...}.|.D.]J
+000004c0: 7d04 6408 7c04 7600 7298 7c04 6408 1900  }.d.|.v.r.|.d...
+000004d0: 6409 6b02 7298 7c03 640a 1900 6412 1900  d.k.r.|.d...d...
+000004e0: 6408 0500 1900 6403 3700 0300 3c00 717f  d.....d.7...<.q.
+000004f0: 640b 7c04 7600 72a9 7c03 640a 1900 6412  d.|.v.r.|.d...d.
+00000500: 1900 640c 0500 1900 6403 3700 0300 3c00  ..d.....d.7...<.
+00000510: 717f 7c03 640a 1900 640d 1900 640e 0500  q.|.d...d...d...
+00000520: 1900 7c04 640a 1900 640e 1900 3700 0300  ..|.d...d...7...
+00000530: 3c00 7c03 640a 1900 640d 1900 640c 0500  <.|.d...d...d...
+00000540: 1900 7c04 640a 1900 640c 1900 3700 0300  ..|.d...d...7...
+00000550: 3c00 717f 7c03 5300 7404 6413 7c02 9b00  <.q.|.S.t.d.|...
+00000560: 6414 9d03 8301 8201 2915 4eda 0f69 6e74  d.......).N..int
+00000570: 726f 5f76 6172 6961 626c 6573 da12 6167  ro_variables..ag
+00000580: 6772 6567 6174 696f 6e5f 666f 726d 6174  gregation_format
+00000590: e901 0000 0072 0100 0000 2902 da06 7061  .....r....)...pa
+000005a0: 7373 6573 da06 616c 6172 6d73 2903 721a  sses..alarms).r.
+000005b0: 0000 00da 0565 6d70 7479 da06 6368 6563  .....empty..chec
+000005c0: 6b73 2903 da05 7061 7468 7372 1a00 0000  ks)...pathsr....
+000005d0: da05 7374 6174 7372 1b00 0000 5472 1e00  ..statsr....Tr..
+000005e0: 0000 7207 0000 0072 1a00 0000 721c 0000  ..r....r....r...
+000005f0: 0072 1900 0000 e902 0000 0029 0272 1a00  .r.........).r..
+00000600: 0000 721b 0000 0029 0272 1d00 0000 721c  ..r....).r....r.
+00000610: 0000 0072 1d00 0000 7a14 6167 6772 6567  ...r....z.aggreg
+00000620: 6174 696f 6e20 666f 726d 6174 2027 7a14  ation format 'z.
+00000630: 2720 6e6f 7420 6163 636f 756e 7465 6420  ' not accounted 
+00000640: 666f 722e 2905 7215 0000 00da 0c61 6c61  for.).r......ala
+00000650: 726d 5f70 6172 7365 72da 0573 7461 7274  rm_parser..start
+00000660: 7202 0000 0072 0c00 0000 2905 720f 0000  r....r....).r...
+00000670: 0072 1a00 0000 7217 0000 00da 0673 7461  .r....r......sta
+00000680: 7475 7372 0600 0000 7213 0000 0072 1300  tusr....r....r..
+00000690: 0000 7214 0000 00da 0f61 6767 7265 6761  ..r......aggrega
+000006a0: 7465 5f73 7461 7473 6f00 0000 735a 0000  te_statso...sZ..
+000006b0: 0006 010a 010c 0208 0202 0202 0102 0202  ................
+000006c0: 0102 0202 0104 fe04 fd06 fd08 0d14 0114  ................
+000006d0: 0102 0108 0214 0102 0120 0222 0104 0308  ......... ."....
+000006e0: 0202 0202 0102 0302 0104 fe02 0502 0104  ................
+000006f0: fe04 fb06 fd08 0f14 0118 0102 0108 0218  ................
+00000700: 0102 0120 0222 0104 0310 0372 2300 0000  ... .".....r#...
+00000710: 290a da07 5f5f 646f 635f 5fda 3962 696f  )...__doc__.9bio
+00000720: 7465 6368 2e70 726f 6365 6475 7265 732e  tech.procedures.
+00000730: 6167 6772 6567 6174 6f72 5f70 726f 6365  aggregator_proce
+00000740: 6475 7265 2e70 726f 6365 7373 2e76 6172  dure.process.var
+00000750: 6961 626c 6573 7202 0000 00da 1b62 696f  iablesr......bio
+00000760: 7465 6368 2e74 6f70 6963 732e 616c 6172  tech.topics.alar
+00000770: 6d5f 7061 7273 6572 da06 746f 7069 6373  m_parser..topics
+00000780: 7220 0000 00da 1c62 696f 7465 6368 2e74  r .....biotech.t
+00000790: 6f70 6963 732e 7368 6f77 2e76 6172 6961  opics.show.varia
+000007a0: 626c 6572 0300 0000 7215 0000 0072 2300  bler....r....r#.
+000007b0: 0000 7213 0000 0072 1300 0000 7213 0000  ..r....r....r...
+000007c0: 0072 1400 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000007d0: 0100 0000 7316 0000 0004 0402 0602 050c  ....s...........
+000007e0: 1e12 010c 0202 0202 0c08 0a02 220c 04    ............"..
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 20:48:34 2024 UTC, .py size: 1072 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-00000000: 6f0d 0d0a 0000 0000 22e4 1e66 3004 0000  o......."..f0...
+00000000: 6f0d 0d0a 0000 0000 ba2c 2066 4404 0000  o........, fD...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 6d03 5a03 0100 6404 6405 8400 5a04 6402  m.Z...d.d...Z.d.
-00000050: 5300 2906 7a59 0a09 7374 6f70 5f70 726f  S.).zY..stop_pro
-00000060: 6365 7373 2028 0a09 0922 686f 7573 655f  cess (..."house_
-00000070: 6d69 782e 7079 222c 0a09 0973 7461 7475  mix.py",...statu
-00000080: 7320 3d20 7b0a 0909 0922 616c 6172 6d22  s = {...."alarm"
-00000090: 3a20 2274 696d 6520 6c69 6d69 7420 6578  : "time limit ex
-000000a0: 6365 6564 6564 220a 0909 7d0a 0929 0ae9  ceeded"...}..)..
-000000b0: 0000 0000 4e29 01da 1c69 6d70 6c69 6369  ....N)...implici
-000000c0: 745f 7072 6f63 6564 7572 655f 7661 7269  t_procedure_vari
-000000d0: 6162 6c65 7363 0200 0000 0000 0000 0000  ablesc..........
-000000e0: 0000 0200 0000 0400 0000 4300 0000 73a4  ..........C...s.
-000000f0: 0000 0064 0174 0064 0219 007c 0019 0064  ...d.t.d...|...d
-00000100: 0319 0064 043c 0064 057c 0069 017c 01a5  ...d.<.d.|.i.|..
-00000110: 0174 0064 0219 007c 0019 0064 063c 0074  .t.d...|...d.<.t
-00000120: 0174 02a0 02a1 0083 0174 0064 0219 007c  .t.......t.d...|
-00000130: 0019 0064 0719 0064 083c 0074 0374 0064  ...d...d.<.t.t.d
-00000140: 0219 007c 0019 0064 0719 0064 0819 0083  ...|...d...d....
-00000150: 0174 0374 0064 0219 007c 0019 0064 0719  .t.t.d...|...d..
-00000160: 0064 0919 0083 0118 0074 0064 0219 007c  .d.......t.d...|
-00000170: 0019 0064 0719 0064 0a3c 0074 0064 0219  ...d...d.<.t.d..
-00000180: 007c 0019 0064 0b19 0064 0b19 00a0 04a1  .|...d...d......
-00000190: 0001 0064 0053 0029 0c4e da04 646f 6e65  ...d.S.).N..done
-000001a0: da11 696e 7465 726e 616c 5f73 7461 7475  ..internal_statu
-000001b0: 7365 73da 0673 7461 7475 73da 0473 6361  ses..status..sca
-000001c0: 6eda 0470 6174 68da 0f72 6573 756c 7473  n..path..results
-000001d0: 5f6f 665f 7363 616e da05 7469 6d65 73da  _of_scan..times.
-000001e0: 0565 6e64 6564 da07 7374 6172 7465 64da  .ended..started.
-000001f0: 0765 6c61 7073 6564 da07 7072 6f63 6573  .elapsed..proces
-00000200: 7329 0572 0200 0000 da03 7374 72da 0474  s).r......str..t
-00000210: 696d 65da 0566 6c6f 6174 da09 7465 726d  ime..float..term
-00000220: 696e 6174 6529 02da 0874 6865 5f70 6174  inate)...the_pat
-00000230: 6872 0500 0000 a900 7213 0000 00fa 5a2f  hr......r.....Z/
-00000240: 6269 6f74 6563 682f 7665 6e75 6573 2f73  biotech/venues/s
-00000250: 7461 6765 732f 6269 6f74 6563 682f 7072  tages/biotech/pr
-00000260: 6f63 6564 7572 6573 2f69 6d70 6c69 6369  ocedures/implici
-00000270: 745f 7072 6f63 6564 7572 652f 7072 6f63  t_procedure/proc
-00000280: 6573 732f 6d6f 7665 732f 7374 6f70 5f70  ess/moves/stop_p
-00000290: 726f 6365 7373 2e70 79da 0c73 746f 705f  rocess.py..stop_
-000002a0: 7072 6f63 6573 7310 0000 0073 1600 0000  process....s....
-000002b0: 1405 0402 02ff 0202 10fe 1c05 1603 1601  ................
-000002c0: 02ff 12ff 1c09 7215 0000 0029 05da 075f  ......r....)..._
-000002d0: 5f64 6f63 5f5f 720f 0000 00da 3762 696f  _doc__r.....7bio
-000002e0: 7465 6368 2e70 726f 6365 6475 7265 732e  tech.procedures.
-000002f0: 696d 706c 6963 6974 5f70 726f 6365 6475  implicit_procedu
-00000300: 7265 2e70 726f 6365 7373 2e76 6172 6961  re.process.varia
-00000310: 626c 6573 7202 0000 0072 1500 0000 7213  blesr....r....r.
-00000320: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000330: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000340: 7308 0000 0004 0208 090c 020c 02         s............
+00000020: 0002 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
+00000030: 5a00 0900 6401 6402 6c01 5a01 6401 6403  Z...d.d.l.Z.d.d.
+00000040: 6c02 6d03 5a03 0100 6404 6405 8400 5a04  l.m.Z...d.d...Z.
+00000050: 6402 5300 2906 7a59 0a09 7374 6f70 5f70  d.S.).zY..stop_p
+00000060: 726f 6365 7373 2028 0a09 0922 686f 7573  rocess (..."hous
+00000070: 655f 6d69 782e 7079 222c 0a09 0973 7461  e_mix.py",...sta
+00000080: 7475 7320 3d20 7b0a 0909 0922 616c 6172  tus = {...."alar
+00000090: 6d22 3a20 2274 696d 6520 6c69 6d69 7420  m": "time limit 
+000000a0: 6578 6365 6564 6564 220a 0909 7d0a 0929  exceeded"...}..)
+000000b0: 0ae9 0000 0000 4e29 01da 1c69 6d70 6c69  ......N)...impli
+000000c0: 6369 745f 7072 6f63 6564 7572 655f 7661  cit_procedure_va
+000000d0: 7269 6162 6c65 7363 0200 0000 0000 0000  riablesc........
+000000e0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+000000f0: 73a4 0000 0064 0174 0064 0219 007c 0019  s....d.t.d...|..
+00000100: 0064 0319 0064 043c 0064 057c 0069 017c  .d...d.<.d.|.i.|
+00000110: 01a5 0174 0064 0219 007c 0019 0064 063c  ...t.d...|...d.<
+00000120: 0074 0174 02a0 02a1 0083 0174 0064 0219  .t.t.......t.d..
+00000130: 007c 0019 0064 0719 0064 083c 0074 0374  .|...d...d.<.t.t
+00000140: 0064 0219 007c 0019 0064 0719 0064 0819  .d...|...d...d..
+00000150: 0083 0174 0374 0064 0219 007c 0019 0064  ...t.t.d...|...d
+00000160: 0719 0064 0919 0083 0118 0074 0064 0219  ...d.......t.d..
+00000170: 007c 0019 0064 0719 0064 0a3c 0074 0064  .|...d...d.<.t.d
+00000180: 0219 007c 0019 0064 0b19 0064 0b19 00a0  ...|...d...d....
+00000190: 04a1 0001 0064 0053 0029 0c4e da04 646f  .....d.S.).N..do
+000001a0: 6e65 da11 696e 7465 726e 616c 5f73 7461  ne..internal_sta
+000001b0: 7475 7365 73da 0673 7461 7475 73da 0473  tuses..status..s
+000001c0: 6361 6eda 0470 6174 68da 0f72 6573 756c  can..path..resul
+000001d0: 7473 5f6f 665f 7363 616e da05 7469 6d65  ts_of_scan..time
+000001e0: 73da 0565 6e64 6564 da07 7374 6172 7465  s..ended..starte
+000001f0: 64da 0765 6c61 7073 6564 da07 7072 6f63  d..elapsed..proc
+00000200: 6573 7329 0572 0200 0000 da03 7374 72da  ess).r......str.
+00000210: 0474 696d 65da 0566 6c6f 6174 da09 7465  .time..float..te
+00000220: 726d 696e 6174 6529 02da 0874 6865 5f70  rminate)...the_p
+00000230: 6174 6872 0500 0000 a900 7213 0000 00fa  athr......r.....
+00000240: 5a2f 6269 6f74 6563 682f 7665 6e75 6573  Z/biotech/venues
+00000250: 2f73 7461 6765 732f 6269 6f74 6563 682f  /stages/biotech/
+00000260: 7072 6f63 6564 7572 6573 2f69 6d70 6c69  procedures/impli
+00000270: 6369 745f 7072 6f63 6564 7572 652f 7072  cit_procedure/pr
+00000280: 6f63 6573 732f 6d6f 7665 732f 7374 6f70  ocess/moves/stop
+00000290: 5f70 726f 6365 7373 2e70 79da 0c73 746f  _process.py..sto
+000002a0: 705f 7072 6f63 6573 7315 0000 0073 1600  p_process....s..
+000002b0: 0000 1404 0402 02ff 0202 10fe 1c05 1603  ................
+000002c0: 1601 02ff 12ff 1c09 7215 0000 0029 05da  ........r....)..
+000002d0: 075f 5f64 6f63 5f5f 720f 0000 00da 3762  .__doc__r.....7b
+000002e0: 696f 7465 6368 2e70 726f 6365 6475 7265  iotech.procedure
+000002f0: 732e 696d 706c 6963 6974 5f70 726f 6365  s.implicit_proce
+00000300: 6475 7265 2e70 726f 6365 7373 2e76 6172  dure.process.var
+00000310: 6961 626c 6573 7202 0000 0072 1500 0000  iablesr....r....
+00000320: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00000330: 1400 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000340: 0000 730a 0000 0004 0202 0908 050c 020c  ..s.............
+00000350: 02                                       .
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/aggregate_stats.py` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/aggregate_stats.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 '''
 	aggregate_stats (
 		path_statuses
 	)
 '''
 
 '''
+	Summary:
+		This aggregates the stats after every scan is done.
+'''
+
+'''
 	format 1:
 		{
 			"paths": path_statuses,
 			"stats": {
 				"alarms": 0,
 				"empty": 0,
 				"checks": {
@@ -34,17 +39,18 @@
 					"passes": 0,
 					"alarms": 0
 				}
 			}
 		}
 '''
 
-from biotech.procedures.implicit_procedure.process.variables import implicit_procedure_variables
+from biotech.procedures.aggregator_procedure.process.variables import aggregator_variables
 import biotech.topics.alarm_parser as alarm_parser
 
+from biotech.topics.show.variable import show_variable
 
 '''
 	{
 		"path": "../status_1.py",
 		"empty": false,
 		"parsed": true,
 		"stats": {
@@ -63,41 +69,54 @@
 			"alarms": 1
 		},
 		"checks": []
 '''
 def parse_path_statuses ():
 	path_statuses = []
 
-	internal_statuses = implicit_procedure_variables ["internal_statuses"]
+	internal_statuses = aggregator_variables ["internal_statuses"]
 	for scan_path in internal_statuses:
 		results_of_scan = internal_statuses [ scan_path ] ["results_of_scan"]
 		if (results_of_scan == None):
-			path_statuses.append ({
+			
+			the_packet = {
 				"path": scan_path,
+				"alarm": "no results"
+			}
+		
+			try:
+				the_packet ["occurrences"] = internal_statuses [ scan_path ] ["occurrences"]
+			except Exception as E:
+				print ("results of scan exception 1:", E)
+				show_variable (internal_statuses [ scan_path ], mode = "show")
+				
+			try:
+				the_packet ["records"] = internal_statuses [ scan_path ] ["records"]
+			except Exception as E:
+				print ("results of scan exception 2:", E)
+				show_variable (internal_statuses [ scan_path ], mode = "show")
 				
-				"alarm": "exitted",
-				"alarm note": "The process exitted before results could be sent.",
+			path_statuses.append (the_packet)
 				
-				"exited": True
-			})
+			
 
 		else:
 			path_statuses.append (results_of_scan)
 		
 	return path_statuses
 
 '''
 	This function aggregates (or summarizes) the stats from
 	all of the checks.
 '''
 def aggregate_stats ():
 	path_statuses = parse_path_statuses ()
 	alarms = alarm_parser.start (path_statuses)	
 
-	aggregation_format = implicit_procedure_variables ["intro_variables"] ["aggregation_format"];
+	aggregation_format = aggregator_variables ["intro_variables"] ["aggregation_format"];
 
 	if (aggregation_format == 1):
 		status = {
 			"paths": path_statuses,
 			"alarms": alarms,
 			"stats": {
 				"alarms": 0,
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/done_with_scan.py` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/done_with_scan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,110 @@
 
 
 '''
-	This turns off the scan process.
+	done_with_scan_move ({
+		"path": 
+		"result":
+	})
 '''
 
-import json
-import pathlib
-import os
-from os.path import dirname, join, normpath
-import sys
-import threading
-import time
-
-from flask import Flask, request
-
-import rich
+'''
+	Summary:
+		This turns off the scan process.
+'''
 
+'''
+	Maybe called by:
+		global time limit reached.
+'''
 
-from biotech.procedures.implicit_procedure.process.variables import implicit_procedure_variables
 
+#----
+#
+from ..variables import aggregator_variables
 from .aggregate_stats import aggregate_stats
+#
+from biotech.topics.process_on.p_expect.parse_records import parse_p_expect_records
+from biotech.topics.show.variable import show_variable
+#
+#
+import rich
+#
+#
+import time
+#
+#----
 
-
-
-def done_with_scan_move (
-	the_packet = ""
-):
+def done_with_scan_move (the_packet):
 	the_path = the_packet ["path"]
 	the_result = the_packet ["result"]
-	the_pid = the_packet ["pid"]
+	#the_pid = the_packet ["pid"]
 	
-	'''
-		turn off the scan process
-	'''
-	#print ('turning off scan process with pid:', the_pid)
-	#os.kill (the_pid, 9)
 	
+	show_variable ({
+		"done with scan, stopping:": the_packet
+	}, mode = "show")
+
+
+	#---
 	#
-	#	stopping
+	#	Once the status of the scan has been established,
+	# 	then the scan process can be stopped.
 	#
-	print ("stopping:", implicit_procedure_variables ["internal_statuses"] [ the_path ] ["process"] ["process"])
+	aggregator_variables ["internal_statuses"] [ the_path ] ["process"] ["process"].terminate ()
+	aggregator_variables ["internal_statuses"] [ the_path ] ["times"] ["ended"] = str (time.time ());
+	aggregator_variables ["internal_statuses"] [ the_path ] ["times"] ["elapsed"] = (
+		float (aggregator_variables ["internal_statuses"] [ the_path ] ["times"] ["ended"]) - 
+		float (aggregator_variables ["internal_statuses"] [ the_path ] ["times"] ["started"])
+	);
+	aggregator_variables ["internal_statuses"] [ the_path ] ["occurrences"] ["scan process was stopped"] = "yes"
 	
+	#print ('turning off scan process with pid:', the_pid)
+	#os.kill (the_pid, 9)
+	#
+	#----
+	
+	show_variable ({
+		"times": aggregator_variables ["internal_statuses"] [ the_path ] ["times"]
+	}, mode = "show")
+	
+	
+	
+	try:
+		aggregator_variables ["internal_statuses"] [ the_path ] ["records"] = parse_p_expect_records (
+			records = aggregator_variables ["internal_statuses"] [ the_path ] ["process"] ["records"] (),
+			format = "UTF8"
+		)
+	except Exception:
+		show_variable ("The records could not be parsed!")
 	
-	status = {
-		"path": the_path,
-		** the_result
+	the_results_packet = {
+		"path": the_path
 	}
-	#implicit_procedure_variables ["paths_statuses"].append (status)
 	
+	try:
+		the_results_packet ["records"] = aggregator_variables ["internal_statuses"] [ the_path ] ["records"]
+	except Exception:
+		show_variable ("The records could not be added to the results packet!")
 	
-	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["status"] ["scan"] = "done"
-	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["results_of_scan"] = status
-
-	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["times"] ["ended"] = str (time.time ());
-
-	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["times"] ["elapsed"] = (
-		float (implicit_procedure_variables ["internal_statuses"] [ the_path ] ["times"] ["ended"]) - 
-		float (implicit_procedure_variables ["internal_statuses"] [ the_path ] ["times"] ["started"])
-	);
+	try:
+		for result in the_result:
+			the_results_packet [ result ] = the_result [ result ]
+	except Exception:
+		show_variable ("A result in the results could not be added!")
 	
-	#
-	#	Once the status of the scan has been established,
-	# 	then the scan process can be stopped.
-	#
-	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["process"] ["process"].terminate ()
+	aggregator_variables ["internal_statuses"] [ the_path ] ["results_of_scan"] = the_results_packet
+	
+	aggregator_variables ["internal_statuses"] [ the_path ] ["occurrences"] ["scan records were retrieved"] = "yes"
+	
+	
+	show_variable ("done with scan")
 	
 	
+	
+	time.sleep (1)
+	
+	'''
+		This is only variable that is waited on.
+	'''
+	aggregator_variables ["internal_statuses"] [ the_path ] ["status"] ["process"] = "done"
+
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/implicit_procedure/process/moves/venture_finish.py` & `biotech-1.1.0/venues/stages/biotech/procedures/aggregator_procedure/process/moves/status_check_monitor/send_done_if_finished.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,46 @@
 
-'''
+#----
+#
+from biotech.procedures.aggregator_procedure.process.variables import aggregator_variables
+#	
+from ..send_done import send_done
+from ..aggregate_stats import aggregate_stats#
+#
+#----
 
-'''
-
-import rich
-
-from biotech.procedures.implicit_procedure.process.variables import implicit_procedure_variables
-
-from .send_done import send_done
-from .aggregate_stats import aggregate_stats
-
-
-def venture_finish ():
-	print ()
-	print ("checking if is done")
-	print ()
-	
-	the_internal_statuses = implicit_procedure_variables ["internal_statuses"]
-
-	if (implicit_procedure_variables ["internal_statuses_built"] != "yes"):
+def send_done_if_finished (unfinished):
+	if (len (unfinished) >= 1):
 		return;
-	
+		
+	'''
+		This loop might be redundant.
+	'''
+	the_internal_statuses = aggregator_variables ["internal_statuses"]
 	for internal_status in the_internal_statuses:
-		rich.print_json (
-			data = {
-				"internal status": {
-					internal_status: the_internal_statuses [internal_status] [ "status" ] 
-				}
-			}
-		)
-	
 	
 		#
 		#	if the process is done, then the scan:
 		#	
 		#		( ) exitted
 		#		( ) sent /done_with_scan
 		#
 		#		( ) unlikely -> neither?
 		#
-		
 		#if (the_internal_statuses [ internal_status ] [ "status" ] [ "scan" ] != "done"):
-		#	return "no";
-			
+		#	return;
+	
 		if (the_internal_statuses [ internal_status ] [ "status" ] [ "process" ] != "done"):
-			return "no";
-		
+			return;
+	
+
 	'''
 		if not bounced, then send done
 	'''	
 	send_done (
-		host = implicit_procedure_variables ["intro_harbor"] ["host"],
-		port = implicit_procedure_variables ["intro_harbor"] ["port"],
+		host = aggregator_variables ["intro_harbor"] ["host"],
+		port = aggregator_variables ["intro_harbor"] ["port"],
 		
 		proceeds = aggregate_stats ()
-	)
+	)
+	
+	return "sent"
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/intro/process/coms/aggregator_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 20:48:34 2024 UTC, .py size: 634 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,57 @@
-00000000: 6f0d 0d0a 0000 0000 22e4 1e66 7a02 0000  o......."..fz...
+00000000: 6f0d 0d0a 0000 0000 49a2 2266 6602 0000  o.......I."ff...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 5a00 6401 6402 6c01 6d02 0200 0100 6d03  Z.d.d.l.m.....m.
 00000040: 5a04 0100 6401 6403 6c05 6d06 5a07 0100  Z...d.d.l.m.Z...
 00000050: 6401 6402 6c08 5a08 6404 6900 6602 6405  d.d.l.Z.d.i.f.d.
-00000060: 6406 8401 5a09 6402 5300 2907 7a80 0a09  d...Z.d.S.).z...
+00000060: 6406 8401 5a09 6402 5300 2907 7a9e 0a09  d...Z.d.S.).z...
 00000070: 6672 6f6d 2062 696f 7465 6368 2e70 726f  from biotech.pro
 00000080: 6365 6475 7265 732e 696e 7472 6f2e 636f  cedures.intro.co
-00000090: 6d73 2e69 6d70 6c69 6369 745f 7072 6f63  ms.implicit_proc
-000000a0: 6564 7572 652e 7365 6e64 5f70 6174 6873  edure.send_paths
-000000b0: 2069 6d70 6f72 7420 7365 6e64 5f70 6174   import send_pat
-000000c0: 6873 0a09 7365 6e64 5f70 6174 6873 2028  hs..send_paths (
-000000d0: 0a09 0970 6f72 7420 3d20 302c 0a09 0970  ...port = 0,...p
-000000e0: 6163 6b65 7420 3d20 7b7d 0a09 290a e900  acket = {}..)...
-000000f0: 0000 004e 2901 da08 7072 6573 656e 7473  ...N)...presents
-00000100: da00 6302 0000 0000 0000 0000 0000 0004  ..c.............
-00000110: 0000 0004 0000 0043 0000 0073 4200 0000  .......C...sB...
-00000120: 7400 6401 8301 0100 6402 7c00 9b00 6403  t.d.....d.|...d.
-00000130: 9d03 7d02 7401 6a02 7c02 7c01 6404 8d02  ..}.t.j.|.|.d...
-00000140: 7d03 7c03 6a03 6405 6b02 721d 7c03 6a04  }.|.j.d.k.r.|.j.
-00000150: 6406 6b02 721d 6407 5300 7405 6408 8301  d.k.r.d.S.t.d...
-00000160: 8201 2909 4e7a 3261 7761 6974 696e 6720  ..).Nz2awaiting 
-00000170: 7468 6520 6f70 656e 206f 6620 7468 6520  the open of the 
-00000180: 696d 706c 6963 6974 2070 726f 6365 6475  implicit procedu
-00000190: 7265 2068 6172 626f 727a 0f68 7474 703a  re harborz.http:
-000001a0: 2f2f 302e 302e 302e 303a 7a06 2f70 6174  //0.0.0.0:z./pat
-000001b0: 6873 2901 da04 6a73 6f6e e9c8 0000 00da  hs)...json......
-000001c0: 0872 6563 6569 7665 6454 7a48 416e 2065  .receivedTzHAn e
-000001d0: 7863 6570 7469 6f6e 206f 6363 7572 7265  xception occurre
-000001e0: 6420 7768 696c 6520 7365 6e64 696e 6720  d while sending 
-000001f0: 7468 6520 7061 7468 7320 746f 2074 6865  the paths to the
-00000200: 2069 6d70 6c69 6369 7420 7072 6f63 6564   implicit proced
-00000210: 7572 652e 2906 da05 7072 696e 74da 0872  ure.)...print..r
-00000220: 6571 7565 7374 73da 0570 6174 6368 da0b  equests..patch..
-00000230: 7374 6174 7573 5f63 6f64 65da 0474 6578  status_code..tex
-00000240: 74da 0945 7863 6570 7469 6f6e 2904 da04  t..Exception)...
-00000250: 706f 7274 da06 7061 636b 6574 da03 5552  port..packet..UR
-00000260: 4cda 0872 6573 706f 6e73 65a9 0072 1100  L..response..r..
-00000270: 0000 fa55 2f62 696f 7465 6368 2f76 656e  ...U/biotech/ven
-00000280: 7565 732f 7374 6167 6573 2f62 696f 7465  ues/stages/biote
-00000290: 6368 2f70 726f 6365 6475 7265 732f 696e  ch/procedures/in
-000002a0: 7472 6f2f 636f 6d73 2f69 6d70 6c69 6369  tro/coms/implici
-000002b0: 745f 7072 6f63 6564 7572 652f 7365 6e64  t_procedure/send
-000002c0: 5f70 6174 6873 2e70 79da 0a73 656e 645f  _paths.py..send_
-000002d0: 7061 7468 730f 0000 0073 0c00 0000 0804  paths....s......
-000002e0: 0c03 0e01 1401 0401 0802 7213 0000 0029  ..........r....)
-000002f0: 0ada 075f 5f64 6f63 5f5f da14 626f 7461  ...__doc__..bota
-00000300: 6e69 7374 2e63 7963 6c65 2e6c 6f6f 7073  nist.cycle.loops
-00000310: da05 6379 636c 65da 056c 6f6f 7073 da0b  ..cycle..loops..
-00000320: 6379 636c 655f 6c6f 6f70 73da 1762 6f74  cycle_loops..bot
-00000330: 616e 6973 742e 6379 636c 652e 7072 6573  anist.cycle.pres
-00000340: 656e 7473 7202 0000 00da 0e63 7963 6c65  entsr......cycle
-00000350: 5f70 7265 7365 6e74 7372 0800 0000 7213  _presentsr....r.
-00000360: 0000 0072 1100 0000 7211 0000 0072 1100  ...r....r....r..
-00000370: 0000 7212 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000380: 3e01 0000 0073 0e00 0000 0401 1208 0c01  >....s..........
-00000390: 0802 0203 0201 0efe                      ........
+00000090: 6d73 2e61 6767 7265 6761 746f 725f 7072  ms.aggregator_pr
+000000a0: 6f63 6564 7572 652e 7365 6e64 5f70 6174  ocedure.send_pat
+000000b0: 6873 2069 6d70 6f72 7420 7365 6e64 5f70  hs import send_p
+000000c0: 6174 6873 5f74 6f5f 6167 6772 6567 6174  aths_to_aggregat
+000000d0: 6f72 0a09 7365 6e64 5f70 6174 6873 5f74  or..send_paths_t
+000000e0: 6f5f 6167 6772 6567 6174 6f72 2028 0a09  o_aggregator (..
+000000f0: 0970 6f72 7420 3d20 302c 0a09 0970 6163  .port = 0,...pac
+00000100: 6b65 7420 3d20 7b7d 0a09 290a e900 0000  ket = {}..).....
+00000110: 004e 2901 da08 7072 6573 656e 7473 da00  .N)...presents..
+00000120: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+00000130: 0004 0000 0043 0000 0073 3a00 0000 6401  .....C...s:...d.
+00000140: 7c00 9b00 6402 9d03 7d02 7400 6a01 7c02  |...d...}.t.j.|.
+00000150: 7c01 6403 8d02 7d03 7c03 6a02 6404 6b02  |.d...}.|.j.d.k.
+00000160: 7219 7c03 6a03 6405 6b02 7219 6406 5300  r.|.j.d.k.r.d.S.
+00000170: 7404 6407 8301 8201 2908 4e7a 0f68 7474  t.d.....).Nz.htt
+00000180: 703a 2f2f 302e 302e 302e 303a 7a06 2f70  p://0.0.0.0:z./p
+00000190: 6174 6873 2901 da04 6a73 6f6e e9c8 0000  aths)...json....
+000001a0: 00da 0872 6563 6569 7665 6454 7a48 416e  ...receivedTzHAn
+000001b0: 2065 7863 6570 7469 6f6e 206f 6363 7572   exception occur
+000001c0: 7265 6420 7768 696c 6520 7365 6e64 696e  red while sendin
+000001d0: 6720 7468 6520 7061 7468 7320 746f 2074  g the paths to t
+000001e0: 6865 2069 6d70 6c69 6369 7420 7072 6f63  he implicit proc
+000001f0: 6564 7572 652e 2905 da08 7265 7175 6573  edure.)...reques
+00000200: 7473 da05 7061 7463 68da 0b73 7461 7475  ts..patch..statu
+00000210: 735f 636f 6465 da04 7465 7874 da09 4578  s_code..text..Ex
+00000220: 6365 7074 696f 6e29 04da 0470 6f72 74da  ception)...port.
+00000230: 0670 6163 6b65 74da 0355 524c da08 7265  .packet..URL..re
+00000240: 7370 6f6e 7365 a900 7210 0000 00fa 5f2f  sponse..r....._/
+00000250: 6269 6f74 6563 682f 7665 6e75 6573 2f73  biotech/venues/s
+00000260: 7461 6765 732f 6269 6f74 6563 682f 7072  tages/biotech/pr
+00000270: 6f63 6564 7572 6573 2f69 6e74 726f 2f70  ocedures/intro/p
+00000280: 726f 6365 7373 2f63 6f6d 732f 6167 6772  rocess/coms/aggr
+00000290: 6567 6174 6f72 5f70 726f 6365 6475 7265  egator_procedure
+000002a0: 2f73 656e 645f 7061 7468 732e 7079 da18  /send_paths.py..
+000002b0: 7365 6e64 5f70 6174 6873 5f74 6f5f 6167  send_paths_to_ag
+000002c0: 6772 6567 6174 6f72 0f00 0000 730a 0000  gregator....s...
+000002d0: 000c 040e 0114 0104 0108 0272 1200 0000  ...........r....
+000002e0: 290a da07 5f5f 646f 635f 5fda 1462 6f74  )...__doc__..bot
+000002f0: 616e 6973 742e 6379 636c 652e 6c6f 6f70  anist.cycle.loop
+00000300: 73da 0563 7963 6c65 da05 6c6f 6f70 73da  s..cycle..loops.
+00000310: 0b63 7963 6c65 5f6c 6f6f 7073 da17 626f  .cycle_loops..bo
+00000320: 7461 6e69 7374 2e63 7963 6c65 2e70 7265  tanist.cycle.pre
+00000330: 7365 6e74 7372 0200 0000 da0e 6379 636c  sentsr......cycl
+00000340: 655f 7072 6573 656e 7473 7207 0000 0072  e_presentsr....r
+00000350: 1200 0000 7210 0000 0072 1000 0000 7210  ....r....r....r.
+00000360: 0000 0072 1100 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000370: 653e 0100 0000 730e 0000 0004 0112 080c  e>....s.........
+00000380: 0108 0202 0302 010e fe                   .........
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/intro/coms/implicit_procedure/send_paths.py` & `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/coms/aggregator_procedure/send_paths.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 '''
-	from biotech.procedures.intro.coms.implicit_procedure.send_paths import send_paths
+	from biotech.procedures.intro.coms.aggregator_procedure.send_paths import send_paths
 	send_paths (
 		port = 0,
 		packet = {}
 	)
 '''
 
 import botanist.cycle.loops as cycle_loops
@@ -12,16 +12,13 @@
 
 import requests
 
 def send_paths (
 	port = "",
 	packet = {}
 ):
-	print ("awaiting the open of the implicit procedure harbor")
-
-
 	URL = f"http://0.0.0.0:{ port }/paths"
 	response = requests.patch (URL, json = packet)
 	if (response.status_code == 200 and response.text == "received"):
 		return True;
 
 	raise Exception ("An exception occurred while sending the paths to the implicit procedure.")
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/intro/keg/__init__.py` & `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,65 @@
 
 '''
+	This one is used because there is not a
+	solid programmatic flask off toggle.
 	
+		perhaps uvicorn + ... ?
+		
+		perhaps start the intro in pexpect...
+		
+			intro 
+				aggregator
+					health_scan
 '''
 
-
+#----
+#
+from biotech.topics.show.variable import show_variable
+#
+#
+import rich
+#
+#
 from http.server import BaseHTTPRequestHandler, HTTPServer
 import json
 import threading
 import time
+#
+#----
 
-import rich
-
+'''
+	netstat -tuln | grep 52434
+'''
 
 
 def open_harbor (
 	port = 0,
 	records = 0,
 	
 	health_scans_done = lambda *args, **kwargs: None
 ):
-	class RequestHandler(BaseHTTPRequestHandler):
-		def do_GET(self):
-			self.send_response(200)
-			self.send_header('Content-type', 'text/html')
-			self.end_headers()
-			self.wfile.write(b"Hello, World!")
-
-		def do_PATCH(self):
-			print ("""
-				
-				intro harbor @ [patch] /done
-				
-			""")	
+	class RequestHandler (BaseHTTPRequestHandler):
+		def do_GET (self):
+			self.send_response (200)
+			self.send_header ('Content-type', 'text/html')
+			self.end_headers ()
+			self.wfile.write (b"Hello, World!")
+
+		def do_PATCH (self):
+			show_variable ({
+				"intro harbor": "@ [patch] /done"
+			})	
 		
 			content_length = int(self.headers['Content-Length'])
-			post_data = self.rfile.read(content_length)
+			post_data = self.rfile.read (content_length)
 			try:
 				the_packet = json.loads (post_data.decode('utf-8'))
 				
-				rich.print_json (data = {
+				show_variable ({
 					"intro harbor /done: the_packet": the_packet
 				})
 			
 				health_scans_done (the_packet)
 				
 				self.send_response(200)
 			except json.JSONDecodeError:
@@ -54,24 +71,31 @@
 		def __init__(self, host='0.0.0.0', port=5000):
 			self.host = host
 			self.port = port
 			self.httpd = None
 			self.Harbor_thread = None
 
 		def start(self):
+			show_variable ({
+				"starting intro harbor:": {
+					"port": self.port,
+					"host": self.host
+				}
+			})
+		
 			self.httpd = HTTPServer ((self.host, self.port), RequestHandler)
 			self.Harbor_thread = threading.Thread(target=self.httpd.serve_forever)
 			self.Harbor_thread.start()
-			print(f"Harbor started on {self.host}:{self.port}")
+			show_variable (f"intro harbor started on {self.host}:{self.port}")
 
 		def stop(self):
 			if self.httpd:
-				self.httpd.shutdown()
-				self.Harbor_thread.join()
-				print("Harbor stopped.")
+				self.httpd.shutdown ()
+				self.Harbor_thread.join ()
+				show_variable ("intro harbor stopped.")
 
 	harbor = Harbor (
 		port = port
 	)
 	
 	
 	return [ harbor ]
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/intro/keg/__init__v1.py` & `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__init__v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 			port = port,
 			debug = False
 		)
 		
 		#return app;
 	
 	stop_event = threading.Event ()
-	
 	harbor = threading.Thread (target = start, args=(stop_event, ))
 	harbor.daemon = True  # automatically exit when the main program exits
 	#harbor.start ()
 	
 	
 	
 	# harbor = Process (target = start)
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 15 20:59:54 2024 UTC, .py size: 1541 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,162 +1,181 @@
-00000000: 6f0d 0d0a 0000 0000 4a95 1d66 0506 0000  o.......J..f....
+00000000: 6f0d 0d0a 0000 0000 0998 2066 c707 0000  o......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
-00000040: 0100 6401 6403 6c04 5a04 6401 6403 6c05  ..d.d.l.Z.d.d.l.
-00000050: 5a05 6401 6403 6c06 5a06 6401 6403 6c07  Z.d.d.l.Z.d.d.l.
-00000060: 5a07 6401 6401 6404 6405 8400 6603 6406  Z.d.d.d.d...f.d.
-00000070: 6407 8401 5a08 6403 5300 2908 7a03 0a09  d...Z.d.S.).z...
-00000080: 0ae9 0000 0000 2902 da16 4261 7365 4854  ......)...BaseHT
-00000090: 5450 5265 7175 6573 7448 616e 646c 6572  TPRequestHandler
-000000a0: da0a 4854 5450 5365 7276 6572 4e63 0000  ..HTTPServerNc..
-000000b0: 0000 0000 0000 0000 0000 0200 0000 0100  ................
-000000c0: 0000 4f00 0000 7304 0000 0064 0053 00a9  ..O...s....d.S..
-000000d0: 014e a900 2902 da04 6172 6773 da06 6b77  .N..)...args..kw
-000000e0: 6172 6773 7205 0000 0072 0500 0000 fa3b  argsr....r.....;
-000000f0: 2f76 6f6c 7473 2f76 656e 7565 732f 7374  /volts/venues/st
-00000100: 6167 6573 2f76 6f6c 7473 2f70 726f 6365  ages/volts/proce
-00000110: 6475 7265 732f 696e 7472 6f2f 6b65 672f  dures/intro/keg/
-00000120: 5f5f 696e 6974 5f5f 2e70 79da 083c 6c61  __init__.py..<la
-00000130: 6d62 6461 3e14 0000 0073 0200 0000 0400  mbda>....s......
-00000140: 7209 0000 0063 0300 0000 0000 0000 0000  r....c..........
-00000150: 0000 0500 0000 0400 0000 0300 0000 7336  ..............s6
-00000160: 0000 0047 0087 0166 0164 0164 0284 0864  ...G...f.d.d...d
-00000170: 0274 0083 0389 0047 0087 0066 0164 0364  .t.....G...f.d.d
-00000180: 0484 0864 0483 027d 037c 037c 0064 058d  ...d...}.|.|.d..
-00000190: 017d 047c 0467 0153 0029 064e 6300 0000  .}.|.g.S.).Nc...
-000001a0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-000001b0: 0000 0000 0073 2000 0000 6500 5a01 6400  .....s ...e.Z.d.
-000001c0: 5a02 6401 6402 8400 5a03 8700 6601 6403  Z.d.d...Z...f.d.
-000001d0: 6404 8408 5a04 6405 5300 2906 7a23 6f70  d...Z.d.S.).z#op
-000001e0: 656e 5f68 6172 626f 722e 3c6c 6f63 616c  en_harbor.<local
-000001f0: 733e 2e52 6571 7565 7374 4861 6e64 6c65  s>.RequestHandle
-00000200: 7263 0100 0000 0000 0000 0000 0000 0100  rc..............
-00000210: 0000 0400 0000 5300 0000 732e 0000 007c  ......S...s....|
-00000220: 00a0 0064 01a1 0101 007c 00a0 0164 0264  ...d.....|...d.d
-00000230: 03a1 0201 007c 00a0 02a1 0001 007c 006a  .....|.......|.j
-00000240: 03a0 0464 04a1 0101 0064 0053 0029 054e  ...d.....d.S.).N
-00000250: e9c8 0000 007a 0c43 6f6e 7465 6e74 2d74  .....z.Content-t
-00000260: 7970 657a 0974 6578 742f 6874 6d6c 730d  ypez.text/htmls.
-00000270: 0000 0048 656c 6c6f 2c20 576f 726c 6421  ...Hello, World!
-00000280: 2905 da0d 7365 6e64 5f72 6573 706f 6e73  )...send_respons
-00000290: 65da 0b73 656e 645f 6865 6164 6572 da0b  e..send_header..
-000002a0: 656e 645f 6865 6164 6572 73da 0577 6669  end_headers..wfi
-000002b0: 6c65 da05 7772 6974 65a9 01da 0473 656c  le..write....sel
-000002c0: 6672 0500 0000 7205 0000 0072 0800 0000  fr....r....r....
-000002d0: da06 646f 5f47 4554 1700 0000 7308 0000  ..do_GET....s...
-000002e0: 000a 010c 0108 0110 017a 2a6f 7065 6e5f  .........z*open_
-000002f0: 6861 7262 6f72 2e3c 6c6f 6361 6c73 3e2e  harbor.<locals>.
-00000300: 5265 7175 6573 7448 616e 646c 6572 2e64  RequestHandler.d
-00000310: 6f5f 4745 5463 0100 0000 0000 0000 0000  o_GETc..........
-00000320: 0000 0400 0000 0800 0000 1300 0000 7384  ..............s.
-00000330: 0000 0074 0064 0183 0101 0074 017c 006a  ...t.d.....t.|.j
-00000340: 0264 0219 0083 017d 017c 006a 03a0 047c  .d.....}.|.j...|
-00000350: 01a1 017d 027a 1b74 05a0 067c 02a0 0764  ...}.z.t...|...d
-00000360: 03a1 01a1 017d 0374 086a 0964 047c 0369  .....}.t.j.d.|.i
-00000370: 0164 058d 0101 0088 007c 0383 0101 007c  .d.......|.....|
-00000380: 00a0 0a64 06a1 0101 0057 006e 0f04 0074  ...d.....W.n...t
-00000390: 056a 0b79 3b01 0001 0001 007c 00a0 0a64  .j.y;......|...d
-000003a0: 07a1 0101 0059 006e 0177 007c 00a0 0ca1  .....Y.n.w.|....
-000003b0: 0001 0064 0053 0029 084e 7a2f 0a09 0909  ...d.S.).Nz/....
-000003c0: 090a 0909 0909 696e 7472 6f20 6861 7262  ......intro harb
-000003d0: 6f72 2040 205b 7061 7463 685d 202f 646f  or @ [patch] /do
-000003e0: 6e65 0a09 0909 090a 0909 097a 0e43 6f6e  ne.........z.Con
-000003f0: 7465 6e74 2d4c 656e 6774 687a 0575 7466  tent-Lengthz.utf
-00000400: 2d38 7a1e 696e 7472 6f20 6861 7262 6f72  -8z.intro harbor
-00000410: 202f 646f 6e65 3a20 7468 655f 7061 636b   /done: the_pack
-00000420: 6574 2901 da04 6461 7461 720a 0000 0069  et)...datar....i
-00000430: 9001 0000 290d da05 7072 696e 74da 0369  ....)...print..i
-00000440: 6e74 da07 6865 6164 6572 73da 0572 6669  nt..headers..rfi
-00000450: 6c65 da04 7265 6164 da04 6a73 6f6e da05  le..read..json..
-00000460: 6c6f 6164 73da 0664 6563 6f64 65da 0472  loads..decode..r
-00000470: 6963 68da 0a70 7269 6e74 5f6a 736f 6e72  ich..print_jsonr
-00000480: 0b00 0000 da0f 4a53 4f4e 4465 636f 6465  ......JSONDecode
-00000490: 4572 726f 7272 0d00 0000 2904 7211 0000  Errorr....).r...
-000004a0: 00da 0e63 6f6e 7465 6e74 5f6c 656e 6774  ...content_lengt
-000004b0: 68da 0970 6f73 745f 6461 7461 da0a 7468  h..post_data..th
-000004c0: 655f 7061 636b 6574 a901 da11 6865 616c  e_packet....heal
-000004d0: 7468 5f73 6361 6e73 5f64 6f6e 6572 0500  th_scans_doner..
-000004e0: 0000 7208 0000 00da 0864 6f5f 5041 5443  ..r......do_PATC
-000004f0: 481d 0000 0073 1c00 0000 0801 0e06 0c01  H....s..........
-00000500: 0201 1001 0402 0401 08ff 0804 0e02 0e01  ................
-00000510: 0e01 02ff 0c03 7a2c 6f70 656e 5f68 6172  ......z,open_har
-00000520: 626f 722e 3c6c 6f63 616c 733e 2e52 6571  bor.<locals>.Req
-00000530: 7565 7374 4861 6e64 6c65 722e 646f 5f50  uestHandler.do_P
-00000540: 4154 4348 4e29 05da 085f 5f6e 616d 655f  ATCHN)...__name_
-00000550: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000560: 5f71 7561 6c6e 616d 655f 5f72 1200 0000  _qualname__r....
-00000570: 7224 0000 0072 0500 0000 7222 0000 0072  r$...r....r"...r
-00000580: 0500 0000 7208 0000 00da 0e52 6571 7565  ....r......Reque
-00000590: 7374 4861 6e64 6c65 7216 0000 0073 0600  stHandler....s..
-000005a0: 0000 0800 0801 1006 7228 0000 0063 0000  ........r(...c..
-000005b0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000005c0: 0000 0000 0000 732a 0000 0065 005a 0164  ......s*...e.Z.d
-000005d0: 005a 0264 0a64 0364 0484 015a 0387 0066  .Z.d.d.d...Z...f
-000005e0: 0164 0564 0684 085a 0464 0764 0884 005a  .d.d...Z.d.d...Z
-000005f0: 0564 0953 0029 0b7a 1b6f 7065 6e5f 6861  .d.S.).z.open_ha
-00000600: 7262 6f72 2e3c 6c6f 6361 6c73 3e2e 4861  rbor.<locals>.Ha
-00000610: 7262 6f72 fa07 302e 302e 302e 30e9 8813  rbor..0.0.0.0...
-00000620: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00000630: 0000 0002 0000 0053 0000 0073 1c00 0000  .......S...s....
-00000640: 7c01 7c00 5f00 7c02 7c00 5f01 6400 7c00  |.|._.|.|._.d.|.
-00000650: 5f02 6400 7c00 5f03 6400 5300 7204 0000  _.d.|._.d.S.r...
-00000660: 0029 04da 0468 6f73 74da 0470 6f72 74da  .)...host..port.
-00000670: 0568 7474 7064 da0d 4861 7262 6f72 5f74  .httpd..Harbor_t
-00000680: 6872 6561 6429 0372 1100 0000 722b 0000  hread).r....r+..
-00000690: 0072 2c00 0000 7205 0000 0072 0500 0000  .r,...r....r....
-000006a0: 7208 0000 00da 085f 5f69 6e69 745f 5f36  r......__init__6
-000006b0: 0000 0073 0800 0000 0601 0601 0601 0a01  ...s............
-000006c0: 7a24 6f70 656e 5f68 6172 626f 722e 3c6c  z$open_harbor.<l
-000006d0: 6f63 616c 733e 2e48 6172 626f 722e 5f5f  ocals>.Harbor.__
-000006e0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
-000006f0: 0000 0001 0000 0005 0000 0013 0000 0073  ...............s
-00000700: 4c00 0000 7400 7c00 6a01 7c00 6a02 6602  L...t.|.j.|.j.f.
-00000710: 8800 8302 7c00 5f03 7404 6a05 7c00 6a03  ....|._.t.j.|.j.
-00000720: 6a06 6401 8d01 7c00 5f07 7c00 6a07 a008  j.d...|._.|.j...
-00000730: a100 0100 7409 6402 7c00 6a01 9b00 6403  ....t.d.|.j...d.
-00000740: 7c00 6a02 9b00 9d04 8301 0100 6400 5300  |.j.........d.S.
-00000750: 2904 4e29 01da 0674 6172 6765 747a 1248  ).N)...targetz.H
-00000760: 6172 626f 7220 7374 6172 7465 6420 6f6e  arbor started on
-00000770: 20fa 013a 290a 7203 0000 0072 2b00 0000   ..:).r....r+...
-00000780: 722c 0000 0072 2d00 0000 da09 7468 7265  r,...r-.....thre
-00000790: 6164 696e 67da 0654 6872 6561 64da 0d73  ading..Thread..s
-000007a0: 6572 7665 5f66 6f72 6576 6572 722e 0000  erve_foreverr...
-000007b0: 00da 0573 7461 7274 7214 0000 0072 1000  ...startr....r..
-000007c0: 0000 a901 7228 0000 0072 0500 0000 7208  ....r(...r....r.
-000007d0: 0000 0072 3500 0000 3c00 0000 7308 0000  ...r5...<...s...
-000007e0: 0014 0112 010a 011c 017a 216f 7065 6e5f  .........z!open_
-000007f0: 6861 7262 6f72 2e3c 6c6f 6361 6c73 3e2e  harbor.<locals>.
-00000800: 4861 7262 6f72 2e73 7461 7274 6301 0000  Harbor.startc...
-00000810: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000820: 0053 0000 0073 2a00 0000 7c00 6a00 7213  .S...s*...|.j.r.
-00000830: 7c00 6a00 a001 a100 0100 7c00 6a02 a003  |.j.......|.j...
-00000840: a100 0100 7404 6401 8301 0100 6400 5300  ....t.d.....d.S.
-00000850: 6400 5300 2902 4e7a 0f48 6172 626f 7220  d.S.).Nz.Harbor 
-00000860: 7374 6f70 7065 642e 2905 722d 0000 00da  stopped.).r-....
-00000870: 0873 6875 7464 6f77 6e72 2e00 0000 da04  .shutdownr......
-00000880: 6a6f 696e 7214 0000 0072 1000 0000 7205  joinr....r....r.
-00000890: 0000 0072 0500 0000 7208 0000 00da 0473  ...r....r......s
-000008a0: 746f 7042 0000 0073 0a00 0000 0601 0a01  topB...s........
-000008b0: 0a01 0c01 04fd 7a20 6f70 656e 5f68 6172  ......z open_har
-000008c0: 626f 722e 3c6c 6f63 616c 733e 2e48 6172  bor.<locals>.Har
-000008d0: 626f 722e 7374 6f70 4e29 0272 2900 0000  bor.stopN).r)...
-000008e0: 722a 0000 0029 0672 2500 0000 7226 0000  r*...).r%...r&..
-000008f0: 0072 2700 0000 722f 0000 0072 3500 0000  .r'...r/...r5...
-00000900: 7239 0000 0072 0500 0000 7236 0000 0072  r9...r....r6...r
-00000910: 0500 0000 7208 0000 00da 0648 6172 626f  ....r......Harbo
-00000920: 7235 0000 0073 0800 0000 0800 0a01 0c06  r5...s..........
-00000930: 0c06 723a 0000 0029 0172 2c00 0000 2901  ..r:...).r,...).
-00000940: 7202 0000 0029 0572 2c00 0000 da07 7265  r....).r,.....re
-00000950: 636f 7264 7372 2300 0000 723a 0000 00da  cordsr#...r:....
-00000960: 0668 6172 626f 7272 0500 0000 2902 7228  .harborr....).r(
-00000970: 0000 0072 2300 0000 7208 0000 00da 0b6f  ...r#...r......o
-00000980: 7065 6e5f 6861 7262 6f72 1000 0000 730c  pen_harbor....s.
-00000990: 0000 0014 0612 1f02 1302 0106 ff06 0572  ...............r
-000009a0: 3d00 0000 2909 da07 5f5f 646f 635f 5fda  =...)...__doc__.
-000009b0: 0b68 7474 702e 7365 7276 6572 7202 0000  .http.serverr...
-000009c0: 0072 0300 0000 7219 0000 0072 3200 0000  .r....r....r2...
-000009d0: da04 7469 6d65 721c 0000 0072 3d00 0000  ..timer....r=...
-000009e0: 7205 0000 0072 0500 0000 7205 0000 0072  r....r....r....r
-000009f0: 0800 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000a00: 0000 7314 0000 0004 0110 0508 0108 0108  ..s.............
-00000a10: 0108 0202 0502 0106 020e fc              ...........
+00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
+00000050: 6d06 5a06 0100 6401 6403 6c07 5a07 6401  m.Z...d.d.l.Z.d.
+00000060: 6403 6c08 5a08 6401 6403 6c09 5a09 0900  d.l.Z.d.d.l.Z...
+00000070: 6401 6401 6405 6406 8400 6603 6407 6408  d.d.d.d...f.d.d.
+00000080: 8401 5a0a 6403 5300 2909 7ac4 0a09 5468  ..Z.d.S.).z...Th
+00000090: 6973 206f 6e65 2069 7320 7573 6564 2062  is one is used b
+000000a0: 6563 6175 7365 2074 6865 7265 2069 7320  ecause there is 
+000000b0: 6e6f 7420 610a 0973 6f6c 6964 2070 726f  not a..solid pro
+000000c0: 6772 616d 6d61 7469 6320 666c 6173 6b20  grammatic flask 
+000000d0: 6f66 6620 746f 6767 6c65 2e0a 090a 0909  off toggle......
+000000e0: 7065 7268 6170 7320 7576 6963 6f72 6e20  perhaps uvicorn 
+000000f0: 2b20 2e2e 2e20 3f0a 0909 0a09 0970 6572  + ... ?......per
+00000100: 6861 7073 2073 7461 7274 2074 6865 2069  haps start the i
+00000110: 6e74 726f 2069 6e20 7065 7870 6563 742e  ntro in pexpect.
+00000120: 2e2e 0a09 090a 0909 0969 6e74 726f 200a  .........intro .
+00000130: 0909 0909 6167 6772 6567 6174 6f72 0a09  ....aggregator..
+00000140: 0909 0909 6865 616c 7468 5f73 6361 6e0a  ....health_scan.
+00000150: e900 0000 0029 01da 0d73 686f 775f 7661  .....)...show_va
+00000160: 7269 6162 6c65 4e29 02da 1642 6173 6548  riableN)...BaseH
+00000170: 5454 5052 6571 7565 7374 4861 6e64 6c65  TTPRequestHandle
+00000180: 72da 0a48 5454 5053 6572 7665 7263 0000  r..HTTPServerc..
+00000190: 0000 0000 0000 0000 0000 0200 0000 0100  ................
+000001a0: 0000 4f00 0000 7304 0000 0064 0053 00a9  ..O...s....d.S..
+000001b0: 014e a900 2902 da04 6172 6773 da06 6b77  .N..)...args..kw
+000001c0: 6172 6773 7206 0000 0072 0600 0000 fa3f  argsr....r.....?
+000001d0: 2f62 696f 7465 6368 2f76 656e 7565 732f  /biotech/venues/
+000001e0: 7374 6167 6573 2f62 696f 7465 6368 2f70  stages/biotech/p
+000001f0: 726f 6365 6475 7265 732f 696e 7472 6f2f  rocedures/intro/
+00000200: 6b65 672f 5f5f 696e 6974 5f5f 2e70 79da  keg/__init__.py.
+00000210: 083c 6c61 6d62 6461 3e27 0000 0073 0200  .<lambda>'...s..
+00000220: 0000 0400 720a 0000 0063 0300 0000 0000  ....r....c......
+00000230: 0000 0000 0000 0500 0000 0400 0000 0300  ................
+00000240: 0000 7336 0000 0047 0087 0166 0164 0164  ..s6...G...f.d.d
+00000250: 0284 0864 0274 0083 0389 0047 0087 0066  ...d.t.....G...f
+00000260: 0164 0364 0484 0864 0483 027d 037c 037c  .d.d...d...}.|.|
+00000270: 0064 058d 017d 047c 0467 0153 0029 064e  .d...}.|.g.S.).N
+00000280: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000290: 0003 0000 0000 0000 0073 2000 0000 6500  .........s ...e.
+000002a0: 5a01 6400 5a02 6401 6402 8400 5a03 8700  Z.d.Z.d.d...Z...
+000002b0: 6601 6403 6404 8408 5a04 6405 5300 2906  f.d.d...Z.d.S.).
+000002c0: 7a23 6f70 656e 5f68 6172 626f 722e 3c6c  z#open_harbor.<l
+000002d0: 6f63 616c 733e 2e52 6571 7565 7374 4861  ocals>.RequestHa
+000002e0: 6e64 6c65 7263 0100 0000 0000 0000 0000  ndlerc..........
+000002f0: 0000 0100 0000 0400 0000 5300 0000 732e  ..........S...s.
+00000300: 0000 007c 00a0 0064 01a1 0101 007c 00a0  ...|...d.....|..
+00000310: 0164 0264 03a1 0201 007c 00a0 02a1 0001  .d.d.....|......
+00000320: 007c 006a 03a0 0464 04a1 0101 0064 0053  .|.j...d.....d.S
+00000330: 0029 054e e9c8 0000 007a 0c43 6f6e 7465  .).N.....z.Conte
+00000340: 6e74 2d74 7970 657a 0974 6578 742f 6874  nt-typez.text/ht
+00000350: 6d6c 730d 0000 0048 656c 6c6f 2c20 576f  mls....Hello, Wo
+00000360: 726c 6421 2905 da0d 7365 6e64 5f72 6573  rld!)...send_res
+00000370: 706f 6e73 65da 0b73 656e 645f 6865 6164  ponse..send_head
+00000380: 6572 da0b 656e 645f 6865 6164 6572 73da  er..end_headers.
+00000390: 0577 6669 6c65 da05 7772 6974 65a9 01da  .wfile..write...
+000003a0: 0473 656c 6672 0600 0000 7206 0000 0072  .selfr....r....r
+000003b0: 0900 0000 da06 646f 5f47 4554 2a00 0000  ......do_GET*...
+000003c0: 7308 0000 000a 010c 0108 0110 017a 2a6f  s............z*o
+000003d0: 7065 6e5f 6861 7262 6f72 2e3c 6c6f 6361  pen_harbor.<loca
+000003e0: 6c73 3e2e 5265 7175 6573 7448 616e 646c  ls>.RequestHandl
+000003f0: 6572 2e64 6f5f 4745 5463 0100 0000 0000  er.do_GETc......
+00000400: 0000 0000 0000 0400 0000 0800 0000 1300  ................
+00000410: 0000 7384 0000 0074 0064 0164 0269 0183  ..s....t.d.d.i..
+00000420: 0101 0074 017c 006a 0264 0319 0083 017d  ...t.|.j.d.....}
+00000430: 017c 006a 03a0 047c 01a1 017d 027a 1974  .|.j...|...}.z.t
+00000440: 05a0 067c 02a0 0764 04a1 01a1 017d 0374  ...|...d.....}.t
+00000450: 0064 057c 0369 0183 0101 0088 007c 0383  .d.|.i.......|..
+00000460: 0101 007c 00a0 0864 06a1 0101 0057 006e  ...|...d.....W.n
+00000470: 0f04 0074 056a 0979 3b01 0001 0001 007c  ...t.j.y;......|
+00000480: 00a0 0864 07a1 0101 0059 006e 0177 007c  ...d.....Y.n.w.|
+00000490: 00a0 0aa1 0001 0064 0053 0029 084e 7a0c  .......d.S.).Nz.
+000004a0: 696e 7472 6f20 6861 7262 6f72 7a0f 4020  intro harborz.@ 
+000004b0: 5b70 6174 6368 5d20 2f64 6f6e 657a 0e43  [patch] /donez.C
+000004c0: 6f6e 7465 6e74 2d4c 656e 6774 687a 0575  ontent-Lengthz.u
+000004d0: 7466 2d38 7a1e 696e 7472 6f20 6861 7262  tf-8z.intro harb
+000004e0: 6f72 202f 646f 6e65 3a20 7468 655f 7061  or /done: the_pa
+000004f0: 636b 6574 720b 0000 0069 9001 0000 290b  cketr....i....).
+00000500: 7202 0000 00da 0369 6e74 da07 6865 6164  r......int..head
+00000510: 6572 73da 0572 6669 6c65 da04 7265 6164  ers..rfile..read
+00000520: da04 6a73 6f6e da05 6c6f 6164 73da 0664  ..json..loads..d
+00000530: 6563 6f64 6572 0c00 0000 da0f 4a53 4f4e  ecoder......JSON
+00000540: 4465 636f 6465 4572 726f 7272 0e00 0000  DecodeErrorr....
+00000550: 2904 7212 0000 00da 0e63 6f6e 7465 6e74  ).r......content
+00000560: 5f6c 656e 6774 68da 0970 6f73 745f 6461  _length..post_da
+00000570: 7461 da0a 7468 655f 7061 636b 6574 a901  ta..the_packet..
+00000580: da11 6865 616c 7468 5f73 6361 6e73 5f64  ..health_scans_d
+00000590: 6f6e 6572 0600 0000 7209 0000 00da 0864  oner....r......d
+000005a0: 6f5f 5041 5443 4830 0000 0073 2000 0000  o_PATCH0...s ...
+000005b0: 0201 0401 06ff 0e04 0c01 0201 1001 0202  ................
+000005c0: 0401 06ff 0804 0e02 0e01 0e01 02ff 0c03  ................
+000005d0: 7a2c 6f70 656e 5f68 6172 626f 722e 3c6c  z,open_harbor.<l
+000005e0: 6f63 616c 733e 2e52 6571 7565 7374 4861  ocals>.RequestHa
+000005f0: 6e64 6c65 722e 646f 5f50 4154 4348 4e29  ndler.do_PATCHN)
+00000600: 05da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000610: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000620: 616d 655f 5f72 1300 0000 7221 0000 0072  ame__r....r!...r
+00000630: 0600 0000 721f 0000 0072 0600 0000 7209  ....r....r....r.
+00000640: 0000 00da 0e52 6571 7565 7374 4861 6e64  .....RequestHand
+00000650: 6c65 7229 0000 0073 0600 0000 0800 0801  ler)...s........
+00000660: 1006 7225 0000 0063 0000 0000 0000 0000  ..r%...c........
+00000670: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00000680: 732a 0000 0065 005a 0164 005a 0264 0a64  s*...e.Z.d.Z.d.d
+00000690: 0364 0484 015a 0387 0066 0164 0564 0684  .d...Z...f.d.d..
+000006a0: 085a 0464 0764 0884 005a 0564 0953 0029  .Z.d.d...Z.d.S.)
+000006b0: 0b7a 1b6f 7065 6e5f 6861 7262 6f72 2e3c  .z.open_harbor.<
+000006c0: 6c6f 6361 6c73 3e2e 4861 7262 6f72 fa07  locals>.Harbor..
+000006d0: 302e 302e 302e 30e9 8813 0000 6303 0000  0.0.0.0.....c...
+000006e0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+000006f0: 0053 0000 0073 1c00 0000 7c01 7c00 5f00  .S...s....|.|._.
+00000700: 7c02 7c00 5f01 6400 7c00 5f02 6400 7c00  |.|._.d.|._.d.|.
+00000710: 5f03 6400 5300 7205 0000 0029 04da 0468  _.d.S.r....)...h
+00000720: 6f73 74da 0470 6f72 74da 0568 7474 7064  ost..port..httpd
+00000730: da0d 4861 7262 6f72 5f74 6872 6561 6429  ..Harbor_thread)
+00000740: 0372 1200 0000 7228 0000 0072 2900 0000  .r....r(...r)...
+00000750: 7206 0000 0072 0600 0000 7209 0000 00da  r....r....r.....
+00000760: 085f 5f69 6e69 745f 5f47 0000 0073 0800  .__init__G...s..
+00000770: 0000 0601 0601 0601 0a01 7a24 6f70 656e  ..........z$open
+00000780: 5f68 6172 626f 722e 3c6c 6f63 616c 733e  _harbor.<locals>
+00000790: 2e48 6172 626f 722e 5f5f 696e 6974 5f5f  .Harbor.__init__
+000007a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000007b0: 0005 0000 0013 0000 0073 6200 0000 7400  .........sb...t.
+000007c0: 6401 7c00 6a01 7c00 6a02 6402 9c02 6901  d.|.j.|.j.d...i.
+000007d0: 8301 0100 7403 7c00 6a02 7c00 6a01 6602  ....t.|.j.|.j.f.
+000007e0: 8800 8302 7c00 5f04 7405 6a06 7c00 6a04  ....|._.t.j.|.j.
+000007f0: 6a07 6403 8d01 7c00 5f08 7c00 6a08 a009  j.d...|._.|.j...
+00000800: a100 0100 7400 6404 7c00 6a02 9b00 6405  ....t.d.|.j...d.
+00000810: 7c00 6a01 9b00 9d04 8301 0100 6400 5300  |.j.........d.S.
+00000820: 2906 4e7a 1673 7461 7274 696e 6720 696e  ).Nz.starting in
+00000830: 7472 6f20 6861 7262 6f72 3a29 0272 2900  tro harbor:).r).
+00000840: 0000 7228 0000 0029 01da 0674 6172 6765  ..r(...)...targe
+00000850: 747a 1869 6e74 726f 2068 6172 626f 7220  tz.intro harbor 
+00000860: 7374 6172 7465 6420 6f6e 20fa 013a 290a  started on ..:).
+00000870: 7202 0000 0072 2900 0000 7228 0000 0072  r....r)...r(...r
+00000880: 0400 0000 722a 0000 00da 0974 6872 6561  ....r*.....threa
+00000890: 6469 6e67 da06 5468 7265 6164 da0d 7365  ding..Thread..se
+000008a0: 7276 655f 666f 7265 7665 7272 2b00 0000  rve_foreverr+...
+000008b0: da05 7374 6172 7472 1100 0000 a901 7225  ..startr......r%
+000008c0: 0000 0072 0600 0000 7209 0000 0072 3200  ...r....r....r2.
+000008d0: 0000 4d00 0000 7314 0000 0002 0102 0104  ..M...s.........
+000008e0: 0104 0104 fe06 ff14 0712 010a 011c 017a  ...............z
+000008f0: 216f 7065 6e5f 6861 7262 6f72 2e3c 6c6f  !open_harbor.<lo
+00000900: 6361 6c73 3e2e 4861 7262 6f72 2e73 7461  cals>.Harbor.sta
+00000910: 7274 6301 0000 0000 0000 0000 0000 0001  rtc.............
+00000920: 0000 0002 0000 0053 0000 0073 2a00 0000  .......S...s*...
+00000930: 7c00 6a00 7213 7c00 6a00 a001 a100 0100  |.j.r.|.j.......
+00000940: 7c00 6a02 a003 a100 0100 7404 6401 8301  |.j.......t.d...
+00000950: 0100 6400 5300 6400 5300 2902 4e7a 1569  ..d.S.d.S.).Nz.i
+00000960: 6e74 726f 2068 6172 626f 7220 7374 6f70  ntro harbor stop
+00000970: 7065 642e 2905 722a 0000 00da 0873 6875  ped.).r*.....shu
+00000980: 7464 6f77 6e72 2b00 0000 da04 6a6f 696e  tdownr+.....join
+00000990: 7202 0000 0072 1100 0000 7206 0000 0072  r....r....r....r
+000009a0: 0600 0000 7209 0000 00da 0473 746f 705a  ....r......stopZ
+000009b0: 0000 0073 0a00 0000 0601 0a01 0a01 0c01  ...s............
+000009c0: 04fd 7a20 6f70 656e 5f68 6172 626f 722e  ..z open_harbor.
+000009d0: 3c6c 6f63 616c 733e 2e48 6172 626f 722e  <locals>.Harbor.
+000009e0: 7374 6f70 4e29 0272 2600 0000 7227 0000  stopN).r&...r'..
+000009f0: 0029 0672 2200 0000 7223 0000 0072 2400  .).r"...r#...r$.
+00000a00: 0000 722c 0000 0072 3200 0000 7236 0000  ..r,...r2...r6..
+00000a10: 0072 0600 0000 7233 0000 0072 0600 0000  .r....r3...r....
+00000a20: 7209 0000 00da 0648 6172 626f 7246 0000  r......HarborF..
+00000a30: 0073 0800 0000 0800 0a01 0c06 0c0d 7237  .s............r7
+00000a40: 0000 0029 0172 2900 0000 2901 7203 0000  ...).r)...).r...
+00000a50: 0029 0572 2900 0000 da07 7265 636f 7264  .).r).....record
+00000a60: 7372 2000 0000 7237 0000 00da 0668 6172  sr ...r7.....har
+00000a70: 626f 7272 0600 0000 2902 7225 0000 0072  borr....).r%...r
+00000a80: 2000 0000 7209 0000 00da 0b6f 7065 6e5f   ...r......open_
+00000a90: 6861 7262 6f72 2300 0000 730c 0000 0014  harbor#...s.....
+00000aa0: 0612 1d02 1a02 0106 ff06 0572 3a00 0000  ...........r:...
+00000ab0: 290b da07 5f5f 646f 635f 5fda 1c62 696f  )...__doc__..bio
+00000ac0: 7465 6368 2e74 6f70 6963 732e 7368 6f77  tech.topics.show
+00000ad0: 2e76 6172 6961 626c 6572 0200 0000 da04  .variabler......
+00000ae0: 7269 6368 da0b 6874 7470 2e73 6572 7665  rich..http.serve
+00000af0: 7272 0300 0000 7204 0000 0072 1800 0000  rr....r....r....
+00000b00: 722f 0000 00da 0474 696d 6572 3a00 0000  r/.....timer:...
+00000b10: 7206 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
+00000b20: 0900 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000b30: 0000 7318 0000 0004 010c 0f08 0310 0308  ..s.............
+00000b40: 0108 0108 0102 0402 0602 0106 020e fc    ...............
```

### Comparing `biotech-1.0.3/venues/stages/biotech/procedures/intro/keg/quart__init__.py` & `biotech-1.1.0/venues/stages/biotech/procedures/intro_v1/keg/quart__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/aggregate/__init__.py` & `biotech-1.1.0/venues/stages/biotech/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/alarm_parser/__init__.py` & `biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/implicit/thread/__init__.py` & `biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	def implicit_task():
 		while True:
 			time.sleep (5)
 			print ("implicit")
 			
 	implicit_thread = threading.Thread (target = implicit_task)
 	implicit_thread.daemon = True
-	implicit_thread.start()
+	implicit_thread.start ()
 '''
 
 import threading
 import time
 
 def implicit_thread (
 	task = None
```

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 20:48:34 2024 UTC, .py size: 1154 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 22e4 1e66 8204 0000  o......."..f....
+00000000: 6f0d 0d0a 0000 0000 b9b3 2066 8304 0000  o......... f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 5a00 0900 0900 0900 6401 6402 6c01 5a01  Z.......d.d.l.Z.
 00000040: 6401 6402 6c02 5a02 0902 6405 6403 6404  d.d.l.Z...d.d.d.
 00000050: 8401 5a03 6402 5300 2906 7a14 0a09 6974  ..Z.d.S.).z...it
 00000060: 696e 6572 6172 793a 0a09 095b 205d 200a  inerary:...[ ] .
 00000070: e900 0000 004e 6301 0000 0000 0000 0000  .....Nc.........
```

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/printout/passes.py` & `biotech-1.1.0/venues/stages/biotech/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/process_on/p_expect/__init__.py` & `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,16 +19,24 @@
 import atexit
 import os
 
 from multiprocessing import Process, Queue
 
 def off (venture):
 	try:
-		venture.close ()
-	except Exception:
+		print ("""
+		
+			attemping to stop the tethered venture
+		
+		""")
+		#venture.close ()
+		venture.terminate ()
+	except Exception as E:
+		print ("venture off exception:", E)
+	
 		pass;
 
 	
 
 def process_on (
 	process_string,
 	#
@@ -36,15 +44,15 @@
 	CWD = None,
 	env = {},
 	
 	name = "process",
 	
 	stop_event = None
 ):
-	#print ("process_string:", process_string)
+	print ("process_string:", process_string)
 	#print ("the_queue:", the_queue)
 	#print ("CWD:", CWD)
 	#print ("env:", env)
 
 	if (CWD == None):
 		CWD = os.getcwd ()
 		
@@ -54,23 +62,28 @@
 	report = {
 		"journal": []
 	}
 	p = pexpect.spawn (
 		process_string,
 		cwd = CWD,
 		env = env,
-		timeout = None
+		timeout = None,
+		
+		# encoding='utf-8'
 	)
 	def awareness_EOF (p):
 		while not p.eof ():
 		
 			line = p.readline ()
 
 			try:
 				UTF8_line = line.decode ('UTF8')
+				#UTF8_line = line.decode('ascii')				
+				#UTF8_line = line;
+				
 				UTF8_parsed = "yes"
 			except Exception:
 				UTF8_line = ""
 				UTF8_parsed = "no"
 				
 			try:
 				hexadecimal_line = line.hex ()
@@ -92,15 +105,17 @@
 			};
 			
 			the_queue.put (line_parsed)
 			
 			report ["journal"].append (line_parsed)
 			
 			if (UTF8_parsed == "yes"):
-				print (f'[{ name }:UTF8]', UTF8_line, end = '')
+				#print (f'[{ name }:UTF8]', UTF8_line, end = '')
+				print (f'[{ name }]', UTF8_line, end = '')
+				
 			else:
 				print ('unparseable UTF8 line')
 			
 			# rich.print_json (data = line_parsed)
 
 	awareness_EOF (p)
```

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 20:48:34 2024 UTC, .py size: 1461 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,114 @@
-00000000: 6f0d 0d0a 0000 0000 22e4 1e66 b505 0000  o......."..f....
+00000000: 6f0d 0d0a 0000 0000 97bd 2266 e606 0000  o........."f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
+00000020: 0004 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
-00000050: 6403 6c05 5a05 6401 6403 6c06 5a06 6401  d.l.Z.d.d.l.Z.d.
-00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 6401  d.l.m.Z.m.Z...d.
-00000070: 6403 6c07 5a07 6403 6403 6900 6405 6604  d.l.Z.d.d.i.d.f.
-00000080: 6406 6407 8401 5a0a 6403 5300 2908 6144  d.d...Z.d.S.).aD
-00000090: 0100 000a 0966 726f 6d20 6269 6f74 6563  .....from biotec
-000000a0: 682e 746f 7069 6373 2e70 726f 6365 7373  h.topics.process
-000000b0: 5f6f 6e2e 705f 6578 7065 6374 2e69 6d70  _on.p_expect.imp
-000000c0: 6c69 6369 7420 696d 706f 7274 2070 726f  licit import pro
-000000d0: 6365 7373 5f6f 6e5f 696d 706c 6963 6974  cess_on_implicit
-000000e0: 0a09 0a09 7665 6e74 7572 6520 3d20 7072  ....venture = pr
-000000f0: 6f63 6573 735f 6f6e 5f69 6d70 6c69 6369  ocess_on_implici
-00000100: 7420 280a 0909 2727 2c0a 0909 0a09 0943  t (...'',......C
-00000110: 5744 203d 204e 6f6e 652c 0a09 0965 6e76  WD = None,...env
-00000120: 203d 207b 7d0a 0929 0a09 0a09 230a 0923   = {}..)....#..#
-00000130: 2073 7461 7475 730a 0923 0a09 230a 0970   status..#..#..p
-00000140: 7269 6e74 2028 2773 7461 7475 733a 272c  rint ('status:',
-00000150: 2076 656e 7475 7265 205b 2270 726f 6365   venture ["proce
-00000160: 7373 225d 2e69 735f 616c 6976 6520 2829  ss"].is_alive ()
-00000170: 290a 090a 0923 0a09 2309 7374 6f70 2074  )....#..#.stop t
-00000180: 6865 2070 726f 6365 7373 0a09 230a 0923  he process..#..#
-00000190: 0a09 7665 6e74 7572 6520 5b22 7072 6f63  ..venture ["proc
-000001a0: 6573 7322 5d2e 7465 726d 696e 6174 6520  ess"].terminate 
-000001b0: 2829 0a09 0a09 7265 636f 7264 7320 3d20  ()....records = 
-000001c0: 7665 6e74 7572 6520 5b22 7265 636f 7264  venture ["record
-000001d0: 7322 5d20 2829 0ae9 0000 0000 2901 da0a  s"] ()......)...
-000001e0: 7072 6f63 6573 735f 6f6e 4e29 02da 0750  process_onN)...P
-000001f0: 726f 6365 7373 da05 5175 6575 65da 0770  rocess..Queue..p
-00000200: 726f 6365 7373 6305 0000 0000 0000 0000  rocessc.........
-00000210: 0000 0008 0000 0009 0000 0003 0000 0073  ...............s
-00000220: 5600 0000 7400 8300 8901 7401 a002 a100  V...t.....t.....
-00000230: 8900 7403 7404 7c00 6701 8801 7c02 7c03  ..t.t.|.g...|.|.
-00000240: 7c04 8800 6401 9c05 6402 8d03 7d05 7c05  |...d...d...}.|.
-00000250: a005 a100 0100 8701 6601 6403 6404 8408  ........f.d.d...
-00000260: 7d06 8700 6601 6405 6406 8408 7d07 7c05  }...f.d.d...}.|.
-00000270: 7c06 7c07 6407 9c03 5300 2908 4e29 05da  |.|.d...S.).N)..
-00000280: 0974 6865 5f71 7565 7565 da03 4357 44da  .the_queue..CWD.
-00000290: 0365 6e76 da04 6e61 6d65 da0a 7374 6f70  .env..name..stop
-000002a0: 5f65 7665 6e74 2903 da06 7461 7267 6574  _event)...target
-000002b0: da04 6172 6773 da06 6b77 6172 6773 6300  ..args..kwargsc.
-000002c0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-000002d0: 0000 0013 0000 0073 2600 0000 6700 7d00  .......s&...g.}.
-000002e0: 8800 a000 a100 7311 7c00 a001 8800 a002  ......s.|.......
-000002f0: a100 a101 0100 8800 a000 a100 7206 7c00  ............r.|.
-00000300: 5300 a901 4e29 03da 0565 6d70 7479 da06  S...N)...empty..
-00000310: 6170 7065 6e64 da03 6765 7429 01da 0870  append..get)...p
-00000320: 726f 6365 6564 7329 0172 0600 0000 a900  roceeds).r......
-00000330: fa45 2f62 696f 7465 6368 2f76 656e 7565  .E/biotech/venue
-00000340: 732f 7374 6167 6573 2f62 696f 7465 6368  s/stages/biotech
-00000350: 2f74 6f70 6963 732f 7072 6f63 6573 735f  /topics/process_
-00000360: 6f6e 2f70 5f65 7870 6563 742f 696d 706c  on/p_expect/impl
-00000370: 6963 6974 2e70 79da 0b70 6172 7365 5f71  icit.py..parse_q
-00000380: 7565 7565 4e00 0000 730a 0000 0004 0108  ueueN...s.......
-00000390: 010e 0108 ff04 037a 2870 726f 6365 7373  .......z(process
-000003a0: 5f6f 6e5f 696d 706c 6963 6974 2e3c 6c6f  _on_implicit.<lo
-000003b0: 6361 6c73 3e2e 7061 7273 655f 7175 6575  cals>.parse_queu
-000003c0: 6563 0000 0000 0000 0000 0000 0000 0000  ec..............
-000003d0: 0000 0200 0000 1300 0000 730c 0000 0088  ..........s.....
-000003e0: 00a0 00a1 0001 0064 0053 0072 0e00 0000  .......d.S.r....
-000003f0: 2901 da03 7365 7472 1300 0000 2901 720a  )...setr....).r.
-00000400: 0000 0072 1300 0000 7214 0000 00da 036f  ...r....r......o
-00000410: 6666 5700 0000 7302 0000 000c 027a 2070  ffW...s......z p
-00000420: 726f 6365 7373 5f6f 6e5f 696d 706c 6963  rocess_on_implic
-00000430: 6974 2e3c 6c6f 6361 6c73 3e2e 6f66 6629  it.<locals>.off)
-00000440: 0372 0500 0000 da07 7265 636f 7264 7372  .r......recordsr
-00000450: 1700 0000 2906 7204 0000 00da 0f6d 756c  ....).r......mul
-00000460: 7469 7072 6f63 6573 7369 6e67 da05 4576  tiprocessing..Ev
-00000470: 656e 7472 0300 0000 7202 0000 00da 0573  entr....r......s
-00000480: 7461 7274 2908 da0e 7072 6f63 6573 735f  tart)...process_
-00000490: 7374 7269 6e67 7206 0000 0072 0700 0000  stringr....r....
-000004a0: 7208 0000 0072 0900 0000 da10 696d 706c  r....r......impl
-000004b0: 6963 6974 5f70 726f 6365 7373 7215 0000  icit_processr...
-000004c0: 0072 1700 0000 7213 0000 0029 0272 0a00  .r....r....).r..
-000004d0: 0000 7206 0000 0072 1400 0000 da13 7072  ..r....r......pr
-000004e0: 6f63 6573 735f 6f6e 5f69 6d70 6c69 6369  ocess_on_implici
-000004f0: 7426 0000 0073 2800 0000 0609 0802 0202  t&...s(.........
-00000500: 0201 0203 02ff 0205 0201 0201 0201 0202  ................
-00000510: 04fa 06f9 0811 0c0a 0c09 0205 0201 0201  ................
-00000520: 06fd 721e 0000 0029 0bda 075f 5f64 6f63  ..r....)...__doc
-00000530: 5f5f da22 6269 6f74 6563 682e 746f 7069  __."biotech.topi
-00000540: 6373 2e70 726f 6365 7373 5f6f 6e2e 705f  cs.process_on.p_
-00000550: 6578 7065 6374 7202 0000 00da 0770 6578  expectr......pex
-00000560: 7065 6374 da04 7269 6368 da06 6174 6578  pect..rich..atex
-00000570: 6974 da02 6f73 7219 0000 0072 0300 0000  it..osr....r....
-00000580: 7204 0000 0072 1e00 0000 7213 0000 0072  r....r....r....r
-00000590: 1300 0000 7213 0000 0072 1400 0000 da08  ....r....r......
-000005a0: 3c6d 6f64 756c 653e 0100 0000 731a 0000  <module>....s...
-000005b0: 0004 010c 1908 0208 0108 0208 0110 0108  ................
-000005c0: 0102 0602 0102 0102 020e f9              ...........
+00000050: 6403 6c05 5a05 6401 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
+00000060: 6d08 5a08 0100 6401 6403 6c06 5a06 6401  m.Z...d.d.l.Z.d.
+00000070: 6403 6c09 5a09 6405 6406 8400 5a0a 6403  d.l.Z.d.d...Z.d.
+00000080: 6403 6900 6407 6604 6408 6409 8401 5a0b  d.i.d.f.d.d...Z.
+00000090: 6403 5300 290a 6144 0100 000a 0966 726f  d.S.).aD.....fro
+000000a0: 6d20 6269 6f74 6563 682e 746f 7069 6373  m biotech.topics
+000000b0: 2e70 726f 6365 7373 5f6f 6e2e 705f 6578  .process_on.p_ex
+000000c0: 7065 6374 2e69 6d70 6c69 6369 7420 696d  pect.implicit im
+000000d0: 706f 7274 2070 726f 6365 7373 5f6f 6e5f  port process_on_
+000000e0: 696d 706c 6963 6974 0a09 0a09 7665 6e74  implicit....vent
+000000f0: 7572 6520 3d20 7072 6f63 6573 735f 6f6e  ure = process_on
+00000100: 5f69 6d70 6c69 6369 7420 280a 0909 2727  _implicit (...''
+00000110: 2c0a 0909 0a09 0943 5744 203d 204e 6f6e  ,......CWD = Non
+00000120: 652c 0a09 0965 6e76 203d 207b 7d0a 0929  e,...env = {}..)
+00000130: 0a09 0a09 230a 0923 2073 7461 7475 730a  ....#..# status.
+00000140: 0923 0a09 230a 0970 7269 6e74 2028 2773  .#..#..print ('s
+00000150: 7461 7475 733a 272c 2076 656e 7475 7265  tatus:', venture
+00000160: 205b 2270 726f 6365 7373 225d 2e69 735f   ["process"].is_
+00000170: 616c 6976 6520 2829 290a 090a 0923 0a09  alive ())....#..
+00000180: 2309 7374 6f70 2074 6865 2070 726f 6365  #.stop the proce
+00000190: 7373 0a09 230a 0923 0a09 7665 6e74 7572  ss..#..#..ventur
+000001a0: 6520 5b22 7072 6f63 6573 7322 5d2e 7465  e ["process"].te
+000001b0: 726d 696e 6174 6520 2829 0a09 0a09 7265  rminate ()....re
+000001c0: 636f 7264 7320 3d20 7665 6e74 7572 6520  cords = venture 
+000001d0: 5b22 7265 636f 7264 7322 5d20 2829 0ae9  ["records"] ()..
+000001e0: 0000 0000 2901 da0a 7072 6f63 6573 735f  ....)...process_
+000001f0: 6f6e 4e29 02da 0750 726f 6365 7373 da05  onN)...Process..
+00000200: 5175 6575 6563 0100 0000 0000 0000 0000  Queuec..........
+00000210: 0000 0200 0000 0a00 0000 4300 0000 7348  ..........C...sH
+00000220: 0000 007a 0b74 0064 0183 0101 007c 00a0  ...z.t.d.....|..
+00000230: 01a1 0001 0057 0064 0053 0004 0074 0279  .....W.d.S...t.y
+00000240: 2301 007d 0101 007a 0c74 0064 027c 0183  #..}...z.t.d.|..
+00000250: 0201 0057 0059 0064 007d 017e 0164 0053  ...W.Y.d.}.~.d.S
+00000260: 0064 007d 017e 0177 0177 0029 034e 7a33  .d.}.~.w.w.).Nz3
+00000270: 0a09 090a 0909 0961 7474 656d 7069 6e67  .......attemping
+00000280: 2074 6f20 7374 6f70 2074 6865 2069 6d70   to stop the imp
+00000290: 6c69 6369 7420 7665 6e74 7572 650a 0909  licit venture...
+000002a0: 0a09 097a 1f76 656e 7475 7265 2069 6d70  ...z.venture imp
+000002b0: 6c69 6369 7420 6f66 6620 6578 6365 7074  licit off except
+000002c0: 696f 6e3a 2903 da05 7072 696e 74da 0974  ion:)...print..t
+000002d0: 6572 6d69 6e61 7465 da09 4578 6365 7074  erminate..Except
+000002e0: 696f 6e29 02da 1069 6d70 6c69 6369 745f  ion)...implicit_
+000002f0: 7072 6f63 6573 73da 0145 a900 720a 0000  process..E..r...
+00000300: 00fa 452f 6269 6f74 6563 682f 7665 6e75  ..E/biotech/venu
+00000310: 6573 2f73 7461 6765 732f 6269 6f74 6563  es/stages/biotec
+00000320: 682f 746f 7069 6373 2f70 726f 6365 7373  h/topics/process
+00000330: 5f6f 6e2f 705f 6578 7065 6374 2f69 6d70  _on/p_expect/imp
+00000340: 6c69 6369 742e 7079 da03 6f66 6625 0000  licit.py..off%..
+00000350: 0073 1000 0000 0201 0801 0e05 0e01 0a01  .s..............
+00000360: 0e02 0880 02fd 720c 0000 00da 0770 726f  ......r......pro
+00000370: 6365 7373 6305 0000 0000 0000 0000 0000  cessc...........
+00000380: 0008 0000 0009 0000 0003 0000 0073 6200  .............sb.
+00000390: 0000 7400 8300 8901 7401 a002 a100 8900  ..t.....t.......
+000003a0: 7403 7404 7c00 6701 8801 7c02 7c03 7c04  t.t.|.g...|.|.|.
+000003b0: 8800 6401 9c05 6402 8d03 7d05 7c05 a005  ..d...d...}.|...
+000003c0: a100 0100 8701 6601 6403 6404 8408 7d06  ......f.d.d...}.
+000003d0: 8700 6601 6405 6406 8408 7d07 7406 a007  ..f.d.d...}.t...
+000003e0: 7408 7c05 a102 0100 7c05 7c06 7c07 6407  t.|.....|.|.|.d.
+000003f0: 9c03 5300 2908 4e29 05da 0974 6865 5f71  ..S.).N)...the_q
+00000400: 7565 7565 da03 4357 44da 0365 6e76 da04  ueue..CWD..env..
+00000410: 6e61 6d65 da0a 7374 6f70 5f65 7665 6e74  name..stop_event
+00000420: 2903 da06 7461 7267 6574 da04 6172 6773  )...target..args
+00000430: da06 6b77 6172 6773 6300 0000 0000 0000  ..kwargsc.......
+00000440: 0000 0000 0001 0000 0004 0000 0013 0000  ................
+00000450: 0073 2600 0000 6700 7d00 8800 a000 a100  .s&...g.}.......
+00000460: 7311 7c00 a001 8800 a002 a100 a101 0100  s.|.............
+00000470: 8800 a000 a100 7206 7c00 5300 a901 4e29  ......r.|.S...N)
+00000480: 03da 0565 6d70 7479 da06 6170 7065 6e64  ...empty..append
+00000490: da03 6765 7429 01da 0870 726f 6365 6564  ..get)...proceed
+000004a0: 7329 0172 0e00 0000 720a 0000 0072 0b00  s).r....r....r..
+000004b0: 0000 da0b 7061 7273 655f 7175 6575 655a  ....parse_queueZ
+000004c0: 0000 0073 0a00 0000 0401 0801 0e01 08ff  ...s............
+000004d0: 0403 7a28 7072 6f63 6573 735f 6f6e 5f69  ..z(process_on_i
+000004e0: 6d70 6c69 6369 742e 3c6c 6f63 616c 733e  mplicit.<locals>
+000004f0: 2e70 6172 7365 5f71 7565 7565 6300 0000  .parse_queuec...
+00000500: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00000510: 0013 0000 0073 0c00 0000 8800 a000 a100  .....s..........
+00000520: 0100 6400 5300 7216 0000 0029 01da 0373  ..d.S.r....)...s
+00000530: 6574 720a 0000 0029 0172 1200 0000 720a  etr....).r....r.
+00000540: 0000 0072 0b00 0000 da05 6f66 665f 3163  ...r......off_1c
+00000550: 0000 0073 0200 0000 0c02 7a22 7072 6f63  ...s......z"proc
+00000560: 6573 735f 6f6e 5f69 6d70 6c69 6369 742e  ess_on_implicit.
+00000570: 3c6c 6f63 616c 733e 2e6f 6666 5f31 2903  <locals>.off_1).
+00000580: 720d 0000 00da 0772 6563 6f72 6473 720c  r......recordsr.
+00000590: 0000 0029 0972 0400 0000 da0f 6d75 6c74  ...).r......mult
+000005a0: 6970 726f 6365 7373 696e 67da 0545 7665  iprocessing..Eve
+000005b0: 6e74 7203 0000 0072 0200 0000 da05 7374  ntr....r......st
+000005c0: 6172 74da 0661 7465 7869 74da 0872 6567  art..atexit..reg
+000005d0: 6973 7465 7272 0c00 0000 2908 da0e 7072  isterr....)...pr
+000005e0: 6f63 6573 735f 7374 7269 6e67 720e 0000  ocess_stringr...
+000005f0: 0072 0f00 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000600: 7208 0000 0072 1b00 0000 721d 0000 0072  r....r....r....r
+00000610: 0a00 0000 2902 7212 0000 0072 0e00 0000  ....).r....r....
+00000620: 720b 0000 00da 1370 726f 6365 7373 5f6f  r......process_o
+00000630: 6e5f 696d 706c 6963 6974 3200 0000 732a  n_implicit2...s*
+00000640: 0000 0006 0908 0202 0202 0102 0302 ff02  ................
+00000650: 0502 0102 0102 0102 0204 fa06 f908 110c  ................
+00000660: 0a0c 090c 0402 0302 0102 0506 f972 2500  .............r%.
+00000670: 0000 290c da07 5f5f 646f 635f 5fda 2262  ..)...__doc__."b
+00000680: 696f 7465 6368 2e74 6f70 6963 732e 7072  iotech.topics.pr
+00000690: 6f63 6573 735f 6f6e 2e70 5f65 7870 6563  ocess_on.p_expec
+000006a0: 7472 0200 0000 da07 7065 7870 6563 74da  tr......pexpect.
+000006b0: 0472 6963 68da 026f 7372 1f00 0000 7203  .rich..osr....r.
+000006c0: 0000 0072 0400 0000 7222 0000 0072 0c00  ...r....r"...r..
+000006d0: 0000 7225 0000 0072 0a00 0000 720a 0000  ..r%...r....r...
+000006e0: 0072 0a00 0000 720b 0000 00da 083c 6d6f  .r....r......<mo
+000006f0: 6475 6c65 3e01 0000 0073 1c00 0000 0401  dule>....s......
+00000700: 0c19 0802 0801 0802 1001 0801 0801 0802  ................
+00000710: 0210 0201 0201 0202 0ef9                 ..........
```

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py` & `biotech-1.1.0/venues/stages/biotech/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `biotech-1.1.0/venues/stages/biotech/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/venues/stages/biotech/topics/start--/simultaneously.py` & `biotech-1.1.0/venues/stages/biotech/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `biotech-1.0.3/PKG-INFO` & `biotech-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: biotech
-Version: 1.0.3
+Version: 1.1.0
 Summary: A health monitoring stack
 License: GPL-3.0-only
 Keywords: alarms,screening,monitors,cybernetics,neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: body-scan (>=1.1.1,<2.0.0)
 Requires-Dist: botanist (>=1.0.0,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: coverage (>=7.4.4,<8.0.0)
 Requires-Dist: flask (>=3.0.3,<4.0.0)
+Requires-Dist: mako (>=1.3.3,<2.0.0)
 Requires-Dist: pexpect (>=4.9.0,<5.0.0)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Requires-Dist: redis (>=5.0.3,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: sanic (>=23.12.1,<24.0.0)
-Requires-Dist: shares (>=3.1.9,<4.0.0)
 Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Project-URL: GitLab, https://gitlab.com/status600/climates/biotech
 Description-Content-Type: text/markdown
 
 
 
 ## certificate
```

