# Comparing `tmp/doppkit-0.4rc1.tar.gz` & `tmp/doppkit-0.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppkit-0.4rc1.tar", last modified: Fri Apr 12 19:30:35 2024, max compression
+gzip compressed data, was "doppkit-0.4.0rc2.tar", last modified: Fri Apr 19 19:09:52 2024, max compression
```

## Comparing `doppkit-0.4rc1.tar` & `doppkit-0.4.0rc2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:30:35.573920 doppkit-0.4rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 19:30:25.000000 doppkit-0.4rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-12 19:30:35.573920 doppkit-0.4rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-12 19:30:25.000000 doppkit-0.4rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:30:35.573920 doppkit-0.4rc1/doppkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-12 19:30:35.000000 doppkit-0.4rc1/doppkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 19:30:35.000000 doppkit-0.4rc1/doppkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:30:35.000000 doppkit-0.4rc1/doppkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-12 19:30:35.000000 doppkit-0.4rc1/doppkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 19:30:35.000000 doppkit-0.4rc1/doppkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 19:30:35.000000 doppkit-0.4rc1/doppkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-12 19:30:25.000000 doppkit-0.4rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:30:35.573920 doppkit-0.4rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:30:35.565920 doppkit-0.4rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:30:35.569920 doppkit-0.4rc1/src/doppkit/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:30:35.569920 doppkit-0.4rc1/src/doppkit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/cli/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/cli/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:30:35.569920 doppkit-0.4rc1/src/doppkit/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/ExportView.py
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/LogWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/MenuBar.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/SettingsDialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/UploadView.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:30:35.569920 doppkit-0.4rc1/src/doppkit/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22945 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/gui/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-12 19:30:25.000000 doppkit-0.4rc1/src/doppkit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:09:52.138018 doppkit-0.4.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-19 19:09:52.138018 doppkit-0.4.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:09:52.138018 doppkit-0.4.0rc2/doppkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-19 19:09:52.000000 doppkit-0.4.0rc2/doppkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 19:09:52.000000 doppkit-0.4.0rc2/doppkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:09:52.000000 doppkit-0.4.0rc2/doppkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 19:09:52.000000 doppkit-0.4.0rc2/doppkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-19 19:09:52.000000 doppkit-0.4.0rc2/doppkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 19:09:52.000000 doppkit-0.4.0rc2/doppkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:09:52.138018 doppkit-0.4.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:09:52.130018 doppkit-0.4.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:09:52.134018 doppkit-0.4.0rc2/src/doppkit/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:09:52.134018 doppkit-0.4.0rc2/src/doppkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/cli/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/cli/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:09:52.138018 doppkit-0.4.0rc2/src/doppkit/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/ExportView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/LogWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/MagicLinkDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/MenuBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/SettingsDialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/UploadView.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:09:52.138018 doppkit-0.4.0rc2/src/doppkit/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26028 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/gui/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-19 19:09:41.000000 doppkit-0.4.0rc2/src/doppkit/util.py
```

### Comparing `doppkit-0.4rc1/LICENSE` & `doppkit-0.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/PKG-INFO` & `doppkit-0.4.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.4rc1/README.md` & `doppkit-0.4.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/doppkit.egg-info/PKG-INFO` & `doppkit-0.4.0rc2/doppkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppkit
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: Tool to allow retrival of USACE GRiD data
 Maintainer-email: Ognyan Moore <ogi@hobu.co>, Howard Butler <howard@hobu.co>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `doppkit-0.4rc1/doppkit.egg-info/SOURCES.txt` & `doppkit-0.4.0rc2/doppkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/doppkit/cli/__init__.py
 src/doppkit/cli/__main__.py
 src/doppkit/cli/cache.py
 src/doppkit/cli/list.py
 src/doppkit/cli/sync.py
 src/doppkit/gui/ExportView.py
 src/doppkit/gui/LogWidget.py
+src/doppkit/gui/MagicLinkDialog.py
 src/doppkit/gui/MenuBar.py
 src/doppkit/gui/SettingsDialog.py
 src/doppkit/gui/UploadView.py
 src/doppkit/gui/__init__.py
 src/doppkit/gui/__main__.py
 src/doppkit/gui/cache.py
 src/doppkit/gui/window.py
```

### Comparing `doppkit-0.4rc1/pyproject.toml` & `doppkit-0.4.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/app.py` & `doppkit-0.4.0rc2/src/doppkit/app.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/cache.py` & `doppkit-0.4.0rc2/src/doppkit/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 
 async def cache(
         app: 'Application',
         urls: Iterable[DownloadUrl],
         headers: dict[str, str],
         progress: Optional[Progress] = None
-) -> Iterable[Union[Content, Exception, httpx.Response]]:
+) -> Iterable[Union[Content, BaseException, httpx.Response]]:
     limits = httpx.Limits(
         max_keepalive_connections=app.threads, max_connections=app.threads
     )
     timeout = httpx.Timeout(20.0, connect=40.0)
     headers['user-agent'] = f"doppkit/{__version__}/{app.run_method}"
     headers["Authorization"] = f"Bearer {app.token}"
     async with httpx.AsyncClient(
```

### Comparing `doppkit-0.4rc1/src/doppkit/cli/__main__.py` & `doppkit-0.4.0rc2/src/doppkit/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/cli/cache.py` & `doppkit-0.4.0rc2/src/doppkit/cli/cache.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/cli/list.py` & `doppkit-0.4.0rc2/src/doppkit/cli/list.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/cli/sync.py` & `doppkit-0.4.0rc2/src/doppkit/cli/sync.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/grid.py` & `doppkit-0.4.0rc2/src/doppkit/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,16 +122,14 @@
     exports: list[Export]
     raster_intersects: list[RasterProduct]
     mesh_intersects: list[MeshProduct]
     pointcloud_intersects: list[PointcloudProduct]
     vector_intersects: list[VectorProduct]
 
 
-
-
 class Grid:
     def __init__(self, args):
         self.args = args
         # let's quiet down the HTTPX logger
         logging.getLogger("httpx").setLevel(logging.WARNING)
         logger.setLevel(self.args.log_level)
```

### Comparing `doppkit-0.4rc1/src/doppkit/gui/ExportView.py` & `doppkit-0.4.0rc2/src/doppkit/gui/ExportView.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/gui/LogWidget.py` & `doppkit-0.4.0rc2/src/doppkit/gui/LogWidget.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/gui/MenuBar.py` & `doppkit-0.4.0rc2/src/doppkit/gui/MenuBar.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,49 +3,53 @@
 
 
 from qtpy.QtCore import Slot, QDir
 from qtpy.QtGui import QKeySequence
 from qtpy.QtWidgets import QAction, QApplication, QFileDialog, QMenu, QMenuBar, QMainWindow
 
 from .SettingsDialog import SettingsDialog
+from .MagicLinkDialog import MagicLinkDialog
 
 class MenuBar(QMenuBar):
 
     def __init__(self) -> None:
         # intentionally do not pass a parent to the menu bar...
         super().__init__(None)
 
         for widget in QApplication.instance().topLevelWidgets():
             if isinstance(widget, QMainWindow):
                 self.mainWindow = widget
                 break
         else:
             raise RuntimeError("Main Window not Found")
-        self.fileMenu = FileMenu(self)
-        self.viewMenu = ViewMenu(self)
+        self.fileMenu = FileMenu(parent=self)
+        self.viewMenu = ViewMenu(parent=self)
         self.helpMenu = QMenu("Help", self)
 
         for menu in [self.fileMenu, self.viewMenu, self.helpMenu]:
             self.addMenu(menu)
 
-        self.settingsDialog: typing.Optional[SettingsDialog] = None
 
 class FileMenu(QMenu):
 
-    def __init__(self, title: typing.Optional[str] = None, parent: MenuBar = None) -> None:
-        if isinstance(title, str):
-            super().__init__(title, parent)
-        else:
-            parent, title = title, ""
-            super().__init__(parent)
+    def __init__(
+        self,
+        title: typing.Optional[str] = None,
+        parent: typing.Optional[MenuBar] = None
+    ) -> None:
+        if title is None:
+            title = ""
+        super().__init__(title, parent)
         self.setTitle("File")
         self.settingsDialog: typing.Optional['SettingsDialog'] = None
+        self.magicLinkDialog: typing.Optional['MagicLinkDialog'] = None
         self._settingsAction()
         self._uploadFileAction()
         self._uploadDirectoryAction()
+        self._provideMagicLinkAction()
         self._quitAction()
 
     def _settingsAction(self) -> None:
         settingsAction = QAction("Preferences", self)
         settingsAction.setStatusTip("Settings")
         settingsAction.setMenuRole(QAction.MenuRole.PreferencesRole)
         settingsAction.triggered.connect(self.invokeSettings)
@@ -55,14 +59,22 @@
     def invokeSettings(self):
         if self.settingsDialog is None:
             self.settingsDialog = SettingsDialog(self)
             self.settingsDialog.rejected.connect(self._resetSettingsDialog)
             self.settingsDialog.show()
 
     @Slot()
+    def invokeMagicLinkDialog(self):
+        if self.magicLinkDialog is None:
+            self.magicLinkDialog = MagicLinkDialog(parent=self)
+            mainWindow = self.parent().mainWindow
+            self.magicLinkDialog.magicLinkText.connect(mainWindow.parseMagicLink)
+        self.magicLinkDialog.show()
+
+    @Slot()
     def uploadFileDialog(self):
         filename, filter_ = QFileDialog.getOpenFileName(
             self,
             "Upload File",
             QDir.home().absolutePath(),
             options=QFileDialog.Option.ReadOnly
         )
@@ -135,14 +147,19 @@
 
     def _uploadDirectoryAction(self):
         uploadDirectoryAction = QAction("Upload Directory Contents", self)
         uploadDirectoryAction.setStatusTip("Upload Directory Contents")
         uploadDirectoryAction.triggered.connect(self.uploadDirectoryDialog)
         self.addAction(uploadDirectoryAction)
 
+    def _provideMagicLinkAction(self):
+        provideMagicLinkAction = QAction("Import Magic Link", self)
+        provideMagicLinkAction.triggered.connect(self.invokeMagicLinkDialog)
+        self.addAction(provideMagicLinkAction)
+
 
 class ViewMenu(QMenu):
 
     def __init__(self, title: typing.Optional[str] = None, parent: MenuBar = None) -> None:
         if isinstance(title, str):
             super().__init__(title, parent)
         else:
```

### Comparing `doppkit-0.4rc1/src/doppkit/gui/SettingsDialog.py` & `doppkit-0.4.0rc2/src/doppkit/gui/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/gui/UploadView.py` & `doppkit-0.4.0rc2/src/doppkit/gui/UploadView.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/gui/__main__.py` & `doppkit-0.4.0rc2/src/doppkit/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/gui/cache.py` & `doppkit-0.4.0rc2/src/doppkit/gui/cache.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/gui/window.py` & `doppkit-0.4.0rc2/src/doppkit/gui/window.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 from .. import __version__
 from ..grid import Grid, AOI
 from .cache import cache, DownloadUrl
 from qtpy import QtCore, QtGui, QtWidgets
+import contextlib
 from typing import Optional, NamedTuple, Union
 from collections import defaultdict
 from dataclasses import dataclass
 import pathlib
 import logging
 import math
 import time
 from urllib.parse import urlparse
 
 import qasync
 
-
 from .ExportView import ExportModel, ExportDelegate
 from .UploadView import UploadModel, UploadItem, UploadDelegate
 from .LogWidget import LoggingDialog
 from .MenuBar import MenuBar
 
 logger = logging.getLogger("doppkit")
 
@@ -183,23 +183,30 @@
             state = QtGui.QValidator.State.Intermediate
         return state, input_, pos
 
 
 class URLValidator(QtGui.QValidator):
 
     def validate(self, input_: str, pos: int) -> tuple[QtGui.QValidator.State, str, int]:
-        # url = QtCore.QUrl(input_)
         url = QtCore.QUrl.fromUserInput(input_)
         if url.isValid():
             state = QtGui.QValidator.State.Acceptable
         else:
             state = QtGui.QValidator.State.Intermediate
         return state, input_, pos
 
 
+class ExportValidator(QtGui.QRegularExpressionValidator):
+
+    def validate(self, input_: str, pos: int) -> tuple[QtGui.QValidator.State, str, int]:
+        state = super().validate(input_, pos)
+        # allows for styling changes on potentially bogus input...
+        return state
+
+
 class TreeView(QtWidgets.QTreeView):
 
     def __init__(self, parent: Optional[QtCore.QObject] = None) -> None:
         super().__init__(parent)
 
 
 class Window(QtWidgets.QMainWindow):
@@ -207,14 +214,15 @@
     def __init__(self, doppkit_application, *args):
         super().__init__(*args)
 
         self.setGeometry(300, 300, 300, 220)
         self.setWindowTitle(f"doppkit - {__version__}")
         self.doppkit = doppkit_application
         self.AOI_ids: list[int] = []
+        self.export_ids: list[int] = []
         self.AOIs: list[AOI] = []  # populated from GRiD
 
         self.exportProgressTracker = QtExportProgress()
 
         # Download Progress Viewer
         self.exportView = None
 
@@ -229,48 +237,61 @@
 
         layout = QtWidgets.QVBoxLayout(contents)
 
         # URL Widgets
         urlLabel = QtWidgets.QLabel("&Server")
         labelFont = urlLabel.font()
         labelFont.setPointSize(10)
-        urlLineComboBox = QtWidgets.QComboBox()
-        urlLineComboBox.addItems(
+        self.urlLineComboBox = QtWidgets.QComboBox()
+        self.urlLineComboBox.addItems(
             [
                 "https://grid.nga.mil/grid",
                 "https://grid.nga.smil.mil",
                 "https://grid.nga.ic.gov"
             ]
         )
-        urlLineComboBox.setEditable(True)
-        urlLineComboBox.currentTextChanged.connect(self.gridURLChanged)
+        self.urlLineComboBox.setEditable(True)
+        self.urlLineComboBox.currentTextChanged.connect(self.gridURLChanged)
         urlLabel.setFont(labelFont)
-        urlLabel.setBuddy(urlLineComboBox)
+        urlLabel.setBuddy(self.urlLineComboBox)
         urlValidator = URLValidator(parent=None)
-        urlLineComboBox.setValidator(urlValidator)
+        self.urlLineComboBox.setValidator(urlValidator)
 
         # Token Widgets
         tokenLabel = QtWidgets.QLabel("&Token")
         tokenLabel.setFont(labelFont)
-        tokenLineEdit = QtWidgets.QLineEdit()
-        tokenLineEdit.setEchoMode(QtWidgets.QLineEdit.EchoMode.PasswordEchoOnEdit)
-        tokenLineEdit.editingFinished.connect(self.tokenChanged)
-        tokenLabel.setBuddy(tokenLineEdit)
+        self.tokenLineEdit = QtWidgets.QLineEdit()
+        self.tokenLineEdit.setEchoMode(QtWidgets.QLineEdit.EchoMode.PasswordEchoOnEdit)
+        self.tokenLineEdit.editingFinished.connect(self.tokenChanged)
+        tokenLabel.setBuddy(self.tokenLineEdit)
 
         # AOI Widgets
         aoiLabel = QtWidgets.QLabel("&AOI")
         aoiLabel.setFont(labelFont)
-        aoiLineEdit = QtWidgets.QLineEdit()
+        self.aoiLineEdit = QtWidgets.QLineEdit()
 
         # TODO: don't use IntValidator, should accept coma separated values
-        aoiValidator = QtGui.QIntValidator(parent=None, bottom=0)
+        aoiValidator = QtGui.QIntValidator(parent=None)
         aoiValidator.setBottom(0)
-        aoiLineEdit.setValidator(aoiValidator)
-        aoiLineEdit.editingFinished.connect(self.aoisChanged)
-        aoiLabel.setBuddy(aoiLineEdit)
+        self.aoiLineEdit.setValidator(aoiValidator)
+        self.aoiLineEdit.editingFinished.connect(self.aoisChanged)
+        aoiLabel.setBuddy(self.aoiLineEdit)
+
+        # Export IDs
+        exportLabel = QtWidgets.QLabel("&Exports")
+        exportLabel.setFont(labelFont)
+        self.exportLineEdit = QtWidgets.QLineEdit()
+        self.exportLineEdit.editingFinished.connect(self.exportsChanged)
+        exportLabel.setBuddy(self.exportLineEdit)
+        self.exportLineEdit.setToolTip(
+            "Coma separated list of exports to download.\n" +
+            "Leaving blank will download all available exports."
+        )
+        exportValidator = ExportValidator(QtCore.QRegularExpression(r"\d+(?:\s*,\s*\d+)*"))
+        self.exportLineEdit.setValidator(exportValidator)
 
         # Download Location
         downloadLabel = QtWidgets.QLabel("&Download Location")
         downloadLabel.setFont(labelFont)
         downloadLineEdit = QtWidgets.QLineEdit()
         downloadLabel.setBuddy(downloadLineEdit)
         downloadLineEdit.setValidator(DirectoryValidator(parent=None))
@@ -282,46 +303,50 @@
             downloadIcon,
             QtWidgets.QLineEdit.ActionPosition.LeadingPosition
         )
 
         downloadAction.triggered.connect(self.showDownloadDialog)
 
         self.buttonList = QtWidgets.QPushButton("List Exports")
-        self.buttonList.clicked.connect(aoiLineEdit.editingFinished)
-        self.buttonList.clicked.connect(tokenLineEdit.editingFinished)
+        self.buttonList.clicked.connect(self.aoiLineEdit.editingFinished)
+        self.buttonList.clicked.connect(self.tokenLineEdit.editingFinished)
         # we connect using a queued connection to ensure that the AOILineEdit
         # registers the finished signal
         self.buttonList.clicked.connect(
             self.listExports,
             QtCore.Qt.ConnectionType.QueuedConnection
         )
         self.buttonDownload = QtWidgets.QPushButton("Download Exports")
-        self.buttonDownload.clicked.connect(aoiLineEdit.editingFinished)
-        self.buttonDownload.clicked.connect(tokenLineEdit.editingFinished)
+        self.buttonDownload.clicked.connect(self.aoiLineEdit.editingFinished)
+        self.buttonDownload.clicked.connect(self.tokenLineEdit.editingFinished)
         self.buttonDownload.clicked.connect(downloadLineEdit.editingFinished)
         self.buttonDownload.clicked.connect(
             self.downloadExports,
             QtCore.Qt.ConnectionType.QueuedConnection
         )
         grouping = {
             "aoi": (
                 aoiLabel,
-                aoiLineEdit
+                self.aoiLineEdit
+            ),
+            "export": (
+                exportLabel,
+                self.exportLineEdit
             ),
             "token": (
                 tokenLabel,
-                tokenLineEdit
+                self.tokenLineEdit
             ),
             "destination": (
                 downloadLabel,
                 downloadLineEdit
             ),
             "url": (
                 urlLabel,
-                urlLineComboBox
+                self.urlLineComboBox
             ),
         }
 
         buttonLayout = QtWidgets.QHBoxLayout()
         buttonLayout.addWidget(self.buttonList)
         buttonLayout.addWidget(self.buttonDownload)
 
@@ -342,18 +367,18 @@
         ssl_white_list = settings.value("grid/ssl_url_white_list", None)
         if ssl_white_list is None:
             # setting default URLs to skip
             ssl_white_list = ["https://grid.nga.smil.mil", "https://grid.nga.ic.gov"]
             settings.setValue("grid/ssl_url_white_list", ssl_white_list)
 
         # populate fields with previously stored values or defaults otherwise
-        tokenLineEdit.setText(settings.value("grid/token"))
+        self.tokenLineEdit.setText(settings.value("grid/token"))
         self.doppkit.token = settings.value("grid/token")
 
-        urlLineComboBox.setEditText(str(settings.value("grid/url", "https://grid.nga.mil/grid")))
+        self.urlLineComboBox.setEditText(str(settings.value("grid/url", "https://grid.nga.mil/grid")))
         
         downloadLineEdit.setText(
             str(
                 settings.value(
                     "grid/download",
                     QtCore.QStandardPaths.standardLocations(
                         QtCore.QStandardPaths.StandardLocation.DownloadLocation
@@ -362,16 +387,15 @@
             )
         )
 
         self.progressInterconnect = QtExportProgress()
         self.uploadProgressInterconnect = QtUploadProgress()
         self.show()
 
-
-    def closeEvent(self, evt: QtGui.QCloseEvent) -> None:
+    def closeEvent(self, event: QtGui.QCloseEvent) -> None:
         settings = QtCore.QSettings()
         settings.beginGroup("MainWindow")
         settings.setValue("geometry", self.saveGeometry())
         settings.endGroup()
 
     def showDownloadDialog(self, checked:bool = False):
         directory = QtWidgets.QFileDialog.getExistingDirectory(
@@ -382,18 +406,19 @@
         )
 
         if directory == "":
             # dialog was cancelled
             return None
         
         lineEdit = self.sender().parent()
-        lineEdit.setText(directory)
+        if isinstance(lineEdit, QtWidgets.QLineEdit):
+            lineEdit.setText(directory)
 
     def showLogView(self):
-        raise self.logView.show()
+        self.logView.show()
 
     def gridURLChanged(self):
         self.doppkit.url = QtCore.QUrl.fromUserInput(self.sender().currentText()).url()
         setting = QtCore.QSettings()
         setting.setValue("grid/url", self.doppkit.url)
 
     def downloadDirectoryChanged(self):
@@ -403,18 +428,49 @@
     
     def aoisChanged(self) -> None:
         try:
             self.AOI_ids = [int(aoi) for aoi in self.sender().text().split(",")]
         except (IndexError, ValueError):
             self.AOI_ids = []
 
+    def exportsChanged(self) -> None:
+        sender = self.sender()
+        if isinstance(sender, QtWidgets.QLineEdit):
+            try:
+                self.export_ids = [
+                    int(export_id)
+                    for export_id in sender.text().split(',')
+                ]
+            except (IndexError, ValueError):
+                self.export_ids = []
+
+    @QtCore.Slot(object)
+    def parseMagicLink(self, text: str) -> None:
+
+        fields = [
+            self.exportLineEdit,
+            self.aoiLineEdit,
+            self.tokenLineEdit,
+            self.urlLineComboBox
+        ]
+
+        for value, field in zip(text.split("|"), fields):
+            if isinstance(field, QtWidgets.QComboBox):
+                field.setEditText(f"https://{value}")
+                field.currentTextChanged.emit()
+            else:
+                field.setText(value)
+                field.editingFinished.emit()
+
     def tokenChanged(self) -> None:
-        self.doppkit.token = self.sender().text().strip()
-        setting = QtCore.QSettings()
-        setting.setValue("grid/token", self.doppkit.token)
+        sender = self.sender()
+        if isinstance(sender, QtWidgets.QLineEdit):
+            self.doppkit.token = sender.text().strip()
+            setting = QtCore.QSettings()
+            setting.setValue("grid/token", self.doppkit.token)
 
     @qasync.asyncSlot()
     async def uploadFiles(
         self,
         files: list[str],
         directory: Optional[Union[str, pathlib.Path]]=None
     ):
@@ -464,15 +520,19 @@
         # need to determine if we should skip SSL verification...
         # first, is SSL verification enabled?
         settings = QtCore.QSettings()
         enable_ssl = settings.value("grid/ssl_verification", type=bool)
         # if enabled, check the other elements...
         if enable_ssl:
             # check if the GRiD URL is in the white-list
-            whitelisted_urls = settings.value("grid/ssl_url_white_list", [], type=list)
+            whitelisted_urls: list[str] = settings.value(
+                "grid/ssl_url_white_list",
+                [],
+                type=list
+            )  #type: ignore
             whitelisted_host_names = {urlparse(url).hostname for url in whitelisted_urls}
             hostname = urlparse(self.doppkit.url).hostname
             if hostname in whitelisted_host_names:
                 enable_ssl = False
         enabled = "enabled" if enable_ssl else "disabled"
         logger.debug(f"POSTing to GRiD with SSL {enabled}")
         self.doppkit.disable_ssl_verification = not enable_ssl
@@ -530,16 +590,25 @@
         api = Grid(self.doppkit)
         # now we get information to each exportfile
 
         download_dir = pathlib.Path(self.doppkit.directory)
         download_dir.mkdir(exist_ok=True)
 
         urls = []
+        export_ids_filtered = set()
+        export_ids_to_filter = self.export_ids.copy()
         for aoi in self.AOIs:
             for export in aoi["exports"]:
+                export_id = export["id"]
+                if export_ids_to_filter:
+                    # if boolean, we're filtering
+                    if export_id in export_ids_to_filter:
+                        # move the export_id from ones to filter to the ones that have
+                        # been filtered
+                        export_ids_filtered.add(export_ids_to_filter.pop(export_id))
                 files = await api.get_exports(export["id"])
 
                 download_size = 0
                 for download_file in files:
                     filename = download_file.name
                     download_destination = download_dir.joinpath(download_file.save_path)
 
@@ -559,19 +628,25 @@
                     aoi_name=aoi["name"],
                     current=0,
                     total=download_size   # export["complete_size"] is inaccurate for the time being...
                 )
                 self.progressInterconnect.export_progress[export["id"]] = progress_tracker
                 self.progressInterconnect.aois[aoi["id"]].append(progress_tracker)
 
-        try:
+        if export_ids_to_filter:
+            # there are some exports we intended to filter for, but weren't present in the AOIs
+            logger.warning(
+                f"The following export_ids were entered to filter for, but were not seen in the given AOIs: {export_ids_to_filter}"
+            )
+        with contextlib.suppress(Exception):
             _ = await cache(self.doppkit, urls, {}, progress=self.progressInterconnect)
-            logger.info("Download AOI Exports Complete")
-        finally:
-            self.buttonDownload.setEnabled(True)
+        logger.info("Download AOI Exports Complete")
+
+        self.buttonDownload.setEnabled(True)
+
 
 
 @dataclass
 class UploadProgressTracking:
     path: str
     current: int
     total: int
```

### Comparing `doppkit-0.4rc1/src/doppkit/upload.py` & `doppkit-0.4.0rc2/src/doppkit/upload.py`

 * *Files identical despite different names*

### Comparing `doppkit-0.4rc1/src/doppkit/util.py` & `doppkit-0.4.0rc2/src/doppkit/util.py`

 * *Files identical despite different names*

