# Comparing `tmp/evg-2.7.0.tar.gz` & `tmp/evg-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evg-2.7.0.tar", last modified: Thu Apr 11 09:14:50 2024, max compression
+gzip compressed data, was "evg-2.7.1.tar", last modified: Fri Apr 19 21:40:22 2024, max compression
```

## Comparing `evg-2.7.0.tar` & `evg-2.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 09:14:50.562546 evg-2.7.0/
--rw-rw-rw-   0        0        0     2147 2024-04-11 09:14:50.562546 evg-2.7.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 09:14:50.551527 evg-2.7.0/evg/
--rw-rw-rw-   0        0        0     1518 2023-02-03 11:35:46.000000 evg-2.7.0/evg/__init__.py
--rw-rw-rw-   0        0        0     3684 2024-04-11 08:43:13.000000 evg-2.7.0/evg/core.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:14:50.561549 evg-2.7.0/evg.egg-info/
--rw-rw-rw-   0        0        0     2147 2024-04-11 09:14:50.000000 evg-2.7.0/evg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2024-04-11 09:14:50.000000 evg-2.7.0/evg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 09:14:50.000000 evg-2.7.0/evg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-11 09:14:50.000000 evg-2.7.0/evg.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2024-04-11 09:14:50.000000 evg-2.7.0/evg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 09:14:50.563545 evg-2.7.0/setup.cfg
--rw-rw-rw-   0        0        0      517 2024-04-11 09:13:53.000000 evg-2.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:40:22.996633 evg-2.7.1/
+-rw-rw-rw-   0        0        0     2133 2024-04-19 21:40:22.995357 evg-2.7.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 21:40:22.984867 evg-2.7.1/evg/
+-rw-rw-rw-   0        0        0     1518 2023-02-03 11:35:46.000000 evg-2.7.1/evg/__init__.py
+-rw-rw-rw-   0        0        0     3665 2024-04-19 21:37:37.000000 evg-2.7.1/evg/core.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:40:22.995357 evg-2.7.1/evg.egg-info/
+-rw-rw-rw-   0        0        0     2133 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2024-04-19 21:40:22.000000 evg-2.7.1/evg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 21:40:22.996633 evg-2.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      517 2024-04-19 21:21:19.000000 evg-2.7.1/setup.py
```

### Comparing `evg-2.7.0/PKG-INFO` & `evg-2.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evg
-Version: 2.7.0
+Version: 2.7.1
 Summary: Discord translator & translation of Discord functions/interactions
 Home-page: https://github.com/IceOne-i/evg
 Author: Nikita Belan
 Author-email: nikitabelan9@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -54,19 +54,19 @@
 OR
 ```python
 import evg
 from nextcord import Interaction, PartialInteractionMessage
 
 async def hi(ctx: Interaction) -> PartialInteractionMessage:
     _ = evg.MSG(ctx.locale).msg
-    return await ctx.send(content=(_("hello2")).format(name="Nikita"))
+    return await ctx.send(content=(_("hello2", name="Nikita")))
 
 async def hi2(ctx: Interaction) -> PartialInteractionMessage:
     _ = evg.MSG(ctx.locale).msg
-    return await ctx.send(content=(_("hello3")).format("Bob"))
+    return await ctx.send(content=(_("hello3", "Bob")))
 ```
 <b>Output text</b>: 
 * Hello Nikita!
 * Hello Bob!
 
 ### Change settings
 #### Default language
```

### Comparing `evg-2.7.0/evg/__init__.py` & `evg-2.7.1/evg/__init__.py`

 * *Files identical despite different names*

### Comparing `evg-2.7.0/evg/core.py` & `evg-2.7.1/evg/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,13 +119,12 @@
             return answer
 
     def msg(self, msg: str, default: str = None, random: bool = True, *args, **kwargs):
         language: dict = languages[self.language]
         answer = language.get(msg)
         if answer is None:
             if default is not None:
-                return default
+                answer = default
             else:
-                return languages[default_language].get(msg, default_text)
-        else:
-            answer = self.__list_or_str(answer=answer, random=random)
-            return answer.format(*args, **kwargs)
+                answer = languages[default_language].get(msg, default_text)
+        answer = self.__list_or_str(answer=answer, random=random).format(*args, **kwargs)
+        return answer
```

### Comparing `evg-2.7.0/evg.egg-info/PKG-INFO` & `evg-2.7.1/evg.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evg
-Version: 2.7.0
+Version: 2.7.1
 Summary: Discord translator & translation of Discord functions/interactions
 Home-page: https://github.com/IceOne-i/evg
 Author: Nikita Belan
 Author-email: nikitabelan9@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -54,19 +54,19 @@
 OR
 ```python
 import evg
 from nextcord import Interaction, PartialInteractionMessage
 
 async def hi(ctx: Interaction) -> PartialInteractionMessage:
     _ = evg.MSG(ctx.locale).msg
-    return await ctx.send(content=(_("hello2")).format(name="Nikita"))
+    return await ctx.send(content=(_("hello2", name="Nikita")))
 
 async def hi2(ctx: Interaction) -> PartialInteractionMessage:
     _ = evg.MSG(ctx.locale).msg
-    return await ctx.send(content=(_("hello3")).format("Bob"))
+    return await ctx.send(content=(_("hello3", "Bob")))
 ```
 <b>Output text</b>: 
 * Hello Nikita!
 * Hello Bob!
 
 ### Change settings
 #### Default language
```

### Comparing `evg-2.7.0/setup.py` & `evg-2.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("../README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='evg',
-      version='2.7.0',
+      version='2.7.1',
       url='https://github.com/IceOne-i/evg',
       license='MIT',
       author='Nikita Belan',
       author_email='nikitabelan9@gmail.com',
       description='Discord translator & translation of Discord functions/interactions',
       long_description=long_description,
       long_description_content_type="text/markdown",
```

