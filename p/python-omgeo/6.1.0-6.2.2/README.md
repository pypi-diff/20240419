# Comparing `tmp/python-omgeo-6.1.0.tar.gz` & `tmp/python_omgeo-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-omgeo-6.1.0.tar", last modified: Tue Jul 20 19:17:26 2021, max compression
+gzip compressed data, was "python_omgeo-6.2.2.tar", last modified: Fri Apr 19 15:56:14 2024, max compression
```

## Comparing `python-omgeo-6.1.0.tar` & `python_omgeo-6.2.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 19:17:26.651056 python-omgeo-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     6842 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6842 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-07-20 19:17:26.651056 python-omgeo-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 19:17:26.647056 python-omgeo-6.1.0/omgeo/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6310 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/geocoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     9674 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/places.py
--rw-r--r--   0 runner    (1001) docker     (121)    23023 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (121)    12131 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 19:17:26.647056 python-omgeo-6.1.0/omgeo/services/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8725 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/services/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4903 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/services/bing.py
--rw-r--r--   0 runner    (1001) docker     (121)    11020 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/services/esri.py
--rw-r--r--   0 runner    (1001) docker     (121)     4072 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/services/google.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/services/mapquest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/services/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/services/pelias.py
--rw-r--r--   0 runner    (1001) docker     (121)     3347 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/services/us_census.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 19:17:26.647056 python-omgeo-6.1.0/omgeo/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    35310 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/omgeo/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 19:17:26.651056 python-omgeo-6.1.0/python_omgeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2021-07-20 19:17:26.000000 python-omgeo-6.1.0/python_omgeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      690 2021-07-20 19:17:26.000000 python-omgeo-6.1.0/python_omgeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-20 19:17:26.000000 python-omgeo-6.1.0/python_omgeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-07-20 19:17:26.000000 python-omgeo-6.1.0/python_omgeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-07-20 19:17:26.000000 python-omgeo-6.1.0/python_omgeo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-07-20 19:17:26.651056 python-omgeo-6.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      981 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      318 2021-07-20 19:17:18.000000 python-omgeo-6.1.0/test.dummy.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:56:14.860789 python_omgeo-6.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-19 15:56:14.860789 python_omgeo-6.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:56:14.856789 python_omgeo-6.2.2/omgeo/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/geocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/places.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23023 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:56:14.856789 python_omgeo-6.2.2/omgeo/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/services/bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/services/esri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/services/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/services/mapquest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/services/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/services/pelias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/services/us_census.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:56:14.856789 python_omgeo-6.2.2/omgeo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35886 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/omgeo/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:56:14.860789 python_omgeo-6.2.2/python_omgeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-19 15:56:14.000000 python_omgeo-6.2.2/python_omgeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-19 15:56:14.000000 python_omgeo-6.2.2/python_omgeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:56:14.000000 python_omgeo-6.2.2/python_omgeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 15:56:14.000000 python_omgeo-6.2.2/python_omgeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 15:56:14.000000 python_omgeo-6.2.2/python_omgeo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-19 15:56:14.860789 python_omgeo-6.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      981 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      318 2024-04-19 15:56:07.000000 python_omgeo-6.2.2/test.dummy.sh
```

### Comparing `python-omgeo-6.1.0/CHANGES.rst` & `python_omgeo-6.2.2/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -224,7 +224,18 @@
  * Fix template string error in AttrListIncludes and AttrListExcludes __repr__
 
 v6.1.0, 2021-07-20
 ------------------
  * Populate match_region using RegionAbbr rather than Region from EsriWGS. For
    example, when using the EsriWGS geocoder, expect 'PA' rather than
    'Pennsylvania' in match_region.
+
+v6.2.0, 2024-01-22
+------------------
+ * Fix /findAddressCandidates calls for EsriWGS when using magicKey. They
+   previously would provide an internal Loc_name field in the response which
+   is no longer supplied, which broke the API. Making that field optional in
+   our code fixes this.
+
+v6.2.1, 2024-04-15
+------------------
+ * Update PyPI publishing integration
```

### Comparing `python-omgeo-6.1.0/CHANGES.txt` & `python_omgeo-6.2.2/CHANGES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -224,7 +224,18 @@
  * Fix template string error in AttrListIncludes and AttrListExcludes __repr__
 
 v6.1.0, 2021-07-20
 ------------------
  * Populate match_region using RegionAbbr rather than Region from EsriWGS. For
    example, when using the EsriWGS geocoder, expect 'PA' rather than
    'Pennsylvania' in match_region.
+
+v6.2.0, 2024-01-22
+------------------
+ * Fix /findAddressCandidates calls for EsriWGS when using magicKey. They
+   previously would provide an internal Loc_name field in the response which
+   is no longer supplied, which broke the API. Making that field optional in
+   our code fixes this.
+
+v6.2.1, 2024-04-15
+------------------
+ * Update PyPI publishing integration
```

### Comparing `python-omgeo-6.1.0/LICENSE.txt` & `python_omgeo-6.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/README.rst` & `python_omgeo-6.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/README.txt` & `python_omgeo-6.2.2/README.txt`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/geocoder.py` & `python_omgeo-6.2.2/omgeo/geocoder.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/places.py` & `python_omgeo-6.2.2/omgeo/places.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/postprocessors.py` & `python_omgeo-6.2.2/omgeo/postprocessors.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/preprocessors.py` & `python_omgeo-6.2.2/omgeo/preprocessors.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/processor.py` & `python_omgeo-6.2.2/omgeo/processor.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/services/base.py` & `python_omgeo-6.2.2/omgeo/services/base.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/services/bing.py` & `python_omgeo-6.2.2/omgeo/services/bing.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/services/esri.py` & `python_omgeo-6.2.2/omgeo/services/esri.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,23 @@
     }
 
     DEFAULT_PREPROCESSORS = [CancelIfPOBox()]
 
     DEFAULT_POSTPROCESSORS = [
         AttrFilter(['PointAddress',
                     'StreetAddress',
+                    'Locality',
                     # 'PostalExt',
                     # 'Postal'
                     ],
                    'locator_type'),
         # AttrExclude(['USA_Postal'], 'locator'), #accept postal from everywhere but US (need PostalExt)
         AttrSorter(['PointAddress',
                     'StreetAddress',
+                    'Locality',
                     # 'PostalExt',
                     # 'Postal'
                     ],
                    'locator_type'),
         AttrRename('locator', LOCATOR_MAP),  # after filter to avoid searching things we toss out
         UseHighScoreIfAtLeast(99.8),
         ScoreSorter(),
@@ -191,30 +193,31 @@
         returned_candidates = []  # this will be the list returned
         try:
             locations = response_obj['candidates']
             for location in locations:
                 c = Candidate()
                 attributes = location['attributes']
                 c.match_addr = attributes['Match_addr']
-                c.locator = attributes['Loc_name']
+                c.locator = attributes.get('Loc_name', '')
                 c.locator_type = attributes['Addr_type']
                 c.score = attributes['Score']
                 c.x = attributes['DisplayX']  # represents the actual location of the address.
                 c.y = attributes['DisplayY']
                 c.wkid = response_obj['spatialReference']['wkid']
                 c.geoservice = self.__class__.__name__
 
                 # Optional address component fields.
                 for in_key, out_key in [('City', 'match_city'), ('Subregion', 'match_subregion'),
                                         ('RegionAbbr', 'match_region'), ('Postal', 'match_postal'),
                                         ('Country', 'match_country')]:
                     setattr(c, out_key, attributes.get(in_key, ''))
                 setattr(c, 'match_streetaddr', self._street_addr_from_response(attributes))
                 returned_candidates.append(c)
-        except KeyError:
+        except KeyError as e:
+            logger.warning('Missing key: ' + e)
             pass
         return returned_candidates
 
     def _street_addr_from_response(self, attributes):
         """Construct a street address (no city, region, etc.) from a geocoder response.
 
         :param attributes: A dict of address attributes as returned by the Esri geocoder.
```

### Comparing `python-omgeo-6.1.0/omgeo/services/google.py` & `python_omgeo-6.2.2/omgeo/services/google.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/services/mapquest.py` & `python_omgeo-6.2.2/omgeo/services/mapquest.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/services/nominatim.py` & `python_omgeo-6.2.2/omgeo/services/nominatim.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/services/pelias.py` & `python_omgeo-6.2.2/omgeo/services/pelias.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/services/us_census.py` & `python_omgeo-6.2.2/omgeo/services/us_census.py`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/omgeo/tests/tests.py` & `python_omgeo-6.2.2/omgeo/tests/tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,28 +175,28 @@
     def test_geocode_esri_wgs_senado_mx(self):
         """
         Attempt to geocode ``Paseo de la Reforma 135, Tabacalera,
         Cuauhtémoc, Distrito Federal, 06030``.
         """
         candidates = self.g_esri_wgs.get_candidates(self.pq['senado_mx'])
         self.assertOneCandidate(candidates)
-        search_text = 'Paseo de la Reforma 135'
+        search_text = 'Paseo de La Reforma 135'
         self.assertEqual(search_text in candidates[0].match_addr, True,
                          '"%s" not found in match_addr. Got "%s".'
                          % (search_text, candidates[0].match_addr))
 
     def test_geocode_structured_esri_wgs_senado_mx(self):
         """
         Attempt to geocode ``Paseo de la Reforma 135, Tabacalera,
         Cuauhtémoc, Distrito Federal, 06030`` using a structured query to
         EsriWGS.
         """
         candidates = self.g_esri_wgs.get_candidates(self.pq['senado_mx_struct'])
         self.assertOneCandidate(candidates)
-        search_text = 'Paseo de la Reforma 135'
+        search_text = 'Paseo de La Reforma 135'
         self.assertEqual(search_text in candidates[0].match_addr, True,
                          '"%s" not found in match_addr. Got "%s".'
                          % (search_text, candidates[0].match_addr))
 
     def test_geocode_esri_wgs_340_12th_bounded(self):
         """
         Trying to geocode ``340 12th St, Philadelphia PA`` would normally return results
@@ -204,14 +204,24 @@
         we should only get the former.
         """
         candidates = self.g_esri_wgs.get_candidates(self.pq['bounded_340_12th'])
         self.assertOneCandidate(candidates)
         self.assertEqual('340 N 12th' in candidates[0].match_addr, True,
                          '"340 N 12th" not found in match_addr. Got "%s"' % candidates[0].match_addr)
 
+    def test_geocode_esri_wgs_magicKey(self):
+        """Check that geocoding New York, USA with a magicKey returns one result."""
+        esri = self.g_esri_wgs._sources[0]
+        suggestions = esri._get_json_obj(
+            f'{esri._endpoint}/suggest',
+            {'f': 'json', 'text': 'New York, USA'})['suggestions']
+        pq = PlaceQuery(suggestions[0]['text'], key=suggestions[0]['magicKey'])
+        candidates = self.g_esri_wgs.get_candidates(pq)
+        self.assertOneCandidate(candidates)
+
     def test_geocode_esri_wgs_zip_plus_4(self):
         """Check that geocoding 19127-1112 returns one result."""
         candidates = self.g_esri_wgs_postal_ok.get_candidates(self.pq['zip_plus_4_in_postal_plus_country'])
         self.assertOneCandidate(candidates)
 
     def test_geocode_esri_wgs_multipart(self):
         """Check that geocoding multipart address returns one result."""
@@ -225,14 +235,15 @@
         self.assertOneCandidate(candidates)
 
     def test_esri_short_region(self):
         """Ensure that Esri uses region abbreviations"""
         candidate = self.g_esri_wgs.get_candidates(self.pq["azavea"])[0]
         self.assertEqual(candidate.match_region, "PA")
 
+    @unittest.skipIf(GOOGLE_API_KEY is None, GOOGLE_KEY_REQUIRED_MSG)
     def test_google_short_region(self):
         """Ensure that Google uses region abbreviations"""
         candidate = self.g_google.get_candidates(self.pq["azavea"])[0]
         self.assertEqual(candidate.match_region, "PA")
 
     @unittest.skipIf(BING_MAPS_API_KEY is None, BING_KEY_REQUIRED_MSG)
     def test_geocode_bing(self):
@@ -268,16 +279,16 @@
         x_type = type(candidates[0].x)
         y_type = type(candidates[0].y)
         self.assertEqual(x_type == float, True, 'x coord is of type %s instead of float' % x_type)
         self.assertEqual(y_type == float, True, 'y coord is of type %s instead of float' % y_type)
         self.assertEqual(len(candidates) > 0, True, 'No candidates returned.')
 
     def test_geocode_census(self):
-        """Test Azavea's address using US Census geocoder."""
-        candidates = self.g_census.get_candidates(PlaceQuery('1200 Callowhill St, Philadelphia, PA'))
+        """Test Element 84's address using US Census geocoder."""
+        candidates = self.g_census.get_candidates(PlaceQuery('210 N. Lee Street, Alexandria, VA'))
         self.assertEqual(len(candidates) > 0, True, 'No candidates returned.')
 
     def test_EsriWGS_address_components(self):
         """Make sure EsriWGS returns address components"""
         candidate = self.g_esri_wgs.get_candidates(self.pq['azavea'])[0]
         self._test_address_components(candidate)
```

### Comparing `python-omgeo-6.1.0/python_omgeo.egg-info/SOURCES.txt` & `python_omgeo-6.2.2/python_omgeo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-omgeo-6.1.0/setup.py` & `python_omgeo-6.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="python-omgeo",
-    version="6.1.0",
+    version="6.2.2",
     description="Geocoding Library using ESRI, Google, Bing Maps, US Census, OpenStreetMap, Pelias, and MapQuest geocoders",
     author="Azavea, Inc.",
     author_email="info@azavea.com",
     url="http://github.com/azavea/python-omgeo",
     license="MIT",
     long_description=read('README.rst'),
     packages=find_packages(),
```

