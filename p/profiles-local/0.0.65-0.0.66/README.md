# Comparing `tmp/profiles-local-0.0.65.tar.gz` & `tmp/profiles_local-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profiles-local-0.0.65.tar", last modified: Mon Feb  5 06:42:04 2024, max compression
+gzip compressed data, was "profiles_local-0.0.66.tar", last modified: Fri Apr 19 11:37:13 2024, max compression
```

## Comparing `profiles-local-0.0.65.tar` & `profiles_local-0.0.66.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 06:42:04.383648 profiles-local-0.0.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-05 06:42:04.383648 profiles-local-0.0.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-05 06:41:27.000000 profiles-local-0.0.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 06:42:04.379648 profiles-local-0.0.65/profiles_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 06:42:04.379648 profiles-local-0.0.65/profiles_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 06:41:27.000000 profiles-local-0.0.65/profiles_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10555 2024-02-05 06:41:27.000000 profiles-local-0.0.65/profiles_local/src/comprehensive_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-05 06:41:27.000000 profiles-local-0.0.65/profiles_local/src/constants_profiles_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-02-05 06:41:27.000000 profiles-local-0.0.65/profiles_local/src/profiles_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 06:42:04.383648 profiles-local-0.0.65/profiles_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-05 06:42:04.000000 profiles-local-0.0.65/profiles_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-05 06:42:04.000000 profiles-local-0.0.65/profiles_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 06:42:04.000000 profiles-local-0.0.65/profiles_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-05 06:42:04.000000 profiles-local-0.0.65/profiles_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-05 06:42:04.000000 profiles-local-0.0.65/profiles_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-05 06:41:27.000000 profiles-local-0.0.65/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 06:42:04.383648 profiles-local-0.0.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-02-05 06:41:27.000000 profiles-local-0.0.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:37:13.261252 profiles_local-0.0.66/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 11:37:13.261252 profiles_local-0.0.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-19 11:36:35.000000 profiles_local-0.0.66/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:37:13.261252 profiles_local-0.0.66/profiles_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:37:13.261252 profiles_local-0.0.66/profiles_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:36:35.000000 profiles_local-0.0.66/profiles_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-19 11:36:35.000000 profiles_local-0.0.66/profiles_local/src/comprehensive_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-19 11:36:35.000000 profiles_local-0.0.66/profiles_local/src/constants_profiles_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-19 11:36:35.000000 profiles_local-0.0.66/profiles_local/src/profiles_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:37:13.261252 profiles_local-0.0.66/profiles_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 11:37:13.000000 profiles_local-0.0.66/profiles_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 11:36:35.000000 profiles_local-0.0.66/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:37:13.261252 profiles_local-0.0.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-19 11:36:35.000000 profiles_local-0.0.66/setup.py
```

### Comparing `profiles-local-0.0.65/PKG-INFO` & `profiles_local-0.0.66/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profiles-local
-Version: 0.0.65
+Version: 0.0.66
 Summary: This is a package for sharing common crud operation to profile schema in the db
 Home-page: https://github.com/circles-zone/profiles-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,14 @@
 Requires-Dist: operational-hours-local>=0.0.19
 Requires-Dist: person-local>=0.0.20
 Requires-Dist: gender-local>=0.0.6
 Requires-Dist: location-local>=0.0.81
 Requires-Dist: reaction-local>=0.0.8
 Requires-Dist: profile-reaction-local>=0.0.16
 Requires-Dist: profile-profile-local>=0.0.9
-Requires-Dist: language-local>=0.0.6
+Requires-Dist: language-remote>=0.0.6
 Requires-Dist: user-context-remote>=0.0.33
 Requires-Dist: storage-local>=0.1.27
 Requires-Dist: email-address-local>=0.0.16
 Requires-Dist: group-profile-remote>=0.0.14
 
 This is a package for sharing common profile functions used in different repositories
```

### Comparing `profiles-local-0.0.65/README.md` & `profiles_local-0.0.66/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # Installation and upgrade
 
-To install this package run `pip install profile-local`
-To upgrade this package run `pip install --upgrade profile-local`
+To install this package run `pip install -U profiles-local`
 
 # Import
 
-`from profile_local.generic_profile_insert import generic_profile_insert`
+`from profiles_local.comprehensive_profile import ComprehensiveProfilesLocal`
 
 # Use example
 
 ```json
 data = {
   'location': LOCATION_DATA,
   'profile': PROFILE_DATA,
   'storage': STORAGE_DATA,
   'reaction': REACTION_JSON,
   'operational_hours': OPERATIONAL_HOURS
 }
 ```
 
 Where LOCATION_DATA, PROFILE_DATA, STORAGE_DATA, REACTION_JSON, OPERATIONAL_HOURS are dictionaries with the relevant
-data for the table
+data for the table.  
 i.e. for profile_table:
 
 ```json
 PROFILE_DATA = {
   'name': NAME,
   'name_approved': NAME_APPROVED,
   'lang_code': LANG_CODE,
@@ -39,18 +38,15 @@
   'is_rip': is_rip,
   'gender_id': GENDER_ID,
   'stars': STARS,
   'last_dialog_workflow_state_id': LAST_DIALOG_WORKFLOW_STATE_ID
 }
 ```
 
-Then call json.dumps:
-`data_json=json.dumps(data)`
+Now we can call the generic_profile_insert function:  
+`profile_id = ComprehensiveProfilesLocal.insert(data)`
 
-Now we can call the generic_profile_insert function:
-`profile_id = generic_profile_insert(data_json)`
-
-If the function inserted a profile successfully it returns the profile_id of the inserted profile.
+If the function inserted a profile successfully it returns the profile_id of the inserted profile.  
 The function doesn't have to always insert a profile, for example you can use it to insert only a location with
 `data = {'location': LOCATION_DATA}`
 
 and then the returned profile_id will be 'None'.
```

### Comparing `profiles-local-0.0.65/profiles_local/src/comprehensive_profile.py` & `profiles_local-0.0.66/profiles_local/src/comprehensive_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-import json
 from typing import Dict
 
 from circles_local_aws_s3_storage_python import StorageConstants
 from circles_local_aws_s3_storage_python.CirclesStorage import circles_storage
-from database_mysql_local.to_sql_interface import Point
+from database_mysql_local.point import Point
 from email_address_local.email_address import EmailAddressesLocal
-from gender_local.src.gender import Gender
+from gender_local.gender import Gender
 from group_profile_remote.group_profile import GroupProfilesRemote
-from language_local.lang_code import LangCode
+from group_remote.group_remote import GroupsRemote
+from language_remote.lang_code import LangCode
 from location_local.locations_local_crud import LocationsLocal
 from logger_local.MetaLogger import MetaLogger
 from operational_hours_local.src.operational_hours import OperationalHours
 from profile_profile_local.src.profile_profile import ProfileProfile
 from profile_reaction_local.src.profile_reaction import ProfileReactions
-from reaction_local.src.reaction import Reaction
+from reaction_local.reaction import ReactionsLocal
 
-from .constants_profiles_local import PROFILE_LOCAL_PYTHON_LOGGER_CODE
+from .constants_profiles_local import PROFILE_LOCAL_PYTHON_LOGGER_CODE, DEFAULT_LANG_CODE
 from .profiles_local import ProfilesLocal
 
 
 class ComprehensiveProfilesLocal(metaclass=MetaLogger, object=PROFILE_LOCAL_PYTHON_LOGGER_CODE):
     def __init__(self):
         self.location_local = LocationsLocal()
         self.profiles_local = ProfilesLocal()
         self.storage = circles_storage()
         self.gender = Gender()
         self.profile_profile = ProfileProfile()
         self.group_profiles_remote = GroupProfilesRemote()
         self.email_addresses_local = EmailAddressesLocal()
         self.operational_hours = OperationalHours()
-        self.reaction = Reaction()
+        self.reaction = ReactionsLocal()
 
-    def insert(self, profile_json: str, lang_code: LangCode) -> int:
+    def insert(self, profile_json: dict, lang_code: LangCode) -> int:
         """Returns the profile_id of the inserted profile"""
 
-        data = json.loads(profile_json)
         profile_id = location_id = None
 
-        if "location" in data:
-            location_entry: Dict[str, any] = data["location"]
+        if "location" in profile_json:
+            location_entry: Dict[str, any] = profile_json["location"]
             location_data: Dict[str, any] = {
                 "coordinate": Point(longitude=location_entry["coordinate"].get("latitude"),
                                     latitude=location_entry["coordinate"].get("longitude")),
                 "address_local_language": location_entry.get("address_local_language"),
                 "address_english": location_entry.get("address_english"),
                 "postal_code": location_entry.get("postal_code"),
                 "plus_code": location_entry.get("plus_code"),
@@ -51,17 +50,17 @@
                 "region": location_entry.get("region"),
                 "state": location_entry.get("state"),
                 "country": location_entry.get("country")
             }
             location_id = self.location_local.insert(data=location_data, lang_code=lang_code, is_approved=False)
 
         # Insert person to db
-        if 'person' in data:
+        if 'person' in profile_json:
             # TODO person_entry -> person_dict
-            person_entry: Dict[str, any] = data['person']
+            person_entry: Dict[str, any] = profile_json['person']
 
             # TODO I would expect the 1st thing we do with person_dict is "person: PersonLocal(person_dict)". Can we do this approach on all entities?
 
             # TODO: I prefer we use "person.getGender()"
             gender_id = self.gender.get_gender_id_by_title(person_entry.get('gender'))
             person_data: Dict[str, any] = {
                 'last_coordinate': person_entry.get('last_coordinate'),
@@ -79,126 +78,98 @@
                 person_id,
                 lang_code,
                 person_data.get('first_name'),
                 person_data.get('last_name'))
             '''
 
         # Insert profile to db
-        if 'profile' in data and 'person_id' in data.get("person", {}):
-            profile_entry: Dict[str, any] = data['profile']
-            profile_json: Dict[str, any] = {
-                'name': profile_entry.get('name'),
-                'name_approved': profile_entry.get('name_approved'),
-                'lang_code': profile_entry.get('lang_code'),
-                'user_id': profile_entry.get('user_id'),
-                'is_main': profile_entry.get('is_main'),
-                'visibility_id': profile_entry.get('visibility_id'),
-                'is_approved': profile_entry.get('is_approved'),
-                'profile_type_id': profile_entry.get('profile_type_id'),
-                # preferred_lang_code the current preferred language of the user in the specific profile.
-                # Default: english
-                'preferred_lang_code': profile_entry.get('preferred_lang_code', LangCode.ENGLISH.value),
-                'experience_years_min': profile_entry.get('experience_years_min'),
-                'main_phone_id': profile_entry.get('main_phone_id'),
-                'is_rip': profile_entry.get('is_rip'),
-                'gender_id': profile_entry.get('gender_id'),
-                'stars': profile_entry.get('stars'),
-                'last_dialog_workflow_state_id': profile_entry.get('last_dialog_workflow_state_id'),
-                "about": profile_entry.get('about')
-            }
-            profile_id = self.profiles_local.insert(profile_json=profile_json,
-                                                    person_id=data["person"]['person_id'])
+        if 'profile' in profile_json and 'person_id' in profile_json.get("person", {}):
+            profile_id = self.profiles_local.insert(profile_json=profile_json['profile'],
+                                                    person_id=profile_json['person']['person_id'])
 
         # insert profile_profile to db
-        if 'profile_profile' in data:
-            profile_profile_entry: Dict[str, any] = data['profile_profile']
+        if 'profile_profile' in profile_json:
+            profile_profile_entry: Dict[str, any] = profile_json['profile_profile']
             for i in profile_profile_entry:
                 profile_profile_part_entry: Dict[str, any] = profile_profile_entry[i]
                 profile_profile_data: Dict[str, any] = {
                     'profile_id': profile_profile_part_entry.get('profile_id'),
                     'relationship_type_id': profile_profile_part_entry.get('relationship_type_id'),
                     'job_title': profile_profile_part_entry.get('job_title', None)
                 }
                 profile_profile_id = self.profile_profile.insert_profile_profile(
                     profile_id1=profile_profile_data['profile_id'], profile_id2=profile_id,
                     relationship_type_id=profile_profile_data['relationship_type_id'],
                     job_title=profile_profile_data['job_title'])
                 self.logger.info(object={"profile_profile_id": profile_profile_id})
 
         # insert group to db
-        # TODO: uncomment section
-        # if 'group' in keys:
-        # group_entry: Dict[str, any] = data['group']
-        # group_data: Dict[str, any] = {
-        #     'title': group_entry.get('title'),
-        #     'lang_code': group_entry.get('lang_code'),
-        #     'parent_group_id': group_entry.get('parent_group_id'),
-        #     'is_interest': group_entry.get('is_interest'),
-        #     'image': group_entry.get('image', None),
-        # }
-        # group_id = GroupsRemote().create_group(group_data)
+        if 'group' in profile_json:
+            group_entry: Dict[str, any] = profile_json['group']
+            group_id = GroupsRemote().create_group(title=group_entry.get('title'),
+                                                   title_lang_code=group_entry.get('lang_code', DEFAULT_LANG_CODE).value,
+                                                   parent_group_id=group_entry.get('parent_group_id'),
+                                                   is_interest=group_entry.get('is_interest'),
+                                                   image=group_entry.get('image', None))
+            self.logger.info(object={"group_id": group_id})
 
         # insert group_profile to db
-        if 'group_profile' in data:
-            group_profile_entry: Dict[str, any] = data['group_profile']
+        if 'group_profile' in profile_json:
+            group_profile_entry: Dict[str, any] = profile_json['group_profile']
             group_profile_data: Dict[str, any] = {
                 'group_id': group_profile_entry.get('group_id'),
                 'relationship_type_id': group_profile_entry.get('relationship_type_id'),
             }
             group_profile_id = self.group_profiles_remote.create(
                 group_id=group_profile_data['group_id'],
                 relationship_type_id=group_profile_data['relationship_type_id'])
             self.logger.info(object={"group_profile_id": group_profile_id})
 
         # insert email to db
-        if 'email' in data:
-            email_entry: Dict[str, any] = data['email']
-            email_address_data: Dict[str, any] = {
+        if 'email' in profile_json:
+            email_entry: Dict[str, any] = profile_json['email']
+            email_address_json: Dict[str, any] = {
                 'email_address': email_entry.get('email_address'),
-                'lang_code': (email_entry.get('lang_code')),
+                'lang_code': email_entry.get('lang_code', DEFAULT_LANG_CODE).value,
                 'name': email_entry.get('name'),
             }
             email_address_id = self.email_addresses_local.insert(
-                email_address_data['email_address'], LangCode[email_address_data['lang_code']],
-                email_address_data['name'])
+                email_address_json['email_address'], LangCode[email_address_json['lang_code']],
+                email_address_json['name'])
             self.logger.info(object={"email_address_id ": email_address_id})
 
         # Insert storage to db
-        if "storage" in data:
+        if "storage" in profile_json:
             storage_data = {
-                "path": data["storage"].get("path"),
-                "filename": data["storage"].get("filename"),
-                "region": data["storage"].get("region"),
-                "url": data["storage"].get("url"),
-                "file_extension": data["storage"].get("file_extension"),
-                "file_type": data["storage"].get("file_type")
+                "path": profile_json["storage"].get("path"),
+                "filename": profile_json["storage"].get("filename"),
+                "region": profile_json["storage"].get("region"),
+                "url": profile_json["storage"].get("url"),
+                "file_extension": profile_json["storage"].get("file_extension"),
+                "file_type": profile_json["storage"].get("file_type")
             }
             if storage_data["file_type"] == "Profile Image":
                 self.storage.save_image_in_storage_by_url(image_url=storage_data["url"],
                                                           local_filename=storage_data["filename"],
                                                           profile_id=profile_id,
                                                           entity_type_id=StorageConstants.PROFILE_IMAGE),
 
         # Insert reaction to db
-        if "reaction" in data:
+        if "reaction" in profile_json:
             reaction_json = {
-                "value": data["reaction"].get("value"),
-                "image": data["reaction"].get("image"),
-                "title": data["reaction"].get("title"),
-                "description": data["reaction"].get("description"),
-            }
-            # TODO Reaction is not only on profile_id, user can react on anything i.e. news, group, event ...
-            #  We should provide a generic approach.
-            #   remove profile_id parameter from reaction-local insert method
-            # TODO: fix typing
-            # TODO: Reaction -> ReactionsLocal
-            reaction_id = self.reaction.insert(reaction_json, profile_id, lang_code)
+                "value": profile_json["reaction"].get("value"),
+                "image": profile_json["reaction"].get("image"),
+                "title": profile_json["reaction"].get("title"),
+                "description": profile_json["reaction"].get("description"),
+            }
+
+            reaction_id = self.reaction.insert(reaction_json, lang_code)
             # Insert profile-reactions to db
             ProfileReactions.insert(reaction_id, profile_id)
 
         # Insert operational hours to db
-        if "operational_hours" in data:
+        if "operational_hours" in profile_json:
             operational_hours_list_of_dicts = OperationalHours.create_hours_array(
-                data["operational_hours"])
+                profile_json["operational_hours"])
             self.operational_hours.insert(profile_id, location_id, operational_hours_list_of_dicts)
 
         return profile_id
```

### Comparing `profiles-local-0.0.65/profiles_local/src/constants_profiles_local.py` & `profiles_local-0.0.66/profiles_local/src/constants_profiles_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
+from language_remote.lang_code import LangCode
+
+DEFAULT_LANG_CODE = LangCode.ENGLISH
 
 PROFILE_LOCAL_PYTHON_PACKAGE_COMPONENT_ID = 170
-PROFILE_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME = 'profile-local python package'
+PROFILE_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME = 'profiles-local python package'
 
 PROFILE_LOCAL_PYTHON_LOGGER_CODE = {
     'component_id': PROFILE_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
     'component_name': PROFILE_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': 'tal.g@circ.zone'
 }
```

### Comparing `profiles-local-0.0.65/profiles_local.egg-info/PKG-INFO` & `profiles_local-0.0.66/profiles_local.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profiles-local
-Version: 0.0.65
+Version: 0.0.66
 Summary: This is a package for sharing common crud operation to profile schema in the db
 Home-page: https://github.com/circles-zone/profiles-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,14 @@
 Requires-Dist: operational-hours-local>=0.0.19
 Requires-Dist: person-local>=0.0.20
 Requires-Dist: gender-local>=0.0.6
 Requires-Dist: location-local>=0.0.81
 Requires-Dist: reaction-local>=0.0.8
 Requires-Dist: profile-reaction-local>=0.0.16
 Requires-Dist: profile-profile-local>=0.0.9
-Requires-Dist: language-local>=0.0.6
+Requires-Dist: language-remote>=0.0.6
 Requires-Dist: user-context-remote>=0.0.33
 Requires-Dist: storage-local>=0.1.27
 Requires-Dist: email-address-local>=0.0.16
 Requires-Dist: group-profile-remote>=0.0.14
 
 This is a package for sharing common profile functions used in different repositories
```

### Comparing `profiles-local-0.0.65/setup.py` & `profiles_local-0.0.66/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "profiles-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.65',  # https://pypi.org/project/profiles-local/
+    version='0.0.66',  # https://pypi.org/project/profiles-local/
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     description="This is a package for sharing common crud operation to profile schema in the db",
@@ -26,14 +26,14 @@
                       "operational-hours-local>=0.0.19",
                       "person-local>=0.0.20",
                       "gender-local>=0.0.6",
                       "location-local>=0.0.81",
                       "reaction-local>=0.0.8",
                       "profile-reaction-local>=0.0.16",
                       "profile-profile-local>=0.0.9",
-                      "language-local>=0.0.6",
+                      "language-remote>=0.0.6",
                       "user-context-remote>=0.0.33",
                       "storage-local>=0.1.27",
                       "email-address-local>=0.0.16",
                       "group-profile-remote>=0.0.14"
                       ]
 )
```

