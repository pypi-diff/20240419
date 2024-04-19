# Comparing `tmp/pyjvc-4.4.3.tar.gz` & `tmp/pyjvc-4.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjvc-4.4.3.tar", last modified: Tue Apr  9 00:31:39 2024, max compression
+gzip compressed data, was "pyjvc-4.4.4.tar", last modified: Fri Apr 19 14:59:38 2024, max compression
```

## Comparing `pyjvc-4.4.3.tar` & `pyjvc-4.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-09 00:31:39.183811 pyjvc-4.4.3/
--rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.3/LICENSE
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-09 00:31:39.183601 pyjvc-4.4.3/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.3/README.md
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-09 00:31:39.180739 pyjvc-4.4.3/jvc_projector/
--rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.3/jvc_projector/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)    10106 2024-04-08 21:43:07.000000 pyjvc-4.4.3/jvc_projector/command_runner.py
--rw-r--r--   0 ilan       (501) staff       (20)    10031 2024-04-08 21:43:07.000000 pyjvc-4.4.3/jvc_projector/commands.py
--rw-r--r--   0 ilan       (501) staff       (20)      250 2024-04-08 21:43:07.000000 pyjvc-4.4.3/jvc_projector/error_classes.py
--rw-r--r--   0 ilan       (501) staff       (20)    18018 2024-04-08 22:18:12.000000 pyjvc-4.4.3/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-09 00:31:39.183254 pyjvc-4.4.3/pyJVC.egg-info/
--rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-09 00:31:39.000000 pyjvc-4.4.3/pyJVC.egg-info/PKG-INFO
--rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-09 00:31:39.000000 pyjvc-4.4.3/pyJVC.egg-info/SOURCES.txt
--rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-09 00:31:39.000000 pyjvc-4.4.3/pyJVC.egg-info/dependency_links.txt
--rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-09 00:31:39.000000 pyjvc-4.4.3/pyJVC.egg-info/top_level.txt
--rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-09 00:31:39.183860 pyjvc-4.4.3/setup.cfg
--rw-r--r--   0 ilan       (501) staff       (20)      634 2024-04-08 22:18:50.000000 pyjvc-4.4.3/setup.py
-drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-09 00:31:39.182804 pyjvc-4.4.3/tests/
--rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.3/tests/__init__.py
--rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.3/tests/test_commander.py
--rw-r--r--   0 ilan       (501) staff       (20)     8923 2024-04-08 21:43:07.000000 pyjvc-4.4.3/tests/test_coordinator.py
--rw-r--r--   0 ilan       (501) staff       (20)    20373 2024-04-08 21:43:07.000000 pyjvc-4.4.3/tests/test_loop.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 14:59:38.801500 pyjvc-4.4.4/
+-rw-r--r--   0 ilan       (501) staff       (20)     1074 2023-06-01 23:44:00.000000 pyjvc-4.4.4/LICENSE
+-rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-19 14:59:38.801312 pyjvc-4.4.4/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)     5769 2024-02-18 15:27:26.000000 pyjvc-4.4.4/README.md
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 14:59:38.798757 pyjvc-4.4.4/jvc_projector/
+-rw-r--r--   0 ilan       (501) staff       (20)      151 2024-02-16 01:57:22.000000 pyjvc-4.4.4/jvc_projector/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)    10329 2024-04-19 14:59:00.000000 pyjvc-4.4.4/jvc_projector/command_runner.py
+-rw-r--r--   0 ilan       (501) staff       (20)    10031 2024-04-08 21:43:07.000000 pyjvc-4.4.4/jvc_projector/commands.py
+-rw-r--r--   0 ilan       (501) staff       (20)      250 2024-04-08 21:43:07.000000 pyjvc-4.4.4/jvc_projector/error_classes.py
+-rw-r--r--   0 ilan       (501) staff       (20)    18249 2024-04-19 14:50:45.000000 pyjvc-4.4.4/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 14:59:38.801109 pyjvc-4.4.4/pyJVC.egg-info/
+-rw-r--r--   0 ilan       (501) staff       (20)     6181 2024-04-19 14:59:38.000000 pyjvc-4.4.4/pyJVC.egg-info/PKG-INFO
+-rw-r--r--   0 ilan       (501) staff       (20)      491 2024-04-19 14:59:38.000000 pyjvc-4.4.4/pyJVC.egg-info/SOURCES.txt
+-rw-r--r--   0 ilan       (501) staff       (20)        1 2024-04-19 14:59:38.000000 pyjvc-4.4.4/pyJVC.egg-info/dependency_links.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       20 2024-04-19 14:59:38.000000 pyjvc-4.4.4/pyJVC.egg-info/top_level.txt
+-rw-r--r--   0 ilan       (501) staff       (20)       38 2024-04-19 14:59:38.801542 pyjvc-4.4.4/setup.cfg
+-rw-r--r--   0 ilan       (501) staff       (20)      634 2024-04-19 14:59:34.000000 pyjvc-4.4.4/setup.py
+drwxr-xr-x   0 ilan       (501) staff       (20)        0 2024-04-19 14:59:38.800769 pyjvc-4.4.4/tests/
+-rw-r--r--   0 ilan       (501) staff       (20)        0 2024-02-17 16:27:53.000000 pyjvc-4.4.4/tests/__init__.py
+-rw-r--r--   0 ilan       (501) staff       (20)     2337 2024-03-20 01:40:47.000000 pyjvc-4.4.4/tests/test_commander.py
+-rw-r--r--   0 ilan       (501) staff       (20)     8923 2024-04-08 21:43:07.000000 pyjvc-4.4.4/tests/test_coordinator.py
+-rw-r--r--   0 ilan       (501) staff       (20)    20373 2024-04-08 21:43:07.000000 pyjvc-4.4.4/tests/test_loop.py
```

### Comparing `pyjvc-4.4.3/LICENSE` & `pyjvc-4.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.3/PKG-INFO` & `pyjvc-4.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.3
+Version: 4.4.4
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.3/README.md` & `pyjvc-4.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.3/jvc_projector/command_runner.py` & `pyjvc-4.4.4/jvc_projector/command_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,14 @@
         self,
         send_command: Union[list[str], str],
         command_type: bytes = b"!",
         ack: bytes = None,
     ):
         pass
 
-    # TODO: must catch broken pipe
-    # TODO: support remote
     async def send_command(self, command: str, command_type: bytes) -> str:
         """
         Sends a command with a flag to expect an ack.
 
         The PJ API returns nothing if a command is in flight
         or if a command is not successful
 
@@ -114,14 +112,17 @@
                 data = await asyncio.wait_for(self.reader.read(1024), timeout=0.5)
                 if not data:
                     # If no data is received, the buffer is empty
                     break
             except asyncio.TimeoutError:
                 # If a timeout occurs, assume the buffer is empty and break the loop
                 break
+            except BrokenPipeError:
+                # If a broken pipe error occurs, the connection is closed
+                raise ConnectionClosedError("Broken pipe")
             except Exception as e:
                 # Handle any other exceptions that may occur during reading
                 self.logger.error("Error while clearing read buffer: %s", e)
                 break
 
     async def _do_command(
         self,
@@ -158,15 +159,17 @@
             # an ack, followed by the actual message. Check to see if the ack sent by
             # projector is correct, then return the message.
 
             # if the command_type is operation, the ack doesnt matter we should read until empty
             # read until empty
             if command_type == Header.operation.value:
                 self.logger.debug("command_type is operation skipping ack check")
-                return await self.read_until_empty()
+                await self.read_until_empty()
+                # return ok to indicate the command was sent otherwise it will think it failed
+                return "ok"
 
             ack_value = (
                 Header.ack.value + Header.pj_unit.value + ack + Footer.close.value
             )
             self.logger.debug("constructed ack_value: %s", ack_value)
 
             # Receive the acknowledgement from PJ
```

### Comparing `pyjvc-4.4.3/jvc_projector/commands.py` & `pyjvc-4.4.4/jvc_projector/commands.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.3/jvc_projector/jvc_projector.py` & `pyjvc-4.4.4/jvc_projector/jvc_projector.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,23 +154,28 @@
         self.logger.debug("Model result is %s", model_res)
 
         return model_map.get(model_res[-4:], "Unsupported")
 
     async def reset_everything(self) -> None:
         """
         resets everything and tries to empty current jvc buffer. Used on error to just clear everything and start over
+
+        Raises ConnectionClosedError
         """
         try:
             if not self.connection_open:
                 await self.open_connection()
 
             # clear the buffer
             await self.commander.read_until_empty()
 
             return
+        except ConnectionClosedError as e:
+            self.logger.error("Error resetting everything: %s", e)
+            raise
         except Exception as e:
             self.logger.error("Error resetting everything: %s", e)
             return
 
     async def open_connection(self) -> bool:
         """Open a connection to the projector asynchronously"""
         # If the connection is already open, return True
@@ -241,14 +246,15 @@
             self.logger.debug(
                 "exec_command Executing command: %s - %s", command, command_type
             )
             retries = 0
             while retries < 3:
                 try:
                     res = await self.commander.send_command(command, command_type)
+                    self.logger.debug("Command result: %s", res)
                     if not res:
                         self.logger.debug("Command failed. Retrying")
                         retries += 1
                         continue
                     return res
                 # this means stuff is actually broken
                 except (
```

### Comparing `pyjvc-4.4.3/pyJVC.egg-info/PKG-INFO` & `pyjvc-4.4.4/pyJVC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjvc
-Version: 4.4.3
+Version: 4.4.4
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea2
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `pyjvc-4.4.3/setup.py` & `pyjvc-4.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyjvc",
-    version="4.4.3",
+    version="4.4.4",
     author="iloveicedgreentea2",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `pyjvc-4.4.3/tests/test_commander.py` & `pyjvc-4.4.4/tests/test_commander.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.3/tests/test_coordinator.py` & `pyjvc-4.4.4/tests/test_coordinator.py`

 * *Files identical despite different names*

### Comparing `pyjvc-4.4.3/tests/test_loop.py` & `pyjvc-4.4.4/tests/test_loop.py`

 * *Files identical despite different names*

