# Comparing `tmp/city-ch-autocomplete-0.2.tar.gz` & `tmp/city_ch_autocomplete-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "city-ch-autocomplete-0.2.tar", last modified: Thu Mar 28 20:23:30 2024, max compression
+gzip compressed data, was "city_ch_autocomplete-0.3.tar", last modified: Fri Apr 19 16:31:51 2024, max compression
```

## Comparing `city-ch-autocomplete-0.2.tar` & `city_ch_autocomplete-0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-03-28 20:23:30.777912 city-ch-autocomplete-0.2/
--rw-r--r--   0 claude    (1000) www-data    (33)     1516 2024-03-28 17:35:15.000000 city-ch-autocomplete-0.2/LICENSE
--rw-r--r--   0 claude    (1000) www-data    (33)       48 2024-03-28 17:08:28.000000 city-ch-autocomplete-0.2/MANIFEST.in
--rw-r--r--   0 claude    (1000) www-data    (33)     2956 2024-03-28 20:23:30.777912 city-ch-autocomplete-0.2/PKG-INFO
--rw-r--r--   0 claude    (1000) www-data    (33)     1892 2024-03-28 19:23:16.000000 city-ch-autocomplete-0.2/README.rst
-drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-03-28 20:23:30.773913 city-ch-autocomplete-0.2/city_ch_autocomplete/
--rw-r--r--   0 claude    (1000) www-data    (33)      148 2024-03-28 16:25:10.000000 city-ch-autocomplete-0.2/city_ch_autocomplete/apps.py
--rw-r--r--   0 claude    (1000) www-data    (33)     3549 2024-03-28 19:55:42.000000 city-ch-autocomplete-0.2/city_ch_autocomplete/forms.py
-drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-03-28 20:23:30.773913 city-ch-autocomplete-0.2/city_ch_autocomplete/migrations/
--rw-r--r--   0 claude    (1000) www-data    (33)      781 2024-03-28 17:51:40.000000 city-ch-autocomplete-0.2/city_ch_autocomplete/migrations/0001_initial.py
--rw-r--r--   0 claude    (1000) www-data    (33)        0 2024-03-28 18:01:29.000000 city-ch-autocomplete-0.2/city_ch_autocomplete/migrations/__init__.py
--rw-r--r--   0 claude    (1000) www-data    (33)      906 2024-03-28 17:49:35.000000 city-ch-autocomplete-0.2/city_ch_autocomplete/models.py
-drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-03-28 20:23:30.777912 city-ch-autocomplete-0.2/city_ch_autocomplete/static/
--rw-r--r--   0 claude    (1000) www-data    (33)     6377 2024-03-28 19:54:12.000000 city-ch-autocomplete-0.2/city_ch_autocomplete/static/city_ch_autocomplete.js
--rw-r--r--   0 claude    (1000) www-data    (33)      189 2024-03-28 17:06:56.000000 city-ch-autocomplete-0.2/city_ch_autocomplete/urls.py
--rw-r--r--   0 claude    (1000) www-data    (33)     2847 2024-03-28 19:23:16.000000 city-ch-autocomplete-0.2/city_ch_autocomplete/views.py
-drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-03-28 20:23:30.777912 city-ch-autocomplete-0.2/city_ch_autocomplete.egg-info/
--rw-r--r--   0 claude    (1000) www-data    (33)     2956 2024-03-28 20:23:30.000000 city-ch-autocomplete-0.2/city_ch_autocomplete.egg-info/PKG-INFO
--rw-r--r--   0 claude    (1000) www-data    (33)      557 2024-03-28 20:23:30.000000 city-ch-autocomplete-0.2/city_ch_autocomplete.egg-info/SOURCES.txt
--rw-r--r--   0 claude    (1000) www-data    (33)        1 2024-03-28 20:23:30.000000 city-ch-autocomplete-0.2/city_ch_autocomplete.egg-info/dependency_links.txt
--rw-r--r--   0 claude    (1000) www-data    (33)       18 2024-03-28 20:23:30.000000 city-ch-autocomplete-0.2/city_ch_autocomplete.egg-info/requires.txt
--rw-r--r--   0 claude    (1000) www-data    (33)       21 2024-03-28 20:23:30.000000 city-ch-autocomplete-0.2/city_ch_autocomplete.egg-info/top_level.txt
--rw-r--r--   0 claude    (1000) www-data    (33)     1101 2024-03-28 20:23:12.000000 city-ch-autocomplete-0.2/pyproject.toml
--rw-r--r--   0 claude    (1000) www-data    (33)       38 2024-03-28 20:23:30.777912 city-ch-autocomplete-0.2/setup.cfg
+drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-04-19 16:31:51.386256 city_ch_autocomplete-0.3/
+-rw-r--r--   0 claude    (1000) www-data    (33)     1516 2024-03-28 17:35:15.000000 city_ch_autocomplete-0.3/LICENSE
+-rw-r--r--   0 claude    (1000) www-data    (33)       48 2024-03-28 17:08:28.000000 city_ch_autocomplete-0.3/MANIFEST.in
+-rw-r--r--   0 claude    (1000) www-data    (33)     3036 2024-04-19 16:31:51.386256 city_ch_autocomplete-0.3/PKG-INFO
+-rw-r--r--   0 claude    (1000) www-data    (33)     1972 2024-04-19 16:28:37.000000 city_ch_autocomplete-0.3/README.rst
+drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-04-19 16:31:51.382256 city_ch_autocomplete-0.3/city_ch_autocomplete/
+-rw-r--r--   0 claude    (1000) www-data    (33)      148 2024-04-19 16:28:32.000000 city_ch_autocomplete-0.3/city_ch_autocomplete/apps.py
+-rw-r--r--   0 claude    (1000) www-data    (33)     3566 2024-04-19 16:28:37.000000 city_ch_autocomplete-0.3/city_ch_autocomplete/forms.py
+drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-04-19 16:31:51.386256 city_ch_autocomplete-0.3/city_ch_autocomplete/migrations/
+-rw-r--r--   0 claude    (1000) www-data    (33)      781 2024-03-28 17:51:40.000000 city_ch_autocomplete-0.3/city_ch_autocomplete/migrations/0001_initial.py
+-rw-r--r--   0 claude    (1000) www-data    (33)        0 2024-03-28 18:01:29.000000 city_ch_autocomplete-0.3/city_ch_autocomplete/migrations/__init__.py
+-rw-r--r--   0 claude    (1000) www-data    (33)      906 2024-03-28 17:49:35.000000 city_ch_autocomplete-0.3/city_ch_autocomplete/models.py
+drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-04-19 16:31:51.386256 city_ch_autocomplete-0.3/city_ch_autocomplete/static/
+-rw-r--r--   0 claude    (1000) www-data    (33)     6377 2024-03-28 19:54:12.000000 city_ch_autocomplete-0.3/city_ch_autocomplete/static/city_ch_autocomplete.js
+-rw-r--r--   0 claude    (1000) www-data    (33)      189 2024-03-28 17:06:56.000000 city_ch_autocomplete-0.3/city_ch_autocomplete/urls.py
+-rw-r--r--   0 claude    (1000) www-data    (33)     2847 2024-03-28 19:23:16.000000 city_ch_autocomplete-0.3/city_ch_autocomplete/views.py
+drwxr-sr-x   0 claude    (1000) www-data    (33)        0 2024-04-19 16:31:51.386256 city_ch_autocomplete-0.3/city_ch_autocomplete.egg-info/
+-rw-r--r--   0 claude    (1000) www-data    (33)     3036 2024-04-19 16:31:51.000000 city_ch_autocomplete-0.3/city_ch_autocomplete.egg-info/PKG-INFO
+-rw-r--r--   0 claude    (1000) www-data    (33)      557 2024-04-19 16:31:51.000000 city_ch_autocomplete-0.3/city_ch_autocomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 claude    (1000) www-data    (33)        1 2024-04-19 16:31:51.000000 city_ch_autocomplete-0.3/city_ch_autocomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 claude    (1000) www-data    (33)       18 2024-04-19 16:31:51.000000 city_ch_autocomplete-0.3/city_ch_autocomplete.egg-info/requires.txt
+-rw-r--r--   0 claude    (1000) www-data    (33)       21 2024-04-19 16:31:51.000000 city_ch_autocomplete-0.3/city_ch_autocomplete.egg-info/top_level.txt
+-rw-r--r--   0 claude    (1000) www-data    (33)     1101 2024-04-19 16:29:28.000000 city_ch_autocomplete-0.3/pyproject.toml
+-rw-r--r--   0 claude    (1000) www-data    (33)       38 2024-04-19 16:31:51.386256 city_ch_autocomplete-0.3/setup.cfg
```

### Comparing `city-ch-autocomplete-0.2/LICENSE` & `city_ch_autocomplete-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `city-ch-autocomplete-0.2/PKG-INFO` & `city_ch_autocomplete-0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: city-ch-autocomplete
-Version: 0.2
+Version: 0.3
 Summary: A Django app to query the Swiss Post API for postcodes and localities.
 Author-email: Claude Paroz <claude@2xlibre.net>
 Project-URL: Homepage, https://codeberg.org/claudep/city_ch_autocomplete
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -55,25 +55,25 @@
    https://developer.apis.post.ch/ui/home). Note the process can take some
    time.
    Then add the POST_API_USER and POST_API_PASSWORD settings to your project.
 
    Optionally you can get the data from a CSV and put it in a database table.
    Read below for more details.
 
-3. In the target form(s) of your project, add the `CityCHMixin` to your
+3. In the target form(s) of your project, add the `CityChMixin` to your
    form inheritance and a `CityChField` as a form field::
 
-    from city_ch_autocomplete.forms import CityCHField, CityCHMixin
+    from city_ch_autocomplete.forms import CityChField, CityChMixin
 
-    class YourForm(CityCHMixin, forms.ModelForm):
+    class YourForm(CityChMixin, forms.ModelForm):
         class Meta:
-            fields = [..., 'plz', 'ort', ...]
-        city_auto = CityCHField(...)
-        postal_code_model_field = 'plz'
-        city_model_field = 'ort'
+            fields = [..., '<my_postcode_model_field>', '<my_city_model_field>', ...]
+        city_auto = CityChField(...)
+        postal_code_model_field = '<my_postcode_model_field>'
+        city_model_field = '<my_city_model_field>'
 
    Don't forget to include `{{ form.media }}` in the templates where you are using
    the form.
 
 Searching from the database
 ---------------------------
```

### Comparing `city-ch-autocomplete-0.2/README.rst` & `city_ch_autocomplete-0.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -29,25 +29,25 @@
    https://developer.apis.post.ch/ui/home). Note the process can take some
    time.
    Then add the POST_API_USER and POST_API_PASSWORD settings to your project.
 
    Optionally you can get the data from a CSV and put it in a database table.
    Read below for more details.
 
-3. In the target form(s) of your project, add the `CityCHMixin` to your
+3. In the target form(s) of your project, add the `CityChMixin` to your
    form inheritance and a `CityChField` as a form field::
 
-    from city_ch_autocomplete.forms import CityCHField, CityCHMixin
+    from city_ch_autocomplete.forms import CityChField, CityChMixin
 
-    class YourForm(CityCHMixin, forms.ModelForm):
+    class YourForm(CityChMixin, forms.ModelForm):
         class Meta:
-            fields = [..., 'plz', 'ort', ...]
-        city_auto = CityCHField(...)
-        postal_code_model_field = 'plz'
-        city_model_field = 'ort'
+            fields = [..., '<my_postcode_model_field>', '<my_city_model_field>', ...]
+        city_auto = CityChField(...)
+        postal_code_model_field = '<my_postcode_model_field>'
+        city_model_field = '<my_city_model_field>'
 
    Don't forget to include `{{ form.media }}` in the templates where you are using
    the form.
 
 Searching from the database
 ---------------------------
```

### Comparing `city-ch-autocomplete-0.2/city_ch_autocomplete/forms.py` & `city_ch_autocomplete-0.3/city_ch_autocomplete/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         if not self.label:
             self.label = _("NPA Localité")
 
     def clean(self, value):
-        return str(value)
+        return str(value) if value else ""
 
 
 class CityChMixin:
     """
     Applied to forms having a CityChField, to split postal_code/city in
     two parts.
     """
```

### Comparing `city-ch-autocomplete-0.2/city_ch_autocomplete/migrations/0001_initial.py` & `city_ch_autocomplete-0.3/city_ch_autocomplete/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `city-ch-autocomplete-0.2/city_ch_autocomplete/models.py` & `city_ch_autocomplete-0.3/city_ch_autocomplete/models.py`

 * *Files identical despite different names*

### Comparing `city-ch-autocomplete-0.2/city_ch_autocomplete/static/city_ch_autocomplete.js` & `city_ch_autocomplete-0.3/city_ch_autocomplete/static/city_ch_autocomplete.js`

 * *Files identical despite different names*

### Comparing `city-ch-autocomplete-0.2/city_ch_autocomplete/views.py` & `city_ch_autocomplete-0.3/city_ch_autocomplete/views.py`

 * *Files identical despite different names*

### Comparing `city-ch-autocomplete-0.2/city_ch_autocomplete.egg-info/PKG-INFO` & `city_ch_autocomplete-0.3/city_ch_autocomplete.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: city-ch-autocomplete
-Version: 0.2
+Version: 0.3
 Summary: A Django app to query the Swiss Post API for postcodes and localities.
 Author-email: Claude Paroz <claude@2xlibre.net>
 Project-URL: Homepage, https://codeberg.org/claudep/city_ch_autocomplete
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -55,25 +55,25 @@
    https://developer.apis.post.ch/ui/home). Note the process can take some
    time.
    Then add the POST_API_USER and POST_API_PASSWORD settings to your project.
 
    Optionally you can get the data from a CSV and put it in a database table.
    Read below for more details.
 
-3. In the target form(s) of your project, add the `CityCHMixin` to your
+3. In the target form(s) of your project, add the `CityChMixin` to your
    form inheritance and a `CityChField` as a form field::
 
-    from city_ch_autocomplete.forms import CityCHField, CityCHMixin
+    from city_ch_autocomplete.forms import CityChField, CityChMixin
 
-    class YourForm(CityCHMixin, forms.ModelForm):
+    class YourForm(CityChMixin, forms.ModelForm):
         class Meta:
-            fields = [..., 'plz', 'ort', ...]
-        city_auto = CityCHField(...)
-        postal_code_model_field = 'plz'
-        city_model_field = 'ort'
+            fields = [..., '<my_postcode_model_field>', '<my_city_model_field>', ...]
+        city_auto = CityChField(...)
+        postal_code_model_field = '<my_postcode_model_field>'
+        city_model_field = '<my_city_model_field>'
 
    Don't forget to include `{{ form.media }}` in the templates where you are using
    the form.
 
 Searching from the database
 ---------------------------
```

### Comparing `city-ch-autocomplete-0.2/city_ch_autocomplete.egg-info/SOURCES.txt` & `city_ch_autocomplete-0.3/city_ch_autocomplete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `city-ch-autocomplete-0.2/pyproject.toml` & `city_ch_autocomplete-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "city-ch-autocomplete"
-version = "0.2"
+version = "0.3"
 dependencies = [
     "httpx",
     "django>=4.2",
 ]
 description = "A Django app to query the Swiss Post API for postcodes and localities."
 readme = "README.rst"
 requires-python = ">= 3.9"
```

