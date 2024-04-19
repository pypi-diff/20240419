# Comparing `tmp/NucDetect-0.6.2.dev4.tar.gz` & `tmp/NucDetect-0.6.3.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\NucDetect-0.6.2.dev4.tar", last modified: Thu Nov  7 12:31:11 2019, max compression
+gzip compressed data, was "dist\NucDetect-0.6.3.dev5.tar", last modified: Mon Nov 18 10:33:17 2019, max compression
```

## Comparing `NucDetect-0.6.2.dev4.tar` & `NucDetect-0.6.3.dev5.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxrwxrwx   0        0        0        0 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/
--rw-rw-rw-   0        0        0      292 2019-11-07 11:04:30.000000 NucDetect-0.6.2.dev4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/NucDetect.egg-info/
--rw-rw-rw-   0        0        0     2216 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/NucDetect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/NucDetect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/NucDetect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/NucDetect.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/NucDetect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2216 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2019-11-06 14:02:16.000000 NucDetect-0.6.2.dev4/README.md
-drwxrwxrwx   0        0        0        0 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/core/
--rw-rw-rw-   0        0        0    25130 2019-11-07 11:01:01.000000 NucDetect-0.6.2.dev4/core/Detector.py
--rw-rw-rw-   0        0        0     4499 2019-10-28 13:59:21.000000 NucDetect-0.6.2.dev4/core/JittedFunctions.py
--rw-rw-rw-   0        0        0    11759 2019-11-07 11:01:12.000000 NucDetect-0.6.2.dev4/core/ROI.py
--rw-rw-rw-   0        0        0     7686 2019-11-07 12:26:23.000000 NucDetect-0.6.2.dev4/core/ROIHandler.py
--rw-rw-rw-   0        0        0        2 2019-07-30 13:23:07.000000 NucDetect-0.6.2.dev4/core/__init__.py
--rw-rw-rw-   0        0        0   670708 2019-08-05 10:16:44.000000 NucDetect-0.6.2.dev4/demo.tif
-drwxrwxrwx   0        0        0        0 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/gui/
--rw-rw-rw-   0        0        0   102907 2019-11-07 12:06:49.000000 NucDetect-0.6.2.dev4/gui/NucDetectAppQT.py
--rw-rw-rw-   0        0        0        2 2019-07-30 13:23:07.000000 NucDetect-0.6.2.dev4/gui/__init__.py
--rw-rw-rw-   0        0        0     2577 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/analyse_all_dialog.ui
--rw-rw-rw-   0        0        0    62508 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/banner.png
--rw-rw-rw-   0        0        0    58942 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/banner_norm.png
--rw-rw-rw-   0        0        0     2202 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/classification_dialog.ui
--rw-rw-rw-   0        0        0     7248 2019-10-22 12:56:57.000000 NucDetect-0.6.2.dev4/gui/experiment_dialog.ui
--rw-rw-rw-   0        0        0    46743 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/logo.png
--rw-rw-rw-   0        0        0    10049 2019-10-29 13:24:22.000000 NucDetect-0.6.2.dev4/gui/modification_dialog.ui
--rw-rw-rw-   0        0        0    18567 2019-11-06 10:42:26.000000 NucDetect-0.6.2.dev4/gui/nucdetect.ui
--rw-rw-rw-   0        0        0      690 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/result_correction_dialog.ui
--rw-rw-rw-   0        0        0     3849 2019-07-30 13:20:11.000000 NucDetect-0.6.2.dev4/gui/result_image_dialog.ui
-drwxrwxrwx   0        0        0        0 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/gui/settings/
--rw-rw-rw-   0        0        0     8770 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/Settings.py
--rw-rw-rw-   0        0        0        2 2019-07-30 13:23:07.000000 NucDetect-0.6.2.dev4/gui/settings/__init__.py
--rw-rw-rw-   0        0        0     2587 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/menu_checkbox.ui
--rw-rw-rw-   0        0        0     2416 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/menu_combo.ui
--rw-rw-rw-   0        0        0     2294 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/menu_decimal_spin.ui
--rw-rw-rw-   0        0        0     3534 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/menu_dial.ui
--rw-rw-rw-   0        0        0     2747 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/menu_slider.ui
--rw-rw-rw-   0        0        0     2388 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/menu_spin.ui
--rw-rw-rw-   0        0        0     1476 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/menu_text.ui
--rw-rw-rw-   0        0        0     1372 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/menu_widget.ui
--rw-rw-rw-   0        0        0       11 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings/settings.ini
--rw-rw-rw-   0        0        0     1049 2019-10-07 09:55:02.000000 NucDetect-0.6.2.dev4/gui/settings/settings.json
--rw-rw-rw-   0        0        0     8962 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings_about.ui
--rw-rw-rw-   0        0        0     3803 2019-04-02 14:31:55.000000 NucDetect-0.6.2.dev4/gui/settings_dialog.ui
--rw-rw-rw-   0        0        0     9298 2019-07-30 13:20:11.000000 NucDetect-0.6.2.dev4/gui/statistics_dialog.ui
--rw-rw-rw-   0        0        0      131 2019-11-04 15:10:43.000000 NucDetect-0.6.2.dev4/requirements.txt
--rw-rw-rw-   0        0        0       42 2019-11-07 12:31:11.000000 NucDetect-0.6.2.dev4/setup.cfg
--rw-rw-rw-   0        0        0     1098 2019-11-07 12:29:27.000000 NucDetect-0.6.2.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/
+-rw-rw-rw-   0        0        0      296 2019-11-07 13:22:09.000000 NucDetect-0.6.3.dev5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/NucDetect.egg-info/
+-rw-rw-rw-   0        0        0     2216 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/NucDetect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/NucDetect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/NucDetect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/NucDetect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/NucDetect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2216 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2019-11-06 14:02:16.000000 NucDetect-0.6.3.dev5/README.md
+drwxrwxrwx   0        0        0        0 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/core/
+-rw-rw-rw-   0        0        0    25130 2019-11-07 11:01:01.000000 NucDetect-0.6.3.dev5/core/Detector.py
+-rw-rw-rw-   0        0        0     4499 2019-10-28 13:59:21.000000 NucDetect-0.6.3.dev5/core/JittedFunctions.py
+-rw-rw-rw-   0        0        0    11759 2019-11-07 11:01:12.000000 NucDetect-0.6.3.dev5/core/ROI.py
+-rw-rw-rw-   0        0        0     7686 2019-11-07 12:26:23.000000 NucDetect-0.6.3.dev5/core/ROIHandler.py
+-rw-rw-rw-   0        0        0        2 2019-07-30 13:23:07.000000 NucDetect-0.6.3.dev5/core/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/gui/
+-rw-rw-rw-   0        0        0   103480 2019-11-18 10:13:53.000000 NucDetect-0.6.3.dev5/gui/NucDetectAppQT.py
+-rw-rw-rw-   0        0        0        2 2019-07-30 13:23:07.000000 NucDetect-0.6.3.dev5/gui/__init__.py
+-rw-rw-rw-   0        0        0     2577 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/analyse_all_dialog.ui
+-rw-rw-rw-   0        0        0    62508 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/banner.png
+-rw-rw-rw-   0        0        0    58942 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/banner_norm.png
+-rw-rw-rw-   0        0        0     2202 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/classification_dialog.ui
+-rw-rw-rw-   0        0        0     7248 2019-10-22 12:56:57.000000 NucDetect-0.6.3.dev5/gui/experiment_dialog.ui
+-rw-rw-rw-   0        0        0    46743 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/logo.png
+-rw-rw-rw-   0        0        0    10049 2019-10-29 13:24:22.000000 NucDetect-0.6.3.dev5/gui/modification_dialog.ui
+-rw-rw-rw-   0        0        0    18567 2019-11-06 10:42:26.000000 NucDetect-0.6.3.dev5/gui/nucdetect.ui
+-rw-rw-rw-   0        0        0      690 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/result_correction_dialog.ui
+-rw-rw-rw-   0        0        0     3849 2019-07-30 13:20:11.000000 NucDetect-0.6.3.dev5/gui/result_image_dialog.ui
+drwxrwxrwx   0        0        0        0 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/gui/settings/
+-rw-rw-rw-   0        0        0     8770 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/Settings.py
+-rw-rw-rw-   0        0        0        2 2019-07-30 13:23:07.000000 NucDetect-0.6.3.dev5/gui/settings/__init__.py
+-rw-rw-rw-   0        0        0     2587 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/menu_checkbox.ui
+-rw-rw-rw-   0        0        0     2416 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/menu_combo.ui
+-rw-rw-rw-   0        0        0     2294 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/menu_decimal_spin.ui
+-rw-rw-rw-   0        0        0     3534 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/menu_dial.ui
+-rw-rw-rw-   0        0        0     2747 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/menu_slider.ui
+-rw-rw-rw-   0        0        0     2388 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/menu_spin.ui
+-rw-rw-rw-   0        0        0     1476 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/menu_text.ui
+-rw-rw-rw-   0        0        0     1372 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/menu_widget.ui
+-rw-rw-rw-   0        0        0       11 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings/settings.ini
+-rw-rw-rw-   0        0        0     1049 2019-10-07 09:55:02.000000 NucDetect-0.6.3.dev5/gui/settings/settings.json
+-rw-rw-rw-   0        0        0     8962 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings_about.ui
+-rw-rw-rw-   0        0        0     3803 2019-04-02 14:31:55.000000 NucDetect-0.6.3.dev5/gui/settings_dialog.ui
+-rw-rw-rw-   0        0        0     9298 2019-07-30 13:20:11.000000 NucDetect-0.6.3.dev5/gui/statistics_dialog.ui
+-rw-rw-rw-   0        0        0       42 2019-11-18 10:33:17.000000 NucDetect-0.6.3.dev5/setup.cfg
+-rw-rw-rw-   0        0        0     1098 2019-11-18 10:33:09.000000 NucDetect-0.6.3.dev5/setup.py
```

### Comparing `NucDetect-0.6.2.dev4/NucDetect.egg-info/PKG-INFO` & `NucDetect-0.6.3.dev5/NucDetect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NucDetect
-Version: 0.6.2.dev4
+Version: 0.6.3.dev5
 Summary: Module to identify intranuclear proteins on basis of fluorescence images.
 Home-page: https://github.com/SilMon/NucDetect
 Author: Romano Weiss
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/NucDetect.svg)](https://badge.fury.io/py/NucDetect)
         
         NucDetect - A python package for Detection and Quantification of DNA Doublestrand Breaks (v0.5)
```

### Comparing `NucDetect-0.6.2.dev4/NucDetect.egg-info/SOURCES.txt` & `NucDetect-0.6.3.dev5/NucDetect.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MANIFEST.in
 README.md
-demo.tif
-requirements.txt
 setup.py
 NucDetect.egg-info/PKG-INFO
 NucDetect.egg-info/SOURCES.txt
 NucDetect.egg-info/dependency_links.txt
 NucDetect.egg-info/requires.txt
 NucDetect.egg-info/top_level.txt
 core/Detector.py
```

### Comparing `NucDetect-0.6.2.dev4/PKG-INFO` & `NucDetect-0.6.3.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NucDetect
-Version: 0.6.2.dev4
+Version: 0.6.3.dev5
 Summary: Module to identify intranuclear proteins on basis of fluorescence images.
 Home-page: https://github.com/SilMon/NucDetect
 Author: Romano Weiss
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/NucDetect.svg)](https://badge.fury.io/py/NucDetect)
         
         NucDetect - A python package for Detection and Quantification of DNA Doublestrand Breaks (v0.5)
```

### Comparing `NucDetect-0.6.2.dev4/README.md` & `NucDetect-0.6.3.dev5/README.md`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/core/Detector.py` & `NucDetect-0.6.3.dev5/core/Detector.py`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/core/JittedFunctions.py` & `NucDetect-0.6.3.dev5/core/JittedFunctions.py`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/core/ROI.py` & `NucDetect-0.6.3.dev5/core/ROI.py`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/core/ROIHandler.py` & `NucDetect-0.6.3.dev5/core/ROIHandler.py`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/NucDetectAppQT.py` & `NucDetect-0.6.3.dev5/gui/NucDetectAppQT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1619,16 +1619,14 @@
         # Initialize interactivity of graphics view
         self.set_current_image()
 
     def set_list_images(self, images: List[np.ndarray]) -> None:
         self.lst_nuc_model.clear()
         for image in images:
             item = QStandardItem()
-            # TODO test3.tif
-            # ValueError: The truth value of an array with more than one element is ambiguous. Use a.any() or a.all()
             item.setTextAlignment(QtCore.Qt.AlignLeft)
             pmap = QPixmap()
             pmap.convertFromImage(NucView.get_qimage_from_numpy(image[...,
                                                                       self.handler.idents.index(self.handler.main)]
                                                                 ))
             ic = QIcon(pmap)
             item.setIcon(ic)
@@ -1637,14 +1635,15 @@
     def on_nucleus_selection_change(self) -> None:
         self.cur_channel = self.ui.sb_channel.value()
         self.set_current_image()
 
     def on_button_click(self) -> None:
         """
         Method to handle button clicks
+
         :return: None
         """
         ident = self.sender().objectName()
         if ident == "btn_show":
             self.show = self.ui.btn_show.isChecked()
             if self.show:
                 self.ui.btn_show.setIcon(qta.icon("fa5.eye", color=self.btn_col))
@@ -2007,27 +2006,34 @@
             x_offset = nuc_dat["minX"]
             y_offset = nuc_dat["minY"]
             for y in range(len(mask)):
                 for x in range(len(mask[0])):
                     if mask[y][x] > 0:
                         inten = cur_nump[y][x]
                         cur_roi.add_point((x + x_offset, y + y_offset), inten)
-                        self.commands.append(
-                            ("INSERT INTO points VALUES(?, ?, ?, ?)",
-                            (-1, x + x_offset, y + y_offset, np.int(inten)))
-                        )
+                        self.commands.append(("INSERT INTO points VALUES(?, ?, ?, ?)",
+                                              (-1, x + x_offset, y + y_offset, np.int(inten))))
             self.handler.rois.append(cur_roi)
+            # TODO
             roidat = cur_roi.calculate_dimensions()
+            stats = cur_roi.calculate_statistics()
+            ellp = cur_roi.calculate_ellipse_parameters()
             imghash = self.handler.ident
             self.commands.extend(
                 (("INSERT INTO roi VALUES(?, ?, ?, ?, ?, ?, ?, ?)",
                  (hash(cur_roi), imghash, False, cur_roi.ident, str(roidat["center"]), roidat["width"],
                   roidat["height"], hash(self.cur_nuc))),
                  ("UPDATE points SET hash=? WHERE hash=-1",
-                 (hash(cur_roi),)))
+                 (hash(cur_roi),)),
+                 ("INSERT OR IGNORE INTO statistics VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)",
+                 (hash(cur_roi), imghash, stats["area"], stats["intensity average"], stats["intensity median"],
+                  stats["intensity maximum"], stats["intensity minimum"], stats["intensity std"],
+                  str(ellp["center"]), str(ellp["major_axis"][0]), str(ellp["major_axis"][1]),
+                  ellp["major_slope"], ellp["major_length"], ellp["major_angle"], str(ellp["minor_axis"][0]),
+                  str(ellp["minor_axis"][1]), ellp["minor_length"], ellp["shape_match"])))
             )
             self.foc_group.append(self.temp_foc)
             self.map[self.temp_foc] = cur_roi
             self.pos = None
             self.temp_foc = None
             self.scene().update()
             self.assmap = Detector.create_association_map(self.handler.rois)
```

### Comparing `NucDetect-0.6.2.dev4/gui/analyse_all_dialog.ui` & `NucDetect-0.6.3.dev5/gui/analyse_all_dialog.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/banner.png` & `NucDetect-0.6.3.dev5/gui/banner.png`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/banner_norm.png` & `NucDetect-0.6.3.dev5/gui/banner_norm.png`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/classification_dialog.ui` & `NucDetect-0.6.3.dev5/gui/classification_dialog.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/experiment_dialog.ui` & `NucDetect-0.6.3.dev5/gui/experiment_dialog.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/logo.png` & `NucDetect-0.6.3.dev5/gui/logo.png`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/modification_dialog.ui` & `NucDetect-0.6.3.dev5/gui/modification_dialog.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/nucdetect.ui` & `NucDetect-0.6.3.dev5/gui/nucdetect.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/result_correction_dialog.ui` & `NucDetect-0.6.3.dev5/gui/result_correction_dialog.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/result_image_dialog.ui` & `NucDetect-0.6.3.dev5/gui/result_image_dialog.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/Settings.py` & `NucDetect-0.6.3.dev5/gui/settings/Settings.py`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/menu_checkbox.ui` & `NucDetect-0.6.3.dev5/gui/settings/menu_checkbox.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/menu_combo.ui` & `NucDetect-0.6.3.dev5/gui/settings/menu_combo.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/menu_decimal_spin.ui` & `NucDetect-0.6.3.dev5/gui/settings/menu_decimal_spin.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/menu_dial.ui` & `NucDetect-0.6.3.dev5/gui/settings/menu_dial.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/menu_slider.ui` & `NucDetect-0.6.3.dev5/gui/settings/menu_slider.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/menu_spin.ui` & `NucDetect-0.6.3.dev5/gui/settings/menu_spin.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/menu_text.ui` & `NucDetect-0.6.3.dev5/gui/settings/menu_text.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/menu_widget.ui` & `NucDetect-0.6.3.dev5/gui/settings/menu_widget.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings/settings.json` & `NucDetect-0.6.3.dev5/gui/settings/settings.json`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings_about.ui` & `NucDetect-0.6.3.dev5/gui/settings_about.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/settings_dialog.ui` & `NucDetect-0.6.3.dev5/gui/settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/gui/statistics_dialog.ui` & `NucDetect-0.6.3.dev5/gui/statistics_dialog.ui`

 * *Files identical despite different names*

### Comparing `NucDetect-0.6.2.dev4/setup.py` & `NucDetect-0.6.3.dev5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="NucDetect",
-    version="0.6.2.dev4",
+    version="0.6.3.dev5",
     description=("Module to identify intranuclear proteins on basis of "
                  "fluorescence images."),
     author="Romano Weiss",
     url="https://github.com/SilMon/NucDetect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

