# Comparing `tmp/ele2364-0.1.0.tar.gz` & `tmp/ele2364-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ele2364-0.1.0.tar", last modified: Fri Feb  2 16:11:01 2024, max compression
+gzip compressed data, was "ele2364-0.1.1.tar", last modified: Fri Apr 19 14:23:02 2024, max compression
```

## Comparing `ele2364-0.1.0.tar` & `ele2364-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,54 @@
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-02-02 16:11:01.732041 ele2364-0.1.0/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     1123 2024-02-02 16:01:48.000000 ele2364-0.1.0/LICENSE
--rw-r--r--   0 wouter    (1000) wouter    (1000)     2632 2024-02-02 16:11:01.732041 ele2364-0.1.0/PKG-INFO
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     1962 2024-02-02 16:01:25.000000 ele2364-0.1.0/README.md
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-02-02 16:11:01.728041 ele2364-0.1.0/ele2364/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     4775 2024-02-01 17:28:48.000000 ele2364-0.1.0/ele2364/__init__.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     9823 2024-02-02 13:46:55.000000 ele2364-0.1.0/ele2364/environments.py
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-02-02 16:11:01.728041 ele2364-0.1.0/ele2364/flappy_bird_gym/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     1751 2024-02-01 18:32:57.000000 ele2364-0.1.0/ele2364/flappy_bird_gym/__init__.py
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-02-02 16:11:01.732041 ele2364-0.1.0/ele2364/flappy_bird_gym/envs/
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     1286 2024-01-30 18:13:58.000000 ele2364-0.1.0/ele2364/flappy_bird_gym/envs/__init__.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     7045 2024-02-02 13:47:05.000000 ele2364-0.1.0/ele2364/flappy_bird_gym/envs/flappy_bird_env_simple.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     9911 2023-02-15 12:26:21.000000 ele2364-0.1.0/ele2364/flappy_bird_gym/envs/game_logic.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     7123 2024-01-30 18:14:43.000000 ele2364-0.1.0/ele2364/flappy_bird_gym/envs/renderer.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)     5870 2023-02-14 19:48:18.000000 ele2364-0.1.0/ele2364/flappy_bird_gym/envs/utils.py
--rw-rw-r--   0 wouter    (1000) wouter    (1000)    14029 2024-02-01 19:29:42.000000 ele2364-0.1.0/ele2364/networks.py
-drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-02-02 16:11:01.732041 ele2364-0.1.0/ele2364.egg-info/
--rw-r--r--   0 wouter    (1000) wouter    (1000)     2632 2024-02-02 16:11:01.000000 ele2364-0.1.0/ele2364.egg-info/PKG-INFO
--rw-rw-r--   0 wouter    (1000) wouter    (1000)      498 2024-02-02 16:11:01.000000 ele2364-0.1.0/ele2364.egg-info/SOURCES.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)        1 2024-02-02 16:11:01.000000 ele2364-0.1.0/ele2364.egg-info/dependency_links.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       29 2024-02-02 16:11:01.000000 ele2364-0.1.0/ele2364.egg-info/requires.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)        8 2024-02-02 16:11:01.000000 ele2364-0.1.0/ele2364.egg-info/top_level.txt
--rw-rw-r--   0 wouter    (1000) wouter    (1000)       38 2024-02-02 16:11:01.732041 ele2364-0.1.0/setup.cfg
--rw-rw-r--   0 wouter    (1000) wouter    (1000)      960 2024-02-02 16:00:37.000000 ele2364-0.1.0/setup.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-04-19 14:23:02.719379 ele2364-0.1.1/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1123 2024-02-02 16:01:48.000000 ele2364-0.1.1/LICENSE
+-rw-r--r--   0 wouter    (1000) wouter    (1000)     2632 2024-04-19 14:23:02.719379 ele2364-0.1.1/PKG-INFO
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1962 2024-02-02 16:01:25.000000 ele2364-0.1.1/README.md
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-04-19 14:23:02.671378 ele2364-0.1.1/ele2364/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     4775 2024-02-01 17:28:48.000000 ele2364-0.1.1/ele2364/__init__.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     9866 2024-02-07 14:11:41.000000 ele2364-0.1.1/ele2364/environments.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-04-19 14:23:02.671378 ele2364-0.1.1/ele2364/flappy_bird_gym/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1751 2024-02-01 18:32:57.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/__init__.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-04-19 14:23:02.671378 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)        0 2024-04-19 14:22:44.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/__init__.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-04-19 14:23:02.715379 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      339 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/0.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      336 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/1.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      345 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/2.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      339 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/3.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      346 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/4.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      345 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/5.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      344 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/6.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      345 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/7.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      338 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/8.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      343 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/9.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)        0 2024-04-19 14:22:38.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/__init__.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     7026 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/background-day.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1101 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/background-night.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      470 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/base.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      431 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/bluebird-downflap.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      430 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/bluebird-midflap.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      431 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/bluebird-upflap.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      758 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/gameover.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1602 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/message.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     2527 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/pipe-green.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     2439 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/pipe-red.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      425 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/redbird-downflap.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      426 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/redbird-midflap.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      425 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/redbird-upflap.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      426 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/yellowbird-downflap.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      425 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/yellowbird-midflap.png
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      427 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/assets/sprites/yellowbird-upflap.png
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-04-19 14:23:02.719379 ele2364-0.1.1/ele2364/flappy_bird_gym/envs/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1286 2024-01-30 18:13:58.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/envs/__init__.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     7045 2024-02-02 13:47:05.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/envs/flappy_bird_env_simple.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     9911 2023-02-15 12:26:21.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/envs/game_logic.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     7123 2024-01-30 18:14:43.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/envs/renderer.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     5870 2023-02-14 19:48:18.000000 ele2364-0.1.1/ele2364/flappy_bird_gym/envs/utils.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)    14029 2024-02-01 19:29:42.000000 ele2364-0.1.1/ele2364/networks.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2024-04-19 14:23:02.719379 ele2364-0.1.1/ele2364.egg-info/
+-rw-r--r--   0 wouter    (1000) wouter    (1000)     2632 2024-04-19 14:23:02.000000 ele2364-0.1.1/ele2364.egg-info/PKG-INFO
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1960 2024-04-19 14:23:02.000000 ele2364-0.1.1/ele2364.egg-info/SOURCES.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)        1 2024-04-19 14:23:02.000000 ele2364-0.1.1/ele2364.egg-info/dependency_links.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       29 2024-04-19 14:23:02.000000 ele2364-0.1.1/ele2364.egg-info/requires.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)        8 2024-04-19 14:23:02.000000 ele2364-0.1.1/ele2364.egg-info/top_level.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       38 2024-04-19 14:23:02.719379 ele2364-0.1.1/setup.cfg
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1034 2024-04-19 14:18:19.000000 ele2364-0.1.1/setup.py
```

### Comparing `ele2364-0.1.0/LICENSE` & `ele2364-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/PKG-INFO` & `ele2364-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ele2364
-Version: 0.1.0
+Version: 0.1.1
 Summary: ELE2364 (reinforcement learning) support package
 Home-page: http://github.com/wcaarls/ele2364
 Author: Wouter Caarls
 Author-email: wouter@puc-rio.br
 License: MIT
 Keywords: reinforcement learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ele2364-0.1.0/README.md` & `ele2364-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/ele2364/__init__.py` & `ele2364-0.1.1/ele2364/__init__.py`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/ele2364/environments.py` & `ele2364-0.1.1/ele2364/environments.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,18 @@
            obs = env.reset() returns the start state observation.
         """
         return self.env.reset()[0]
     
     def step(self, u):
         """Step environment.
         
-           obs, r, done, info = env.step(u) takes action u and
-           returns the next state observation, reward, whether
-           the episode terminated, and extra information.
+           obs, r, terminal, truncated, info = env.step(u) takes
+           action u and returns the next state observation, reward,
+           whether the episode terminated or was truncated, and
+           extra information.
         """
         observation, reward, terminal, truncated, info = self.env.step(u)
         return (observation, reward, terminal, truncated, info)
     
     def render(self):
         """Render environment.
```

### Comparing `ele2364-0.1.0/ele2364/flappy_bird_gym/__init__.py` & `ele2364-0.1.1/ele2364/flappy_bird_gym/__init__.py`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/ele2364/flappy_bird_gym/envs/__init__.py` & `ele2364-0.1.1/ele2364/flappy_bird_gym/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/ele2364/flappy_bird_gym/envs/flappy_bird_env_simple.py` & `ele2364-0.1.1/ele2364/flappy_bird_gym/envs/flappy_bird_env_simple.py`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/ele2364/flappy_bird_gym/envs/game_logic.py` & `ele2364-0.1.1/ele2364/flappy_bird_gym/envs/game_logic.py`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/ele2364/flappy_bird_gym/envs/renderer.py` & `ele2364-0.1.1/ele2364/flappy_bird_gym/envs/renderer.py`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/ele2364/flappy_bird_gym/envs/utils.py` & `ele2364-0.1.1/ele2364/flappy_bird_gym/envs/utils.py`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/ele2364/networks.py` & `ele2364-0.1.1/ele2364/networks.py`

 * *Files identical despite different names*

### Comparing `ele2364-0.1.0/ele2364.egg-info/PKG-INFO` & `ele2364-0.1.1/ele2364.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ele2364
-Version: 0.1.0
+Version: 0.1.1
 Summary: ELE2364 (reinforcement learning) support package
 Home-page: http://github.com/wcaarls/ele2364
 Author: Wouter Caarls
 Author-email: wouter@puc-rio.br
 License: MIT
 Keywords: reinforcement learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ele2364-0.1.0/setup.py` & `ele2364-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     with open('README.md', 'r') as fh:
         long_description = fh.read()
 except:
     long_description = ''
 
 setup(name='ele2364',
-      version='0.1.0',
+      version='0.1.1',
       description='ELE2364 (reinforcement learning) support package',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='http://github.com/wcaarls/ele2364',
       author='Wouter Caarls',
       author_email='wouter@puc-rio.br',
       license='MIT',
@@ -20,10 +20,11 @@
       'License :: OSI Approved :: MIT License',
       'Programming Language :: Python :: 3',
       'Topic :: Education',
       'Topic :: Scientific/Engineering :: Artificial Intelligence',
       ],
       keywords='reinforcement learning',
       packages=find_packages(),
+      package_data={'ele2364.flappy_bird_gym.assets.sprites': ['*.png']},
       install_requires=['numpy', 'gymnasium', 'torch >= 2.1.0'],
       entry_points = {}
      )
```

