# Comparing `tmp/django_includecontents-0.4.tar.gz` & `tmp/django_includecontents-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.4.tar", last modified: Thu Apr 18 04:25:32 2024, max compression
+gzip compressed data, was "django_includecontents-0.4.1.tar", last modified: Fri Apr 19 04:29:28 2024, max compression
```

## Comparing `django_includecontents-0.4.tar` & `django_includecontents-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4998 2024-04-18 04:23:29.581817 django_includecontents-0.4/README.md
--rw-r--r--   0        0        0     1218 2024-04-18 04:25:32.355405 django_includecontents-0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 01:37:55.796699 django_includecontents-0.4/src/djangox/__init__.py
--rw-r--r--   0        0        0      144 2024-04-09 04:42:05.196722 django_includecontents-0.4/tests/settings.py
--rw-r--r--   0        0        0      168 2024-04-18 02:43:29.856564 django_includecontents-0.4/tests/templates/components/card.html
--rw-r--r--   0        0        0      160 2024-04-18 03:09:23.179458 django_includecontents-0.4/tests/templates/components/card_extend.html
--rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.4/tests/templates/multiline.html
--rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.4/tests/templates/test_component/attrs.html
--rw-r--r--   0        0        0      162 2024-04-18 03:24:57.041361 django_includecontents-0.4/tests/templates/test_component/extend_class.html
--rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.4/tests/templates/test_component/index.html
--rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.4/tests/templates/test_component/missing_attr.html
--rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.4/tests/templates/test_component/missing_closing_tag.html
--rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.4/tests/templates/test_tag/basic.html
--rw-r--r--   0        0        0       57 2024-04-09 04:52:09.297567 django_includecontents-0.4/tests/templates/test_tag/inner.html
--rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.4/tests/templates/test_tag/with_attr.html
--rw-r--r--   0        0        0     1478 2024-04-18 04:13:01.650516 django_includecontents-0.4/tests/test_component.py
--rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.4/tests/test_multiline.py
--rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.4/tests/test_tag.py
--rw-r--r--   0        0        0     6012 1970-01-01 00:00:00.000000 django_includecontents-0.4/PKG-INFO
+-rw-r--r--   0        0        0     5293 2024-04-19 04:27:39.460145 django_includecontents-0.4.1/README.md
+-rw-r--r--   0        0        0     1220 2024-04-19 04:29:28.260370 django_includecontents-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 01:37:55.796699 django_includecontents-0.4.1/src/djangox/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-09 04:42:05.196722 django_includecontents-0.4.1/tests/settings.py
+-rw-r--r--   0        0        0      168 2024-04-18 05:37:15.283141 django_includecontents-0.4.1/tests/templates/components/card.html
+-rw-r--r--   0        0        0      160 2024-04-18 05:37:15.283141 django_includecontents-0.4.1/tests/templates/components/card_extend.html
+-rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.4.1/tests/templates/multiline.html
+-rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.4.1/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0      162 2024-04-18 05:37:15.283141 django_includecontents-0.4.1/tests/templates/test_component/extend_class.html
+-rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.4.1/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.4.1/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.4.1/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.4.1/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0       57 2024-04-09 04:52:09.297567 django_includecontents-0.4.1/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.4.1/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0     1478 2024-04-18 05:37:15.283141 django_includecontents-0.4.1/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.4.1/tests/test_multiline.py
+-rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.4.1/tests/test_tag.py
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 django_includecontents-0.4.1/PKG-INFO
```

### Comparing `django_includecontents-0.4/README.md` & `django_includecontents-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ```
 
 To use the custom template engine, replace the default `DjangoTemplates` backend in your settings:
 
 ```python
 TEMPLATES = [
     {
-        'BACKEND': 'includecontents.backends.Templates',
+        'BACKEND': 'includecontents.backend.Templates',
         ...
     },
 ]
 ```
 
 This engine also adds `includecontents` to the built-in tags so there is no need to load it.
 
@@ -131,15 +131,15 @@
 <include:card title="Hello">
   <p>World</p>
 </include:card>
 ```
 
 You can use named [`{% contents %}` blocks](#named-contents-blocks), just like with the `includecontents` tag.
 
-Some HTML formatters (like prettier) insist on quoting HTML attribute values, you can avoid this by wrapping template values in `{}`:
+Some HTML formatters (like prettier) insist on quoting HTML attribute values, you can avoid this by optionally wrapping template values in `{}`:
 
 ```html
 <include:card title={mytitle}></include:card>
 ``` 
 
 ### Component Props
 
@@ -194,7 +194,21 @@
 ```jinja
 {# props large=False #}
 
 {% attrs class="lg" %}     {# sets class attribute to "lg" but can be overridden #}
 {% attrs class:lg %}       {# always adds 'lg' class #}
 {% attrs class:lg=large %} {# adds 'lg' class if large prop is truthy #}
 ```
+
+You can use this same conditional format on the template tag / component itself too:
+
+```html
+<include:card title="Hello" class:lg={is_large}>
+  <p>World</p>
+</include:card>
+```
+
+```jinja
+{% includecontents "hello.html" class:lg=is_large %}
+  <p>World</p>
+{% endincludecontents %}
+```
```

### Comparing `django_includecontents-0.4/pyproject.toml` & `django_includecontents-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-includecontents"
-version = "0.4"
+version = "0.4.1"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django",
 ]
```

### Comparing `django_includecontents-0.4/tests/test_component.py` & `django_includecontents-0.4.1/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `django_includecontents-0.4/PKG-INFO` & `django_includecontents-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-includecontents
-Version: 0.4
+Version: 0.4.1
 Summary: Django includecontents component-like tag
 Author-Email: Chris Beaven <smileychris@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -66,15 +66,15 @@
 ```
 
 To use the custom template engine, replace the default `DjangoTemplates` backend in your settings:
 
 ```python
 TEMPLATES = [
     {
-        'BACKEND': 'includecontents.backends.Templates',
+        'BACKEND': 'includecontents.backend.Templates',
         ...
     },
 ]
 ```
 
 This engine also adds `includecontents` to the built-in tags so there is no need to load it.
 
@@ -157,15 +157,15 @@
 <include:card title="Hello">
   <p>World</p>
 </include:card>
 ```
 
 You can use named [`{% contents %}` blocks](#named-contents-blocks), just like with the `includecontents` tag.
 
-Some HTML formatters (like prettier) insist on quoting HTML attribute values, you can avoid this by wrapping template values in `{}`:
+Some HTML formatters (like prettier) insist on quoting HTML attribute values, you can avoid this by optionally wrapping template values in `{}`:
 
 ```html
 <include:card title={mytitle}></include:card>
 ``` 
 
 ### Component Props
 
@@ -220,7 +220,21 @@
 ```jinja
 {# props large=False #}
 
 {% attrs class="lg" %}     {# sets class attribute to "lg" but can be overridden #}
 {% attrs class:lg %}       {# always adds 'lg' class #}
 {% attrs class:lg=large %} {# adds 'lg' class if large prop is truthy #}
 ```
+
+You can use this same conditional format on the template tag / component itself too:
+
+```html
+<include:card title="Hello" class:lg={is_large}>
+  <p>World</p>
+</include:card>
+```
+
+```jinja
+{% includecontents "hello.html" class:lg=is_large %}
+  <p>World</p>
+{% endincludecontents %}
+```
```

