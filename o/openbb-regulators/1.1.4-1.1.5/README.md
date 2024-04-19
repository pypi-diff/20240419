# Comparing `tmp/openbb_regulators-1.1.4.tar.gz` & `tmp/openbb_regulators-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_regulators-1.1.4.tar", max compression
+gzip compressed data, was "openbb_regulators-1.1.5.tar", max compression
```

## Comparing `openbb_regulators-1.1.4.tar` & `openbb_regulators-1.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      470 2024-02-29 11:03:36.742659 openbb_regulators-1.1.4/README.md
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.742882 openbb_regulators-1.1.4/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-02-29 11:03:36.742976 openbb_regulators-1.1.4/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1885 2024-03-13 16:36:51.582869 openbb_regulators-1.1.4/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      370 2024-02-29 11:03:36.743107 openbb_regulators-1.1.4/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.743161 openbb_regulators-1.1.4/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-13 16:36:51.583283 openbb_regulators-1.1.4/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0      502 2024-04-01 14:19:19.714644 openbb_regulators-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 openbb_regulators-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      470 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/README.md
+-rw-r--r--   0        0        0       35 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-17 12:33:20.505645 openbb_regulators-1.1.5/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0      502 2024-04-19 16:39:42.707029 openbb_regulators-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 openbb_regulators-1.1.5/PKG-INFO
```

### Comparing `openbb_regulators-1.1.4/openbb_regulators/cftc/cftc_router.py` & `openbb_regulators-1.1.5/openbb_regulators/cftc/cftc_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,9 +55,9 @@
 )
 async def cot(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """Commitment of Traders Reports."""
+    """Get Commitment of Traders Reports."""
     return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_regulators-1.1.4/openbb_regulators/sec/sec_router.py` & `openbb_regulators-1.1.5/openbb_regulators/sec/sec_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 )
 async def schema_files(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """A tool for navigating the directory of SEC XML schema files by year."""
+    """Use tool for navigating the directory of SEC XML schema files by year."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="SymbolMap",
     examples=[APIEx(parameters={"query": "0000789019", "provider": "sec"})],
 )
@@ -104,15 +104,15 @@
 )
 async def rss_litigation(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
     extra_params: ExtraParams,
 ) -> OBBject:
-    """The RSS feed provides links to litigation releases concerning civil lawsuits brought by the Commission in federal court."""  # noqa: E501 pylint: disable=C0301
+    """Get the RSS feed that provides links to litigation releases concerning civil lawsuits brought by the Commission in federal court."""  # noqa: E501 pylint: disable=C0301
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="SicSearch",
     examples=[
         APIEx(parameters={"provider": "sec"}),
```

### Comparing `openbb_regulators-1.1.4/PKG-INFO` & `openbb_regulators-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: openbb-regulators
-Version: 1.1.4
+Version: 1.1.5
 Summary: Markets and Agency Regulators extension for OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.1.5,<2.0.0)
+Requires-Dist: openbb-core (>=1.1.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Regulators Extension
 
 This extension provides a structure for data sourced from various global market regulators.
 
 ## Installation
```

