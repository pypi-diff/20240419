# Comparing `tmp/Velkoz-0.0.61.tar.gz` & `tmp/Velkoz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Velkoz-0.0.61.tar", last modified: Tue Apr 16 22:01:26 2024, max compression
+gzip compressed data, was "Velkoz-0.1.0.tar", last modified: Fri Apr 19 11:05:44 2024, max compression
```

## Comparing `Velkoz-0.0.61.tar` & `Velkoz-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 22:01:26.374920 Velkoz-0.0.61/
--rw-rw-rw-   0        0        0      563 2024-04-16 22:01:26.373920 Velkoz-0.0.61/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 22:01:26.300153 Velkoz-0.0.61/Velkoz/
--rw-rw-rw-   0        0        0      816 2024-04-16 21:12:33.000000 Velkoz-0.0.61/Velkoz/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:01:26.335704 Velkoz-0.0.61/Velkoz/data/
--rw-rw-rw-   0        0        0       48 2024-04-13 20:58:45.000000 Velkoz-0.0.61/Velkoz/data/__init__.py
--rw-rw-rw-   0        0        0     2832 2024-04-16 16:28:25.000000 Velkoz-0.0.61/Velkoz/data/champion.py
--rw-rw-rw-   0        0        0     2197 2024-04-16 20:27:43.000000 Velkoz-0.0.61/Velkoz/data/common.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:01:26.344454 Velkoz-0.0.61/Velkoz/eye/
--rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.0.61/Velkoz/eye/__init__.py
--rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.0.61/Velkoz/eye/account.py
--rw-rw-rw-   0        0        0      930 2024-04-16 21:57:33.000000 Velkoz-0.0.61/Velkoz/eye/champion_mastery.py
--rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.0.61/Velkoz/eye/common.py
--rw-rw-rw-   0        0        0     7581 2024-04-12 12:51:42.000000 Velkoz-0.0.61/Velkoz/eye/match.py
--rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.0.61/Velkoz/eye/summoner.py
--rw-rw-rw-   0        0        0     3276 2024-04-16 15:09:23.000000 Velkoz-0.0.61/Velkoz/settings.py
--rw-rw-rw-   0        0        0     1032 2024-04-16 22:00:45.000000 Velkoz-0.0.61/Velkoz/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:01:26.355529 Velkoz-0.0.61/Velkoz/supp/
--rw-rw-rw-   0        0        0      154 2024-04-16 10:08:55.000000 Velkoz-0.0.61/Velkoz/supp/__init__.py
--rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.0.61/Velkoz/supp/account.py
--rw-rw-rw-   0        0        0      280 2024-04-16 11:05:52.000000 Velkoz-0.0.61/Velkoz/supp/champion.py
--rw-rw-rw-   0        0        0     1165 2024-04-16 21:56:09.000000 Velkoz-0.0.61/Velkoz/supp/champion_mastery.py
--rw-rw-rw-   0        0        0      270 2024-04-11 21:19:18.000000 Velkoz-0.0.61/Velkoz/supp/match.py
--rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.0.61/Velkoz/supp/summoner.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:01:26.371385 Velkoz-0.0.61/Velkoz/tentacles/
--rw-rw-rw-   0        0        0      213 2024-04-11 21:19:17.000000 Velkoz-0.0.61/Velkoz/tentacles/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-03-22 11:07:43.000000 Velkoz-0.0.61/Velkoz/tentacles/account.py
--rw-rw-rw-   0        0        0     3340 2024-04-16 21:57:59.000000 Velkoz-0.0.61/Velkoz/tentacles/champion_mastery.py
--rw-rw-rw-   0        0        0     4543 2024-04-12 22:57:44.000000 Velkoz-0.0.61/Velkoz/tentacles/common.py
--rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.0.61/Velkoz/tentacles/config.py
--rw-rw-rw-   0        0        0     1650 2024-03-22 13:51:43.000000 Velkoz-0.0.61/Velkoz/tentacles/match.py
--rw-rw-rw-   0        0        0     1416 2024-03-22 11:06:12.000000 Velkoz-0.0.61/Velkoz/tentacles/summoner.py
--rw-rw-rw-   0        0        0     6814 2024-04-16 21:13:06.000000 Velkoz-0.0.61/Velkoz/velkoz.py
-drwxrwxrwx   0        0        0        0 2024-04-16 22:01:26.372901 Velkoz-0.0.61/Velkoz.egg-info/
--rw-rw-rw-   0        0        0      563 2024-04-16 22:01:26.000000 Velkoz-0.0.61/Velkoz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2024-04-16 22:01:26.000000 Velkoz-0.0.61/Velkoz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 22:01:26.000000 Velkoz-0.0.61/Velkoz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-16 22:01:26.000000 Velkoz-0.0.61/Velkoz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 22:01:26.000000 Velkoz-0.0.61/Velkoz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 22:01:26.374920 Velkoz-0.0.61/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 11:05:44.093959 Velkoz-0.1.0/
+-rw-rw-rw-   0        0        0      562 2024-04-19 11:05:44.091948 Velkoz-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 11:05:43.953654 Velkoz-0.1.0/Velkoz/
+-rw-rw-rw-   0        0        0      841 2024-04-17 23:02:52.000000 Velkoz-0.1.0/Velkoz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:05:43.993575 Velkoz-0.1.0/Velkoz/data/
+-rw-rw-rw-   0        0        0       48 2024-04-13 20:58:45.000000 Velkoz-0.1.0/Velkoz/data/__init__.py
+-rw-rw-rw-   0        0        0     2868 2024-04-19 11:03:13.000000 Velkoz-0.1.0/Velkoz/data/champion.py
+-rw-rw-rw-   0        0        0     2245 2024-04-19 11:03:14.000000 Velkoz-0.1.0/Velkoz/data/common.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:05:44.037037 Velkoz-0.1.0/Velkoz/eye/
+-rw-rw-rw-   0        0        0      150 2024-03-23 23:06:35.000000 Velkoz-0.1.0/Velkoz/eye/__init__.py
+-rw-rw-rw-   0        0        0      523 2024-04-10 19:31:41.000000 Velkoz-0.1.0/Velkoz/eye/account.py
+-rw-rw-rw-   0        0        0      930 2024-04-16 21:57:33.000000 Velkoz-0.1.0/Velkoz/eye/champion_mastery.py
+-rw-rw-rw-   0        0        0        8 2024-03-22 13:50:02.000000 Velkoz-0.1.0/Velkoz/eye/common.py
+-rw-rw-rw-   0        0        0     7581 2024-04-12 12:51:42.000000 Velkoz-0.1.0/Velkoz/eye/match.py
+-rw-rw-rw-   0        0        0     1976 2024-04-10 19:31:40.000000 Velkoz-0.1.0/Velkoz/eye/summoner.py
+-rw-rw-rw-   0        0        0     3276 2024-04-16 23:44:45.000000 Velkoz-0.1.0/Velkoz/settings.py
+-rw-rw-rw-   0        0        0      956 2024-04-19 11:04:56.000000 Velkoz-0.1.0/Velkoz/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:05:44.073003 Velkoz-0.1.0/Velkoz/supp/
+-rw-rw-rw-   0        0        0      154 2024-04-16 23:45:00.000000 Velkoz-0.1.0/Velkoz/supp/__init__.py
+-rw-rw-rw-   0        0        0      601 2024-04-10 19:50:35.000000 Velkoz-0.1.0/Velkoz/supp/account.py
+-rw-rw-rw-   0        0        0      280 2024-04-16 23:45:00.000000 Velkoz-0.1.0/Velkoz/supp/champion.py
+-rw-rw-rw-   0        0        0     1165 2024-04-16 21:56:09.000000 Velkoz-0.1.0/Velkoz/supp/champion_mastery.py
+-rw-rw-rw-   0        0        0      270 2024-04-16 23:45:01.000000 Velkoz-0.1.0/Velkoz/supp/match.py
+-rw-rw-rw-   0        0        0     1681 2024-04-10 19:50:14.000000 Velkoz-0.1.0/Velkoz/supp/summoner.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:05:44.089663 Velkoz-0.1.0/Velkoz/tentacles/
+-rw-rw-rw-   0        0        0      213 2024-04-11 21:19:17.000000 Velkoz-0.1.0/Velkoz/tentacles/__init__.py
+-rw-rw-rw-   0        0        0     1208 2024-04-17 15:21:12.000000 Velkoz-0.1.0/Velkoz/tentacles/account.py
+-rw-rw-rw-   0        0        0     3276 2024-04-17 15:22:52.000000 Velkoz-0.1.0/Velkoz/tentacles/champion_mastery.py
+-rw-rw-rw-   0        0        0     4543 2024-04-12 22:57:44.000000 Velkoz-0.1.0/Velkoz/tentacles/common.py
+-rw-rw-rw-   0        0        0       60 2024-04-05 19:09:48.000000 Velkoz-0.1.0/Velkoz/tentacles/config.py
+-rw-rw-rw-   0        0        0     1618 2024-04-17 15:23:09.000000 Velkoz-0.1.0/Velkoz/tentacles/match.py
+-rw-rw-rw-   0        0        0     1389 2024-04-17 15:14:01.000000 Velkoz-0.1.0/Velkoz/tentacles/summoner.py
+-rw-rw-rw-   0        0        0     7331 2024-04-19 11:02:20.000000 Velkoz-0.1.0/Velkoz/velkoz.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:05:44.090315 Velkoz-0.1.0/Velkoz.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-04-19 11:05:43.000000 Velkoz-0.1.0/Velkoz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2024-04-19 11:05:43.000000 Velkoz-0.1.0/Velkoz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:05:43.000000 Velkoz-0.1.0/Velkoz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 11:05:43.000000 Velkoz-0.1.0/Velkoz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-19 11:05:43.000000 Velkoz-0.1.0/Velkoz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 11:05:44.093959 Velkoz-0.1.0/setup.cfg
```

### Comparing `Velkoz-0.0.61/PKG-INFO` & `Velkoz-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.61
+Version: 0.1.0
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Velkoz-0.0.61/Velkoz/__init__.py` & `Velkoz-0.1.0/Velkoz/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,16 @@
         get_all_masteries,
         get_champion_mastery,
         get_top_masteries,
         get_masteryscore,
         get_champion,
         get_champ_image,
         get_champName_by_key,
-        get_key_by_champName
+        get_key_by_champName,
+        write_champion
 
         )
 
 from .settings import *
```

### Comparing `Velkoz-0.0.61/Velkoz/data/champion.py` & `Velkoz-0.1.0/Velkoz/data/champion.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         RiotJson.__init__(self, dto)
         self.champ = kwargs.get('champion', None)
         self.championDto = self.data.get(self.champ, None)
         try:
             self._general(self.championDto)
         except Exception as error:
             print(self.champ)
+            raise Exception(error)
    
     def _general(self, Dto:dict):
         self.id = Dto.get('id', self.champ)
         self.key = Dto.get('key', None)
         self.name = Dto.get('name', None)
         self.title = Dto.get('title', None)
```

### Comparing `Velkoz-0.0.61/Velkoz/data/common.py` & `Velkoz-0.1.0/Velkoz/data/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,23 +40,25 @@
             case _:
                 raise Exception ('Invalid data type')
 
         response = requests.get(path) 
         if response.status_code == 200:
             return response.json()
         else:
+            #print(path)
             raise Exception (f'Invalid response code: {response.status_code}')
 
 
     def _get_champion_image(self, **kwargs):
         get_type = kwargs.get('get_type', 'splash')
         num = kwargs.get('num', 0)
         champ = kwargs.get('champion', 'Aatrox')
         wants_url = kwargs.get('return_url', False)
         path = f'https://ddragon.leagueoflegends.com/cdn/img/champion/{get_type}/{champ}_{num}.jpg'
+        #print(path)
         if wants_url == True:
             return path
         else:
             response = requests.get(path)
             return ImageLoader.open(BytesIO(response.content))
         # return data
```

### Comparing `Velkoz-0.0.61/Velkoz/eye/account.py` & `Velkoz-0.1.0/Velkoz/eye/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.61/Velkoz/eye/champion_mastery.py` & `Velkoz-0.1.0/Velkoz/eye/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.61/Velkoz/eye/match.py` & `Velkoz-0.1.0/Velkoz/eye/match.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.61/Velkoz/eye/summoner.py` & `Velkoz-0.1.0/Velkoz/eye/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.61/Velkoz/settings.py` & `Velkoz-0.1.0/Velkoz/settings.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.61/Velkoz/setup.py` & `Velkoz-0.1.0/Velkoz/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup, find_packages
 
  #python setup.py sdist bdist_wheel
-VERSION = '0.0.61' 
+VERSION = '0.1.0' 
 DESCRIPTION = 'Velkoz Riot Api package'
 LONG_DESCRIPTION = 'Package that uses RiotApi to get information.\n Made to gain experience so it is not something as advanced as the other packages that do the same. Would not recommend.'
 
 # Setting up
 setup(
         name="Velkoz", 
         version=VERSION,
         author="Nabattis",
         author_email="<ferreirafernando6205@gmail.com>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['requests','pillow'], # add any additional packages that 
-        # needs to be installed along with your package. Eg: 'caer'
+        install_requires=['requests','pillow'], # add any additional packages
         
         keywords=['python', 'riotapi', 'api', 'velkoz'],
         classifiers= [
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
         ]
```

### Comparing `Velkoz-0.0.61/Velkoz/supp/account.py` & `Velkoz-0.1.0/Velkoz/supp/account.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.61/Velkoz/supp/champion_mastery.py` & `Velkoz-0.1.0/Velkoz/supp/champion_mastery.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.61/Velkoz/supp/summoner.py` & `Velkoz-0.1.0/Velkoz/supp/summoner.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.61/Velkoz/tentacles/account.py` & `Velkoz-0.1.0/Velkoz/tentacles/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,10 +19,10 @@
             routing = parameters['routing']
             url = f'https://{routing.lower()}.api.riotgames.com/riot/account/v1/accounts/by-puuid/{puuid}'
         else:
             raise Exception ('HOW DID WE GET HERE LMAO')
 
         try:
             return self._get(url=url, parameters=parameters)
-        except requests.exceptions.APINotFoundError as error:
-            return error
+        except Exception as error:
+            raise Exception (error)
```

### Comparing `Velkoz-0.0.61/Velkoz/tentacles/champion_mastery.py` & `Velkoz-0.1.0/Velkoz/tentacles/champion_mastery.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         
         region = parameters['region'].lower()
         puuid = parameters['puuid']
         try:
             url =f'https://{region}.api.riotgames.com/lol/champion-mastery/v4/champion-masteries/by-puuid/{puuid}' 
             return self._get(url=url, parameters=parameters)
 
-        except requests.exceptions.APINotFoundError as error:
-            return error
+        except Exception as error:
+            raise Exception (error)
 
     
     def get_mastery(
         self,
         parameters:dict
     ):
         necessary_parameters={}
@@ -35,16 +35,16 @@
         puuid = parameters['puuid']
         championId = parameters['championId']
         try:
             url = f'https://{region}.api.riotgames.com/lol/champion-mastery/v4/champion-masteries/by-puuid/{puuid}/by-champion/{championId}'
 
             return self._get(url=url, parameters=parameters)
 
-        except requests.exceptions.APINotFoundError as error:
-            return error
+        except Exception as error:
+            raise Exception (error)
 
     def get_top_masteries(
         self,
         parameters:dict
     ):
         necessary_parameters = {}
         needed_parameters = {'puuid', 'region', 'query'}
@@ -62,16 +62,16 @@
         region = parameters['region'].lower()
         puuid = parameters['puuid']
         try:
             url = f'https://{region}.api.riotgames.com/lol/champion-mastery/v4/champion-masteries/by-puuid/{puuid}/top{query_params}'
  
             return self._get(url=url, parameters=parameters)
 
-        except requests.exceptions.APINotFoundError as error:
-            return error
+        except Exception as error:
+            raise Exception (error)
 
     def get_masteryscore(
         self,
         parameters:dict
     ):
         necessary_parameters = {}
         needed_parameters = {'puuid', 'region'}
@@ -82,14 +82,14 @@
         puuid = parameters['puuid']
         region = parameters['region'].lower()
         try:
             url = f'https://{region}.api.riotgames.com/lol/champion-mastery/v4/scores/by-puuid/{puuid}'
 
             return self._get(url=url, parameters=parameters)
 
-        except requests.exceptions.APINotFoundError as error:
-            return error
+        except Exception as error:
+            raise Exception (error)
```

### Comparing `Velkoz-0.0.61/Velkoz/tentacles/common.py` & `Velkoz-0.1.0/Velkoz/tentacles/common.py`

 * *Files identical despite different names*

### Comparing `Velkoz-0.0.61/Velkoz/tentacles/match.py` & `Velkoz-0.1.0/Velkoz/tentacles/summoner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,40 @@
 from .common import RiotApiService
 
-class MatchApi(RiotApiService):
+class SummonerApi(RiotApiService):
 
-    def get_match_list(
+    def get_summoner(
         self,
         parameters:dict
     ):
-        necessary_parameters = {'puuid'}
-        needed_parameters = {'routing', 'query'}
+        necessary_parameters = {'puuid', 'summonerName', 'accountId'}
+        needed_parameters = {'region'}
         are_param_valid = self._validate_parameters(parameters, necessary_parameters, needed_parameters)
         if not are_param_valid: return self._handle_error('Incorrect Parameters')
- 
-        parameters = self._set_defaults(parameters)
-        routing = parameters['routing'].lower()
-        puuid = parameters['puuid']
-        query = parameters['query']
-        try:
-            url = f'https://{routing}.api.riotgames.com/lol/match/v5/matches/by-puuid/{puuid}/{query}'
 
-            return self._get(url=url, parameters=parameters)
+        region = parameters['region'].lower()
+        
+        # Summonerids are not supported because of potential blacklists
+        if 'puuid' in parameters:
+           puuid = parameters['puuid']
+           url = f'https://{region}.api.riotgames.com/lol/summoner/v4/summoners/by-puuid/{puuid}'
+        
+        elif 'summonerName' in parameters:
+            summonerName = parameters['summonerName']
+            url = f'https://{region}.api.riotgames.com/lol/summoner/v4/summoners/by-name/{summonerName}'
+        
+        elif 'accountId' in parameters:
+            accountId = parameters['accountId']
+            url = f'https://{region}.api.riotgames.com/lol/summoner/v4/summoners/by-account/{accountId}' 
 
-        except requests.exceptions.APINotFoundError as error:
-            return error
 
+        else:
+            return 'HOW DID WE EVEN GET HERE'
 
-    # Will have to handle all the info in match accordingly
-    def get_matchDto(
-        self,
-        parameters:dict
-    ):
-        necessary_parameters = {'matchId'}
-        needed_parameters = {'routing'}
-        are_param_valid = self._validate_parameters(parameters, necessary_parameters, needed_parameters)
-        if not are_param_valid: return self._handle_error('Incorrect Parameters')
- 
-
-        routing = parameters['routing'].lower()
-        matchId = parameters['matchId']
 
         try:
-            url = f'https://{routing}.api.riotgames.com/lol/match/v5/matches/{matchId}'
             return self._get(url=url, parameters=parameters)
 
-        except requests.exceptions.APINotFoundError as error:
+        except Exception as error:
             return error
 
 
-
-
```

### Comparing `Velkoz-0.0.61/Velkoz/velkoz.py` & `Velkoz-0.1.0/Velkoz/velkoz.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,29 +174,40 @@
 
     new_puuid = _get_puuid(puuid, riotId, routing)
 
     query = {}
     for key, value in kwargs.items():
         query[key] = value
 
-    return mastery._get_top_masteries(service, puuid=puuid, query=query, region=region)
+    return mastery._get_top_masteries(service, puuid=new_puuid, query=query, region=region)
 
 
 def get_masteryscore(puuid:str='\0', riotId:str='\0',region:str='euw1', routing:str='europe'):
 
     new_puuid = _get_puuid(puuid, riotId, routing)
 
     return mastery._get_masteryscore(service, puuid=new_puuid, region=region)
 
 ############
 # Champion #
 ############
 
+def _format_champion(champion:str):
+    champion = champion.title()
+    if champion == "Bel'Veth" or champion == "Kha'Zix":
+        champion = champion.capitalize()
+    champion = champion.replace("'", "")
+    champion = champion.replace(' ', '')
+    champion = champion.strip()
+    return champion
+
+
 
 def get_champion(champion:str):
+    champion = _format_champion(champion)
     champDto = ddragon._get_data(get_type='champion', champion=champion)
     champ = Champion(ddragon=ddragon, dto=champDto, champion=champion)
     return champ
 
 def get_champ_image(champion:str, **kwargs):
     champ = get_champion(champion)
     return_url = kwargs.get('return_url', False)
@@ -208,29 +219,35 @@
 
         case 'loading':
             image = champ.skins.get_loading(number,return_url)
 
         case 'centered':
             image = champ.skins.get_centered(number,return_url)
 
-        case 'get_tile':
+        case 'tile':
             image = champ.skins.get_tile(number,return_url)
 
         case _:
             raise Exception ('That type of image doesnt exist')
 
     return image
 
 
 def get_champName_by_key(champId:int):
     return all_champion_id.get(champId, None)
 
 def get_key_by_champName(champName:str):
+    champName = _format_champion(champName)
     return (list(all_champion_id.keys())[list(all_champion_id.values()).index(champName)]) 
-            
+
+def write_champion():
+    array = []
+    for value in all_champion_id.values():
+        array.append(value)
+    print(array)
 
 #############
 # DEBUGGING #
 #############
 
 if __name__ == '__main__':
     pass
```

### Comparing `Velkoz-0.0.61/Velkoz.egg-info/PKG-INFO` & `Velkoz-0.1.0/Velkoz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Velkoz
-Version: 0.0.61
+Version: 0.1.0
 Summary: Velkoz Riot Api package
 Author: Nabattis
 Author-email: <ferreirafernando6205@gmail.com>
 Keywords: python,riotapi,api,velkoz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Velkoz-0.0.61/Velkoz.egg-info/SOURCES.txt` & `Velkoz-0.1.0/Velkoz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

