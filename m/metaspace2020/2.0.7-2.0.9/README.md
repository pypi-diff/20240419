# Comparing `tmp/metaspace2020-2.0.7.tar.gz` & `tmp/metaspace2020-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaspace2020-2.0.7.tar", last modified: Wed Feb  7 14:35:19 2024, max compression
+gzip compressed data, was "metaspace2020-2.0.9.tar", last modified: Fri Apr 19 14:42:44 2024, max compression
```

## Comparing `metaspace2020-2.0.7.tar` & `metaspace2020-2.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:35:19.007277 metaspace2020-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-02-07 14:35:19.007277 metaspace2020-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:35:19.007277 metaspace2020-2.0.7/metaspace/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/metaspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/metaspace/annotation_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/metaspace/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/metaspace/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    29819 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/metaspace/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/metaspace/projects_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    86527 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/metaspace/sm_annotation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/metaspace/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 14:35:19.007277 metaspace2020-2.0.7/metaspace2020.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-02-07 14:35:18.000000 metaspace2020-2.0.7/metaspace2020.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-07 14:35:18.000000 metaspace2020-2.0.7/metaspace2020.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 14:35:18.000000 metaspace2020-2.0.7/metaspace2020.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-07 14:35:18.000000 metaspace2020-2.0.7/metaspace2020.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-07 14:35:18.000000 metaspace2020-2.0.7/metaspace2020.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 14:35:19.007277 metaspace2020-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-02-07 14:35:10.000000 metaspace2020-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:42:44.516795 metaspace2020-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-19 14:42:44.516795 metaspace2020-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:42:44.516795 metaspace2020-2.0.9/metaspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/metaspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/metaspace/annotation_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/metaspace/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/metaspace/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29819 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/metaspace/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/metaspace/projects_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90336 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/metaspace/sm_annotation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/metaspace/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:42:44.516795 metaspace2020-2.0.9/metaspace2020.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-19 14:42:44.000000 metaspace2020-2.0.9/metaspace2020.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-19 14:42:44.000000 metaspace2020-2.0.9/metaspace2020.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:42:44.000000 metaspace2020-2.0.9/metaspace2020.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 14:42:44.000000 metaspace2020-2.0.9/metaspace2020.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 14:42:44.000000 metaspace2020-2.0.9/metaspace2020.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:42:44.516795 metaspace2020-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-19 14:42:35.000000 metaspace2020-2.0.9/setup.py
```

### Comparing `metaspace2020-2.0.7/LICENSE` & `metaspace2020-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metaspace2020-2.0.7/PKG-INFO` & `metaspace2020-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaspace2020
-Version: 2.0.7
+Version: 2.0.9
 Summary: Python library for connecting to the METASPACE platform
 Home-page: https://github.com/metaspace2020/metaspace/tree/master/metaspace/python-client
 Author: Alexandrov Team, EMBL
 Author-email: contact@metaspace2020.eu
 License: UNKNOWN
 Description: # METASPACE Python client
```

### Comparing `metaspace2020-2.0.7/README.md` & `metaspace2020-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `metaspace2020-2.0.7/metaspace/annotation_export.py` & `metaspace2020-2.0.9/metaspace/annotation_export.py`

 * *Files identical despite different names*

### Comparing `metaspace2020-2.0.7/metaspace/dendrogram.py` & `metaspace2020-2.0.9/metaspace/dendrogram.py`

 * *Files identical despite different names*

### Comparing `metaspace2020-2.0.7/metaspace/image_processing.py` & `metaspace2020-2.0.9/metaspace/image_processing.py`

 * *Files identical despite different names*

### Comparing `metaspace2020-2.0.7/metaspace/plotting.py` & `metaspace2020-2.0.9/metaspace/plotting.py`

 * *Files identical despite different names*

### Comparing `metaspace2020-2.0.7/metaspace/projects_client.py` & `metaspace2020-2.0.9/metaspace/projects_client.py`

 * *Files identical despite different names*

### Comparing `metaspace2020-2.0.7/metaspace/sm_annotation_utils.py` & `metaspace2020-2.0.9/metaspace/sm_annotation_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,24 +182,25 @@
                 return resp.json() if not return_headers else resp.headers
             except requests.RequestException as ex:
                 if i == max_retries:
                     raise
                 print(f'{ex}\nRetrying...')
 
     def init_multipart_upload(
-        filename, file_type, headers={}, current_user_id=None, dataset_id=None
+        filename, file_type, headers={}, current_user_id=None, dataset_id=None, size=None
     ):
         url = companion_url + '/s3/multipart'
         data = {
             'filename': filename,
             'type': file_type,
             'metadata': {
                 'name': filename,
                 'type': file_type,
                 'source': 'api',
+                'size': str(size) if size else 'not-provided',
                 'user': current_user_id if current_user_id else 'not-provided',
                 'datasetId': dataset_id if dataset_id else 'not-provided',
                 'uuid': headers['uuid'] if headers.get('uuid') else 'not-provided',
             },
         }
         resp_data = send_request(url, 'POST', json=data, headers=headers)
         return resp_data['key'], resp_data['uploadId']
@@ -268,14 +269,15 @@
                 print(f'Uploading part {part:3}/{n_parts:3} of {Path(local_path).name} file...')
                 yield part, file_data
 
     session = requests.Session()
     key, upload_id = init_multipart_upload(
         Path(local_path).name,
         file_type,
+        size=Path(local_path).stat().st_size,
         headers=headers,
         current_user_id=current_user_id,
         dataset_id=dataset_id,
     )
 
     # Python evaluates the input to ThreadPoolExecutor.map eagerly, which would allow iterate_file
     # to read parts and sign uploads even if there was a significant queue to upload_part.
@@ -482,14 +484,16 @@
         dataset { id name }
         possibleCompounds { name information { url databaseId } }
         isotopeImages { mz url minIntensity maxIntensity totalIntensity }
     """
 
     MOLECULAR_DB_FIELDS = "id name version isPublic archived default"
 
+    SCORING_MODEL_FIELDS = "id name version type isArchived"
+
     def getDataset(self, datasetId):
         query = f"""
             query datasetInfo($id: String!) {{
               dataset(id: $id) {{
                 {self.DATASET_FIELDS}
               }}
             }}
@@ -633,14 +637,19 @@
         return self.query(query, variables)
 
     def get_visible_databases(self):
         query = f"query allMolecularDBs {{ allMolecularDBs {{ {self.MOLECULAR_DB_FIELDS} }} }}"
         result = self.query(query)
         return result['allMolecularDBs']
 
+    def get_visible_scoring_models(self):
+        query = f"query scoringModels {{ scoringModels {{ {self.SCORING_MODEL_FIELDS} }} }}"
+        result = self.query(query)
+        return result['scoringModels']
+
     @staticmethod
     def map_database_name_to_name_version(name: str) -> Tuple[str, str]:
         # For backwards compatibility map old database names to (name, version) tuples
         database_name_version_map = {
             'ChEBI': ('ChEBI', '2016'),
             'LIPID_MAPS': ('LIPID_MAPS', '2016'),
             'SwissLipids': ('SwissLipids', '2016'),
@@ -654,14 +663,25 @@
             'PAMDB-v1.0': ('PAMDB', 'v1.0'),
             'SwissLipids-2018-02-02': ('SwissLipids', '2018-02-02'),
             'HMDB-v4-cotton': ('HMDB-cotton', 'v4'),
             'ECMDB-2018-12': ('ECMDB', '2018-12'),
         }
         return database_name_version_map.get(name, (None, None))
 
+    @staticmethod
+    def map_scoring_model_name_to_name_version(name: str) -> Tuple[str, str]:
+        # For backwards compatibility map old database names to (name, version) tuples
+        scoring_model_name_version_map = {
+            'MSM': ('MSM', 'v1'),
+            'Animal': ('Animal', 'v2.2023-12-14'),
+            'Plant': ('Plant', 'v2.2023-12-14'),
+            'v3_default': ('v3_default', 'v1'),
+        }
+        return scoring_model_name_version_map.get(name, (None, None))
+
     def map_database_to_id(self, database: Union[int, str, Tuple[str, str]]):
         # Forwards/backwards compatibility issue: the GraphQL Schema may soon change from Int ids
         # to ID (i.e. str-based) ids. For now, this supports both types, and passes the type on
         # without modification. When the API has settled, this should be updated to coerce to the
         # correct type, because we shouldn't burden users with having to figure out why calls are
         # failing when they pass IDs that look like integers as integers instead of strings.
         if isinstance(database, int):
@@ -687,14 +707,53 @@
                 f'{list(database_name_id_map.keys())}'
             )
         if len(database_ids) > 1:
             raise Exception(f'Database name "{database}" is not unique. Use database id instead.')
 
         return database_ids[0]
 
+    def map_scoring_model_to_id(self, scoring_model: Union[int, str, Tuple[str, str]]):
+        if isinstance(scoring_model, int):
+            return scoring_model
+
+        if isinstance(scoring_model, str) and re.match(r'^\d+$', scoring_model):
+            return int(scoring_model)
+
+        scoring_model_docs = self.get_visible_scoring_models()
+        scoring_model_name_id_map = defaultdict(list)
+        for sm in scoring_model_docs:
+            scoring_model_name_id_map[(sm['name'], sm['version'])].append(sm['id'])
+
+        if isinstance(scoring_model, tuple):
+            model_name, model_version = scoring_model
+        else:
+            model_name, model_version = self.map_scoring_model_name_to_name_version(scoring_model)
+
+        scoring_model_ids = scoring_model_name_id_map.get((model_name, model_version), [])
+        if len(scoring_model_ids) == 0:
+            default_model = next(
+                (obj for obj in scoring_model_docs if obj['type'] == 'original'), None
+            )
+            if default_model is not None:
+                print(
+                    f'Scoring model not found or you do not have access to it. Setting original MSM as default {default_model["id"]}'
+                )
+                return default_model['id']
+            else:
+                raise Exception(
+                    f'Scoring model not found or you do not have access to it. Available databases: '
+                    f'{list(scoring_model_name_id_map.keys())}'
+                )
+        if len(scoring_model_ids) > 1:
+            raise Exception(
+                f'Scoring model name "{scoring_model}" is not unique. Use scoring model id instead.'
+            )
+
+        return scoring_model_ids[0]
+
     def _get_dataset_upload_uuid(self):
         url = f'{self._config["dataset_upload_url"]}/s3/uuid'
         resp = requests.get(url)
         resp.raise_for_status()
         return resp.json()
 
     def create_dataset(self, input_params, perform_enrichment=False, ds_id=None):
@@ -1516,14 +1575,45 @@
     def __getitem__(self, item):
         """Compatibility shim for accessing properties as dictionary entries, to keep compatibility
         with the TypedDict implementation in `DatabaseDetails`. New code should use the
         class properties directly instead of accessing this like a dict."""
         return self._info[item]
 
 
+class ScoringModel:
+    def __init__(self, info):
+        self._info = info
+
+    @property
+    def id(self) -> int:
+        return self._info['id']
+
+    @property
+    def name(self) -> str:
+        return self._info['name']
+
+    @property
+    def version(self) -> str:
+        return self._info['version']
+
+    @property
+    def type(self) -> str:
+        return self._info['type']
+
+    @property
+    def is_archived(self) -> bool:
+        return self._info['isArchived']
+
+    def __repr__(self):
+        return f'<{self.id}:{self.name}:{self.version}:{self.type}>'
+
+    def __getitem__(self, item):
+        return self._info[item]
+
+
 class SMInstance(object):
     """Client class for communication with the Metaspace API."""
 
     def __init__(
         self,
         host: str = None,
         verify_certificate: bool = True,
@@ -1777,15 +1867,15 @@
         project_ids: Optional[List[str]] = None,
         adducts: Optional[List[str]] = None,
         neutral_losses: Optional[List[str]] = None,
         chem_mods: Optional[List[str]] = None,
         ppm: Optional[float] = None,
         num_isotopic_peaks: Optional[int] = None,
         decoy_sample_size: Optional[int] = None,
-        analysis_version: Optional[int] = None,
+        scoring_model: Optional[int] = None,
         input_path: Optional[str] = None,
         description: Optional[str] = None,
         perform_enrichment: Optional[bool] = False,
     ) -> str:
         """Submit a dataset for processing in METASPACE.
 
         :param imzml_fn: Path to the imzML file to upload
@@ -1805,15 +1895,15 @@
             For radical ions/cations, use the special strings '[M]+' or '[M]-'.
         :param neutral_losses: List of neutral losses, e.g. ['-H2O', '-CO2']
         :param chem_mods:
         :param ppm: m/z tolerance (in ppm) for generating ion images (default 3.0)
         :param num_isotopic_peaks: Number of isotopic peaks to search for (default 4)
         :param decoy_sample_size: Number of implausible adducts to use for generating the decoy
             search database (default 20)
-        :param analysis_version:
+        :param scoring_model:
         :param input_path: To clone an existing dataset, specify input_path using the value of the
             existing dataset's "s3dir".
             When input_path is suppled, imzml_fn and ibd_fn can be set to None.
         :param description: Optional text to describe the dataset
         :param perform_enrichment: Optional enable LION for dataset.
 
         :return: The newly created dataset ID
@@ -1821,14 +1911,15 @@
         .. _submit dataset example notebook: ../examples/submit-dataset.ipynb
         """
         current_user_id = self.current_user_id()
         assert current_user_id, 'You must be logged in to submit a dataset'
 
         primary_group_id = self._gqclient.get_primary_group_id()
         database_ids = [self._gqclient.map_database_to_id(db) for db in databases or []]
+        scoring_model_id = self._gqclient.map_scoring_model_to_id(scoring_model)
 
         if isinstance(metadata, str):
             metadata = json.loads(metadata)
 
         # Set default adducts
         if not adducts:
             polarity = metadata['MS_Analysis']['Polarity']
@@ -1845,34 +1936,40 @@
 
         if description:
             description_json = _str_to_tiptap_markup(description)
         else:
             description_json = None
 
         # Upload the files. Keep this as late as possible to minimize chances of error after upload
+        file_size = None
         if input_path is None:
             assert imzml_fn and ibd_fn, 'imzml_fn and ibd_fn must be supplied'
             input_path = _dataset_upload(
                 imzml_fn, ibd_fn, self._config['dataset_upload_url'], current_user_id
             )
+            file_size = {
+                'imzml_size': Path(imzml_fn).stat().st_size,
+                'ibd_size': Path(ibd_fn).stat().st_size,
+            }
 
         graphql_response = self._gqclient.create_dataset(
             {
                 'name': name,
                 'inputPath': input_path,
                 'description': description_json,
                 'metadataJson': json.dumps(metadata),
+                'sizeHashJson': json.dumps(file_size) if file_size else None,
                 'databaseIds': database_ids,
                 'adducts': adducts,
                 'neutralLosses': neutral_losses,
                 'chemMods': chem_mods,
                 'ppm': ppm,
                 'numPeaks': num_isotopic_peaks,
                 'decoySampleSize': decoy_sample_size,
-                'analysisVersion': analysis_version,
+                'scoringModelId': scoring_model_id,
                 'submitterId': current_user_id,
                 'groupId': primary_group_id,
                 'projectIds': project_ids,
                 'isPublic': is_public,
             },
             perform_enrichment=perform_enrichment,
         )
@@ -1894,15 +1991,15 @@
         adducts: Optional[List[str]] = None,
         neutral_losses: Optional[List[str]] = None,
         chem_mods: Optional[List[str]] = None,
         is_public: Optional[List[str]] = None,
         ppm: Optional[float] = None,
         num_isotopic_peaks: Optional[int] = None,
         decoy_sample_size: Optional[int] = None,
-        analysis_version: Optional[int] = None,
+        scoring_model: Optional[int] = None,
         reprocess: Optional[bool] = None,
         force: bool = False,
         perform_enrichment: Optional[bool] = False,
     ):
         """Updates a dataset's metadata and/or processing settings. Only specify the fields that
         should change. All arguments should be specified as keyword arguments,
         e.g. to update a dataset's adducts:
@@ -1925,15 +2022,15 @@
         :param is_public: If True, the dataset will be publicly visible.
             If False, it will only be visible to yourself, other members of your Group,
             METASPACE administrators, and members of any Projects you add it to
         :param ppm: m/z tolerance (in ppm) for generating ion images (default 3.0)
         :param num_isotopic_peaks: Number of isotopic peaks to search for (default 4)
         :param decoy_sample_size: Number of implausible adducts to use for generating the decoy
             search database (default 20)
-        :param analysis_version:
+        :param scoring_model:
         :param reprocess:
             None (default): Reprocess if needed
             True: Force reprocessing, even if not needed
             False: Raise an error if the changes would require reprocessing
         :param force:
             True: Allow changes to datasets that are already being processed. This should be used
             with caution, as it can cause errors or inconsistent results.
@@ -1961,16 +2058,16 @@
             input_field['isPublic'] = is_public
         if ppm is not None:
             input_field['ppm'] = ppm
         if num_isotopic_peaks is not None:
             input_field['numPeaks'] = num_isotopic_peaks
         if decoy_sample_size is not None:
             input_field['decoySampleSize'] = decoy_sample_size
-        if analysis_version is not None:
-            input_field['analysisVersion'] = analysis_version
+        if scoring_model is not None:
+            input_field['scoringModelId'] = self._gqclient.map_scoring_model_to_id(scoring_model)
 
         try:
             self._gqclient.update_dataset(
                 id, input_field, reprocess or False, force, perform_enrichment
             )
         except GraphQLException as ex:
             if ex.type == 'reprocessing_needed' and reprocess is None:
@@ -2002,14 +2099,18 @@
             name, version = self._gqclient.map_database_name_to_name_version(name)
             for db in databases:
                 if db['name'] == name and db['version'] == version:
                     db_match = db
 
         return db_match and MolecularDB(db_match)
 
+    def scoring_models(self) -> List[ScoringModel]:
+        sms = sorted(self._gqclient.get_visible_scoring_models(), key=lambda sm: sm['id'])
+        return [ScoringModel(sm) for sm in sms]
+
     def databases(self) -> List[MolecularDB]:
         dbs = sorted(self._gqclient.get_visible_databases(), key=lambda db: db['id'])
         return [MolecularDB(db) for db in dbs]
 
     def create_database(
         self, local_path: Union[str, Path], name: str, version: str, is_public: bool = False
     ) -> dict:
@@ -2375,14 +2476,15 @@
 
 
 # Specify __all__ so that Sphinx documents everything in order from most to least interesting
 __all__ = [
     'SMInstance',
     'SMDataset',
     'MolecularDB',
+    'ScoringModel',
     'IsotopeImages',
     'OpticalImage',
     'GraphQLClient',
     'MetaspaceException',
     'DatasetNotFound',
     'GraphQLException',
     'BadRequestException',
```

### Comparing `metaspace2020-2.0.7/metaspace/types.py` & `metaspace2020-2.0.9/metaspace/types.py`

 * *Files identical despite different names*

### Comparing `metaspace2020-2.0.7/metaspace2020.egg-info/PKG-INFO` & `metaspace2020-2.0.9/metaspace2020.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaspace2020
-Version: 2.0.7
+Version: 2.0.9
 Summary: Python library for connecting to the METASPACE platform
 Home-page: https://github.com/metaspace2020/metaspace/tree/master/metaspace/python-client
 Author: Alexandrov Team, EMBL
 Author-email: contact@metaspace2020.eu
 License: UNKNOWN
 Description: # METASPACE Python client
```

### Comparing `metaspace2020-2.0.7/setup.py` & `metaspace2020-2.0.9/setup.py`

 * *Files identical despite different names*

