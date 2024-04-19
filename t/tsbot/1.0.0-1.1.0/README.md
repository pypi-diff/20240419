# Comparing `tmp/tsbot-1.0.0.tar.gz` & `tmp/tsbot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsbot-1.0.0.tar", last modified: Sat Mar 30 01:03:10 2024, max compression
+gzip compressed data, was "tsbot-1.1.0.tar", last modified: Fri Apr 19 00:19:20 2024, max compression
```

## Comparing `tsbot-1.0.0.tar` & `tsbot-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:03:10.298048 tsbot-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-30 01:03:06.000000 tsbot-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-30 01:03:10.298048 tsbot-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-30 01:03:06.000000 tsbot-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-30 01:03:06.000000 tsbot-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 01:03:10.298048 tsbot-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:03:10.290048 tsbot-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-03-30 01:03:06.000000 tsbot-1.0.0/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-30 01:03:06.000000 tsbot-1.0.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-03-30 01:03:06.000000 tsbot-1.0.0/tests/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-30 01:03:06.000000 tsbot-1.0.0/tests/test_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-03-30 01:03:06.000000 tsbot-1.0.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-03-30 01:03:06.000000 tsbot-1.0.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:03:10.294048 tsbot-1.0.0/tsbot/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17667 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:03:10.294048 tsbot-1.0.0/tsbot/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/commands/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/commands/tscommand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:03:10.294048 tsbot-1.0.0/tsbot/default_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/default_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/default_plugins/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/default_plugins/keepalive.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:03:10.294048 tsbot-1.0.0/tsbot/events/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/events/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/events/tsevent.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/events/tsevent_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:03:10.298048 tsbot-1.0.0/tsbot/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/tasks/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/tasks/tstask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-30 01:03:06.000000 tsbot-1.0.0/tsbot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 01:03:10.298048 tsbot-1.0.0/tsbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-30 01:03:10.000000 tsbot-1.0.0/tsbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-30 01:03:10.000000 tsbot-1.0.0/tsbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 01:03:10.000000 tsbot-1.0.0/tsbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-30 01:03:10.000000 tsbot-1.0.0/tsbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-30 01:03:10.000000 tsbot-1.0.0/tsbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.714462 tsbot-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 00:19:04.000000 tsbot-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-19 00:19:20.714462 tsbot-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-19 00:19:04.000000 tsbot-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-19 00:19:04.000000 tsbot-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 00:19:20.714462 tsbot-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.706462 tsbot-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 00:19:04.000000 tsbot-1.1.0/tests/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.706462 tsbot-1.1.0/tsbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/commands/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/default_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/default_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/default_plugins/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/default_plugins/keepalive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/events/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/events/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/query_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/query_builder/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/tasks/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-19 00:19:04.000000 tsbot-1.1.0/tsbot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:19:20.710462 tsbot-1.1.0/tsbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 00:19:20.000000 tsbot-1.1.0/tsbot.egg-info/top_level.txt
```

### Comparing `tsbot-1.0.0/LICENSE` & `tsbot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsbot-1.0.0/PKG-INFO` & `tsbot-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tsbot
-Version: 1.0.0
+Version: 1.1.0
 Summary: Asynchronous framework to build TeamSpeak 3 Server Query bots
 Author: 0x4aK
 Project-URL: repository, https://github.com/0x4aK/tsbot
 Project-URL: documentation, https://tsbot.readthedocs.io/en/latest/
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `tsbot-1.0.0/README.md` & `tsbot-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tsbot-1.0.0/pyproject.toml` & `tsbot-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "tsbot"
-version = "1.0.0"
+version = "1.1.0"
 authors = [{ name = "0x4aK" }]
 description = "Asynchronous framework to build TeamSpeak 3 Server Query bots"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Framework :: AsyncIO",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
 ]
```

### Comparing `tsbot-1.0.0/tests/test_connection.py` & `tsbot-1.1.0/tests/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     assert len(lines_read) == break_after
 
 
 def test_internal_read(connected_conn: connection.TSConnection):
     line = asyncio.run(connected_conn._read())
 
     assert isinstance(line, str)
-    assert line == "line 1\n\r"
+    assert line == "line 1"
 
 
 def test_internal_read_exception_incomplete(
     monkeypatch: pytest.MonkeyPatch, connected_conn: connection.TSConnection
 ):
     def readuntil(*args: Any, **kwargs: Any):
         raise asyncio.IncompleteReadError(b"test exception", expected=0)
```

### Comparing `tsbot-1.0.0/tests/test_query_builder.py` & `tsbot-1.1.0/tests/test_query_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def test_add_params():
     q = query("channelmove")
     assert q._parameters == {}
 
     q = q.params(cid=16, cpid=1, order=0)
-    assert q._parameters == {"cid": "16", "cpid": "1", "order": "0"}
+    assert q._parameters == {"cid": 16, "cpid": 1, "order": 0}
 
 
 def test_add_param_blocks():
     q = query("permidgetbyname")
     assert len(q._parameter_blocks) == 0
 
     q = q.param_block(permsid="b_serverinstance_help_view")
@@ -97,34 +97,44 @@
         ),
     ),
 )
 def test_query_compile(input_query: TSQuery, expected: str) -> None:
     assert input_query.compile() == expected
 
 
-def test_empty_query():
-    with pytest.raises(ValueError):
-        query("")
-
-
 def test_caching():
     q = query("channelmove")
     q.params(cid=16, cpid=1, order=0)
 
     first_compile = q.compile()
 
-    assert q._cached_command
-    assert first_compile == q.compile()
+    assert q._cached_query
+    assert first_compile is q.compile()
 
 
-def test_cache_invalid(q: TSQuery):
+def test_cache_invalid():
+    q = query("channelmove").params(cid=16, cpid=1, order=0)
     first_compile = q.compile()
 
     q = q.option("continueonerror")
 
-    assert not q._cached_command
+    assert not q._cached_query
     assert first_compile != q.compile()
 
 
-@pytest.fixture
-def q():
-    return query("channelmove").params(cid=16, cpid=1, order=0)
+@pytest.mark.parametrize(
+    ("q", "includes"),
+    (
+        pytest.param(
+            query("channeldelete").params(cid=1, force=True),
+            "force=1",
+            id="test_boolean_conversion_true",
+        ),
+        pytest.param(
+            query("channeldelete").params(cid=1, force=False),
+            "force=0",
+            id="test_boolean_conversion_false",
+        ),
+    ),
+)
+def test_boolean_params(q: TSQuery, includes: str):
+    assert includes in q.compile()
```

### Comparing `tsbot-1.0.0/tests/test_ratelimiter.py` & `tsbot-1.1.0/tests/test_ratelimiter.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.0.0/tests/test_response.py` & `tsbot-1.1.0/tests/test_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,76 +7,76 @@
 
 
 @pytest.mark.parametrize(
     ("input_list", "expected_values"),
     (
         pytest.param(
             ["error id=0 msg=ok"],
-            {"data": [], "error_id": 0, "msg": "ok"},
+            {"data": tuple(), "error_id": 0, "msg": "ok"},
             id="test_acknowledgement",
         ),
         pytest.param(
             ["version=3.13.3 build=1608128225 platform=Windows", "error id=0 msg=ok"],
             {
-                "data": [{"version": "3.13.3", "build": "1608128225", "platform": "Windows"}],
+                "data": ({"version": "3.13.3", "build": "1608128225", "platform": "Windows"},),
                 "error_id": 0,
                 "msg": "ok",
             },
             id="test_simple",
         ),
         pytest.param(
             ["error id=256 msg=command\\snot\\sfound"],
-            {"data": [], "error_id": 256, "msg": "command not found"},
+            {"data": tuple(), "error_id": 256, "msg": "command not found"},
             id="test_error",
         ),
         pytest.param(
             ["ip=0.0.0.0|ip=::", "error id=0 msg=ok"],
-            {"data": [{"ip": "0.0.0.0"}, {"ip": "::"}], "error_id": 0, "msg": "ok"},
+            {"data": ({"ip": "0.0.0.0"}, {"ip": "::"}), "error_id": 0, "msg": "ok"},
             id="test_multiple_results",
         ),
     ),
 )
 def test_from_server_response(input_list: list[str], expected_values: dict[str, Any]):
     resp = response.TSResponse.from_server_response(input_list)
 
     assert resp.data == expected_values["data"]
     assert resp.error_id == expected_values["error_id"]
 
 
 def test_first_property():
     resp = response.TSResponse(
-        [{"version": "3.13.3", "build": "1608128225", "platform": "Windows"}], 0, "ok"
+        ({"version": "3.13.3", "build": "1608128225", "platform": "Windows"},), 0, "ok"
     )
     assert resp.first == {"version": "3.13.3", "build": "1608128225", "platform": "Windows"}
 
-    resp = response.TSResponse([{"ip": "0.0.0.0"}, {"ip": "::"}], 0, "ok")
+    resp = response.TSResponse(({"ip": "0.0.0.0"}, {"ip": "::"}), 0, "ok")
     assert resp.first == {"ip": "0.0.0.0"}
 
 
 def test_first_property_empty():
-    resp = response.TSResponse([], 0, "ok")
+    resp = response.TSResponse(tuple(), 0, "ok")
 
     with pytest.raises(IndexError):
         resp.first
 
 
 def test_iter_response():
     resp = response.TSResponse(
-        data=[
+        data=(
             {"clid": "378", "cid": "23", "client_database_id": "21", "client_type": "0"},
             {"clid": "377", "cid": "31", "client_database_id": "549", "client_type": "0"},
             {"clid": "375", "cid": "31", "client_database_id": "46", "client_type": "0"},
             {"clid": "371", "cid": "31", "client_database_id": "385", "client_type": "0"},
             {"clid": "333", "cid": "45", "client_database_id": "27", "client_type": "0"},
             {"clid": "3", "cid": "31", "client_database_id": "160", "client_type": "0"},
-        ],
+        ),
         error_id=0,
         msg="ok",
     )
 
     for client in resp:
         assert isinstance(client, dict)
 
 
 def test_response_repr():
-    resp = response.TSResponse([{"ip": "0.0.0.0"}, {"ip": "::"}], 0, "ok")
+    resp = response.TSResponse(({"ip": "0.0.0.0"}, {"ip": "::"}), 0, "ok")
     assert repr(resp)
```

### Comparing `tsbot-1.0.0/tests/test_utils.py` & `tsbot-1.1.0/tests/test_parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
 import pytest
 
-from tsbot import utils
+from tsbot import parsers
 
 
 @pytest.mark.parametrize(
     ("input_str", "expected"),
     (
-        pytest.param("", [], id="test_empty"),
-        pytest.param("ip=0.0.0.0|ip=::", [{"ip": "0.0.0.0"}, {"ip": "::"}], id="test_simple"),
+        pytest.param("", tuple(), id="test_empty"),
+        pytest.param("ip=0.0.0.0|ip=::", ({"ip": "0.0.0.0"}, {"ip": "::"}), id="test_simple"),
         pytest.param(
             "clid=14 client_nickname=Sven|clid=17 client_nickname=SvenBot",
-            [
+            (
                 {"clid": "14", "client_nickname": "Sven"},
                 {"clid": "17", "client_nickname": "SvenBot"},
-            ],
+            ),
             id="test_multiple_data_simple",
         ),
         pytest.param(
             "cgid=1 name=Channel\\sAdmin type=0 iconid=100 savedb=1 sortid=0 namemode=0 n_modifyp=75 n_member_addp=50 n_member_removep=50|cgid=2 name=Operator type=0 iconid=200 savedb=1 sortid=0 namemode=0 n_modifyp=75 n_member_addp=30 n_member_removep=30|cgid=3 name=Voice type=0 iconid=600 savedb=1 sortid=0 namemode=0 n_modifyp=75 n_member_addp=25 n_member_removep=25|cgid=4 name=Guest type=0 iconid=0 savedb=0 sortid=0 namemode=0 n_modifyp=75 n_member_addp=0 n_member_removep=0|cgid=5 name=Channel\\sAdmin type=1 iconid=100 savedb=1 sortid=0 namemode=0 n_modifyp=75 n_member_addp=50 n_member_removep=50|cgid=6 name=Operator type=1 iconid=200 savedb=1 sortid=0 namemode=0 n_modifyp=75 n_member_addp=30 n_member_removep=30|cgid=7 name=Voice type=1 iconid=600 savedb=1 sortid=0 namemode=0 n_modifyp=75 n_member_addp=25 n_member_removep=25|cgid=8 name=Guest type=1 iconid=0 savedb=0 sortid=0 namemode=0 n_modifyp=75 n_member_addp=0 n_member_removep=0",
-            [
+            (
                 {
                     "cgid": "1",
                     "name": "Channel Admin",
                     "type": "0",
                     "iconid": "100",
                     "savedb": "1",
                     "sortid": "0",
@@ -113,21 +113,21 @@
                     "savedb": "0",
                     "sortid": "0",
                     "namemode": "0",
                     "n_modifyp": "75",
                     "n_member_addp": "0",
                     "n_member_removep": "0",
                 },
-            ],
+            ),
             id="test_multiple_data_complex",
         ),
     ),
 )
 def test_parse_data(input_str: str, expected: list[dict[str, str]]) -> None:
-    assert utils.parse_data(input_str) == expected
+    assert parsers.parse_data(input_str) == expected
 
 
 @pytest.mark.parametrize(
     ("input_str", "expected"),
     (
         pytest.param("", {}, id="test_empty"),
         pytest.param(
@@ -159,58 +159,37 @@
                 "failed_permid": "4",
             },
             id="test_error_line_with_error",
         ),
     ),
 )
 def test_parse_line(input_str: str, expected: dict[str, str]) -> None:
-    assert utils.parse_line(input_str) == expected
+    assert parsers.parse_line(input_str) == expected
 
 
 @pytest.mark.parametrize(
     ("input_str", "expected"),
     (
         pytest.param("clid=12", ("clid", "12"), id="test_simple"),
         pytest.param(
             "client_servergroups=6,16,20",
             ("client_servergroups", "6,16,20"),
             id="test_comma_sepparated",
         ),
-        pytest.param("clid=11|clid=12|clid=13", ("clid", "11,12,13"), id="test_param_block"),
+        pytest.param("clid=11|clid=12|clid=13", ("clid", "11,12,13"), id="test_multiple_values"),
         pytest.param(
             "channel_name=Bot\\sCommands",
             ("channel_name", "Bot Commands"),
             id="test_value_unescape",
         ),
         pytest.param("client_away_message", ("client_away_message", ""), id="test_empty_value"),
     ),
 )
 def test_parse_value(input_str: str, expected: tuple[str, str]) -> None:
-    assert utils.parse_value(input_str) == expected
-
-
-escape_params = (
-    pytest.param("", "", id="test_empty"),
-    pytest.param("TeamSpeak ]|[ Server", r"TeamSpeak\s]\p[\sServer", id="test_default_server_name"),
-    pytest.param(
-        "Test token with custom set", r"Test\stoken\swith\scustom\sset", id="test_sentance"
-    ),
-    pytest.param("		", r"\t\t", id="test_tabs"),
-    pytest.param("| | | | | | |", r"\p\s\p\s\p\s\p\s\p\s\p\s\p", id="test_space_pipes"),
-)
-
-
-@pytest.mark.parametrize(("input_str", "expected"), escape_params)
-def test_escape(input_str: str, expected: str) -> None:
-    assert utils.escape(input_str) == expected
-
-
-@pytest.mark.parametrize(("expected", "input_str"), escape_params)
-def test_unescape(input_str: str, expected: str) -> None:
-    assert utils.unescape(input_str) == expected
+    assert parsers.parse_value(input_str) == expected
 
 
 @pytest.mark.parametrize(
     ("input_str", "expected_args", "expected_kwargs"),
     (
         pytest.param("123 asd test", ("123", "asd", "test"), {}, id="test_args"),
         pytest.param(
@@ -278,8 +257,8 @@
         ),
         pytest.param("asd '", ("asd", "'"), {}, id="test_ending_in_quote"),
     ),
 )
 def test_parse_args_kwargs(
     input_str: str, expected_args: tuple[str], expected_kwargs: dict[str, str]
 ):
-    assert utils.parse_args_kwargs(input_str) == (expected_args, expected_kwargs)
+    assert parsers.parse_args_kwargs(input_str) == (expected_args, expected_kwargs)
```

### Comparing `tsbot-1.0.0/tsbot/bot.py` & `tsbot-1.1.0/tsbot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import inspect
 import logging
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Concatenate,
-    Coroutine,
-    ParamSpec,
-)
+from typing import TYPE_CHECKING, Any, Callable, Concatenate, Coroutine, ParamSpec
 
 from tsbot import (
     commands,
     connection,
     context,
     default_plugins,
     enums,
     events,
     exceptions,
     query_builder,
     ratelimiter,
     response,
     tasks,
+    utils,
 )
 
 if TYPE_CHECKING:
     from tsbot import plugin
 
 _P = ParamSpec("_P")
 
@@ -67,24 +61,24 @@
         self.server_id = server_id
         self.uid: str = ""
 
         self.plugins: dict[str, plugin.TSPlugin] = {}
 
         self._connection = connection.TSConnection(username, password, address, port)
 
-        self.tasks_handler = tasks.TasksHandler()
-        self.event_handler = events.EventHanlder()
-        self.command_handler = commands.CommandHandler(invoker)
+        self._tasks_handler = tasks.TasksHandler()
+        self._event_handler = events.EventHandler()
+        self._command_handler = commands.CommandHandler(invoker)
 
-        self.is_ratelimited = ratelimited
-        self.ratelimiter = ratelimiter.RateLimiter(
+        self._ratelimited = ratelimited
+        self._ratelimiter = ratelimiter.RateLimiter(
             max_calls=ratelimit_calls, period=ratelimit_period
         )
 
-        self.is_closing = False
+        self._closing = False
 
         self._response: asyncio.Future[response.TSResponse]
         self._sending_lock = asyncio.Lock()
         self._query_timeout = query_timeout
 
     def emit(self, event_name: str, ctx: Any | None = None) -> None:
         """
@@ -98,80 +92,80 @@
 
     def emit_event(self, event: events.TSEvent) -> None:
         """
         Emits an event to be handled.
 
         :param event: Event to be emmitted.
         """
-        self.event_handler.event_queue.put_nowait(event)
+        self._event_handler.add_event(event)
 
-    def on(self, event_type: str) -> Callable[[events.TEventH], events.TEventH]:
+    def on(self, event_type: str) -> Callable[[events.TEventHandler], events.TEventHandler]:
         """
         Decorator to register event handlers.
 
         :param event_type: Name of the event.
         """
 
-        def event_decorator(func: events.TEventH) -> events.TEventH:
+        def event_decorator(func: events.TEventHandler) -> events.TEventHandler:
             self.register_event_handler(event_type, func)
             return func
 
         return event_decorator
 
     def register_event_handler(
-        self, event_type: str, handler: events.TEventH
+        self, event_type: str, handler: events.TEventHandler
     ) -> events.TSEventHandler:
         """
-        Register an event handler to be ran on an event
+        Register an event handler to be ran on an event.
 
         :param event_type: Name of the event.
         :param handler: async function to handle the event.
         :return: The instance of :class:`TSEventHandler<tsbot.events.TSEventHandler>` created.
         """
 
         event_handler = events.TSEventHandler(event_type, handler)
-        self.event_handler.register_event_handler(event_handler)
+        self._event_handler.register_event_handler(event_handler)
         return event_handler
 
-    def once(self, event_type: str) -> Callable[[events.TEventH], events.TEventH]:
+    def once(self, event_type: str) -> Callable[[events.TEventHandler], events.TEventHandler]:
         """
         Decorator to register once handler.
 
         :param event_type: Name of the event.
         """
 
-        def once_decorator(func: events.TEventH) -> events.TEventH:
+        def once_decorator(func: events.TEventHandler) -> events.TEventHandler:
             self.register_once_handler(event_type, func)
             return func
 
         return once_decorator
 
     def register_once_handler(
-        self, event_type: str, handler: events.TEventH
+        self, event_type: str, handler: events.TEventHandler
     ) -> events.TSEventOnceHandler:
         """
         Register an event handler to be ran once on an event.
 
         :param event_type: Name of the event.
         :param handler: async function to handle the event.
         :return: The instance of :class:`TSEventOnceHandler<tsbot.events.TSEventOnceHandler>` created.
         """
 
-        event_handler = events.TSEventOnceHandler(event_type, handler, self.event_handler)
-        self.event_handler.register_event_handler(event_handler)
+        event_handler = events.TSEventOnceHandler(event_type, handler, self._event_handler)
+        self._event_handler.register_event_handler(event_handler)
         return event_handler
 
     def remove_event_handler(self, event_handler: events.TSEventHandler) -> None:
         """
         Remove event handler from the event system.
 
         :param event_handler: Instance of the :class:`TSEventHandler<tsbot.events.TSEventHandler>` to be removed.
         """
 
-        self.event_handler.remove_event_handler(event_handler)
+        self._event_handler.remove_event_handler(event_handler)
 
     def command(
         self,
         *command: str,
         help_text: str = "",
         raw: bool = False,
         hidden: bool = False,
@@ -221,113 +215,116 @@
         :param checks: List of async functions to be called before the command is executed.
         :return: The instance of :class:`TSCommand<tsbot.commands.TSCommand>` created.
         """
         if isinstance(command, str):
             command = (command,)
 
         command_handler = commands.TSCommand(command, handler, help_text, raw, hidden, checks or [])
-        self.command_handler.register_command(command_handler)
+        self._command_handler.register_command(command_handler)
         return command_handler
 
     def remove_command(self, command: commands.TSCommand) -> None:
         """
         Remove command handler from the command system.
 
         :param command: Instance of the :class:`TSCommand<tsbot.commands.TSCommand>` to be removed.
         """
-        self.command_handler.remove_command(command)
+        self._command_handler.remove_command(command)
+
+    def get_command_handler(self, command: str) -> commands.TSCommand | None:
+        """
+        Get :class:`TSCommand<tsbot.commands.TSCommand>` instance associated with a given `str`
+
+        :param command: command that invokes :class:`TSCommand<tsbot.commands.TSCommand>`
+        :return: :class:`TSCommand<tsbot.commands.TSCommand>` associated with `command`
+        """
+        return self._command_handler.commands.get(command)
 
     def register_every_task(
         self,
         seconds: float,
-        handler: tasks.TTaskH,
+        handler: tasks.TTaskHandler,
         *,
         name: str | None = None,
     ) -> tasks.TSTask:
         """
         Register task handler to be ran every given second.
 
         :param seconds: How often the task is executed.
         :param handler: async function to be called when the task is executed.
         :param name: Name of the task.
         :return: Instance of :class:`TSTask<tsbot.tasks.TSTask>` created.
         """
         task = tasks.TSTask(handler=tasks.every(handler, seconds), name=name)
-        self.tasks_handler.register_task(self, task)
+        self._tasks_handler.register_task(self, task)
         return task
 
     def register_task(
         self,
-        handler: tasks.TTaskH,
+        handler: tasks.TTaskHandler,
         *,
         name: str | None = None,
     ) -> tasks.TSTask:
         """
         Register task handler as a background task.
 
         :param handler: async function to be called when the task is executed.
         :param name: Name of the task.
         :return: Instance of :class:`TSTask<tsbot.tasks.TSTask>` created.
         """
 
         task = tasks.TSTask(handler=handler, name=name)
-        self.tasks_handler.register_task(self, task)
+        self._tasks_handler.register_task(self, task)
         return task
 
     def remove_task(self, task: tasks.TSTask) -> None:
         """
         Remove a background task from tasks.
 
         :param task: Instance of the :class:`TSTask<tsbot.tasks.TSTask>` to be removed.
         """
-        self.tasks_handler.remove_task(task)
+        self._tasks_handler.remove_task(task)
 
     async def send(self, query: query_builder.TSQuery) -> response.TSResponse:
         """
-        Sends queries to the server, assuring only one of them gets sent at a time
+        Sends queries to the server, assuring only one of them gets sent at a time.
 
         :param query: Instance of :class:`TSQuery<tsbot.query_builder.TSQuery>` to be send to the server.
         :return: Response from the server.
         """
         try:
             return await self.send_raw(query.compile())
         except exceptions.TSResponseError as response_error:
-            if (tb := response_error.__traceback__) and tb.tb_next:
-                response_error = response_error.with_traceback(tb.tb_next.tb_next)
-
-            raise response_error
+            raise utils.pop_traceback(response_error, 2)
 
     async def send_raw(self, raw_query: str) -> response.TSResponse:
         """
         Sends raw commands to the server.
 
         Its recommended to use built-in query builder and
         :func:`send()<tsbot.TSBot.send()>` method instead.
 
         :param raw_query: raw query command to be send to the server.
         :return: Response from the server.
         """
         try:
             return await asyncio.shield(self._send(raw_query))
         except exceptions.TSResponseError as response_error:
-            if (tb := response_error.__traceback__) and tb.tb_next:
-                response_error = response_error.with_traceback(tb.tb_next.tb_next)
-
-            raise response_error
+            raise utils.pop_traceback(response_error, 2)
 
     async def _send(self, raw_query: str) -> response.TSResponse:
         """Method responsibe for actually sending the data."""
 
         async with self._sending_lock:
             self._response = asyncio.Future()
 
-            if self.is_ratelimited:
-                await self.ratelimiter.wait()
+            if self._ratelimited:
+                await self._ratelimiter.wait()
 
-            logger.debug("Sending query: %s", raw_query)
+            logger.debug("Sending query: %r", raw_query)
             self.emit(event_name="send", ctx={"query": raw_query})
             await self._connection.write(raw_query)
 
             server_response = await asyncio.wait_for(
                 asyncio.shield(self._response), self._query_timeout
             )
 
@@ -338,24 +335,24 @@
                 msg=server_response.msg,
                 error_id=server_response.error_id,
                 perm_id=int(server_response.last["failed_permid"]),
             )
 
         if server_response.error_id != 0:
             raise exceptions.TSResponseError(
-                msg=server_response.msg, error_id=int(server_response.error_id)
+                msg=server_response.msg,
+                error_id=int(server_response.error_id),
             )
 
         return server_response
 
     async def _reader_task(self, ready_event: asyncio.Event) -> None:
-        """Task to read messages from the server"""
+        """Task to read messages from the server."""
 
         WELCOME_MESSAGE_LENGTH = 2
-
         async for data in self._connection.read_lines(WELCOME_MESSAGE_LENGTH):
             pass
 
         logger.debug("Skipped welcome message")
         ready_event.set()
 
         response_buffer: list[str] = []
@@ -371,38 +368,35 @@
                 response_buffer.clear()
 
             else:
                 response_buffer.append(data)
 
         logger.debug("Reader task done")
 
-    async def close(self) -> None:
+    def close(self) -> None:
         """
-        Async function to handle closing the bot
+        Method to close the bot.
 
-        Emits `close` event to notify client closing,
+        Emits `close` event to notify that the client is closing,
         cancels background tasks and send quit command.
         """
 
-        if self.is_closing:
-            return
+        if not self._closing:
+            self._closing = True
+            asyncio.create_task(self._close())
 
-        self.is_closing = True
-
-        logger.info("Closing")
+    async def _close(self) -> None:
+        logger.info("Closing bot")
         self.emit(event_name="close")
-
-        await self.tasks_handler.close()
+        await self._tasks_handler.close()
+        await self._event_handler.run_till_empty(self)
 
         with contextlib.suppress(Exception):
             await self.send_raw("quit")
 
-        self.event_handler.run_till_empty(self)
-        await self.event_handler.event_queue.join()
-
         logger.info("Closing done")
 
     async def run(self) -> None:
         """
         Run the bot.
 
         Connects to the server, registers the server to send events
@@ -416,15 +410,15 @@
             reader = asyncio.create_task(self._reader_task(reader_ready))
             await reader_ready.wait()
 
             return reader
 
         async def select_server() -> None:
             """Set current virtual server"""
-            await self.send(query_builder.TSQuery("use", parameters={"sid": str(self.server_id)}))
+            await self.send(query_builder.TSQuery("use", parameters={"sid": self.server_id}))
 
         async def register_notifies() -> None:
             """Coroutine to register server to send events to the bot"""
 
             notify_query = query_builder.TSQuery("servernotifyregister")
 
             await self.send(notify_query.params(event="channel", id=0))
@@ -432,19 +426,19 @@
                 await self.send(notify_query.params(event=event))
 
         async def update_uid() -> None:
             """Gets the uid of the client"""
             resp = await self.send_raw("whoami")
             self.uid = resp.first["client_unique_identifier"]
 
-        self.register_task(self.event_handler.handle_events_task, name="HandleEvents-Task")
-        self.register_event_handler("textmessage", self.command_handler.handle_command_event)
+        self.register_task(self._event_handler.handle_events_task, name="HandleEvents-Task")
+        self.register_event_handler("textmessage", self._command_handler.handle_command_event)
         self.load_plugin(default_plugins.Help(), default_plugins.KeepAlive())
 
-        self.tasks_handler.start(self)
+        self._tasks_handler.start(self)
         self.emit(event_name="run")
 
         logger.info("Setting up connection")
 
         try:
             await self._connection.connect()
             reader_task = await get_reader_task()
@@ -456,15 +450,15 @@
             await register_notifies()
 
             self.emit(event_name="ready")
 
             await reader_task
 
         finally:
-            await self.close()
+            await self._close()
             await self._connection.close()
 
     def load_plugin(self, *plugins: plugin.TSPlugin) -> None:
         """
         Loads :class:`TSPlugin<tsbot.plugins.TSPlugin>` instances into the bot.
 
         :param plugins: Instances of :class:`TSPlugin<tsbot.plugins.TSPlugin>`
@@ -492,15 +486,15 @@
         """
         target_mode = enums.TextMessageTargetMode(ctx["targetmode"])
         target = ctx["invokerid"] if target_mode == enums.TextMessageTargetMode.CLIENT else "0"
 
         await self.send(
             query_builder.TSQuery(
                 "sendtextmessage",
-                parameters={"targetmode": target_mode.value, "target": target, "msg": str(message)},
+                parameters={"targetmode": target_mode.value, "target": target, "msg": message},
             )
         )
 
     async def respond_to_client(self, ctx: context.TSCtx, message: str) -> None:
         """
         Responds to a client with a direct message.
 
@@ -511,11 +505,11 @@
         if target := ctx.get("invokerid"):
             await self.send(
                 query_builder.TSQuery(
                     "sendtextmessage",
                     parameters={
                         "targetmode": enums.TextMessageTargetMode.CLIENT.value,
                         "target": target,
-                        "msg": str(message),
+                        "msg": message,
                     },
                 )
             )
```

### Comparing `tsbot-1.0.0/tsbot/commands/handler.py` & `tsbot-1.1.0/tsbot/commands/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         self.invoker = invoker
         self.commands: dict[str, commands.TSCommand] = {}
 
     def register_command(self, command: commands.TSCommand) -> None:
         self.commands.update({c: command for c in command.commands})
 
         logger.debug(
-            "Registered %s command to execute %r",
+            "Registered %s command to execute handler %r",
             ", ".join(repr(c) for c in command.commands),
-            command.handler,
+            command.handler.__name__,
         )
 
     def remove_command(self, command: commands.TSCommand) -> None:
         for c in command.commands:
             del self.commands[c]
 
     async def handle_command_event(self, bot: bot.TSBot, ctx: context.TSCtx) -> None:
```

### Comparing `tsbot-1.0.0/tsbot/commands/tscommand.py` & `tsbot-1.1.0/tsbot/commands/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import asyncio
 import inspect
 import itertools
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Callable, Coroutine
+from typing import TYPE_CHECKING, Callable, Coroutine, cast
 
-from tsbot import exceptions, utils
+from tsbot import exceptions, parsers
 
 if TYPE_CHECKING:
     from tsbot import bot, context
 
 
 @dataclass(slots=True)
 class TSCommand:
@@ -65,15 +65,18 @@
             pending_task.cancel()
 
         for done_task in done:
             if exception := done_task.exception():
                 raise exception
 
     async def run(self, bot: bot.TSBot, ctx: context.TSCtx, msg: str) -> None:
-        args, kwargs = utils.parse_args_kwargs(msg) if not self.raw else ((msg,) if msg else (), {})
+        if self.raw:
+            args, kwargs = (msg,) if msg else (), cast(dict[str, str], {})
+        else:
+            args, kwargs = parsers.parse_args_kwargs(msg)
 
         if self.checks:
             await self.run_checks(bot, ctx, *args, **kwargs)
 
         try:
             binded_arguments = self.call_signature.bind(bot, ctx, *args, **kwargs)
         except TypeError as e:
```

### Comparing `tsbot-1.0.0/tsbot/connection.py` & `tsbot-1.1.0/tsbot/connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
-import asyncio
 import logging
-from typing import AsyncIterator
+from typing import AsyncGenerator
 
 import asyncssh
 
 logger = logging.getLogger(__name__)
 
 
 class TSConnection:
@@ -39,39 +38,37 @@
 
         if self._connection:
             self._connection.close()
             await self._connection.wait_closed()
 
         logger.info("Connection closed")
 
-    async def read_lines(self, number_of_lines: int = 1) -> AsyncIterator[str]:
+    async def read_lines(self, number_of_lines: int = 1) -> AsyncGenerator[str, None]:
         lines_read = 0
 
-        while lines_read < number_of_lines and (data := await self._read()):
+        while lines_read < number_of_lines and (data := await self._read()) is not None:
             lines_read += 1
-            yield data.strip()
+            yield data
 
-    async def read(self) -> AsyncIterator[str]:
-        while data := await self._read():
-            yield data.strip()
+    async def read(self) -> AsyncGenerator[str, None]:
+        while (data := await self._read()) is not None:
+            yield data
 
         logger.debug("Reading done")
 
     async def _read(self) -> str | None:
         if not self._reader:
             raise ConnectionResetError("Trying to read on a closed connection")
 
         try:
             data = await self._reader.readuntil("\n\r")
-
-        except asyncio.IncompleteReadError:
+        except Exception:
             return None
-
         else:
-            return data
+            return data.rstrip()
 
     async def write(self, msg: str) -> None:
         if not self._writer or self._writer.is_closing():
             raise BrokenPipeError("Trying to write on a closed connection")
 
         self._writer.write(f"{msg}\n\r")
```

### Comparing `tsbot-1.0.0/tsbot/default_plugins/help.py` & `tsbot-1.1.0/tsbot/default_plugins/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Help(plugin.TSPlugin):
     @plugin.command("help", help_text="Prints out the help text of a given command and usage")
     async def help_command(self, bot: bot.TSBot, ctx: context.TSCtx, command: str) -> None:
-        command_handler = bot.command_handler.commands.get(command)
+        command_handler = bot.get_command_handler(command)
 
         if not command_handler or command_handler.hidden:
             raise exceptions.TSCommandError("Command not found")
 
         response_text = "\n"
 
         if help_text := command_handler.help_text:
```

### Comparing `tsbot-1.0.0/tsbot/default_plugins/keepalive.py` & `tsbot-1.1.0/tsbot/default_plugins/keepalive.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.0.0/tsbot/events/handler.py` & `tsbot-1.1.0/tsbot/events/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
+from tsbot import utils
+
 if TYPE_CHECKING:
     from tsbot import bot, events
 
 
 logger = logging.getLogger(__name__)
 
 
-class EventHanlder:
+class EventHandler:
     def __init__(self) -> None:
-        self.event_handlers: defaultdict[str, list[events.TSEventHandler]] = defaultdict(list)
-        self.event_queue: asyncio.Queue[events.TSEvent] = asyncio.Queue()
+        self._event_handlers: defaultdict[str, list[events.TSEventHandler]] = defaultdict(list)
+        self._event_queue: asyncio.Queue[events.TSEvent] = asyncio.Queue()
+        self._closed = False
+
+    def add_event(self, event: events.TSEvent) -> None:
+        if self._closed:
+            logger.warn("Event %r emitted during closing and is ignored", event.event)
+        else:
+            self._event_queue.put_nowait(event)
 
     def handle_event(self, bot: bot.TSBot, event: events.TSEvent) -> None:
-        logger.debug("Got event: %s", event)
-
-        handlers = self.event_handlers.get(event.event)
+        logger.debug("Got event: %r", event)
+        handlers = self._event_handlers.get(event.event)
 
         if not handlers:
-            self.event_queue.task_done()
+            self._event_queue.task_done()
             return
 
         tasks = [asyncio.create_task(h.run(bot, event), name="EventHandler") for h in handlers]
+        watcher = asyncio.create_task(asyncio.wait(tasks), name="EventWatcher")
+        watcher.add_done_callback(lambda _: self._event_queue.task_done())
 
-        task = asyncio.create_task(asyncio.wait(tasks), name="EventWatcher")
-        task.add_done_callback(lambda _: self.event_queue.task_done())
+    async def run_till_empty(self, bot: bot.TSBot) -> None:
+        while not self._event_queue.empty():
+            self.handle_event(bot, self._event_queue.get_nowait())
 
-    def run_till_empty(self, bot: bot.TSBot) -> None:
-        while not self.event_queue.empty():
-            self.handle_event(bot, self.event_queue.get_nowait())
+        await self._event_queue.join()
 
     async def handle_events_task(self, bot: bot.TSBot) -> None:
-        """
-        Task to run events put into the self.event_queue
+        """Task to run events put into the event queue."""
+
+        with utils.toggle(self, "_closed", enter=False, exit=True):
+            try:
+                while True:
+                    self.handle_event(bot, await self._event_queue.get())
 
-        if task is cancelled, it will try to run all the events
-        still in the queue until empty
-        """
-
-        try:
-            while True:
-                self.handle_event(bot, await self.event_queue.get())
-
-        except asyncio.CancelledError:
-            logger.debug("Cancelling event handling")
-            self.run_till_empty(bot)
+            except asyncio.CancelledError:
+                logger.debug("Cancelling event handling")
 
     def register_event_handler(self, event_handler: events.TSEventHandler) -> None:
-        """Registers event handlers that will be called when given event happens"""
-        self.event_handlers[event_handler.event].append(event_handler)
+        """Registers event handlers that will be called when given event happens."""
+        self._event_handlers[event_handler.event].append(event_handler)
 
         logger.debug(
-            "Registered %r event to execute %r", event_handler.event, event_handler.handler
+            "Registered %r event to execute handler %r",
+            event_handler.event,
+            event_handler.handler.__name__,
         )
 
     def remove_event_handler(self, event_handler: events.TSEventHandler) -> None:
-        self.event_handlers[event_handler.event].remove(event_handler)
+        self._event_handlers[event_handler.event].remove(event_handler)
 
-        if not self.event_handlers[event_handler.event]:
-            del self.event_handlers[event_handler.event]
+        if not self._event_handlers[event_handler.event]:
+            del self._event_handlers[event_handler.event]
```

### Comparing `tsbot-1.0.0/tsbot/events/tsevent.py` & `tsbot-1.1.0/tsbot/events/event.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, NamedTuple, TypeVar
 
-from tsbot import context, utils
+from tsbot import context, parsers
 
 _T = TypeVar("_T", bound="TSEvent")
 
 
 class TSEvent(NamedTuple):
     event: str
     ctx: Any
@@ -17,9 +17,9 @@
         Creates a TSEvent instance from server notify
 
         Will remove the 'notify' from the beginning of the 'event'
         """
         event, _, data = raw_data.partition(" ")
         return cls(
             event=event.removeprefix("notify"),
-            ctx=context.TSCtx(utils.parse_line(data)),
+            ctx=context.TSCtx(parsers.parse_line(data)),
         )
```

### Comparing `tsbot-1.0.0/tsbot/events/tsevent_handler.py` & `tsbot-1.1.0/tsbot/events/event_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Callable, Coroutine
 
 if TYPE_CHECKING:
     from tsbot import bot, events
 
 
-TEventH = Callable[["bot.TSBot", Any], Coroutine[None, None, None]]
+TEventHandler = Callable[["bot.TSBot", Any], Coroutine[None, None, None]]
 
 
 @dataclass(slots=True)
 class TSEventHandler:
     event: str
-    handler: TEventH
+    handler: TEventHandler
 
     async def run(self, bot: bot.TSBot, event: events.TSEvent) -> None:
         await self.handler(bot, event.ctx)
 
 
 @dataclass(slots=True)
 class TSEventOnceHandler(TSEventHandler):
-    event_handler: events.EventHanlder
+    event_handler: events.EventHandler
 
     async def run(self, bot: bot.TSBot, event: events.TSEvent) -> None:
         self.event_handler.remove_event_handler(self)
         await self.handler(bot, event.ctx)
```

### Comparing `tsbot-1.0.0/tsbot/exceptions.py` & `tsbot-1.1.0/tsbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.0.0/tsbot/plugin.py` & `tsbot-1.1.0/tsbot/plugin.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.0.0/tsbot/query_builder.py` & `tsbot-1.1.0/tsbot/query_builder/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 from __future__ import annotations
 
+import itertools
 from collections.abc import Mapping
-from typing import Iterable, Protocol, TypeVar
+from typing import TYPE_CHECKING, Iterable, Protocol, TypeVar
+
+from tsbot import encoders
+
+if TYPE_CHECKING:
+    from tsbot import query_builder
 
-from tsbot import utils
 
 _T = TypeVar("_T", bound="TSQuery")
 
 
 class Stringable(Protocol):
     def __str__(self) -> str: ...
 
 
-def query(command: str) -> TSQuery:
+def query(command: query_builder.TCommands) -> TSQuery:
     """
     Function to create :class:`TSQuery<tsbot.query_builder.TSQuery>` instances.
 
     :param command: Base query command.
     :return: The created :class:`TSQuery<tsbot.query_builder.TSQuery>` instance.
     """
     return TSQuery(command)
 
 
-def _to_dict_values(kv: tuple[str, Stringable]) -> tuple[str, str]:
-    return kv[0], str(kv[1])
+def _format_value(key: str, value: Stringable) -> str:
+    return f"{key}={int(value) if isinstance(value, bool) else encoders.escape(str(value))}"
 
 
-def _format_value(kv: tuple[str, str]) -> str:
-    return f"{kv[0]}={utils.escape(kv[1])}"
+def _format_parameters(params: Mapping[str, Stringable]) -> str:
+    return " ".join(itertools.starmap(_format_value, params.items()))
 
 
 class TSQuery:
     """
     Class to represent query commands to the TeamSpeak server.
     """
 
     __slots__ = (
         "_command",
-        "_cached_command",
+        "_cached_query",
         "_options",
         "_parameters",
         "_parameter_blocks",
     )
 
     def __init__(
         self,
-        command: str,
-        options: tuple[str, ...] | None = None,
-        parameters: dict[str, str] | None = None,
-        parameter_blocks: tuple[dict[str, str], ...] | None = None,
+        command: query_builder.TCommands,
+        options: tuple[Stringable, ...] | None = None,
+        parameters: dict[str, Stringable] | None = None,
+        parameter_blocks: tuple[dict[str, Stringable], ...] | None = None,
     ) -> None:
         """
         :param command: Base query command.
         :param options: Options attached to the query.
         :param parameters: Parameters attached to the query.
         :param parameter_blocks: Parameter blocks attached to the query.
         """
-        if not command:
-            raise ValueError("Command cannot be empty")
-
         self._command = command
-
-        self._cached_command: str = ""
+        self._cached_query: str | None = None
 
         self._options = options or tuple()
         self._parameters = parameters or {}
         self._parameter_blocks = parameter_blocks or tuple()
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}({self._command!r})"
@@ -75,32 +76,32 @@
         Add options to the command eg. ``-groups``.
 
         :param args: Tuple of options to be attached.
         :return: New :class:`TSQuery<tsbot.query_builder.TSQuery>` instance with added params
         """
 
         return type(self)(
-            self._command,
-            self._options + tuple(map(str, args)),
+            self._command,  # type: ignore
+            self._options + args,
             self._parameters,
             self._parameter_blocks,
         )
 
     def params(self: _T, **kwargs: Stringable) -> _T:
         """
         Add parameters to the command eg. ``cldbid=12``.
 
         :param kwargs: Keyword to be attached.
         :return: New :class:`TSQuery<tsbot.query_builder.TSQuery>` instance with added parameters
         """
 
         return type(self)(
-            self._command,
+            self._command,  # type:ignore
             self._options,
-            self._parameters | dict(map(_to_dict_values, kwargs.items())),
+            self._parameters | kwargs,
             self._parameter_blocks,
         )
 
     def param_block(
         self: _T,
         blocks: Iterable[Mapping[str, Stringable]] | None = None,
         /,
@@ -112,40 +113,41 @@
         or **one** block at a time.
 
         :param blocks: Iterable of parameter blocks to be attached.
         :param kwargs: Parameters to be attached to single block.
         :return: New :class:`TSQuery<tsbot.query_builder.TSQuery>` instance with added parameter blocks
         """
 
-        param_blocks = tuple(blocks) if blocks else (kwargs,)
+        param_blocks: tuple[dict[str, Stringable], ...] = (
+            tuple(map(dict, blocks)) if blocks else (kwargs,)
+        )
 
         return type(self)(
-            self._command,
+            self._command,  # type:ignore
             self._options,
             self._parameters,
-            self._parameter_blocks
-            + tuple(dict(map(_to_dict_values, block.items())) for block in param_blocks),
+            self._parameter_blocks + param_blocks,
         )
 
     def compile(self) -> str:
         """
         Compiles the query into a raw command.
 
         :return: The compiled query command.
         """
 
-        if self._cached_command:
-            return self._cached_command
+        if self._cached_query:
+            return self._cached_query
 
-        compiled = self._command
+        compiled: str = self._command
 
         if self._parameters:
-            compiled += f" {' '.join(map(_format_value, self._parameters.items()))}"
+            compiled += f" {_format_parameters(self._parameters)}"
 
         if self._parameter_blocks:
-            compiled += f" {'|'.join(' '.join(map(_format_value, parameters.items())) for parameters in self._parameter_blocks)}"
+            compiled += f" {'|'.join(map(_format_parameters, self._parameter_blocks))}"
 
         if self._options:
             compiled += f" {' '.join(f'-{option}' for option in self._options)}"
 
-        self._cached_command = compiled
+        self._cached_query = compiled
         return compiled
```

### Comparing `tsbot-1.0.0/tsbot/ratelimiter.py` & `tsbot-1.1.0/tsbot/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `tsbot-1.0.0/tsbot/response.py` & `tsbot-1.1.0/tsbot/response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Generator, TypeVar
 
-from tsbot import utils
+from tsbot import parsers
 
 _T = TypeVar("_T", bound="TSResponse")
 
 
 @dataclass(slots=True, frozen=True)
 class TSResponse:
     """
     Class to represent the response to a query from a Teamspeak server.
     """
 
-    data: list[dict[str, str]]
+    data: tuple[dict[str, str], ...]
     error_id: int
     msg: str
 
     def __iter__(self) -> Generator[dict[str, str], None, None]:
         yield from self.data
 
     @property
@@ -29,17 +29,17 @@
     @property
     def last(self) -> dict[str, str]:
         """Last datapoint from the response"""
         return self.data[-1]
 
     @classmethod
     def from_server_response(cls: type[_T], raw_data: list[str]) -> _T:
-        response_info = utils.parse_line(raw_data[-1].removeprefix("error "))
-        data = utils.parse_data("".join(raw_data[:-1]))
+        response_info = parsers.parse_line(raw_data[-1].removeprefix("error "))
+        data = parsers.parse_data("".join(raw_data[:-1]))
 
         error_id = int(response_info.pop("id"))
         msg = response_info.pop("msg")
 
         if response_info:
-            data.append(response_info)
+            data += (response_info,)
 
         return cls(data=data, error_id=error_id, msg=msg)
```

### Comparing `tsbot-1.0.0/tsbot/tasks/handler.py` & `tsbot-1.1.0/tsbot/tasks/handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import TYPE_CHECKING
 
-logger = logging.getLogger(__name__)
-
 if TYPE_CHECKING:
     from tsbot import bot, tasks
 
 
+logger = logging.getLogger(__name__)
+
+
 class TasksHandler:
     def __init__(self) -> None:
         self._started = False
         self._tasks: list[tasks.TSTask] = []
         self._starting_tasks: list[tasks.TSTask] = []
 
     def _start_task(self, bot: bot.TSBot, task: tasks.TSTask) -> None:
@@ -24,30 +25,29 @@
 
     def register_task(self, bot: bot.TSBot, task: tasks.TSTask) -> None:
         if not self._started:
             self._starting_tasks.append(task)
         else:
             self._start_task(bot, task)
 
-        logger.debug("Registered a task %r", task.handler)
+        logger.debug("Registered a task handler %r", task.handler.__name__)
 
     def remove_task(self, task: tasks.TSTask) -> None:
         if task.task and not task.task.done():
             task.task.cancel()
 
-        self._tasks = [t for t in self._tasks if t is not task]
+        self._tasks = list(filter(lambda t: t is not task, self._tasks))
 
     def start(self, bot: bot.TSBot) -> None:
         while self._starting_tasks:
             self._start_task(bot, self._starting_tasks.pop())
 
         self._started = True
         logger.debug("Task handler started")
 
     async def close(self) -> None:
-        for task in self._tasks:
-            if task.task:
-                task.task.cancel()
+        for task in filter(bool, map(lambda t: t.task, self._tasks)):
+            task.cancel()  # type: ignore
 
         # Sleep until all the tasks are removed from tasks list
         while self._tasks:
             await asyncio.sleep(0)
```

### Comparing `tsbot-1.0.0/tsbot/tasks/tstask.py` & `tsbot-1.1.0/tsbot/tasks/task.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Callable, Coroutine
 
 if TYPE_CHECKING:
     from tsbot import bot
 
 
-TTaskH = Callable[["bot.TSBot"], Coroutine[None, None, None]]
+TTaskHandler = Callable[["bot.TSBot"], Coroutine[None, None, None]]
 
 
 @dataclass(slots=True)
 class TSTask:
-    handler: TTaskH
+    handler: TTaskHandler
     name: str | None = None
     task: asyncio.Task[None] | None = None
 
 
-def every(every_handler: TTaskH, seconds: float) -> TTaskH:
+def every(every_handler: TTaskHandler, seconds: float) -> TTaskHandler:
     @functools.wraps(every_handler)
     async def every_wrapper(bot: bot.TSBot) -> None:
         while True:
             try:
                 await asyncio.sleep(seconds)
                 await every_handler(bot)
             except asyncio.CancelledError:
```

### Comparing `tsbot-1.0.0/tsbot/utils.py` & `tsbot-1.1.0/tsbot/parsers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
+from tsbot import encoders
+
 KWARG_INDICATOR = "-"
 
 
-def parse_data(input_str: str) -> list[dict[str, str]]:
+def parse_data(input_str: str) -> tuple[dict[str, str], ...]:
     if not input_str:
-        return []
+        return tuple()
 
-    return list(map(parse_line, input_str.split("|")))
+    return tuple(map(parse_line, input_str.split("|")))
 
 
 def parse_line(input_str: str) -> dict[str, str]:
     if not input_str:
         return {}
 
     return dict(map(parse_value, input_str.split(" ")))
 
 
 def parse_value(input_str: str) -> tuple[str, str]:
     key, _, value = input_str.partition("=")
 
     if "|" in value:
         # Multiple values associated with the key. Making values comma separated
-        return key, ",".join(v for v in value.split(f"|{key}="))
+        return key, ",".join(map(encoders.unescape, value.split(f"|{key}=")))
 
-    return key, unescape(value) if value else ""
+    return key, encoders.unescape(value) if value else ""
 
 
 def _parse_quoted_arg(unparsed: str) -> tuple[str, str]:
     """
     Parses a quoted argument, returns it and unparsed part.
 
     If a qoute doesn't have a whitespace behind it, that part is not considered a quote end.
@@ -84,38 +86,7 @@
             args.append(value)
 
         else:
             value, unparsed = _parse_arg(unparsed)
             args.append(value)
 
     return tuple(args), kwargs
-
-
-# https://github.com/benediktschmitt/py-ts3/blob/v2/ts3/escape.py
-
-ESCAPE_MAP = (
-    ("\\", r"\\"),
-    ("/", r"\/"),
-    (" ", r"\s"),
-    ("|", r"\p"),
-    ("\a", r"\a"),
-    ("\b", r"\b"),
-    ("\f", r"\f"),
-    ("\n", r"\n"),
-    ("\r", r"\r"),
-    ("\t", r"\t"),
-    ("\v", r"\v"),
-)
-
-
-def escape(input_str: str) -> str:
-    """Escapes characters that need escaping according to ESCAPE_MAP"""
-    for char, replacement in ESCAPE_MAP:
-        input_str = input_str.replace(char, replacement)
-    return input_str
-
-
-def unescape(input_str: str) -> str:
-    """Undo escaping of characters according to ESCAPE_MAP"""
-    for replacement, char in reversed(ESCAPE_MAP):
-        input_str = input_str.replace(char, replacement)
-    return input_str
```

### Comparing `tsbot-1.0.0/tsbot.egg-info/PKG-INFO` & `tsbot-1.1.0/tsbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tsbot
-Version: 1.0.0
+Version: 1.1.0
 Summary: Asynchronous framework to build TeamSpeak 3 Server Query bots
 Author: 0x4aK
 Project-URL: repository, https://github.com/0x4aK/tsbot
 Project-URL: documentation, https://tsbot.readthedocs.io/en/latest/
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `tsbot-1.0.0/tsbot.egg-info/SOURCES.txt` & `tsbot-1.1.0/tsbot.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 LICENSE
 README.md
 pyproject.toml
 tests/test_connection.py
+tests/test_encoders.py
 tests/test_exceptions.py
+tests/test_parsers.py
 tests/test_query_builder.py
 tests/test_ratelimiter.py
 tests/test_response.py
-tests/test_utils.py
 tsbot/__init__.py
 tsbot/bot.py
 tsbot/connection.py
 tsbot/context.py
+tsbot/encoders.py
 tsbot/enums.py
 tsbot/exceptions.py
+tsbot/parsers.py
 tsbot/plugin.py
 tsbot/py.typed
-tsbot/query_builder.py
 tsbot/ratelimiter.py
 tsbot/response.py
 tsbot/utils.py
 tsbot.egg-info/PKG-INFO
 tsbot.egg-info/SOURCES.txt
 tsbot.egg-info/dependency_links.txt
 tsbot.egg-info/requires.txt
 tsbot.egg-info/top_level.txt
 tsbot/commands/__init__.py
+tsbot/commands/command.py
 tsbot/commands/handler.py
-tsbot/commands/tscommand.py
 tsbot/default_plugins/__init__.py
 tsbot/default_plugins/help.py
 tsbot/default_plugins/keepalive.py
 tsbot/events/__init__.py
+tsbot/events/event.py
+tsbot/events/event_handler.py
 tsbot/events/handler.py
-tsbot/events/tsevent.py
-tsbot/events/tsevent_handler.py
+tsbot/query_builder/__init__.py
+tsbot/query_builder/builder.py
+tsbot/query_builder/commands.py
 tsbot/tasks/__init__.py
 tsbot/tasks/handler.py
-tsbot/tasks/tstask.py
+tsbot/tasks/task.py
```

