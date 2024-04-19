# Comparing `tmp/gm_termcontrol-0.0.2.tar.gz` & `tmp/gm_termcontrol-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gm_termcontrol-0.0.2.tar", last modified: Thu Feb 29 18:10:14 2024, max compression
+gzip compressed data, was "gm_termcontrol-0.0.3.tar", last modified: Fri Apr 19 02:09:24 2024, max compression
```

## Comparing `gm_termcontrol-0.0.2.tar` & `gm_termcontrol-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-02-29 18:10:14.138982 gm_termcontrol-0.0.2/
--rw-------   0 u0_a237  (10237) u0_a237  (10237)    35149 2024-02-29 16:00:11.000000 gm_termcontrol-0.0.2/LICENSE
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      590 2024-02-29 18:10:14.138982 gm_termcontrol-0.0.2/PKG-INFO
--rw-------   0 u0_a237  (10237) u0_a237  (10237)       60 2024-02-29 17:33:53.000000 gm_termcontrol-0.0.2/README.md
-drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-02-29 18:10:14.134981 gm_termcontrol-0.0.2/gm_termcontrol/
--rw-------   0 u0_a237  (10237) u0_a237  (10237)    31704 2024-02-29 18:10:13.000000 gm_termcontrol-0.0.2/gm_termcontrol/__init__.py
--rw-------   0 u0_a237  (10237) u0_a237  (10237)    31704 2024-02-29 16:00:11.000000 gm_termcontrol-0.0.2/gm_termcontrol/termcontrol.py
-drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-02-29 18:10:14.138982 gm_termcontrol-0.0.2/gm_termcontrol.egg-info/
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      590 2024-02-29 18:10:13.000000 gm_termcontrol-0.0.2/gm_termcontrol.egg-info/PKG-INFO
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      297 2024-02-29 18:10:14.000000 gm_termcontrol-0.0.2/gm_termcontrol.egg-info/SOURCES.txt
--rw-------   0 u0_a237  (10237) u0_a237  (10237)        1 2024-02-29 18:10:13.000000 gm_termcontrol-0.0.2/gm_termcontrol.egg-info/dependency_links.txt
--rw-------   0 u0_a237  (10237) u0_a237  (10237)        5 2024-02-29 18:10:13.000000 gm_termcontrol-0.0.2/gm_termcontrol.egg-info/requires.txt
--rw-------   0 u0_a237  (10237) u0_a237  (10237)       15 2024-02-29 18:10:13.000000 gm_termcontrol-0.0.2/gm_termcontrol.egg-info/top_level.txt
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      145 2024-02-29 17:19:45.000000 gm_termcontrol-0.0.2/pyproject.toml
--rw-------   0 u0_a237  (10237) u0_a237  (10237)      576 2024-02-29 18:10:14.138982 gm_termcontrol-0.0.2/setup.cfg
--rwx------   0 u0_a237  (10237) u0_a237  (10237)      717 2024-02-29 18:09:45.000000 gm_termcontrol-0.0.2/setup.py
+drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-04-19 02:09:24.119636 gm_termcontrol-0.0.3/
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)    35149 2024-02-29 16:00:11.000000 gm_termcontrol-0.0.3/LICENSE
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      590 2024-04-19 02:09:24.123636 gm_termcontrol-0.0.3/PKG-INFO
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)       60 2024-02-29 17:33:53.000000 gm_termcontrol-0.0.3/README.md
+drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-04-19 02:09:24.119636 gm_termcontrol-0.0.3/gm_termcontrol/
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)    31837 2024-04-19 02:09:23.000000 gm_termcontrol-0.0.3/gm_termcontrol/__init__.py
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)    31837 2024-04-19 02:05:33.000000 gm_termcontrol-0.0.3/gm_termcontrol/termcontrol.py
+drwx------   0 u0_a237  (10237) u0_a237  (10237)        0 2024-04-19 02:09:24.119636 gm_termcontrol-0.0.3/gm_termcontrol.egg-info/
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      590 2024-04-19 02:09:23.000000 gm_termcontrol-0.0.3/gm_termcontrol.egg-info/PKG-INFO
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      297 2024-04-19 02:09:23.000000 gm_termcontrol-0.0.3/gm_termcontrol.egg-info/SOURCES.txt
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)        1 2024-04-19 02:09:23.000000 gm_termcontrol-0.0.3/gm_termcontrol.egg-info/dependency_links.txt
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)        5 2024-04-19 02:09:23.000000 gm_termcontrol-0.0.3/gm_termcontrol.egg-info/requires.txt
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)       15 2024-04-19 02:09:23.000000 gm_termcontrol-0.0.3/gm_termcontrol.egg-info/top_level.txt
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      145 2024-02-29 17:19:45.000000 gm_termcontrol-0.0.3/pyproject.toml
+-rw-------   0 u0_a237  (10237) u0_a237  (10237)      576 2024-04-19 02:09:24.123636 gm_termcontrol-0.0.3/setup.cfg
+-rwx------   0 u0_a237  (10237) u0_a237  (10237)      717 2024-04-19 02:05:33.000000 gm_termcontrol-0.0.3/setup.py
```

### Comparing `gm_termcontrol-0.0.2/LICENSE` & `gm_termcontrol-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gm_termcontrol-0.0.2/PKG-INFO` & `gm_termcontrol-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gm_termcontrol
-Version: 0.0.2
+Version: 0.0.3
 Summary: python terminal control and basïc gui
 Home-page: https://github.com/gretchycat/termcontrol
 Author: Gretchen Maculo
 Author-email: gretchen.maculo@gmail.com
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gm_termcontrol-0.0.2/gm_termcontrol/__init__.py` & `gm_termcontrol-0.0.3/gm_termcontrol/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -625,39 +625,40 @@
 
     def __del__(self):
         pass
 
     def checkWidgetEvents(self, key, w):
         if key!='':
             esc='\x1b'
-            print(f'{self.t.gotoxy(10,19)}  {key.replace(esc, "<")}         ')
+            #print(f'{self.t.gotoxy(10,19)}  {key.replace(esc, "<")}         ')
         if w.key==key:
             if f'{type(self.action)}' in [ "function", "<class 'method'>" ]:
                 self.invert=True
                 self.action()
             else:
                 print(f'{self.t.gotoxy(10,20)}invalid action for "{key}" type: {type(self.action)}             ')
         for cw in w.widgetList:
             cw.checkWidgetEvents(key, cw)
 
     def guiLoop(self):
-        go=True
-        self.t.disable_cursor()
-        self.t.enable_mouse()
+        self.go=True
+        print(self.t.disable_cursor(), end='')
+        print(self.t.enable_mouse(), end='')
+        print(self.t.alt_screen(), end='')
         buffercache=""
-        while go:
+        while self.go:
             buffer=self.draw()
             if buffer != buffercache:
                 buffercache=buffer
                 print(buffer, end='')
-            #print("\n"*3)
             key=self.kb.read_keyboard_input()
             self.checkWidgetEvents(key, self)
-        self.t.enable_cursor()
-        self.t.disable_mouse()
+        print(self.t.enable_cursor(), end='')
+        print(self.t.disable_mouse(), end='')
+        print(self.t.normal_screen(), end='')
 
     def quit(self):
         exit(0)
 
     def setColors(self, fg, bg):
         self.fg, self.bg=fg, bg
```

### Comparing `gm_termcontrol-0.0.2/gm_termcontrol/termcontrol.py` & `gm_termcontrol-0.0.3/gm_termcontrol/termcontrol.py`

 * *Files 2% similar despite different names*

```diff
@@ -625,39 +625,40 @@
 
     def __del__(self):
         pass
 
     def checkWidgetEvents(self, key, w):
         if key!='':
             esc='\x1b'
-            print(f'{self.t.gotoxy(10,19)}  {key.replace(esc, "<")}         ')
+            #print(f'{self.t.gotoxy(10,19)}  {key.replace(esc, "<")}         ')
         if w.key==key:
             if f'{type(self.action)}' in [ "function", "<class 'method'>" ]:
                 self.invert=True
                 self.action()
             else:
                 print(f'{self.t.gotoxy(10,20)}invalid action for "{key}" type: {type(self.action)}             ')
         for cw in w.widgetList:
             cw.checkWidgetEvents(key, cw)
 
     def guiLoop(self):
-        go=True
-        self.t.disable_cursor()
-        self.t.enable_mouse()
+        self.go=True
+        print(self.t.disable_cursor(), end='')
+        print(self.t.enable_mouse(), end='')
+        print(self.t.alt_screen(), end='')
         buffercache=""
-        while go:
+        while self.go:
             buffer=self.draw()
             if buffer != buffercache:
                 buffercache=buffer
                 print(buffer, end='')
-            #print("\n"*3)
             key=self.kb.read_keyboard_input()
             self.checkWidgetEvents(key, self)
-        self.t.enable_cursor()
-        self.t.disable_mouse()
+        print(self.t.enable_cursor(), end='')
+        print(self.t.disable_mouse(), end='')
+        print(self.t.normal_screen(), end='')
 
     def quit(self):
         exit(0)
 
     def setColors(self, fg, bg):
         self.fg, self.bg=fg, bg
```

### Comparing `gm_termcontrol-0.0.2/gm_termcontrol.egg-info/PKG-INFO` & `gm_termcontrol-0.0.3/gm_termcontrol.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gm-termcontrol
-Version: 0.0.2
+Version: 0.0.3
 Summary: python terminal control and basïc gui
 Home-page: https://github.com/gretchycat/termcontrol
 Author: Gretchen Maculo
 Author-email: gretchen.maculo@gmail.com
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gm_termcontrol-0.0.2/setup.cfg` & `gm_termcontrol-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gm_termcontrol
-version = 0.0.2
+version = 0.0.3
 url = https://github.com/gretchycat/termcontrol
 author = Gretchen Maculo
 author_email = gretchen.maculo@gmail.com
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
```

### Comparing `gm_termcontrol-0.0.2/setup.py` & `gm_termcontrol-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 shutil.copyfile('gm_termcontrol/termcontrol.py', 'gm_termcontrol/__init__.py')
 
 setup(
     name='gm_termcontrol',
-    version='0.0.2',
+    version='0.0.3',
     license='GPL3',
     url='https://github.com/gretchycat/termcontrol',
     author='Gretchen Maculo',
     author_email='gretchen.maculo@gmail.com',
     description='python terminal control and basïc gui',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

