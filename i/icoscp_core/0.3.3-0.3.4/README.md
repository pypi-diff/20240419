# Comparing `tmp/icoscp_core-0.3.3.tar.gz` & `tmp/icoscp_core-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icoscp_core-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "icoscp_core-0.3.4.tar", last modified: Fri Apr 19 16:15:32 2024, max compression
```

## Comparing `icoscp_core-0.3.3.tar` & `icoscp_core-0.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    32422 2024-01-09 12:40:09.457716 icoscp_core-0.3.3/LICENSE
--rw-r--r--   0        0        0    14721 2024-03-20 14:38:49.993564 icoscp_core-0.3.3/README.md
--rw-r--r--   0        0        0      882 2024-03-18 13:03:42.014172 icoscp_core-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      189 2024-03-20 14:38:49.993564 icoscp_core-0.3.3/src/icoscp_core/__init__.py
--rw-r--r--   0        0        0     5902 2024-03-20 14:38:49.993564 icoscp_core-0.3.3/src/icoscp_core/auth.py
--rw-r--r--   0        0        0     1294 2024-03-18 13:03:42.014172 icoscp_core-0.3.3/src/icoscp_core/bootstrap.py
--rw-r--r--   0        0        0      501 2024-01-09 12:47:07.450659 icoscp_core-0.3.3/src/icoscp_core/cities.py
--rw-r--r--   0        0        0    11700 2024-01-09 12:47:07.450659 icoscp_core-0.3.3/src/icoscp_core/cpb.py
--rw-r--r--   0        0        0     7835 2024-03-18 13:03:42.014172 icoscp_core-0.3.3/src/icoscp_core/dataclient.py
--rw-r--r--   0        0        0     1687 2024-01-09 12:40:09.457716 icoscp_core-0.3.3/src/icoscp_core/envri.py
--rw-r--r--   0        0        0     1107 2024-03-20 14:38:49.993564 icoscp_core-0.3.3/src/icoscp_core/geofeaturemeta.py
--rw-r--r--   0        0        0      959 2024-01-09 12:47:07.454659 icoscp_core-0.3.3/src/icoscp_core/http.py
--rw-r--r--   0        0        0     1173 2024-03-18 13:03:42.014172 icoscp_core-0.3.3/src/icoscp_core/icos.py
--rw-r--r--   0        0        0     8980 2024-03-20 14:38:49.993564 icoscp_core-0.3.3/src/icoscp_core/metaclient.py
--rw-r--r--   0        0        0     9873 2024-01-12 12:54:16.643899 icoscp_core-0.3.3/src/icoscp_core/metacore.py
--rw-r--r--   0        0        0      882 2024-01-09 12:47:07.454659 icoscp_core-0.3.3/src/icoscp_core/portaluse_client.py
--rw-r--r--   0        0        0        0 2024-03-18 13:03:42.014172 icoscp_core-0.3.3/src/icoscp_core/py.typed
--rw-r--r--   0        0        0     3092 2024-01-09 12:47:07.454659 icoscp_core-0.3.3/src/icoscp_core/queries/cpbmeta.py
--rw-r--r--   0        0        0     6695 2024-03-20 14:38:49.993564 icoscp_core-0.3.3/src/icoscp_core/queries/dataobjlist.py
--rw-r--r--   0        0        0        0 2024-03-18 13:03:42.014172 icoscp_core-0.3.3/src/icoscp_core/queries/py.typed
--rw-r--r--   0        0        0     2080 2024-01-09 12:40:09.461716 icoscp_core-0.3.3/src/icoscp_core/queries/speclist.py
--rw-r--r--   0        0        0     2362 2024-03-18 13:03:42.014172 icoscp_core-0.3.3/src/icoscp_core/queries/stationlist.py
--rw-r--r--   0        0        0      683 2024-01-09 12:40:09.461716 icoscp_core-0.3.3/src/icoscp_core/rolemeta.py
--rw-r--r--   0        0        0      151 2024-01-09 12:40:09.461716 icoscp_core-0.3.3/src/icoscp_core/sites.py
--rw-r--r--   0        0        0     3840 2024-01-09 12:47:07.454659 icoscp_core-0.3.3/src/icoscp_core/sparql.py
--rw-r--r--   0        0        0    15328 1970-01-01 00:00:00.000000 icoscp_core-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-10-02 15:11:40.615198 icoscp_core-0.3.4/LICENSE
+-rw-r--r--   0        0        0    14721 2024-04-12 13:30:14.477215 icoscp_core-0.3.4/README.md
+-rw-r--r--   0        0        0      882 2024-02-15 10:40:35.534185 icoscp_core-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-04-16 15:12:55.207725 icoscp_core-0.3.4/src/icoscp_core/__init__.py
+-rw-r--r--   0        0        0     5902 2024-04-12 13:30:14.477215 icoscp_core-0.3.4/src/icoscp_core/auth.py
+-rw-r--r--   0        0        0     1294 2024-03-07 15:22:23.951017 icoscp_core-0.3.4/src/icoscp_core/bootstrap.py
+-rw-r--r--   0        0        0      498 2024-04-16 15:12:55.207725 icoscp_core-0.3.4/src/icoscp_core/cities.py
+-rw-r--r--   0        0        0    11700 2024-04-12 13:30:14.477215 icoscp_core-0.3.4/src/icoscp_core/cpb.py
+-rw-r--r--   0        0        0     7905 2024-04-19 15:23:28.324880 icoscp_core-0.3.4/src/icoscp_core/dataclient.py
+-rw-r--r--   0        0        0     1687 2023-10-18 15:05:41.050187 icoscp_core-0.3.4/src/icoscp_core/envri.py
+-rw-r--r--   0        0        0     1107 2024-04-12 13:29:39.856830 icoscp_core-0.3.4/src/icoscp_core/geofeaturemeta.py
+-rw-r--r--   0        0        0      959 2024-01-16 15:17:09.077825 icoscp_core-0.3.4/src/icoscp_core/http.py
+-rw-r--r--   0        0        0     1173 2024-02-15 10:40:35.534185 icoscp_core-0.3.4/src/icoscp_core/icos.py
+-rw-r--r--   0        0        0     9029 2024-04-16 15:13:33.092114 icoscp_core-0.3.4/src/icoscp_core/metaclient.py
+-rw-r--r--   0        0        0     9873 2024-03-12 14:40:53.402515 icoscp_core-0.3.4/src/icoscp_core/metacore.py
+-rw-r--r--   0        0        0      882 2024-01-16 15:17:09.077825 icoscp_core-0.3.4/src/icoscp_core/portaluse_client.py
+-rw-r--r--   0        0        0        0 2024-02-15 10:40:35.534185 icoscp_core-0.3.4/src/icoscp_core/py.typed
+-rw-r--r--   0        0        0     3092 2024-01-16 15:11:22.170377 icoscp_core-0.3.4/src/icoscp_core/queries/cpbmeta.py
+-rw-r--r--   0        0        0     6695 2024-04-12 13:29:39.856830 icoscp_core-0.3.4/src/icoscp_core/queries/dataobjlist.py
+-rw-r--r--   0        0        0        0 2024-02-15 10:40:35.534185 icoscp_core-0.3.4/src/icoscp_core/queries/py.typed
+-rw-r--r--   0        0        0     3512 2024-04-16 14:39:30.059017 icoscp_core-0.3.4/src/icoscp_core/queries/speclist.py
+-rw-r--r--   0        0        0     2362 2024-02-15 10:40:35.534185 icoscp_core-0.3.4/src/icoscp_core/queries/stationlist.py
+-rw-r--r--   0        0        0      683 2023-10-18 15:05:41.050187 icoscp_core-0.3.4/src/icoscp_core/rolemeta.py
+-rw-r--r--   0        0        0      151 2023-10-17 11:42:31.443012 icoscp_core-0.3.4/src/icoscp_core/sites.py
+-rw-r--r--   0        0        0     3840 2024-01-16 15:17:09.077825 icoscp_core-0.3.4/src/icoscp_core/sparql.py
+-rw-r--r--   0        0        0    15328 1970-01-01 00:00:00.000000 icoscp_core-0.3.4/PKG-INFO
```

### Comparing `icoscp_core-0.3.3/LICENSE` & `icoscp_core-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/README.md` & `icoscp_core-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/pyproject.toml` & `icoscp_core-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/auth.py` & `icoscp_core-0.3.4/src/icoscp_core/auth.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/bootstrap.py` & `icoscp_core-0.3.4/src/icoscp_core/bootstrap.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/cpb.py` & `icoscp_core-0.3.4/src/icoscp_core/cpb.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 		return arr.astype('>u4').view(dtype='>U1')
 	elif fmt_str in ["iso8601date", "etcDate"]:
 		return arr.astype('>i8').view(dtype=np.dtype('>datetime64[D]'))
 	elif fmt_str == "iso8601month":
 		return (arr - 1970 * 12).astype('>i8').view(dtype=np.dtype('>datetime64[M]'))
 	elif fmt_str == "iso8601timeOfDay":
 		return arr.astype('>i8').view(dtype=np.dtype('>timedelta64[s]'))
-	elif fmt_str in ["iso8601dateTime", "iso8601LocalDateTime", "etcLocalDateTime"]:
+	elif fmt_str in ["iso8601dateTime", "isoLikeLocalDateTime", "etcLocalDateTime"]:
 		return arr.astype('>i8').view(dtype=np.dtype('>datetime64[ms]'))
 	else:
 		return arr
 
 
 _fmt_to_dtype = {
 	'INT': np.dtype('>i4'),
```

### Comparing `icoscp_core-0.3.3/src/icoscp_core/dataclient.py` & `icoscp_core-0.3.4/src/icoscp_core/dataclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 		self._meta = MetadataClient(conf)
 		self._data_folder_path = data_folder_path
 
 	@property
 	def meta(self) -> MetadataClient:
 		return self._meta
 
+	@property
+	def auth(self) -> AuthTokenProvider:
+		return self._auth
+
 	def get_file_stream(self, dobj: str | DataObjectLite) -> Tuple[str, HTTPResponse]:
 		"""
 		Fetches the original verbatim content of a data- or document
 		object. The method is HTTP-backed and requires authentication
 		if fetching data-, not document, objects.
 
 		:param dobj:
```

### Comparing `icoscp_core-0.3.3/src/icoscp_core/envri.py` & `icoscp_core-0.3.4/src/icoscp_core/envri.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/geofeaturemeta.py` & `icoscp_core-0.3.4/src/icoscp_core/geofeaturemeta.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/http.py` & `icoscp_core-0.3.4/src/icoscp_core/http.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/icos.py` & `icoscp_core-0.3.4/src/icoscp_core/icos.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/metaclient.py` & `icoscp_core-0.3.4/src/icoscp_core/metaclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,17 +127,18 @@
 		:param `station`: either a `StationLite` object (obtainable
 		from `list_stations` method), or a URI identifying a station, or
 		a list of either of the two, or `None` (default) for all
 		stations.
 
 		:param `filters`: a list of filters, each filter being either
 		`TimeFilter` for filtering by submission time, or data start- or
-		stop time, `SizeFilter` for filtering by file size, or
+		stop time, `SizeFilter` for filtering by file size,
 		`SamplingHeightFilter` for filtering by sampling height
-		(applicable only to data objects with sampling height metadata);
+		(applicable only to data objects with sampling height metadata),
+		or `GeoIntersectFilter` for geospatial filtering;
 		the list is empty by default.
 
 		:param `include_deprecated`: boolean flag to include deprecated
 		(i.e. such that have a newer version with explicit metadata
 		link) data objects in the list; `False` by default.
 
 		:param `order_by`: either `OrderByProp` --- a property to sort
```

### Comparing `icoscp_core-0.3.3/src/icoscp_core/metacore.py` & `icoscp_core-0.3.4/src/icoscp_core/metacore.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/portaluse_client.py` & `icoscp_core-0.3.4/src/icoscp_core/portaluse_client.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/queries/cpbmeta.py` & `icoscp_core-0.3.4/src/icoscp_core/queries/cpbmeta.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/queries/dataobjlist.py` & `icoscp_core-0.3.4/src/icoscp_core/queries/dataobjlist.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/queries/stationlist.py` & `icoscp_core-0.3.4/src/icoscp_core/queries/stationlist.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/rolemeta.py` & `icoscp_core-0.3.4/src/icoscp_core/rolemeta.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/src/icoscp_core/sparql.py` & `icoscp_core-0.3.4/src/icoscp_core/sparql.py`

 * *Files identical despite different names*

### Comparing `icoscp_core-0.3.3/PKG-INFO` & `icoscp_core-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icoscp_core
-Version: 0.3.3
+Version: 0.3.4
 Summary: icoscp_core
 Keywords: environment,research,infrastructure,data access
 Author-email: Oleg Mirzov <oleg.mirzov@nateko.lu.se>
 Maintainer-email: Klara Broman <klara.broman@nateko.lu.se>, Jonathan Schenk <jonathan.schenk@nateko.lu.se>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

