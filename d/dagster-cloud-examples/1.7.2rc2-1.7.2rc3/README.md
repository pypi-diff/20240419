# Comparing `tmp/dagster-cloud-examples-1.7.2rc2.tar.gz` & `tmp/dagster-cloud-examples-1.7.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-examples-1.7.2rc2.tar", last modified: Tue Apr 16 20:41:05 2024, max compression
+gzip compressed data, was "dagster-cloud-examples-1.7.2rc3.tar", last modified: Thu Apr 18 21:22:17 2024, max compression
```

## Comparing `dagster-cloud-examples-1.7.2rc2.tar` & `dagster-cloud-examples-1.7.2rc3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:05.760663 dagster-cloud-examples-1.7.2rc2/
--rw-r--r--   0 root         (0) root         (0)      322 2024-04-16 20:41:05.760663 dagster-cloud-examples-1.7.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:05.756663 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:05.756663 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/
--rw-r--r--   0 root         (0) root         (0)       63 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:05.756663 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/jobs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/jobs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:05.760663 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:05.760663 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/
--rw-r--r--   0 root         (0) root         (0)      770 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)      374 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/process_cereals.py
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:05.760663 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/schedules/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      367 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/schedules/daily_process_cereals.py
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:41:05.756663 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples.egg-info/
--rw-r--r--   0 root         (0) root         (0)      322 2024-04-16 20:41:05.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-16 20:41:05.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:41:05.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-16 20:41:05.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-16 20:41:05.000000 dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 20:41:05.760663 dagster-cloud-examples-1.7.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      958 2024-04-16 20:27:18.000000 dagster-cloud-examples-1.7.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:17.744043 dagster-cloud-examples-1.7.2rc3/
+-rw-r--r--   0 root         (0) root         (0)      322 2024-04-18 21:22:17.744043 dagster-cloud-examples-1.7.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:17.740043 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:17.740043 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:17.740043 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/jobs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:17.740043 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:17.740043 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/
+-rw-r--r--   0 root         (0) root         (0)      770 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      374 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/process_cereals.py
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:17.744043 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/schedules/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      367 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/schedules/daily_process_cereals.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:22:17.740043 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      322 2024-04-18 21:22:17.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-18 21:22:17.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:22:17.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-18 21:22:17.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-18 21:22:17.000000 dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 21:22:17.744043 dagster-cloud-examples-1.7.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      958 2024-04-18 21:10:30.000000 dagster-cloud-examples-1.7.2rc3/setup.py
```

### Comparing `dagster-cloud-examples-1.7.2rc2/README.md` & `dagster-cloud-examples-1.7.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py` & `dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples/cereals/jobs/compute_cereal_properties/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-examples-1.7.2rc2/dagster_cloud_examples.egg-info/SOURCES.txt` & `dagster-cloud-examples-1.7.2rc3/dagster_cloud_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-cloud-examples-1.7.2rc2/setup.py` & `dagster-cloud-examples-1.7.2rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ver = get_version()
 # dont pin dev installs to avoid pip dep resolver issues
 pin = "" if ver == "1!0+dev" else f"=={ver}"
 setup(
     name="dagster-cloud-examples",
     version=ver,
     packages=find_packages(exclude=["dagster_cloud_examples_tests*"]),
-    install_requires=["dagster_plus==1.7.2rc2"],
+    install_requires=["dagster_plus==1.7.2rc3"],
     extras_require={"tests": ["mypy", "pylint", "pytest"]},
     author="Elementl",
     author_email="hello@elementl.com",
     license="Apache-2.0",
     classifiers=[
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
```

