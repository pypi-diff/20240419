# Comparing `tmp/HelloPyOnly-0.1.22.tar.gz` & `tmp/HelloPyOnly-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HelloPyOnly-0.1.22.tar", last modified: Fri Feb 23 04:32:26 2024, max compression
+gzip compressed data, was "HelloPyOnly-0.1.23.tar", last modified: Fri Apr 19 07:23:41 2024, max compression
```

## Comparing `HelloPyOnly-0.1.22.tar` & `HelloPyOnly-0.1.23.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 04:32:26.330876 HelloPyOnly-0.1.22/
-drwxrwxrwx   0        0        0        0 2024-02-23 04:32:26.317287 HelloPyOnly-0.1.22/HelloPyOnly.egg-info/
--rw-rw-rw-   0        0        0      553 2024-02-23 04:32:26.000000 HelloPyOnly-0.1.22/HelloPyOnly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      723 2024-02-23 04:32:26.000000 HelloPyOnly-0.1.22/HelloPyOnly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 04:32:26.000000 HelloPyOnly-0.1.22/HelloPyOnly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-02-23 04:32:26.000000 HelloPyOnly-0.1.22/HelloPyOnly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-02-23 04:32:26.000000 HelloPyOnly-0.1.22/HelloPyOnly.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      553 2024-02-23 04:32:26.330876 HelloPyOnly-0.1.22/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-23 04:32:26.323856 HelloPyOnly-0.1.22/hellopy/
--rw-rw-rw-   0        0        0     2064 2023-12-02 03:15:10.000000 HelloPyOnly-0.1.22/hellopy/__init__.py
--rw-rw-rw-   0        0        0     4597 2023-10-20 05:46:44.000000 HelloPyOnly-0.1.22/hellopy/collision.py
--rw-rw-rw-   0        0        0      268 2023-12-02 03:24:54.000000 HelloPyOnly-0.1.22/hellopy/demo.py
--rw-rw-rw-   0        0        0     2773 2023-10-17 14:39:56.000000 HelloPyOnly-0.1.22/hellopy/events.py
-drwxrwxrwx   0        0        0        0 2024-02-23 04:32:26.328856 HelloPyOnly-0.1.22/hellopy/gameobject/
--rw-rw-rw-   0        0        0      389 2023-10-18 06:44:19.000000 HelloPyOnly-0.1.22/hellopy/gameobject/__init__.py
--rw-rw-rw-   0        0        0     2051 2023-10-17 08:13:10.000000 HelloPyOnly-0.1.22/hellopy/gameobject/circle.py
--rw-rw-rw-   0        0        0      220 2023-10-17 06:43:33.000000 HelloPyOnly-0.1.22/hellopy/gameobject/ellipse.py
--rw-rw-rw-   0        0        0      384 2023-10-16 07:28:41.000000 HelloPyOnly-0.1.22/hellopy/gameobject/gameobject.py
--rw-rw-rw-   0        0        0     2467 2023-10-17 06:43:38.000000 HelloPyOnly-0.1.22/hellopy/gameobject/line.py
--rw-rw-rw-   0        0        0     3676 2023-12-28 02:51:59.000000 HelloPyOnly-0.1.22/hellopy/gameobject/polygon.py
--rw-rw-rw-   0        0        0      545 2023-10-19 01:46:38.000000 HelloPyOnly-0.1.22/hellopy/gameobject/rectangle.py
--rw-rw-rw-   0        0        0    10480 2024-02-18 06:06:47.000000 HelloPyOnly-0.1.22/hellopy/gameobject/sprite.py
--rw-rw-rw-   0        0        0     2777 2024-01-06 08:20:48.000000 HelloPyOnly-0.1.22/hellopy/gameobject/text.py
--rw-rw-rw-   0        0        0      649 2023-12-27 01:58:30.000000 HelloPyOnly-0.1.22/hellopy/gameobject/triangle.py
--rw-rw-rw-   0        0        0      258 2023-10-17 06:30:34.000000 HelloPyOnly-0.1.22/hellopy/key.py
--rw-rw-rw-   0        0        0      136 2023-10-16 05:53:09.000000 HelloPyOnly-0.1.22/hellopy/mouse.py
--rw-rw-rw-   0        0        0     1882 2023-10-20 05:46:53.000000 HelloPyOnly-0.1.22/hellopy/resource.py
--rw-rw-rw-   0        0        0      388 2023-10-18 06:58:07.000000 HelloPyOnly-0.1.22/hellopy/sound.py
--rw-rw-rw-   0        0        0      341 2023-10-17 06:42:53.000000 HelloPyOnly-0.1.22/hellopy/util.py
--rw-rw-rw-   0        0        0     3164 2024-01-04 03:37:58.000000 HelloPyOnly-0.1.22/hellopy/window.py
-drwxrwxrwx   0        0        0        0 2024-02-23 04:32:26.329856 HelloPyOnly-0.1.22/onlydemos/
--rw-rw-rw-   0        0        0     5950 2024-02-23 04:30:43.000000 HelloPyOnly-0.1.22/onlydemos/LoongPy.py
--rw-rw-rw-   0        0        0     1797 2023-10-20 05:45:56.000000 HelloPyOnly-0.1.22/onlydemos/__init__.py
--rw-rw-rw-   0        0        0     4352 2023-10-20 07:23:57.000000 HelloPyOnly-0.1.22/onlydemos/pumpkin.py
--rw-rw-rw-   0        0        0       42 2024-02-23 04:32:26.330876 HelloPyOnly-0.1.22/setup.cfg
--rw-rw-rw-   0        0        0     1049 2024-02-23 04:31:05.000000 HelloPyOnly-0.1.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.931085 HelloPyOnly-0.1.23/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.717260 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-19 07:23:41.000000 HelloPyOnly-0.1.23/HelloPyOnly.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      553 2024-04-19 07:23:41.930078 HelloPyOnly-0.1.23/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.819614 HelloPyOnly-0.1.23/hellopy/
+-rw-rw-rw-   0        0        0     2064 2023-12-02 03:15:10.000000 HelloPyOnly-0.1.23/hellopy/__init__.py
+-rw-rw-rw-   0        0        0     4597 2023-10-20 05:46:44.000000 HelloPyOnly-0.1.23/hellopy/collision.py
+-rw-rw-rw-   0        0        0      268 2023-12-02 03:24:54.000000 HelloPyOnly-0.1.23/hellopy/demo.py
+-rw-rw-rw-   0        0        0     2773 2023-10-17 14:39:56.000000 HelloPyOnly-0.1.23/hellopy/events.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.925070 HelloPyOnly-0.1.23/hellopy/gameobject/
+-rw-rw-rw-   0        0        0      389 2023-10-18 06:44:19.000000 HelloPyOnly-0.1.23/hellopy/gameobject/__init__.py
+-rw-rw-rw-   0        0        0     2051 2023-10-17 08:13:10.000000 HelloPyOnly-0.1.23/hellopy/gameobject/circle.py
+-rw-rw-rw-   0        0        0      220 2023-10-17 06:43:33.000000 HelloPyOnly-0.1.23/hellopy/gameobject/ellipse.py
+-rw-rw-rw-   0        0        0      384 2023-10-16 07:28:41.000000 HelloPyOnly-0.1.23/hellopy/gameobject/gameobject.py
+-rw-rw-rw-   0        0        0     2467 2023-10-17 06:43:38.000000 HelloPyOnly-0.1.23/hellopy/gameobject/line.py
+-rw-rw-rw-   0        0        0     3676 2023-12-28 02:51:59.000000 HelloPyOnly-0.1.23/hellopy/gameobject/polygon.py
+-rw-rw-rw-   0        0        0      545 2023-10-19 01:46:38.000000 HelloPyOnly-0.1.23/hellopy/gameobject/rectangle.py
+-rw-rw-rw-   0        0        0    10478 2024-04-06 00:45:00.000000 HelloPyOnly-0.1.23/hellopy/gameobject/sprite.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 00:29:09.000000 HelloPyOnly-0.1.23/hellopy/gameobject/test.py
+-rw-rw-rw-   0        0        0     2777 2024-01-06 08:20:48.000000 HelloPyOnly-0.1.23/hellopy/gameobject/text.py
+-rw-rw-rw-   0        0        0      649 2023-12-27 01:58:30.000000 HelloPyOnly-0.1.23/hellopy/gameobject/triangle.py
+-rw-rw-rw-   0        0        0      258 2023-10-17 06:30:34.000000 HelloPyOnly-0.1.23/hellopy/key.py
+-rw-rw-rw-   0        0        0      136 2023-10-16 05:53:09.000000 HelloPyOnly-0.1.23/hellopy/mouse.py
+-rw-rw-rw-   0        0        0     1882 2023-10-20 05:46:53.000000 HelloPyOnly-0.1.23/hellopy/resource.py
+-rw-rw-rw-   0        0        0      388 2023-10-18 06:58:07.000000 HelloPyOnly-0.1.23/hellopy/sound.py
+-rw-rw-rw-   0        0        0      341 2023-10-17 06:42:53.000000 HelloPyOnly-0.1.23/hellopy/util.py
+-rw-rw-rw-   0        0        0     3164 2024-01-04 03:37:58.000000 HelloPyOnly-0.1.23/hellopy/window.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:23:41.929080 HelloPyOnly-0.1.23/onlydemos/
+-rw-rw-rw-   0        0        0     5983 2024-04-19 07:19:44.000000 HelloPyOnly-0.1.23/onlydemos/LoongPy.py
+-rw-rw-rw-   0        0        0     1797 2023-10-20 05:45:56.000000 HelloPyOnly-0.1.23/onlydemos/__init__.py
+-rw-rw-rw-   0        0        0     4352 2023-10-20 07:23:57.000000 HelloPyOnly-0.1.23/onlydemos/pumpkin.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:23:41.931085 HelloPyOnly-0.1.23/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2024-04-19 07:23:14.000000 HelloPyOnly-0.1.23/setup.py
```

### Comparing `HelloPyOnly-0.1.22/HelloPyOnly.egg-info/PKG-INFO` & `HelloPyOnly-0.1.23/HelloPyOnly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HelloPyOnly
-Version: 0.1.22
+Version: 0.1.23
 Summary: This is the game engine of Only Hello Science project.
 Home-page: https://github.com/zfan0311/hellopy.git
 Author: funk.zhang
 Author-email: zhangfangid@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `HelloPyOnly-0.1.22/HelloPyOnly.egg-info/SOURCES.txt` & `HelloPyOnly-0.1.23/HelloPyOnly.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 hellopy/gameobject/circle.py
 hellopy/gameobject/ellipse.py
 hellopy/gameobject/gameobject.py
 hellopy/gameobject/line.py
 hellopy/gameobject/polygon.py
 hellopy/gameobject/rectangle.py
 hellopy/gameobject/sprite.py
+hellopy/gameobject/test.py
 hellopy/gameobject/text.py
 hellopy/gameobject/triangle.py
 onlydemos/LoongPy.py
 onlydemos/__init__.py
 onlydemos/pumpkin.py
```

### Comparing `HelloPyOnly-0.1.22/PKG-INFO` & `HelloPyOnly-0.1.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HelloPyOnly
-Version: 0.1.22
+Version: 0.1.23
 Summary: This is the game engine of Only Hello Science project.
 Home-page: https://github.com/zfan0311/hellopy.git
 Author: funk.zhang
 Author-email: zhangfangid@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `HelloPyOnly-0.1.22/hellopy/__init__.py` & `HelloPyOnly-0.1.23/hellopy/__init__.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/collision.py` & `HelloPyOnly-0.1.23/hellopy/collision.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/events.py` & `HelloPyOnly-0.1.23/hellopy/events.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/gameobject/circle.py` & `HelloPyOnly-0.1.23/hellopy/gameobject/circle.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/gameobject/line.py` & `HelloPyOnly-0.1.23/hellopy/gameobject/line.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/gameobject/polygon.py` & `HelloPyOnly-0.1.23/hellopy/gameobject/polygon.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/gameobject/rectangle.py` & `HelloPyOnly-0.1.23/hellopy/gameobject/rectangle.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/gameobject/sprite.py` & `HelloPyOnly-0.1.23/hellopy/gameobject/sprite.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from hellopy.gameobject.gameobject import GameObject, rotate_point
 from hellopy.collision import CollisionComponent
 from hellopy.window import window
 from hellopy.resource import rss
 
 cache_images = {}
 
-
 # 绘制图片
 def image(x=100, y=200, width=100,height=100,src="./hellopy/src/images/HelloScienceLogo.png"):
     img = pygame.image.load(rss.get(src))
     img = pygame.transform.scale(img,(width,height))
     window.screen.blit(img,(x-width/2, y-height/2))
 
 # 精灵类
```

### Comparing `HelloPyOnly-0.1.22/hellopy/gameobject/text.py` & `HelloPyOnly-0.1.23/hellopy/gameobject/text.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/gameobject/triangle.py` & `HelloPyOnly-0.1.23/hellopy/gameobject/triangle.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/resource.py` & `HelloPyOnly-0.1.23/hellopy/resource.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/hellopy/window.py` & `HelloPyOnly-0.1.23/hellopy/window.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/onlydemos/LoongPy.py` & `HelloPyOnly-0.1.23/onlydemos/LoongPy.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         self.tail = Sprite(self.bodys[-1].x-65,self.bodys[-1].y,110,45,"https://pic.imgdb.cn/item/65d19e369f345e8d03507793.png")
         self.bodys.append(self.tail)
         self.foot1 = Sprite(100,100,60,120,"https://pic.imgdb.cn/item/65d5b5569f345e8d035dd171.png")
         self.foot2 = Sprite(100,100,60,120,"https://pic.imgdb.cn/item/65d5b5569f345e8d035dd171.png")
     
     # 绘制龙    
     def draw(self):
+        self.head_to(self.head)
         for item in self.bodys[-1::-1]:
             item.draw()
         self.foot1.draw()
         self.foot2.draw()
     
     # 移动龙
     def head_to(self, target):
```

### Comparing `HelloPyOnly-0.1.22/onlydemos/__init__.py` & `HelloPyOnly-0.1.23/onlydemos/__init__.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/onlydemos/pumpkin.py` & `HelloPyOnly-0.1.23/onlydemos/pumpkin.py`

 * *Files identical despite different names*

### Comparing `HelloPyOnly-0.1.22/setup.py` & `HelloPyOnly-0.1.23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HelloPyOnly',  # 您的库的名称
-    version='0.1.22',  # 版本号
+    version='0.1.23',  # 版本号
     author='funk.zhang',  # 您的名字
     author_email='zhangfangid@126.com',  # 您的电子邮件地址
     description='This is the game engine of Only Hello Science project.',  # 您库的简短描述
     long_description='This is the game engine of Only Hello Science project. Based on pygame.',  # 更详细的描述
     # long_description_content_type='text/markdown',  # 描述类型（通常为Markdown）
     url='https://github.com/zfan0311/hellopy.git',  # 您库的代码托管URL
     packages=find_packages(),  # 包含的Python包
```

