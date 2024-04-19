# Comparing `tmp/chemotion_api-0.3.3.tar.gz` & `tmp/chemotion_api-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemotion_api-0.3.3.tar", max compression
+gzip compressed data, was "chemotion_api-0.3.9.tar", max compression
```

## Comparing `chemotion_api-0.3.3.tar` & `chemotion_api-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,39 @@
--rw-r--r--   0        0        0    16291 2023-05-26 13:05:27.256045 chemotion_api-0.3.3/README.md
--rw-r--r--   0        0        0    10428 2023-09-27 10:29:18.789321 chemotion_api-0.3.3/chemotion_api/__init__.py
--rw-r--r--   0        0        0      904 2023-08-02 09:55:59.620981 chemotion_api-0.3.3/chemotion_api/admin/__init__.py
--rw-r--r--   0        0        0    14390 2023-12-06 15:06:28.395562 chemotion_api-0.3.3/chemotion_api/collection.py
--rw-r--r--   0        0        0     2528 2023-08-02 10:24:56.736315 chemotion_api-0.3.3/chemotion_api/connection.py
--rw-r--r--   0        0        0     4330 2023-12-07 12:44:52.145146 chemotion_api-0.3.3/chemotion_api/element_manager.py
--rw-r--r--   0        0        0     4493 2023-12-07 13:33:43.569628 chemotion_api-0.3.3/chemotion_api/elements/__init__.py
--rw-r--r--   0        0        0    12434 2023-12-09 19:05:09.796015 chemotion_api-0.3.3/chemotion_api/elements/abstract_element.py
--rw-r--r--   0        0        0      473 2023-08-02 09:55:59.620981 chemotion_api-0.3.3/chemotion_api/elements/empty_elements/__init__.py
--rw-r--r--   0        0        0      193 2023-12-06 13:33:42.942075 chemotion_api-0.3.3/chemotion_api/elements/empty_elements/container.json
--rw-r--r--   0        0        0      836 2023-12-07 08:30:34.633854 chemotion_api-0.3.3/chemotion_api/elements/empty_elements/reaction.json
--rw-r--r--   0        0        0      261 2023-08-02 09:55:59.620981 chemotion_api-0.3.3/chemotion_api/elements/empty_elements/research_plan.json
--rw-r--r--   0        0        0      959 2023-12-07 08:25:30.046420 chemotion_api-0.3.3/chemotion_api/elements/empty_elements/sample.json
--rw-r--r--   0        0        0    21681 2023-08-02 09:55:59.620981 chemotion_api-0.3.3/chemotion_api/elements/empty_elements/solvents.json
--rw-r--r--   0        0        0      219 2023-08-02 09:55:59.620981 chemotion_api-0.3.3/chemotion_api/elements/empty_elements/wellplate.json
--rw-r--r--   0        0        0      842 2023-12-06 08:45:28.515985 chemotion_api-0.3.3/chemotion_api/elements/generic_element.py
--rw-r--r--   0        0        0     7194 2023-12-07 08:33:23.681853 chemotion_api-0.3.3/chemotion_api/elements/reaction.py
--rw-r--r--   0        0        0      329 2023-12-07 13:57:42.840992 chemotion_api-0.3.3/chemotion_api/elements/research_plan.py
--rw-r--r--   0        0        0    10911 2023-12-08 09:04:20.153654 chemotion_api-0.3.3/chemotion_api/elements/sample.py
--rw-r--r--   0        0        0     2576 2023-12-07 13:58:33.712978 chemotion_api-0.3.3/chemotion_api/elements/wellplate.py
--rw-r--r--   0        0        0     1008 2023-12-07 13:03:51.501589 chemotion_api-0.3.3/chemotion_api/generic_segments.py
--rw-r--r--   0        0        0     6680 2023-12-07 13:57:42.856992 chemotion_api-0.3.3/chemotion_api/user.py
--rw-r--r--   0        0        0     6185 2023-12-07 12:53:31.104869 chemotion_api-0.3.3/chemotion_api/utils/__init__.py
--rw-r--r--   0        0        0      457 2023-12-07 11:15:37.803004 chemotion_api-0.3.3/chemotion_api/utils/solvent_manager.py
--rw-r--r--   0        0        0      485 2023-12-13 15:02:44.149766 chemotion_api-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    16910 1970-01-01 00:00:00.000000 chemotion_api-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    16291 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/README.md
+-rw-r--r--   0        0        0    10885 2024-02-22 10:10:32.726601 chemotion_api-0.3.9/chemotion_api/__init__.py
+-rw-r--r--   0        0        0    10530 2024-03-01 12:23:25.723466 chemotion_api-0.3.9/chemotion_api/__main__.py
+-rw-r--r--   0        0        0      904 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/admin/__init__.py
+-rw-r--r--   0        0        0    15491 2024-02-22 11:11:42.993848 chemotion_api-0.3.9/chemotion_api/collection.py
+-rw-r--r--   0        0        0     8675 2024-03-04 10:13:18.013801 chemotion_api-0.3.9/chemotion_api/commands/__init__.py
+-rw-r--r--   0        0        0     1024 2024-02-29 13:42:34.555754 chemotion_api-0.3.9/chemotion_api/commands/creator.py
+-rw-r--r--   0        0        0        2 2024-02-28 11:56:42.239884 chemotion_api-0.3.9/chemotion_api/commands/templates/productive/.env
+-rw-r--r--   0        0        0     2616 2024-02-29 12:52:19.869580 chemotion_api-0.3.9/chemotion_api/commands/templates/productive/docker-compose.yml
+-rw-r--r--   0        0        0       37 2024-02-28 11:45:44.193163 chemotion_api-0.3.9/chemotion_api/commands/templates/productive/services/converter/htpasswd
+-rw-r--r--   0        0        0       71 2024-02-28 12:12:13.998055 chemotion_api-0.3.9/chemotion_api/commands/templates/productive/shared/pullin/.version
+-rw-r--r--   0        0        0      259 2024-02-15 20:42:56.000000 chemotion_api-0.3.9/chemotion_api/commands/templates/productive/shared/pullin/config/converter.yml
+-rw-r--r--   0        0        0       79 2023-11-20 14:07:08.000000 chemotion_api-0.3.9/chemotion_api/commands/templates/productive/shared/pullin/config/shrine.yml
+-rw-r--r--   0        0        0      131 2024-02-15 09:27:04.000000 chemotion_api-0.3.9/chemotion_api/commands/templates/productive/shared/pullin/config/spectra.yml
+-rw-r--r--   0        0        0     1566 2023-09-26 10:53:40.000000 chemotion_api-0.3.9/chemotion_api/commands/templates/productive/shared/pullin/db/seeds/json/dataset_klasses.json
+-rw-r--r--   0        0        0     1344 2024-03-01 10:01:54.074914 chemotion_api-0.3.9/chemotion_api/commands/updater.py
+-rw-r--r--   0        0        0     2685 2024-02-20 09:26:54.915459 chemotion_api-0.3.9/chemotion_api/connection.py
+-rw-r--r--   0        0        0     4333 2024-02-15 08:52:37.600139 chemotion_api-0.3.9/chemotion_api/element_manager.py
+-rw-r--r--   0        0        0     4493 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/__init__.py
+-rw-r--r--   0        0        0    13130 2024-02-20 13:06:20.473557 chemotion_api-0.3.9/chemotion_api/elements/abstract_element.py
+-rw-r--r--   0        0        0     3502 2024-02-21 20:52:33.757498 chemotion_api-0.3.9/chemotion_api/elements/attachments.py
+-rw-r--r--   0        0        0      473 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/empty_elements/__init__.py
+-rw-r--r--   0        0        0      193 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/empty_elements/container.json
+-rw-r--r--   0        0        0      836 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/empty_elements/reaction.json
+-rw-r--r--   0        0        0      261 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/empty_elements/research_plan.json
+-rw-r--r--   0        0        0      959 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/empty_elements/sample.json
+-rw-r--r--   0        0        0    21681 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/empty_elements/solvents.json
+-rw-r--r--   0        0        0      219 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/empty_elements/wellplate.json
+-rw-r--r--   0        0        0      842 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/generic_element.py
+-rw-r--r--   0        0        0     7194 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/reaction.py
+-rw-r--r--   0        0        0     6969 2024-02-20 13:29:15.369864 chemotion_api-0.3.9/chemotion_api/elements/research_plan.py
+-rw-r--r--   0        0        0    10911 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/sample.py
+-rw-r--r--   0        0        0     2576 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/elements/wellplate.py
+-rw-r--r--   0        0        0     1008 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/generic_segments.py
+-rw-r--r--   0        0        0    12110 2024-02-22 09:57:05.100165 chemotion_api-0.3.9/chemotion_api/user.py
+-rw-r--r--   0        0        0     6185 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/utils/__init__.py
+-rw-r--r--   0        0        0      457 2024-02-09 13:03:54.182528 chemotion_api-0.3.9/chemotion_api/utils/solvent_manager.py
+-rw-r--r--   0        0        0      643 2024-03-15 10:19:06.222833 chemotion_api-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    17117 1970-01-01 00:00:00.000000 chemotion_api-0.3.9/PKG-INFO
```

### Comparing `chemotion_api-0.3.3/README.md` & `chemotion_api-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/__init__.py` & `chemotion_api-0.3.9/chemotion_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,25 +111,36 @@
         The token property returns the JWT (java web token)
 
         :return: JWT
         """
 
         return self._con.bearer_token
 
-    def get_user(self) -> Admin|Person|Group|Device:
+    def get_user(self) -> Admin | Person | Group | Device:
         """
         This get_user methode initializes a new User object. The user object allows you to fetch and edit user data.
 
         :return: a new User instance
 
         :raise PermissionError: if the userdata cannot be fetched. Make sure that you are logged in.
         """
         u = User.load_me(self._con)
         return u
 
+    def find_user_by_name(self, name: str) -> list[Person]:
+
+        """
+        This find_user_by_name methode finds all user by name and returns the three top matches.
+
+        :param name: Potential name or name snippet of a user
+        :return: list u matching user
+
+        :raise PermissionError: if the userdata cannot be fetched. Make sure that you are logged in.
+        """
+        return self.get_user().find_user_by_name(self._con, name)
 
     @property
     def device_manager(self):
         return DeviceManager(self._con)
 
     def get_root_collection(self, reload=True) -> RootCollection:
         if reload or self._root_col is None:
```

### Comparing `chemotion_api-0.3.3/chemotion_api/admin/__init__.py` & `chemotion_api-0.3.9/chemotion_api/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/collection.py` & `chemotion_api-0.3.9/chemotion_api/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 import json
 import os
+from enum import Enum
 from random import random
 from typing import TypeVar
 
+from chemotion_api.user import Person, Group
+
 from chemotion_api.elements.sample import MoleculeManager
 from chemotion_api.connection import Connection
 
 from chemotion_api.element_manager import ElementManager
 from chemotion_api.elements import ElementSet, AbstractElement
 
 TAbstractCollection = TypeVar("TAbstractCollection", bound="AbstractCollection")
 TRootCollection = TypeVar("TRootCollection", bound="RootCollection")
 
 
+class SyncPremission(Enum):
+    Read = 0
+    Write = 1
+    Share = 2
+    Delete = 3
+    ImportElements = 4
+    PassOwnership = 5
+
+
 class AbstractCollection:
     children: list[TAbstractCollection]
     label: str = None
     _parent: TAbstractCollection = None
     id: int = None
 
     @classmethod
@@ -107,15 +119,14 @@
             return root.get_collection(new_path)
 
     def add_collection(self, col_path: str | list[str]):
         if self.is_sync:
             raise Exception("You cannot add a collection to a synced collection!")
         raise NotImplementedError('This collection cannot add a collection')
 
-
     def get_samples(self, per_page=10) -> ElementSet:
         root = self.get_root()
         e = ElementSet(root._session, root._element_manager.all_classes.get('sample'), self.id,
                        self.is_sync)
         e.load_elements(per_page)
         return e
 
@@ -160,15 +171,15 @@
 
 class AbstractEditableCollection(AbstractCollection):
 
     def new_sample(self) -> AbstractElement:
         return self._create_new_element('sample')
 
     def new_sample_smiles(self, smiles_code: str) -> AbstractElement:
-        sample =  self._create_new_element('sample')
+        sample = self._create_new_element('sample')
         mol = MoleculeManager(self.get_root()._session).create_molecule_by_smiles(smiles_code)
         sample.molecule = mol
         return sample
 
     def new_solvent(self, name) -> AbstractElement:
         root = self.get_root()
         new_json = root._element_manager.build_solvent_sample(name, self.id)
@@ -190,15 +201,14 @@
 
     def new_generic_by_label(self, label) -> AbstractElement:
         for (elem_name, elem) in self.get_root()._element_manager.all_classes.items():
             if elem['label'] == label:
                 return self._create_new_element(elem_name)
         raise ValueError(f'Could not find a generic element with the label: "{label}"')
 
-
     def _create_new_element(self, type_name) -> AbstractElement:
         root = self.get_root()
         new_json = root._element_manager.build_new(type_name, self.id)
 
         e = ElementSet(root._session, root._element_manager.all_classes.get(type_name), self.id,
                        self.is_sync)
         return e.new_element(new_json)
@@ -260,14 +270,37 @@
         abs_path = self.get_path()
         self.get_root().delete(abs_path)
 
     def add_collection(self, name):
         abs_path = os.path.join(self.get_path(), name)
         return self.get_root().add_collection(abs_path)
 
+    def share(self, premission_level: SyncPremission, *users: Person | Group):
+        data = {
+            "collection_attributes": {
+                "permission_level": premission_level.value,
+                "sample_detail_level": 10,
+                "reaction_detail_level": 10,
+                "wellplate_detail_level": 10,
+                "screen_detail_level": 10,
+                "element_detail_level": 10
+            },
+            "user_ids": [
+                {'label': f'{user.name} ({user.initials} - {user.user_type})',
+                 'name': user.name,
+                 'value': user.id} for user in users if user.is_group() or user.is_person()
+            ],
+            "id": self.id
+        }
+
+        res = self.get_root()._session.post('/api/v1/syncCollections/', data=data)
+        if res.status_code != 201:
+            raise ConnectionError(f"{res.status_code} -> {res.text}")
+
+
 
 class RootSyncCollection(AbstractCollection):
 
     def __init__(self, session: Connection, element_manager: ElementManager):
         super().__init__()
         self.is_sync = True
         self._session = session
```

### Comparing `chemotion_api-0.3.3/chemotion_api/connection.py` & `chemotion_api-0.3.9/chemotion_api/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     def __init__(self, host_url: str, verify_ssl: bool = True):
         super().__init__()
         self._host_url = host_url.strip('/')
         self._verify = verify_ssl
         self._bearer_token = None
         self.tzinfo = None
 
-
     def reset_bearer_token(self):
         self._bearer_token = None
 
     def set_bearer_token(self, token: str):
         self._bearer_token = token
 
     @property
@@ -39,27 +38,31 @@
     def put(self, url_path: str = '', **kwargs) -> requests.Response:
         return self._send_request('put', url_path, self.get_json_session_header(), kwargs)
 
     def _send_request(self, method: str, url_path: str, default_header: dict, kwargs: dict) -> requests.Response:
         kwargs['verify'] = kwargs.get('verify', self._verify)
         kwargs['url'] = kwargs.get('url', f"{self._host_url}/{url_path.lstrip('/')}")
         kwargs['headers'] = kwargs.get('headers', default_header)
-        kwargs['timeout'] = kwargs.get('timeout', (1,5))
-        if 'data' in kwargs and not isinstance(kwargs['data'], str) and kwargs['headers'].get('Content-Type') == 'application/json':
+        kwargs['timeout'] = kwargs.get('timeout', (2, 15))
+        if 'files' in kwargs:
+            if 'Content-Type' in kwargs['headers']:
+                del kwargs['headers']['Content-Type']
+        elif 'data' in kwargs and not isinstance(kwargs['data'], str) and kwargs['headers'].get(
+                'Content-Type') == 'application/json':
             kwargs['data'] = json.dumps(kwargs.get('data', {}))
+
         res = getattr(super(), method)(**kwargs)
         if self.tzinfo is None:
             if 'Date' in res.headers:
                 self.tzinfo = parsedate(res.headers['Date']).astimezone().tzinfo
         return res
 
     def get_default_session_header(self) -> dict[str, str]:
         headers = {'User-Agent': 'Mozilla/5.0'}
         if self._bearer_token is not None:
             headers["Authorization"] = f"Bearer {self._bearer_token}"
         return headers
 
-
     def get_json_session_header(self) -> dict[str, str]:
         header = self.get_default_session_header()
         header['Content-Type'] = 'application/json'
-        return header
+        return header
```

### Comparing `chemotion_api-0.3.3/chemotion_api/element_manager.py` & `chemotion_api-0.3.9/chemotion_api/element_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     def _get_short_label(self, type_name):
         u = self._get_user()
         if type_name == 'sample':
             return '{}-{}'.format(u.initials, u.counters[type_name + 's'])
         if type_name == 'reaction':
             return '{}-R{}'.format(u.initials, u.counters[type_name + 's'])
-        return f"{u.initials}-{type_name}{u.counters.get(type_name + 's', u.counters.get(type_name))}"
+        return f"{u.initials}-{type_name}{u.counters.get(type_name + 's', u.counters.get(type_name, 0))}"
 
     def build_new(self, type_name, collection_id):
         class_obj = self.all_classes[type_name]
         data = {}
         if not class_obj['is_generic']:
             json_path = os.path.join(os.path.dirname(__file__), 'elements/empty_elements', type_name + '.json')
             if os.path.exists(json_path):
```

### Comparing `chemotion_api-0.3.3/chemotion_api/elements/__init__.py` & `chemotion_api-0.3.9/chemotion_api/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/elements/abstract_element.py` & `chemotion_api-0.3.9/chemotion_api/elements/abstract_element.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 import uuid
 from datetime import datetime
 
 import dateutil.parser
 
 from chemotion_api.connection import Connection
+from chemotion_api.elements.attachments import Attachments
 
 from chemotion_api.generic_segments import GenericSegments
 from chemotion_api.utils import add_to_dict, parse_generic_object_json, \
     clean_generic_object_json, merge_dicts
 
 from requests.exceptions import RequestException
 
@@ -125,19 +126,23 @@
 
 
 class AbstractElement:
     element_type = None
 
     def __init__(self, generic_segments: GenericSegments, session: Connection, json_data: dict = None, id: int = None,
                  element_type: str = None):
+        self.attachments: Attachments | None = None
         self._generic_segments = generic_segments
         self._session = session
         self.name = ''
         self.last_update = None
         if json_data is not None:
+            attachments_data = json_data.get('attachments')
+            if attachments_data is not None:
+                self.attachments = Attachments(self._session, attachments_data)
             self._set_json_data(json_data)
         elif id is not None and element_type is not None:
             self.id = id
             self.element_type = element_type
             self.load()
         else:
             raise ValueError("Either 'json_data' or 'id' and 'element_type' must be provided during initialization")
@@ -145,15 +150,19 @@
     def load(self):
 
         payload = {}
         res = self._session.get("{}/{}.json".format(self.__class__.get_url(self.element_type), self.id),
                                 data=payload)
         if res.status_code != 200:
             raise RequestException("{} -> {}".format(res.status_code, res.text))
-        json_data = res.json()[self.get_response_key(self.element_type)]
+        res_json = res.json()
+        json_data = res_json[self.get_response_key(self.element_type)]
+        attachments_data = res_json.get('attachments')
+        if attachments_data is not None:
+            self.attachments = Attachments(self._session, attachments_data)
         self._set_json_data(json_data)
 
     def _set_json_data(self, json_data):
         self.json_data = json_data
         if json_data.get('updated_at') is not None:
             try:
                 for pattern in ['%Y-%m-%d %H:%M:%S %Z', '%d.%m.%Y, %H:%M:%S %z']:
@@ -201,26 +210,30 @@
             res = self._session.put(self.save_url(), data=json.dumps(data))
         if res.status_code != 200 and res.status_code != 201:
             raise RequestException('{} -> '.format(res.status_code, res.text))
         if is_created:
             res_json = res.json()
             res_json = merge_dicts(self.json_data, res_json.get(self.element_type, res_json.get('element')))
             self._set_json_data(res_json)
+        if self.attachments is not None:
+            self.attachments.save(self.id)
 
     def clean_data(self):
         cleaned_data = {
             'name': self.name,
             'id': self.id or uuid.uuid4().__str__(),
             'is_new': self.id is None,
             'type': self.element_type
         }
         if 'collection_id' in self.json_data:
             cleaned_data['collection_id'] = self.json_data['collection_id']
         if 'container' in self.json_data:
             cleaned_data['container'] = self.json_data['container']
+        if self.attachments is not None:
+            cleaned_data['attachments'] = self.attachments.attachment_data
 
         merge_dicts(cleaned_data, self._clean_segments_data(), self._clean_properties_data(), self._clean_analyses_data())
         return cleaned_data
 
     def save_url(self):
         if self.id is not None:
             return "/api/v1/{}s/{}".format(self.json_data.get('type'), self.id)
```

### Comparing `chemotion_api-0.3.3/chemotion_api/elements/empty_elements/reaction.json` & `chemotion_api-0.3.9/chemotion_api/elements/empty_elements/reaction.json`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/elements/empty_elements/sample.json` & `chemotion_api-0.3.9/chemotion_api/elements/empty_elements/sample.json`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/elements/empty_elements/solvents.json` & `chemotion_api-0.3.9/chemotion_api/elements/empty_elements/solvents.json`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/elements/generic_element.py` & `chemotion_api-0.3.9/chemotion_api/elements/generic_element.py`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/elements/reaction.py` & `chemotion_api-0.3.9/chemotion_api/elements/reaction.py`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/elements/sample.py` & `chemotion_api-0.3.9/chemotion_api/elements/sample.py`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/elements/wellplate.py` & `chemotion_api-0.3.9/chemotion_api/elements/wellplate.py`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/generic_segments.py` & `chemotion_api-0.3.9/chemotion_api/generic_segments.py`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/chemotion_api/utils/__init__.py` & `chemotion_api-0.3.9/chemotion_api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chemotion_api-0.3.3/PKG-INFO` & `chemotion_api-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: chemotion-api
-Version: 0.3.3
+Version: 0.3.9
 Summary: A Chemotion python API
 License: MIT
 Author: Maritn Starman
 Author-email: martin.starman@kit.edu
 Requires-Python: >=3.09,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: pytz (>=2023.3.post1,<2024.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
+Requires-Dist: python-magic (>=0.4.27,<0.5.0)
+Requires-Dist: pytz (>=2024.1,<2025.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ChemotionApi
 
 | PLEASE NOTICE: This version is far from beeing ready. |
 |-------------------------------------------------------|
 ## Open ToDos
```

