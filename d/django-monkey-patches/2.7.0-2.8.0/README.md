# Comparing `tmp/django_monkey_patches-2.7.0.tar.gz` & `tmp/django_monkey_patches-2.8.0.tar.gz`

## Comparing `django_monkey_patches-2.7.0.tar` & `django_monkey_patches-2.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/README_printable.md
--rwxr-xr-x   0        0        0     1646 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/build_and_checks.sh
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/build_readme.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/__init__.py
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
--rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__orm__prefetch.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set__get.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set__get_or_create.py
--rw-r--r--   0        0        0    26767 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_wrapper.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__test_case__tear_down.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/PKG-INFO
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/requires.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/top_level.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/COPYING.LESSER
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/pyproject.toml
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/README_printable.md
+-rwxr-xr-x   0        0        0     1646 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/build_and_checks.sh
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/build_readme.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/__init__.py
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
+-rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django__orm__prefetch.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django__query_set.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django__query_set__get.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django__query_set__get_or_create.py
+-rw-r--r--   0        0        0    29801 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django__query_wrapper.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django__test_case__tear_down.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches.egg-info/requires.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/src/django_monkey_patches.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/COPYING.LESSER
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 django_monkey_patches-2.8.0/PKG-INFO
```

### Comparing `django_monkey_patches-2.7.0/README_printable.md` & `django_monkey_patches-2.8.0/README_printable.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/build_and_checks.sh` & `django_monkey_patches-2.8.0/build_and_checks.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/build_readme.sh` & `django_monkey_patches-2.8.0/build_readme.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django__base_cache__make_cache_key.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django__base_cache__make_cache_key.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django__orm__prefetch.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django__orm__prefetch.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django__query_set.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set__get.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django__query_set__get.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set__get_or_create.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django__query_set__get_or_create.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_wrapper.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django__query_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -252,27 +252,105 @@
         if "site-packages/" not in line
     ]
 
 
 get_light_call_stack_v1.field_name = "light_call_stack_v1"
 
 
+def get_managed_list(manager):
+    """
+    Smaller with auto-completion:
+    get_managed_list(manager)
+    [] if manager is None else manager.list()
+    """
+    if manager is None:
+        return []
+    return manager.list()
+
+
+def get_managed_dict(manager):
+    """
+    Smaller with auto-completion:
+    get_managed_dict(manager)
+    [] if manager is None else manager.dict()
+    """
+    if manager is None:
+        return []
+    return manager.dict()
+
+
+# Unfortunately, there is no "inline" function or macro in Python.
+# Another strange fact, C has inline functions,
+# but no keyword to inline only at some spot.
+# And sometimes, you know where is the spot
+# where it MUST-epsilon be inlined.
+# In theory, the compiler is supposed to know better than you...
+# Search for examples.
+# Of course, you can add assembly in C code instead.
+# Much more convenient.
+# Or you can use ORDER or CHAOS C "macros engines",
+# and recently Zig, but I would prefer more keywords
+# and less limited base macro rules for C,
+# instead of learning something totally new.
+# There may be more advantages to Zig that I don't see,
+# since I only read news about it.
+# And there is Rust with partial memory-safety.
+# But since I almost never do multi-threaded code,
+# I'm more looking at C and languages enabling very fast code,
+# than more safe code.
+# https://github.com/google/comprehensive-rust/issues
+# Something disappeared : I have no "issue",
+# but I still have some memory and a brain and a shiny armor
+# and a sword in the hands of God:
+# Let's hope it is just my tongue
+# to tell the Truth in the name of Jesus.
+# Let's hope I shall use my tongue more frequently aligned/adjusted
+# with God's intention. I have no pretention of perfection.
+# fn main() {
+#   for x in 1..5 {
+#     println!("x: {x}");
+#   }
+#   let bla = [1, 2, 3, 4, 5];
+#   // La bonne excuse,
+#   // c'est l'indécidabilité du problème de l'arrêt
+#   // (cf. le film Didier, certains ne savent pas s'arrêter),
+#   // style Collatz conjecture,
+#   // c'est clair qu'on fait ce genre de blagues
+#   // dans le code tout le temps...
+#   // Non mais sérieux... 99 % du code,
+#   // il doit y avoir des règles simples
+#   // pour ne pas avoir à gérer de problème indécidable...
+#   // Enfin, ce n'est que mon avis.
+#   // Mais je ne bosse pas trop sur des compilateurs ;
+#   // peut-être que c'est un peu plus au niveau méta
+#   // qu'il y a des trucs "amusants" sur le plan scientifique,
+#   // et encore ce n'est pas une certitude.
+#
+#   for elem in 1..10 {
+#     let truc = bla[elem];
+#     println!("elem: {truc}");
+#   }
+# }
+
+
 # pylint: disable-next=too-many-arguments
 def get_extra_data_template_for_set_of_queries_v1(
     query_fields=None,
     min_seconds_threshold=0,
     max_seconds_threshold=float("inf"),
     filter_callback=None,
     insertion_callback=None,
     subsets_extra_data=None,
     allocated_subsets_extra_data=None,
     allocated_subsets_key_callback=None,
     allocated_subsets_init_callback=None,
     top_down_post_processing_callback=None,
     bottom_up_post_processing_callback=None,
+    # You may need that with django-rq or other multiprocesses code:
+    manager=None,
 ):
     """
     Obtain a default extra_data_dict with most of
     the interesting "fields" regarding DB queries analysis.
     If you see something that may be interesting to add here,
     with a good example of why you need it, please,
     submit an issue on my GitHub repository.
@@ -285,54 +363,55 @@
     Basically, I think that if you use your own additional "fields"
     and your own callbacks to fill/use the "fields" below,
     you have no obligation at all.
     But it would be nice to contribute anyway.
     """
 
     if query_fields is None:
-        query_fields = []
+        query_fields = get_managed_list(manager)
     if subsets_extra_data is None:
-        subsets_extra_data = {}
+        subsets_extra_data = get_managed_dict(manager)
     if allocated_subsets_extra_data is None:
-        allocated_subsets_extra_data = {}
+        allocated_subsets_extra_data = get_managed_dict(manager)
     if allocated_subsets_key_callback is None:
-        allocated_subsets_key_callback = {}
+        allocated_subsets_key_callback = get_managed_dict(manager)
     if allocated_subsets_init_callback is None:
-        allocated_subsets_init_callback = {}
+        allocated_subsets_init_callback = get_managed_dict(manager)
 
-    return {
+    result = get_managed_dict(manager)
+    result_content = {
         "query_count": 0,
         "query_fields": query_fields,  # [
         #     "execute",
         #     "sql",
         #     "params",
         #     "many",
         #     "context",
         #     "call_stack",
         #     "start_time",
         #     "result",
         #     "end_time",
         #     "duration",
         #     get_full_query_v1,  # This is a function
         # ],
-        "query_list": [
-            # {
-            #     "execute": None,
-            #     "sql": None,
-            #     "params": None,
-            #     "many": None,
-            #     "context": None,
-            #     "call_stack": None,
-            #     "start_time": None,
-            #     "result": None,
-            #     "end_time": None,
-            #     "duration": None,
-            #     "full_query_v1": None,
-            # },
-        ],
+        "query_list": get_managed_list(manager),  # [
+        # {
+        #     "execute": None,
+        #     "sql": None,
+        #     "params": None,
+        #     "many": None,
+        #     "context": None,
+        #     "call_stack": None,
+        #     "start_time": None,
+        #     "result": None,
+        #     "end_time": None,
+        #     "duration": None,
+        #     "full_query_v1": None,
+        # },
+        # ],
         "total_duration": 0,
         "average_duration": 0,
         "min_duration": float("inf"),
         "max_duration": 0,
         # ------------------------------------------------------------
         # These fields could be at the top,
         # but it would be less didactic I think.
@@ -399,35 +478,43 @@
         # you should rewrite the top-down one.
         # Thus, you can do things in the order that pleases you,
         # recurse when you want, etc.,
         # and you can add flags in the dicts
         # to avoid multi-post-processings
         # on recursed dicts.
         # But clearly, in most cases,
-        # the bottom-up post processing makes more sense.
+        # the bottom-up post-processing makes more sense.
         # (Think sorting sub-results, etc.)
     }
+    result.update(result_content)
+    return result
 
 
-def init_connections_extra_data_v1():
+def init_connections_extra_data_v1(manager=None):
     """
     You should call this function or a custom one
     before using the custom query wrapper.
     """
 
     connections.django_monkey_patches_dict = (
-        get_extra_data_template_for_set_of_queries_v1()
+        get_extra_data_template_for_set_of_queries_v1(manager=manager)
+    )
+    connections.django_monkey_patches_stash_stack = get_managed_list(
+        manager
     )
-    connections.django_monkey_patches_stash_stack = []
     for connection_key in connections:
         connection = connections[connection_key]
         connection.django_monkey_patches_dict = (
-            get_extra_data_template_for_set_of_queries_v1()
+            get_extra_data_template_for_set_of_queries_v1(
+                manager=manager
+            )
+        )
+        connection.django_monkey_patches_stash_stack = (
+            get_managed_list(manager)
         )
-        connection.django_monkey_patches_stash_stack = []
 
 
 # pylint: disable-next=too-many-arguments
 def insert_in_connections_extra_data_v1(
     execute,
     sql,
     params,
```

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django__test_case__tear_down.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django__test_case__tear_down.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django_rest_framework__field__get_request.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django_rest_framework__field__get_request.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py` & `django_monkey_patches-2.8.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/PKG-INFO` & `django_monkey_patches-2.8.0/src/django_monkey_patches.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/SOURCES.txt` & `django_monkey_patches-2.8.0/src/django_monkey_patches.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/COPYING` & `django_monkey_patches-2.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/COPYING.LESSER` & `django_monkey_patches-2.8.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/README.md` & `django_monkey_patches-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.7.0/pyproject.toml` & `django_monkey_patches-2.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-monkey-patches"
-version = "2.7.0"
+version = "2.8.0"
 description = """\
 Add monkey-patches to correct and enhance your favorite framework\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
```

### Comparing `django_monkey_patches-2.7.0/PKG-INFO` & `django_monkey_patches-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-monkey-patches
-Version: 2.7.0
+Version: 2.8.0
 Summary: Add monkey-patches to correct and enhance your favorite framework
 Project-URL: Homepage, https://github.com/LLyaudet/django-monkey-patches
 Project-URL: Bug Tracker, https://github.com/LLyaudet/django-monkey-patches/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

