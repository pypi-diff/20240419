# Comparing `tmp/pyorchestra-0.5.4.tar.gz` & `tmp/pyorchestra-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorchestra-0.5.4.tar", max compression
+gzip compressed data, was "pyorchestra-0.6.0.tar", max compression
```

## Comparing `pyorchestra-0.5.4.tar` & `pyorchestra-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     7652 2024-04-15 14:33:34.358906 pyorchestra-0.5.4/LICENSE
--rwxr-xr-x   0        0        0    25711 2024-04-15 14:33:34.358906 pyorchestra-0.5.4/README.md
--rwxr-xr-x   0        0        0       62 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/__init__.py
--rwxr-xr-x   0        0        0      265 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/__init__.py
--rwxr-xr-x   0        0        0     2514 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/job.py
--rwxr-xr-x   0        0        0      844 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/run.py
--rwxr-xr-x   0        0        0      655 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/schedule_definition.py
--rwxr-xr-x   0        0        0     1294 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/dto/task.py
--rwxr-xr-x   0        0        0      656 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/main.py
--rwxr-xr-x   0        0        0    10283 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/routers/jobs.py
--rwxr-xr-x   0        0        0      531 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/routers/tags.py
--rwxr-xr-x   0        0        0      603 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/api/routers/tasks.py
--rwxr-xr-x   0        0        0     1839 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/backend.py
--rwxr-xr-x   0        0        0    19740 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/core.py
--rwxr-xr-x   0        0        0      873 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/formatting.py
--rwxr-xr-x   0        0        0      168 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/job.py
--rwxr-xr-x   0        0        0     1575 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/models.py
--rwxr-xr-x   0        0        0    10720 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/orchestra/scheduling.py
--rwxr-xr-x   0        0        0     1104 2024-04-15 14:33:34.362906 pyorchestra-0.5.4/pyproject.toml
--rw-r--r--   0        0        0    26585 1970-01-01 00:00:00.000000 pyorchestra-0.5.4/PKG-INFO
+-rwxr-xr-x   0        0        0     7652 2024-04-19 15:00:15.912848 pyorchestra-0.6.0/LICENSE
+-rwxr-xr-x   0        0        0    25961 2024-04-19 15:00:15.912848 pyorchestra-0.6.0/README.md
+-rwxr-xr-x   0        0        0       62 2024-04-19 15:00:15.912848 pyorchestra-0.6.0/orchestra/__init__.py
+-rwxr-xr-x   0        0        0      265 2024-04-19 15:00:15.912848 pyorchestra-0.6.0/orchestra/api/dto/__init__.py
+-rwxr-xr-x   0        0        0     2514 2024-04-19 15:00:15.912848 pyorchestra-0.6.0/orchestra/api/dto/job.py
+-rwxr-xr-x   0        0        0      844 2024-04-19 15:00:15.912848 pyorchestra-0.6.0/orchestra/api/dto/run.py
+-rwxr-xr-x   0        0        0      779 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/api/dto/schedule_definition.py
+-rwxr-xr-x   0        0        0     1294 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/api/dto/task.py
+-rwxr-xr-x   0        0        0      656 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/api/main.py
+-rwxr-xr-x   0        0        0    10318 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/api/routers/jobs.py
+-rwxr-xr-x   0        0        0      531 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/api/routers/tags.py
+-rwxr-xr-x   0        0        0      603 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/api/routers/tasks.py
+-rwxr-xr-x   0        0        0     1839 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/backend.py
+-rwxr-xr-x   0        0        0    20422 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/core.py
+-rwxr-xr-x   0        0        0     1104 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/formatting.py
+-rwxr-xr-x   0        0        0      168 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/job.py
+-rwxr-xr-x   0        0        0     1575 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/models.py
+-rwxr-xr-x   0        0        0    10840 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/orchestra/scheduling.py
+-rwxr-xr-x   0        0        0     1104 2024-04-19 15:00:15.916848 pyorchestra-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    26835 1970-01-01 00:00:00.000000 pyorchestra-0.6.0/PKG-INFO
```

### Comparing `pyorchestra-0.5.4/LICENSE` & `pyorchestra-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.4/README.md` & `pyorchestra-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pyorchestra
+Version: 0.6.0
+Summary: Orchestra is a job scheduler on top of Celery
+Home-page: https://github.com/vidosits/orchestra
+License: LGPLv3
+Author: András Vidosits
+Author-email: andras@hyperplane.hu
+Requires-Python: >=3.11.7,<4.0.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: celery (>=5.3.6,<6.0.0)
+Requires-Dist: fastapi (>=0.110.0,<0.111.0)
+Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
+Requires-Dist: pytz (>=2023.3.post1,<2024.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: scheduler (>=0.8.5,<0.9.0)
+Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0)
+Requires-Dist: uvicorn[standard] (>=0.27.1,<0.28.0)
+Project-URL: Repository, https://github.com/vidosits/orchestra
+Description-Content-Type: text/markdown
+
 # Orchestra
 
 Orchestra is:
 - an asyncio based job scheduler
 - using [Celery](https://docs.celeryq.dev/) (which is a distributed task queue) under the hood for running tasks/jobs
 - using [scheduler](https://digon.io/hyd/project/scheduler/t/master/readme.html) under the hood which is a simple in-process python scheduler library with asyncio, threading and timezone support.
 
@@ -33,14 +56,15 @@
   schedules: # a list of schedules
     - name: "short_task_every_1_second" # name of the task that shows up in the logs, *has to be unique*
       task: short_task # the function in the module decorated by `orchestra.task`
       enabled: false # if it's not enabled it will be ignored
       schedule: 
         timing: "every 00:00:01" # see the examples for a list of understood expressions
         timezone: Europe/Paris # name of a time zone from the tz database
+        resume_from_previous: true # if enabled, Orchestra will attempt to calculate what would be the next run based on the last known run, false by default
       additional_options: # everything in this optional section will be passed to the celery task when invoked
         queue: background-jobs
       tags: # tags are list of string, they may be used to group together tasks
         - cpu
         - fast
 ```
 
@@ -67,14 +91,15 @@
 * 2023-04-01 09:13
 * 2023-04-01 09:13:11
 * next 23:00:00
 * once in 5 hours 2 minutes and 15 seconds
 * once in 1 hour and 10 minutes
 * once in 2 minutes and 10 seconds
 * once in 17 seconds
+* always
 
 By default timing expression with only a time or timestamp (without date) like `11:23:00` will be interpreted as a time instant and will trigger the next time the wall clock shows the specified time.
 
 ### Creating an instance
 `main.py`
 ```python
 import asyncio
@@ -116,22 +141,22 @@
 
 ```
 The output would look something like the following:
 ```bash
 [08:38:50] INFO     Job Simple Task every 48 hours was scheduled to  core.py:214
                     run 2 days, 0:00:00                                         
            INFO     Orchestra starting                                core.py:82
-╭───────────┬────────────┬────────────────────────────────────┬───────────────────────┬───────────────────────────┬─────────────┬───────────┬────────────┬──────╮
-│State      │ Shedule    │ Job name                           │ Module and task       │ Due at                    │ Timezone    │ Due in    │ Attempts   │ Tags │
-├───────────┼────────────┼────────────────────────────────────┼───────────────────────┼───────────────────────────┼─────────────┼───────────┼────────────┼──────┤
-│Running    │ CYCLIC     │ Simple Task every 48 hours         │ main.simple_task      │ 2024-03-05 07:38:50       │ UTC         │ 1 day     │ 0/inf      │      │
-╰───────────┴────────────┴────────────────────────────────────┴───────────────────────┴───────────────────────────┴─────────────┴───────────┴────────────┴──────╯
-╭───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
-╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭───────────┬─────────────┬────────────────────────────────────┬───────────────────────┬───────────────────────────┬─────────────┬───────────┬────────────┬──────╮
+│State      │ Schedule    │ Job name                           │ Module and task       │ Due at                    │ Timezone    │ Due in    │ Attempts   │ Tags │
+├───────────┼─────────────┼────────────────────────────────────┼───────────────────────┼───────────────────────────┼─────────────┼───────────┼────────────┼──────┤
+│Running    │ CYCLIC      │ Simple Task every 48 hours         │ main.simple_task      │ 2024-03-05 07:38:50       │ UTC         │ 1 day     │ 0/inf      │      │
+╰───────────┴─────────────┴────────────────────────────────────┴───────────────────────┴───────────────────────────┴─────────────┴───────────┴────────────┴──────╯
+╭────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 
 You may also use a standalone python module for holding your Celery tasks, but you have to declare Orchestra there as well or import it from the main module:
 
 `tasks.py`
 ```python
@@ -248,43 +273,43 @@
                     scheduled to run 0:31:12                                    
            INFO     Job task_every_Monday_at_03_15_00 was scheduled  core.py:214
                     to run Monday(time=datetime.time(3, 15,                     
                     tzinfo=<DstTzInfo 'Europe/Berlin' LMT+1:16:00             
                     STD>))                                                      
            ...
            INFO     Orchestra starting                                core.py:82
-╭────────┬──────────┬────────────────────────────────────────────┬──────────────────────┬─────────────────────┬─────────────────┬──────────┬──────────┬─────────╮
-│State   │ Shedule  │ Job name                                   │ Module and task      │ Due at              │ Timezone        │ Due in   │ Attempts │ Tags    │
-├────────┼──────────┼────────────────────────────────────────────┼──────────────────────┼─────────────────────┼─────────────────┼──────────┼──────────┼─────────┤
-│Running │ ONCE     │ task_at_9_13                               │ tasks.long_task      │ 2024-03-03 09:13:00 │ Europe/Berlin   │ 0:36:09  │ 0/1      │ gpu     │
-│Running │ HOURLY   │ task_every_hour_at_05_00                   │ tasks.long_task      │ 2024-03-03 09:05:00 │ Europe/Berlin   │ 0:28:09  │ 0/inf    │ gpu     │
-│Running │ CYCLIC   │ exception_task_every_10_second             │ tasks.exception_task │ 2024-03-03 07:36:57 │ UTC             │ 0:00:06  │ 0/inf    │ cpu,fast│
-│Running │ DAILY    │ task_every_day_at_9_15                     │ tasks.long_task      │ 2024-03-03 09:15:00 │ Europe/Berlin   │ 0:38:09  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_next_23_00_00                         │ tasks.long_task      │ 2024-03-03 23:00:00 │ Europe/Berlin   │ 14:23:09 │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_in_13_11_52                      │ tasks.long_task      │ 2024-03-03 20:48:39 │ UTC             │ 13:11:49 │ 0/1      │ gpu     │
-│Running │ CYCLIC   │ task_every_31_minutes_12_seconds           │ tasks.long_task      │ 2024-03-03 08:07:59 │ UTC             │ 0:31:09  │ 0/inf    │ gpu     │
-│Running │ CYCLIC   │ short_task_every_1_second                  │ tasks.short_task     │ 2024-03-03 07:36:51 │ UTC             │ 0:00:00  │ 3/inf    │ cpu,fast│
-│Running │ ONCE     │ task_at_11_23_00                           │ tasks.long_task      │ 2024-03-03 11:23:00 │ Europe/Berlin   │ 2:46:09  │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_in_1_hour_and_10_minutes         │ tasks.long_task      │ 2024-03-03 08:46:47 │ UTC             │ 1:09:57  │ 0/1      │ gpu     │
-│Running │ WEEKLY   │ task_every_Monday_at_03_15_00              │ tasks.long_task      │ 2024-03-04 03:15:00 │ Europe/Berlin   │ 18:38:09 │ 0/inf    │ gpu     │
-│Running │ DAILY    │ task_every_day_at_13_hours                 │ tasks.long_task      │ 2024-03-03 13:00:00 │ Europe/Berlin   │ 4:23:09  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_next_Tuesday_at_13_11_00              │ tasks.long_task      │ 2024-03-05 13:11:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
-│Running │ DAILY    │ task_every_day_on_9_03                     │ tasks.long_task      │ 2024-03-03 09:03:00 │ Europe/Berlin   │ 0:26:09  │ 0/inf    │ gpu     │
-│Running │ MINUTELY │ task_every_minute_at_15_seconds            │ tasks.long_task      │ 2024-03-03 08:37:15 │ Europe/Berlin   │ 0:00:24  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_2024_04_01_09_13                      │ tasks.long_task      │ 2024-04-01 09:13:00 │ Europe/Berlin   │ 28 days  │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_Wednesday_at_01_15_00            │ tasks.long_task      │ 2024-03-06 01:15:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_on_Thursday_00_31_41             │ tasks.long_task      │ 2024-03-07 00:31:41 │ Europe/Berlin   │ 3 days   │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_in_5_hours_2_minutes_and_15_sec… │ tasks.long_task      │ 2024-03-03 12:39:02 │ UTC             │ 5:02:12  │ 0/1      │ gpu     │
-│Running │ DAILY    │ task_every_day_at_09_15_14                 │ tasks.long_task      │ 2024-03-03 09:15:14 │ Europe/Berlin   │ 0:38:23  │ 0/inf    │ gpu     │
-│Running │ CYCLIC   │ task_every_48_hours                        │ tasks.long_task      │ 2024-03-05 07:36:47 │ UTC             │ 1 day    │ 0/inf    │ gpu     │
-│Running │ WEEKLY   │ task_every_Monday_at_03_15_00_US           │ tasks.long_task      │ 2024-03-04 03:15:00 │ America/Boise   │ 1 day    │ 0/inf    │ gpu     │
-╰────────┴──────────┴────────────────────────────────────────────┴──────────────────────┴─────────────────────┴─────────────────┴──────────┴──────────┴─────────╯
-╭───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
-╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭────────┬───────────┬────────────────────────────────────────────┬──────────────────────┬─────────────────────┬─────────────────┬──────────┬──────────┬─────────╮
+│State   │ Schedule  │ Job name                                   │ Module and task      │ Due at              │ Timezone        │ Due in   │ Attempts │ Tags    │
+├────────┼───────────┼────────────────────────────────────────────┼──────────────────────┼─────────────────────┼─────────────────┼──────────┼──────────┼─────────┤
+│Running │ ONCE      │ task_at_9_13                               │ tasks.long_task      │ 2024-03-03 09:13:00 │ Europe/Berlin   │ 0:36:09  │ 0/1      │ gpu     │
+│Running │ HOURLY    │ task_every_hour_at_05_00                   │ tasks.long_task      │ 2024-03-03 09:05:00 │ Europe/Berlin   │ 0:28:09  │ 0/inf    │ gpu     │
+│Running │ CYCLIC    │ exception_task_every_10_second             │ tasks.exception_task │ 2024-03-03 07:36:57 │ UTC             │ 0:00:06  │ 0/inf    │ cpu,fast│
+│Running │ DAILY     │ task_every_day_at_9_15                     │ tasks.long_task      │ 2024-03-03 09:15:00 │ Europe/Berlin   │ 0:38:09  │ 0/inf    │ gpu     │
+│Running │ ONCE      │ task_next_23_00_00                         │ tasks.long_task      │ 2024-03-03 23:00:00 │ Europe/Berlin   │ 14:23:09 │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_in_13_11_52                      │ tasks.long_task      │ 2024-03-03 20:48:39 │ UTC             │ 13:11:49 │ 0/1      │ gpu     │
+│Running │ CYCLIC    │ task_every_31_minutes_12_seconds           │ tasks.long_task      │ 2024-03-03 08:07:59 │ UTC             │ 0:31:09  │ 0/inf    │ gpu     │
+│Running │ CYCLIC    │ short_task_every_1_second                  │ tasks.short_task     │ 2024-03-03 07:36:51 │ UTC             │ 0:00:00  │ 3/inf    │ cpu,fast│
+│Running │ ONCE      │ task_at_11_23_00                           │ tasks.long_task      │ 2024-03-03 11:23:00 │ Europe/Berlin   │ 2:46:09  │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_in_1_hour_and_10_minutes         │ tasks.long_task      │ 2024-03-03 08:46:47 │ UTC             │ 1:09:57  │ 0/1      │ gpu     │
+│Running │ WEEKLY    │ task_every_Monday_at_03_15_00              │ tasks.long_task      │ 2024-03-04 03:15:00 │ Europe/Berlin   │ 18:38:09 │ 0/inf    │ gpu     │
+│Running │ DAILY     │ task_every_day_at_13_hours                 │ tasks.long_task      │ 2024-03-03 13:00:00 │ Europe/Berlin   │ 4:23:09  │ 0/inf    │ gpu     │
+│Running │ ONCE      │ task_next_Tuesday_at_13_11_00              │ tasks.long_task      │ 2024-03-05 13:11:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
+│Running │ DAILY     │ task_every_day_on_9_03                     │ tasks.long_task      │ 2024-03-03 09:03:00 │ Europe/Berlin   │ 0:26:09  │ 0/inf    │ gpu     │
+│Running │ MINUTELY  │ task_every_minute_at_15_seconds            │ tasks.long_task      │ 2024-03-03 08:37:15 │ Europe/Berlin   │ 0:00:24  │ 0/inf    │ gpu     │
+│Running │ ONCE      │ task_2024_04_01_09_13                      │ tasks.long_task      │ 2024-04-01 09:13:00 │ Europe/Berlin   │ 28 days  │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_Wednesday_at_01_15_00            │ tasks.long_task      │ 2024-03-06 01:15:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_on_Thursday_00_31_41             │ tasks.long_task      │ 2024-03-07 00:31:41 │ Europe/Berlin   │ 3 days   │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_in_5_hours_2_minutes_and_15_sec… │ tasks.long_task      │ 2024-03-03 12:39:02 │ UTC             │ 5:02:12  │ 0/1      │ gpu     │
+│Running │ DAILY     │ task_every_day_at_09_15_14                 │ tasks.long_task      │ 2024-03-03 09:15:14 │ Europe/Berlin   │ 0:38:23  │ 0/inf    │ gpu     │
+│Running │ CYCLIC    │ task_every_48_hours                        │ tasks.long_task      │ 2024-03-05 07:36:47 │ UTC             │ 1 day    │ 0/inf    │ gpu     │
+│Running │ WEEKLY    │ task_every_Monday_at_03_15_00_US           │ tasks.long_task      │ 2024-03-04 03:15:00 │ America/Boise   │ 1 day    │ 0/inf    │ gpu     │
+╰────────┴───────────┴────────────────────────────────────────────┴──────────────────────┴─────────────────────┴─────────────────┴──────────┴──────────┴─────────╯
+╭────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
 ### Pausing and resuming jobs
 
 ```python
 import asyncio
@@ -354,24 +379,24 @@
                     scheduled to run Monday(time=datetime.time(16,              
                     30, tzinfo=<DstTzInfo 'Europe/Berlin'                       
                     LMT+0:53:00 STD>))                                          
            INFO     Paused job Simple task every Monday at 16:30 UTC core.py:298
            INFO     Paused job Simple task every 1s                  core.py:298
            INFO     Resumed job Simple task every 1s                 core.py:314
            INFO     Orchestra starting                                core.py:82
-╭─────────┬──────────┬─────────────────────────────────────────┬───────────────────────┬──────────────────────┬───────────────┬─────────┬──────────┬────────────╮
-│State    │ Shedule  │ Job name                                │ Module and task       │ Due at               │ Timezone      │ Due in  │ Attempts │ Tags       │
-├─────────┼──────────┼─────────────────────────────────────────┼───────────────────────┼──────────────────────┼───────────────┼─────────┼──────────┼────────────┤
-│Running  │ CYCLIC   │ Hello World every 10s                   │ hello                 │ 2024-03-03 07:39:51  │ UTC           │ 0:00:04 │ 0/inf    │            │
-│Running  │ CYCLIC   │ Simple task every 1s                    │ __main__.simple_task  │ 2024-03-03 07:39:47  │ UTC           │ 0:00:00 │ 5/inf    │ gpu,latency│
-│Paused   │ WEEKLY   │ Simple task every Monday at 16:30 UTC   │ __main__.simple_task  │ 2024-03-04 16:30:00  │ Europe/Berlin │ 1 day   │ 0/inf    │ cpu        │
-╰─────────┴──────────┴─────────────────────────────────────────┴───────────────────────┴──────────────────────┴───────────────┴─────────┴──────────┴────────────╯
-╭───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
-╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─────────┬───────────┬─────────────────────────────────────────┬───────────────────────┬──────────────────────┬───────────────┬─────────┬──────────┬────────────╮
+│State    │ Schedule  │ Job name                                │ Module and task       │ Due at               │ Timezone      │ Due in  │ Attempts │ Tags       │
+├─────────┼───────────┼─────────────────────────────────────────┼───────────────────────┼──────────────────────┼───────────────┼─────────┼──────────┼────────────┤
+│Running  │ CYCLIC    │ Hello World every 10s                   │ hello                 │ 2024-03-03 07:39:51  │ UTC           │ 0:00:04 │ 0/inf    │            │
+│Running  │ CYCLIC    │ Simple task every 1s                    │ __main__.simple_task  │ 2024-03-03 07:39:47  │ UTC           │ 0:00:00 │ 5/inf    │ gpu,latency│
+│Paused   │ WEEKLY    │ Simple task every Monday at 16:30 UTC   │ __main__.simple_task  │ 2024-03-04 16:30:00  │ Europe/Berlin │ 1 day   │ 0/inf    │ cpu        │
+╰─────────┴───────────┴─────────────────────────────────────────┴───────────────────────┴──────────────────────┴───────────────┴─────────┴──────────┴────────────╯
+╭────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ### Using the API
 
 Orchestra comes with a built-in API accessible by setting `api_server=True` on the `Orchestra` instance.
 You may optionally provide an `api_address` parameter to control which `host:port` gets bound by `uvicorn`.
 
 ```python
@@ -398,7 +423,8 @@
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
 
 You can check the Swagger Docs created by FastAPI at the specified `api_address`, which is [http://localhost:5000](http://localhost:5000) in the above example and by default.
+
```

### Comparing `pyorchestra-0.5.4/orchestra/api/dto/job.py` & `pyorchestra-0.6.0/orchestra/api/dto/job.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.4/orchestra/api/dto/run.py` & `pyorchestra-0.6.0/orchestra/api/dto/run.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.4/orchestra/api/dto/schedule_definition.py` & `pyorchestra-0.6.0/orchestra/api/dto/schedule_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 class ScheduleDefinitionDTO(BaseModel):
     name: str
     task: str
     timing: str
     timezone: str | None = None
     tags: list[str] | None = None
-    resume: bool = False
+    resume_from_previous: bool = False
 
     @classmethod
     def map(cls, definition: dict) -> "ScheduleDefinitionDTO":
         return ScheduleDefinitionDTO(name=definition.get("name"),
                                      task=definition.get("task"),
                                      timing=definition["schedule"].get("timing"),
                                      timezone=definition["schedule"].get("timezone"),
-                                     tags=definition.get("tags"))
+                                     tags=definition.get("tags"),
+                                     resume_from_previous=definition["schedule"].get("resume_from_previous"))
```

### Comparing `pyorchestra-0.5.4/orchestra/api/dto/task.py` & `pyorchestra-0.6.0/orchestra/api/dto/task.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.4/orchestra/api/main.py` & `pyorchestra-0.6.0/orchestra/api/main.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.4/orchestra/api/routers/jobs.py` & `pyorchestra-0.6.0/orchestra/api/routers/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,21 @@
          "schedules": [
              {
                  "name": schedule_definition.name,
                  "task": schedule_definition.task,
                  "enabled": True,
                  "schedule": {
                      "timing": schedule_definition.timing,
-                     "timezone": schedule_definition.timezone or "utc"
+                     "timezone": schedule_definition.timezone or "utc",
+                     "resume_from_previous": schedule_definition.resume_from_previous
                  },
                  "tags": set(schedule_definition.tags or [])
              }
          ]}]
-    instance.add_schedules(module_definition, attempt_resume=schedule_definition.resume or False)
+    instance.add_schedules(module_definition)
 
 
 @router.get("/jobs", tags=["jobs"])
 async def get_jobs(tags: Annotated[list[str] | None, Query(description="Optional list of tags to filter scheduled jobs")] = None,
                    name_fragment: Annotated[str | None, Query(description="Optional string to filter scheduled jobs' names")] = None,
                    job_names: Annotated[list[str] | None, Query(description="An optional set of exact job names to match")] = None,
                    any_tag: Annotated[bool, Query(description="Set to true to match if only at least one tag has to match")] = False,
```

### Comparing `pyorchestra-0.5.4/orchestra/api/routers/tags.py` & `pyorchestra-0.6.0/orchestra/api/routers/tags.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.4/orchestra/api/routers/tasks.py` & `pyorchestra-0.6.0/orchestra/api/routers/tasks.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.4/orchestra/backend.py` & `pyorchestra-0.6.0/orchestra/backend.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.4/orchestra/core.py` & `pyorchestra-0.6.0/orchestra/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from rich.table import Table
 from scheduler.asyncio import Scheduler
 from scheduler.asyncio.job import Job
 from scheduler.trigger.core import Weekday
 from sqlalchemy import select
 from sqlalchemy.orm import joinedload
 
-from orchestra.formatting import pretty_print_block, get_job_state
+from orchestra.formatting import pretty_print_block, get_job_state, get_job_state_for_always_running
 from orchestra.job import StatefulJob
 from orchestra.models import Run, TimingAwareTask
 from orchestra.scheduling import Schedule
 
 logging.basicConfig(
     level="INFO", format="%(message)s", datefmt="[%X]", handlers=[RichHandler(rich_tracebacks=True, tracebacks_show_locals=True)]
 )
@@ -48,14 +48,15 @@
         self.scheduler: Scheduler | None = None
         self.loop = None
         self.enable_api = enable_api
         self.api_address = api_address
         self.loop_resolution_in_seconds = scheduler_loop_resolution_in_seconds
         self.server: uvicorn.Server | None = None
         self.paused_jobs: set[Job] = set()
+        self.always_running_jobs: set[StatefulJob] = set()
 
     def get_event_loop(self, loop):
         self.loop = loop or asyncio.get_running_loop()
 
     async def api_server(self):
         log_config = uvicorn.config.LOGGING_CONFIG
         log_config["loggers"] = []
@@ -156,17 +157,21 @@
         self.scheduler = self.scheduler or Scheduler(tzinfo=pytz.utc, loop=self.get_event_loop(loop))
         if module_definitions is not None:
             self.add_schedules(module_definitions)
 
     def schedule_job(self, job_name: str, module_name: str, task_name: str, schedule: Callable[..., Job], timing: datetime.datetime | datetime.timedelta | datetime.time | Weekday,
                      tags: set[str] | None = None, attempt_resume: bool = False, additional_options: dict = None, schedule_definition: Any = None) -> StatefulJob | None:
         session = self.backend.ResultSession()
+
+        timing_expression: str = schedule_definition.get("schedule").get("timing")
+        job_is_always_running = timing_expression == "always"
+
         with session_cleanup(session):
             resume_parameters: dict = {}
-            if attempt_resume:
+            if attempt_resume and not job_is_always_running:
                 logs = (
                     select(Run)
                     .where(Run.job == job_name)
                     .order_by(Run.triggered_date.desc())
                     .limit(1)
                 )
                 last_run: Run | None = next(session.scalars(logs), None)
@@ -203,25 +208,29 @@
                 alias=job_name,
                 tags=tags or set(),
                 **resume_parameters,
             )
 
             job.definition = schedule_definition or {}
 
+            if job_is_always_running:
+                # we need to keep track of this job even though it's going to get dropped from the scheduler
+                self.always_running_jobs.add(StatefulJob(job, is_paused=False))
+
             if "start" in resume_parameters:
                 logger.warning(
-                    f"Job {job_name} was scheduled to run {timing}, resuming using {last_running_time_local}, tz={last_run.timezone} as reference time."
+                    f"Job {job_name} was scheduled to run {timing_expression} ({timing}), resuming using {last_running_time_local}, tz={last_run.timezone} as reference time."
                     f" Next run at {next_run_local}, tz={last_run.timezone}"
                 )
             else:
-                logger.info(f"Job {job_name} was scheduled to run {timing}")
+                logger.info(f"Job {job_name} was scheduled to run {timing_expression} ({timing})")
 
             return StatefulJob(job, is_paused=False)
 
-    def add_schedules(self, module_definitions: list[dict], attempt_resume: bool = True):
+    def add_schedules(self, module_definitions: list[dict]):
         for index, block in enumerate(module_definitions or []):
             block_name: str = block.get("name", f"{index + 1}. schedule block")
             block_module: str | None = block.get("module")
 
             if block_module is None:
                 error_message: str = f"Module is undefined for {block_name}. Definition:\n\n{pretty_print_block(block)}"
                 logger.error(error_message)
@@ -264,15 +273,15 @@
 
                 self.schedule_job(job_name=job_name,
                                   module_name=block_module,
                                   task_name=task_name,
                                   schedule=schedule.job_type,
                                   timing=schedule.get_timing(),
                                   tags=set(schedule_definition.get("tags", set())),
-                                  attempt_resume=attempt_resume,
+                                  attempt_resume=schedule_definition.get("schedule").get("resume_from_previous", False),
                                   additional_options=schedule_definition.get("additional_options"),
                                   schedule_definition=schedule_definition)
 
     def apply_state_to_jobs(self, jobs: set[Job]) -> set[StatefulJob]:
         return set([StatefulJob(job, is_paused=True if job in self.paused_jobs else False) for job in jobs])
 
     def get_jobs(self, tags: set[str] | None = None, any_tag: bool = True, is_paused: bool | None = None) -> set[StatefulJob]:
@@ -404,28 +413,31 @@
 
         table = Table(expand=True)
         table.border_style = "bright_yellow"
         table.box = box.ROUNDED
         table.pad_edge = False
 
         table.add_column("State")
-        table.add_column("Shedule", style="green")
+        table.add_column("Schedule", style="green")
         table.add_column("Job name", style="blue")
         table.add_column("Module and task", style="magenta")
         table.add_column("Due at", style="red")
         table.add_column("Timezone", style="bright_blue")
         table.add_column("Due in", style="cyan")
         table.add_column("Attempts")
         table.add_column("Tags")
 
         for job in self.scheduler.jobs:
             table.add_row(*(["[green]Running[/]"] + get_job_state(job)))
 
         for job in self.paused_jobs:
             table.add_row(*(["[yellow]Paused[/]"] + get_job_state(job)))
 
+        for job in self.always_running_jobs:
+            table.add_row(*get_job_state_for_always_running(job))
+
         progress = Progress(TextColumn("{task.description}"), BarColumn(bar_width=None), expand=True, transient=True)
         progress.add_task("Orchestrating jobs", total=None)
         grid.add_row(table)
         grid.add_row(Panel(progress, expand=True, border_style="bright_yellow"))
 
         return grid
```

### Comparing `pyorchestra-0.5.4/orchestra/formatting.py` & `pyorchestra-0.6.0/orchestra/formatting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import yaml
-from rich import box
-from rich.panel import Panel
-from rich.progress import Progress, SpinnerColumn, BarColumn, TextColumn
-from rich.table import Table
-from scheduler import Scheduler
 from scheduler.asyncio.job import Job
 
+from orchestra.job import StatefulJob
+
 
 def pretty_print_block(config_block: dict) -> str:
     return yaml.dump(config_block, allow_unicode=True, default_flow_style=False)
 
 
 def transform_timing_to_schedule(timing: str) -> str:
     """
@@ -28,8 +25,23 @@
         row[1] + row[2],
         job.handle.__name__,
         row[3],
         str(job.datetime.tzinfo),
         row[5],
         f"{row[6]}/{row[7]}",
         ",".join(job.tags)
-    ]
+    ]
+
+
+def get_job_state_for_always_running(job: StatefulJob) -> list[str]:
+    row = job.job._str()
+    return [
+        "[yellow]Paused[/]" if job.is_paused else "[green]Running[/]",
+        "Always On",
+        row[1] + row[2],
+        job.job.handle.__name__,
+        "-",
+        str(job.job.datetime.tzinfo),
+        "∞",
+        "1",
+        ",".join(job.job.tags)
+    ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyorchestra-0.5.4/orchestra/models.py` & `pyorchestra-0.6.0/orchestra/models.py`

 * *Files identical despite different names*

### Comparing `pyorchestra-0.5.4/orchestra/scheduling.py` & `pyorchestra-0.6.0/orchestra/scheduling.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,18 +144,22 @@
         2023-04-01 09:13
         2023-04-01 09:13:11
         next 23:00:00
         once in 5 hours 2 minutes and 15 seconds
         once in 1 hour and 10 minutes
         once in 2 minutes and 10 seconds
         once in 17 seconds
+        always
         """
 
         clean_timing = self.clean_timing(self.definition["schedule"]["timing"])
 
+        if clean_timing == "always":
+            return self.scheduler.once, None, timedelta(seconds=0)
+
         # there is a complete datetime in the timing, those can only happen once, without a trigger
         if (
             match := re.search(
                 r"(\d{4})-(\d{2})-(\d{2})\s(\d{2}):(\d{2}):(\d{2})",
                 clean_timing,
             )
         ) is not None:
```

### Comparing `pyorchestra-0.5.4/pyproject.toml` & `pyorchestra-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyorchestra"
-version = "0.5.4"
+version = "0.6.0"
 description = "Orchestra is a job scheduler on top of Celery"
 authors = ["András Vidosits <andras@hyperplane.hu>"]
 readme = "README.md"
 license = "LGPLv3"
 repository = "https://github.com/vidosits/orchestra"
 packages = [
 	{ include = "orchestra" },
```

### Comparing `pyorchestra-0.5.4/PKG-INFO` & `pyorchestra-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pyorchestra
-Version: 0.5.4
-Summary: Orchestra is a job scheduler on top of Celery
-Home-page: https://github.com/vidosits/orchestra
-License: LGPLv3
-Author: András Vidosits
-Author-email: andras@hyperplane.hu
-Requires-Python: >=3.11.7,<4.0.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: celery (>=5.3.6,<6.0.0)
-Requires-Dist: fastapi (>=0.110.0,<0.111.0)
-Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
-Requires-Dist: pytz (>=2023.3.post1,<2024.0)
-Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: scheduler (>=0.8.5,<0.9.0)
-Requires-Dist: sqlalchemy (>=2.0.25,<3.0.0)
-Requires-Dist: uvicorn[standard] (>=0.27.1,<0.28.0)
-Project-URL: Repository, https://github.com/vidosits/orchestra
-Description-Content-Type: text/markdown
-
 # Orchestra
 
 Orchestra is:
 - an asyncio based job scheduler
 - using [Celery](https://docs.celeryq.dev/) (which is a distributed task queue) under the hood for running tasks/jobs
 - using [scheduler](https://digon.io/hyd/project/scheduler/t/master/readme.html) under the hood which is a simple in-process python scheduler library with asyncio, threading and timezone support.
 
@@ -56,14 +33,15 @@
   schedules: # a list of schedules
     - name: "short_task_every_1_second" # name of the task that shows up in the logs, *has to be unique*
       task: short_task # the function in the module decorated by `orchestra.task`
       enabled: false # if it's not enabled it will be ignored
       schedule: 
         timing: "every 00:00:01" # see the examples for a list of understood expressions
         timezone: Europe/Paris # name of a time zone from the tz database
+        resume_from_previous: true # if enabled, Orchestra will attempt to calculate what would be the next run based on the last known run, false by default
       additional_options: # everything in this optional section will be passed to the celery task when invoked
         queue: background-jobs
       tags: # tags are list of string, they may be used to group together tasks
         - cpu
         - fast
 ```
 
@@ -90,14 +68,15 @@
 * 2023-04-01 09:13
 * 2023-04-01 09:13:11
 * next 23:00:00
 * once in 5 hours 2 minutes and 15 seconds
 * once in 1 hour and 10 minutes
 * once in 2 minutes and 10 seconds
 * once in 17 seconds
+* always
 
 By default timing expression with only a time or timestamp (without date) like `11:23:00` will be interpreted as a time instant and will trigger the next time the wall clock shows the specified time.
 
 ### Creating an instance
 `main.py`
 ```python
 import asyncio
@@ -139,22 +118,22 @@
 
 ```
 The output would look something like the following:
 ```bash
 [08:38:50] INFO     Job Simple Task every 48 hours was scheduled to  core.py:214
                     run 2 days, 0:00:00                                         
            INFO     Orchestra starting                                core.py:82
-╭───────────┬────────────┬────────────────────────────────────┬───────────────────────┬───────────────────────────┬─────────────┬───────────┬────────────┬──────╮
-│State      │ Shedule    │ Job name                           │ Module and task       │ Due at                    │ Timezone    │ Due in    │ Attempts   │ Tags │
-├───────────┼────────────┼────────────────────────────────────┼───────────────────────┼───────────────────────────┼─────────────┼───────────┼────────────┼──────┤
-│Running    │ CYCLIC     │ Simple Task every 48 hours         │ main.simple_task      │ 2024-03-05 07:38:50       │ UTC         │ 1 day     │ 0/inf      │      │
-╰───────────┴────────────┴────────────────────────────────────┴───────────────────────┴───────────────────────────┴─────────────┴───────────┴────────────┴──────╯
-╭───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
-╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭───────────┬─────────────┬────────────────────────────────────┬───────────────────────┬───────────────────────────┬─────────────┬───────────┬────────────┬──────╮
+│State      │ Schedule    │ Job name                           │ Module and task       │ Due at                    │ Timezone    │ Due in    │ Attempts   │ Tags │
+├───────────┼─────────────┼────────────────────────────────────┼───────────────────────┼───────────────────────────┼─────────────┼───────────┼────────────┼──────┤
+│Running    │ CYCLIC      │ Simple Task every 48 hours         │ main.simple_task      │ 2024-03-05 07:38:50       │ UTC         │ 1 day     │ 0/inf      │      │
+╰───────────┴─────────────┴────────────────────────────────────┴───────────────────────┴───────────────────────────┴─────────────┴───────────┴────────────┴──────╯
+╭────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 
 You may also use a standalone python module for holding your Celery tasks, but you have to declare Orchestra there as well or import it from the main module:
 
 `tasks.py`
 ```python
@@ -271,43 +250,43 @@
                     scheduled to run 0:31:12                                    
            INFO     Job task_every_Monday_at_03_15_00 was scheduled  core.py:214
                     to run Monday(time=datetime.time(3, 15,                     
                     tzinfo=<DstTzInfo 'Europe/Berlin' LMT+1:16:00             
                     STD>))                                                      
            ...
            INFO     Orchestra starting                                core.py:82
-╭────────┬──────────┬────────────────────────────────────────────┬──────────────────────┬─────────────────────┬─────────────────┬──────────┬──────────┬─────────╮
-│State   │ Shedule  │ Job name                                   │ Module and task      │ Due at              │ Timezone        │ Due in   │ Attempts │ Tags    │
-├────────┼──────────┼────────────────────────────────────────────┼──────────────────────┼─────────────────────┼─────────────────┼──────────┼──────────┼─────────┤
-│Running │ ONCE     │ task_at_9_13                               │ tasks.long_task      │ 2024-03-03 09:13:00 │ Europe/Berlin   │ 0:36:09  │ 0/1      │ gpu     │
-│Running │ HOURLY   │ task_every_hour_at_05_00                   │ tasks.long_task      │ 2024-03-03 09:05:00 │ Europe/Berlin   │ 0:28:09  │ 0/inf    │ gpu     │
-│Running │ CYCLIC   │ exception_task_every_10_second             │ tasks.exception_task │ 2024-03-03 07:36:57 │ UTC             │ 0:00:06  │ 0/inf    │ cpu,fast│
-│Running │ DAILY    │ task_every_day_at_9_15                     │ tasks.long_task      │ 2024-03-03 09:15:00 │ Europe/Berlin   │ 0:38:09  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_next_23_00_00                         │ tasks.long_task      │ 2024-03-03 23:00:00 │ Europe/Berlin   │ 14:23:09 │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_in_13_11_52                      │ tasks.long_task      │ 2024-03-03 20:48:39 │ UTC             │ 13:11:49 │ 0/1      │ gpu     │
-│Running │ CYCLIC   │ task_every_31_minutes_12_seconds           │ tasks.long_task      │ 2024-03-03 08:07:59 │ UTC             │ 0:31:09  │ 0/inf    │ gpu     │
-│Running │ CYCLIC   │ short_task_every_1_second                  │ tasks.short_task     │ 2024-03-03 07:36:51 │ UTC             │ 0:00:00  │ 3/inf    │ cpu,fast│
-│Running │ ONCE     │ task_at_11_23_00                           │ tasks.long_task      │ 2024-03-03 11:23:00 │ Europe/Berlin   │ 2:46:09  │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_in_1_hour_and_10_minutes         │ tasks.long_task      │ 2024-03-03 08:46:47 │ UTC             │ 1:09:57  │ 0/1      │ gpu     │
-│Running │ WEEKLY   │ task_every_Monday_at_03_15_00              │ tasks.long_task      │ 2024-03-04 03:15:00 │ Europe/Berlin   │ 18:38:09 │ 0/inf    │ gpu     │
-│Running │ DAILY    │ task_every_day_at_13_hours                 │ tasks.long_task      │ 2024-03-03 13:00:00 │ Europe/Berlin   │ 4:23:09  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_next_Tuesday_at_13_11_00              │ tasks.long_task      │ 2024-03-05 13:11:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
-│Running │ DAILY    │ task_every_day_on_9_03                     │ tasks.long_task      │ 2024-03-03 09:03:00 │ Europe/Berlin   │ 0:26:09  │ 0/inf    │ gpu     │
-│Running │ MINUTELY │ task_every_minute_at_15_seconds            │ tasks.long_task      │ 2024-03-03 08:37:15 │ Europe/Berlin   │ 0:00:24  │ 0/inf    │ gpu     │
-│Running │ ONCE     │ task_2024_04_01_09_13                      │ tasks.long_task      │ 2024-04-01 09:13:00 │ Europe/Berlin   │ 28 days  │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_Wednesday_at_01_15_00            │ tasks.long_task      │ 2024-03-06 01:15:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_on_Thursday_00_31_41             │ tasks.long_task      │ 2024-03-07 00:31:41 │ Europe/Berlin   │ 3 days   │ 0/1      │ gpu     │
-│Running │ ONCE     │ task_once_in_5_hours_2_minutes_and_15_sec… │ tasks.long_task      │ 2024-03-03 12:39:02 │ UTC             │ 5:02:12  │ 0/1      │ gpu     │
-│Running │ DAILY    │ task_every_day_at_09_15_14                 │ tasks.long_task      │ 2024-03-03 09:15:14 │ Europe/Berlin   │ 0:38:23  │ 0/inf    │ gpu     │
-│Running │ CYCLIC   │ task_every_48_hours                        │ tasks.long_task      │ 2024-03-05 07:36:47 │ UTC             │ 1 day    │ 0/inf    │ gpu     │
-│Running │ WEEKLY   │ task_every_Monday_at_03_15_00_US           │ tasks.long_task      │ 2024-03-04 03:15:00 │ America/Boise   │ 1 day    │ 0/inf    │ gpu     │
-╰────────┴──────────┴────────────────────────────────────────────┴──────────────────────┴─────────────────────┴─────────────────┴──────────┴──────────┴─────────╯
-╭───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
-╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭────────┬───────────┬────────────────────────────────────────────┬──────────────────────┬─────────────────────┬─────────────────┬──────────┬──────────┬─────────╮
+│State   │ Schedule  │ Job name                                   │ Module and task      │ Due at              │ Timezone        │ Due in   │ Attempts │ Tags    │
+├────────┼───────────┼────────────────────────────────────────────┼──────────────────────┼─────────────────────┼─────────────────┼──────────┼──────────┼─────────┤
+│Running │ ONCE      │ task_at_9_13                               │ tasks.long_task      │ 2024-03-03 09:13:00 │ Europe/Berlin   │ 0:36:09  │ 0/1      │ gpu     │
+│Running │ HOURLY    │ task_every_hour_at_05_00                   │ tasks.long_task      │ 2024-03-03 09:05:00 │ Europe/Berlin   │ 0:28:09  │ 0/inf    │ gpu     │
+│Running │ CYCLIC    │ exception_task_every_10_second             │ tasks.exception_task │ 2024-03-03 07:36:57 │ UTC             │ 0:00:06  │ 0/inf    │ cpu,fast│
+│Running │ DAILY     │ task_every_day_at_9_15                     │ tasks.long_task      │ 2024-03-03 09:15:00 │ Europe/Berlin   │ 0:38:09  │ 0/inf    │ gpu     │
+│Running │ ONCE      │ task_next_23_00_00                         │ tasks.long_task      │ 2024-03-03 23:00:00 │ Europe/Berlin   │ 14:23:09 │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_in_13_11_52                      │ tasks.long_task      │ 2024-03-03 20:48:39 │ UTC             │ 13:11:49 │ 0/1      │ gpu     │
+│Running │ CYCLIC    │ task_every_31_minutes_12_seconds           │ tasks.long_task      │ 2024-03-03 08:07:59 │ UTC             │ 0:31:09  │ 0/inf    │ gpu     │
+│Running │ CYCLIC    │ short_task_every_1_second                  │ tasks.short_task     │ 2024-03-03 07:36:51 │ UTC             │ 0:00:00  │ 3/inf    │ cpu,fast│
+│Running │ ONCE      │ task_at_11_23_00                           │ tasks.long_task      │ 2024-03-03 11:23:00 │ Europe/Berlin   │ 2:46:09  │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_in_1_hour_and_10_minutes         │ tasks.long_task      │ 2024-03-03 08:46:47 │ UTC             │ 1:09:57  │ 0/1      │ gpu     │
+│Running │ WEEKLY    │ task_every_Monday_at_03_15_00              │ tasks.long_task      │ 2024-03-04 03:15:00 │ Europe/Berlin   │ 18:38:09 │ 0/inf    │ gpu     │
+│Running │ DAILY     │ task_every_day_at_13_hours                 │ tasks.long_task      │ 2024-03-03 13:00:00 │ Europe/Berlin   │ 4:23:09  │ 0/inf    │ gpu     │
+│Running │ ONCE      │ task_next_Tuesday_at_13_11_00              │ tasks.long_task      │ 2024-03-05 13:11:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
+│Running │ DAILY     │ task_every_day_on_9_03                     │ tasks.long_task      │ 2024-03-03 09:03:00 │ Europe/Berlin   │ 0:26:09  │ 0/inf    │ gpu     │
+│Running │ MINUTELY  │ task_every_minute_at_15_seconds            │ tasks.long_task      │ 2024-03-03 08:37:15 │ Europe/Berlin   │ 0:00:24  │ 0/inf    │ gpu     │
+│Running │ ONCE      │ task_2024_04_01_09_13                      │ tasks.long_task      │ 2024-04-01 09:13:00 │ Europe/Berlin   │ 28 days  │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_Wednesday_at_01_15_00            │ tasks.long_task      │ 2024-03-06 01:15:00 │ Europe/Berlin   │ 2 days   │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_on_Thursday_00_31_41             │ tasks.long_task      │ 2024-03-07 00:31:41 │ Europe/Berlin   │ 3 days   │ 0/1      │ gpu     │
+│Running │ ONCE      │ task_once_in_5_hours_2_minutes_and_15_sec… │ tasks.long_task      │ 2024-03-03 12:39:02 │ UTC             │ 5:02:12  │ 0/1      │ gpu     │
+│Running │ DAILY     │ task_every_day_at_09_15_14                 │ tasks.long_task      │ 2024-03-03 09:15:14 │ Europe/Berlin   │ 0:38:23  │ 0/inf    │ gpu     │
+│Running │ CYCLIC    │ task_every_48_hours                        │ tasks.long_task      │ 2024-03-05 07:36:47 │ UTC             │ 1 day    │ 0/inf    │ gpu     │
+│Running │ WEEKLY    │ task_every_Monday_at_03_15_00_US           │ tasks.long_task      │ 2024-03-04 03:15:00 │ America/Boise   │ 1 day    │ 0/inf    │ gpu     │
+╰────────┴───────────┴────────────────────────────────────────────┴──────────────────────┴─────────────────────┴─────────────────┴──────────┴──────────┴─────────╯
+╭────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
 ### Pausing and resuming jobs
 
 ```python
 import asyncio
@@ -377,24 +356,24 @@
                     scheduled to run Monday(time=datetime.time(16,              
                     30, tzinfo=<DstTzInfo 'Europe/Berlin'                       
                     LMT+0:53:00 STD>))                                          
            INFO     Paused job Simple task every Monday at 16:30 UTC core.py:298
            INFO     Paused job Simple task every 1s                  core.py:298
            INFO     Resumed job Simple task every 1s                 core.py:314
            INFO     Orchestra starting                                core.py:82
-╭─────────┬──────────┬─────────────────────────────────────────┬───────────────────────┬──────────────────────┬───────────────┬─────────┬──────────┬────────────╮
-│State    │ Shedule  │ Job name                                │ Module and task       │ Due at               │ Timezone      │ Due in  │ Attempts │ Tags       │
-├─────────┼──────────┼─────────────────────────────────────────┼───────────────────────┼──────────────────────┼───────────────┼─────────┼──────────┼────────────┤
-│Running  │ CYCLIC   │ Hello World every 10s                   │ hello                 │ 2024-03-03 07:39:51  │ UTC           │ 0:00:04 │ 0/inf    │            │
-│Running  │ CYCLIC   │ Simple task every 1s                    │ __main__.simple_task  │ 2024-03-03 07:39:47  │ UTC           │ 0:00:00 │ 5/inf    │ gpu,latency│
-│Paused   │ WEEKLY   │ Simple task every Monday at 16:30 UTC   │ __main__.simple_task  │ 2024-03-04 16:30:00  │ Europe/Berlin │ 1 day   │ 0/inf    │ cpu        │
-╰─────────┴──────────┴─────────────────────────────────────────┴───────────────────────┴──────────────────────┴───────────────┴─────────┴──────────┴────────────╯
-╭───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
-╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─────────┬───────────┬─────────────────────────────────────────┬───────────────────────┬──────────────────────┬───────────────┬─────────┬──────────┬────────────╮
+│State    │ Schedule  │ Job name                                │ Module and task       │ Due at               │ Timezone      │ Due in  │ Attempts │ Tags       │
+├─────────┼───────────┼─────────────────────────────────────────┼───────────────────────┼──────────────────────┼───────────────┼─────────┼──────────┼────────────┤
+│Running  │ CYCLIC    │ Hello World every 10s                   │ hello                 │ 2024-03-03 07:39:51  │ UTC           │ 0:00:04 │ 0/inf    │            │
+│Running  │ CYCLIC    │ Simple task every 1s                    │ __main__.simple_task  │ 2024-03-03 07:39:47  │ UTC           │ 0:00:00 │ 5/inf    │ gpu,latency│
+│Paused   │ WEEKLY    │ Simple task every Monday at 16:30 UTC   │ __main__.simple_task  │ 2024-03-04 16:30:00  │ Europe/Berlin │ 1 day   │ 0/inf    │ cpu        │
+╰─────────┴───────────┴─────────────────────────────────────────┴───────────────────────┴──────────────────────┴───────────────┴─────────┴──────────┴────────────╯
+╭────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ Orchestrating jobs ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 ### Using the API
 
 Orchestra comes with a built-in API accessible by setting `api_server=True` on the `Orchestra` instance.
 You may optionally provide an `api_address` parameter to control which `host:port` gets bound by `uvicorn`.
 
 ```python
@@ -421,8 +400,7 @@
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
 
 You can check the Swagger Docs created by FastAPI at the specified `api_address`, which is [http://localhost:5000](http://localhost:5000) in the above example and by default.
-
```

