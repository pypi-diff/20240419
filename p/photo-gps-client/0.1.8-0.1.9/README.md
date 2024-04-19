# Comparing `tmp/photo_gps_client-0.1.8.tar.gz` & `tmp/photo_gps_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photo_gps_client-0.1.8.tar", max compression
+gzip compressed data, was "photo_gps_client-0.1.9.tar", max compression
```

## Comparing `photo_gps_client-0.1.8.tar` & `photo_gps_client-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       86 2024-04-17 18:35:03.061611 photo_gps_client-0.1.8/README.md
--rw-r--r--   0        0        0      532 2024-04-17 16:36:49.817402 photo_gps_client-0.1.8/photo_gps/DSCF0311.xmp
--rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.8/photo_gps/DSCF0312.xmp
--rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.8/photo_gps/DSCF0313.xmp
--rw-r--r--   0        0        0        0 2024-04-13 11:43:05.727802 photo_gps_client-0.1.8/photo_gps/__init__.py
--rw-r--r--   0        0        0     2711 2024-04-17 17:05:22.779144 photo_gps_client-0.1.8/photo_gps/commands.py
--rw-r--r--   0        0        0     1272 2024-04-17 17:00:45.203444 photo_gps_client-0.1.8/photo_gps/config.py
--rw-r--r--   0        0        0      551 2024-04-17 18:51:53.580694 photo_gps_client-0.1.8/photo_gps/jinja/xmp.jinja
--rw-r--r--   0        0        0      327 2024-04-17 16:51:39.780517 photo_gps_client-0.1.8/photo_gps/photogps.example.yaml
--rw-r--r--   0        0        0     1112 2024-04-17 17:01:24.642844 photo_gps_client-0.1.8/photo_gps/photogps.py
--rw-r--r--   0        0        0     2982 2024-04-17 19:11:35.852798 photo_gps_client-0.1.8/photo_gps/tools.py
--rw-r--r--   0        0        0      686 2024-04-17 19:11:48.322441 photo_gps_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 photo_gps_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       86 2024-04-17 18:35:03.061611 photo_gps_client-0.1.9/README.md
+-rw-r--r--   0        0        0      532 2024-04-17 16:36:49.817402 photo_gps_client-0.1.9/photo_gps/DSCF0311.xmp
+-rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.9/photo_gps/DSCF0312.xmp
+-rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.9/photo_gps/DSCF0313.xmp
+-rw-r--r--   0        0        0        0 2024-04-13 11:43:05.727802 photo_gps_client-0.1.9/photo_gps/__init__.py
+-rw-r--r--   0        0        0     2711 2024-04-17 17:05:22.779144 photo_gps_client-0.1.9/photo_gps/commands.py
+-rw-r--r--   0        0        0     1272 2024-04-17 17:00:45.203444 photo_gps_client-0.1.9/photo_gps/config.py
+-rw-r--r--   0        0        0      551 2024-04-17 18:51:53.580694 photo_gps_client-0.1.9/photo_gps/jinja/xmp.jinja
+-rw-r--r--   0        0        0      327 2024-04-17 16:51:39.780517 photo_gps_client-0.1.9/photo_gps/photogps.example.yaml
+-rw-r--r--   0        0        0     1112 2024-04-17 17:01:24.642844 photo_gps_client-0.1.9/photo_gps/photogps.py
+-rw-r--r--   0        0        0     3184 2024-04-17 19:18:12.897456 photo_gps_client-0.1.9/photo_gps/tools.py
+-rw-r--r--   0        0        0      686 2024-04-18 08:24:51.208417 photo_gps_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 photo_gps_client-0.1.9/PKG-INFO
```

### Comparing `photo_gps_client-0.1.8/photo_gps/DSCF0311.xmp` & `photo_gps_client-0.1.9/photo_gps/DSCF0311.xmp`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.8/photo_gps/DSCF0312.xmp` & `photo_gps_client-0.1.9/photo_gps/DSCF0312.xmp`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.8/photo_gps/DSCF0313.xmp` & `photo_gps_client-0.1.9/photo_gps/DSCF0313.xmp`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.8/photo_gps/commands.py` & `photo_gps_client-0.1.9/photo_gps/commands.py`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.8/photo_gps/config.py` & `photo_gps_client-0.1.9/photo_gps/config.py`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.8/photo_gps/jinja/xmp.jinja` & `photo_gps_client-0.1.9/photo_gps/jinja/xmp.jinja`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.8/photo_gps/photogps.py` & `photo_gps_client-0.1.9/photo_gps/photogps.py`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.8/photo_gps/tools.py` & `photo_gps_client-0.1.9/photo_gps/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,39 @@
 
     # Конвертация объекта Arrow в Unix timestamp
     unix_timestamp = arrow_obj.int_timestamp
 
     return unix_timestamp
 
 
-def deg_to_dms(deg, lat_or_lon):
+def deg_to_ddm(deg, lat_or_lon):
     letter = ''
     if lat_or_lon == 'lat':
         letter = 'N' if deg > 0 else 'S'
     elif lat_or_lon == 'lon':
         letter = 'E' if deg > 0 else 'W'
     deg = abs(deg)
     d = int(deg)
     md = abs(deg - d) * 60
     return f"{d},{round(md, 5)}{letter}"  # Формат: "d,mm.mmmmmX"
-    # а это для формата "d,m,sX"
-    # m = int(md)
-    # sd = round((md - m) * 60, 2)
-    # return f"{d},{m},{sd}{letter}"
+
+
+def deg_to_dms(deg, lat_or_lon):
+    letter = ''
+    if lat_or_lon == 'lat':
+        letter = 'N' if deg > 0 else 'S'
+    elif lat_or_lon == 'lon':
+        letter = 'E' if deg > 0 else 'W'
+    deg = abs(deg)
+    d = int(deg)
+    md = abs(deg - d) * 60
+    m = int(md)
+    sd = round((md - m) * 60, 2)
+    return f"{d},{m},{sd}{letter}"
+
 
 def get_all_meta(img: Path) -> dict:
     with ExifToolHelper() as et:
         meta = et.get_tags(str(img), [])
         return meta[0]
 
 
@@ -73,15 +84,15 @@
 
 def create_xmp(img: Path, lat: float, lon: float, alt: int):
     env = Environment(
         loader=PackageLoader('photo_gps', 'jinja'),
         autoescape=select_autoescape(['xml'])
     )
     tpl = env.get_template('xmp.jinja')
-    file_content = tpl.render(lat=deg_to_dms(lat, 'lat'), lon=deg_to_dms(lon, 'lon'), alt=alt)
+    file_content = tpl.render(lat=deg_to_ddm(lat, 'lat'), lon=deg_to_ddm(lon, 'lon'), alt=alt)
     xmp_file = img.with_suffix('.xmp')
     with open(xmp_file, 'w') as f:
         f.write(file_content)
 
 
 def set_author(img: Path, name: str):
     with ExifToolHelper() as et:
```

### Comparing `photo_gps_client-0.1.8/pyproject.toml` & `photo_gps_client-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "photo-gps-client"
-version = "0.1.8"  # set by antonio-py-dynamic-version
+version = "0.1.9"  # set by antonio-py-dynamic-version
 description = ""
 authors = ["antonio <mr.antonsilin@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "photo_gps"},
 ]
```

### Comparing `photo_gps_client-0.1.8/PKG-INFO` & `photo_gps_client-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photo-gps-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: antonio
 Author-email: mr.antonsilin@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.3.0,<2.0.0)
```

