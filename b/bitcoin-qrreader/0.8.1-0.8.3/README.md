# Comparing `tmp/bitcoin_qrreader-0.8.1.tar.gz` & `tmp/bitcoin_qrreader-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_qrreader-0.8.1.tar", max compression
+gzip compressed data, was "bitcoin_qrreader-0.8.3.tar", max compression
```

## Comparing `bitcoin_qrreader-0.8.1.tar` & `bitcoin_qrreader-0.8.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.8.1/LICENSE
--rw-r--r--   0        0        0     1474 2024-02-08 11:20:06.244073 bitcoin_qrreader-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/__init__.py
--rw-r--r--   0        0        0    29426 2024-02-18 19:28:44.842292 bitcoin_qrreader-0.8.1/bitcoin_qrreader/bitcoin_qr.py
--rw-r--r--   0        0        0     3551 2024-02-08 12:16:55.776825 bitcoin_qrreader-0.8.1/bitcoin_qrreader/bitcoin_qr_gui.py
--rw-r--r--   0        0        0     4181 2024-02-18 16:04:51.954266 bitcoin_qrreader-0.8.1/bitcoin_qrreader/multipath_descriptor.py
--rw-r--r--   0        0        0     5760 2024-02-08 17:56:53.952578 bitcoin_qrreader-0.8.1/bitcoin_qrreader/qr_qui.py
--rw-r--r--   0        0        0     2854 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/LICENSE
--rw-r--r--   0        0        0        0 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/__init__.py
--rw-r--r--   0        0        0     4940 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/bytewords.py
--rw-r--r--   0        0        0    11219 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/cbor_lite.py
--rw-r--r--   0        0        0      179 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/constants.py
--rw-r--r--   0        0        0      729 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/crc32.py
--rw-r--r--   0        0        0     9747 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/fountain_decoder.py
--rw-r--r--   0        0        0     4971 2024-01-07 17:59:04.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/fountain_encoder.py
--rw-r--r--   0        0        0     1603 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/fountain_utils.py
--rw-r--r--   0        0        0     1568 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/random_sampler.py
--rw-r--r--   0        0        0      491 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/ur.py
--rw-r--r--   0        0        0     5091 2024-01-07 17:59:04.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/ur_decoder.py
--rw-r--r--   0        0        0     2016 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/ur_encoder.py
--rw-r--r--   0        0        0     1638 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/utils.py
--rw-r--r--   0        0        0     4422 2024-01-08 11:22:55.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/xoshiro256.py
--rw-r--r--   0        0        0     1076 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/LICENSE.md
--rw-r--r--   0        0        0      318 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/README.md
--rw-r--r--   0        0        0     1157 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/__init__.py
--rw-r--r--   0        0        0     1582 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/bytes.py
--rw-r--r--   0        0        0     1119 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/COPYING
--rw-r--r--   0        0        0     1247 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/__init__.py
--rw-r--r--   0        0        0     2165 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/data.py
--rw-r--r--   0        0        0     6630 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/decoder.py
--rw-r--r--   0        0        0     4831 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/encoder.py
--rw-r--r--   0        0        0     1315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/__init__.py
--rw-r--r--   0        0        0     2343 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/account.py
--rw-r--r--   0        0        0     1845 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/bip39.py
--rw-r--r--   0        0        0     1954 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/coin_info.py
--rw-r--r--   0        0        0     2193 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/ec_key.py
--rw-r--r--   0        0        0     8881 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/hd_key.py
--rw-r--r--   0        0        0     3686 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/keypath.py
--rw-r--r--   0        0        0     2425 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/multi_key.py
--rw-r--r--   0        0        0     6338 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/output.py
--rw-r--r--   0        0        0     1296 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/psbt.py
--rw-r--r--   0        0        0     2290 2024-01-08 11:22:27.000000 bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/registry.py
--rw-r--r--   0        0        0      749 2024-02-18 19:29:38.346827 bitcoin_qrreader-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 bitcoin_qrreader-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1474 2024-02-08 11:20:06.244073 bitcoin_qrreader-0.8.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/__init__.py
+-rw-r--r--   0        0        0    29516 2024-04-19 13:26:17.067784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/bitcoin_qr.py
+-rw-r--r--   0        0        0     3559 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/bitcoin_qr_gui.py
+-rw-r--r--   0        0        0     4182 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/multipath_descriptor.py
+-rw-r--r--   0        0        0     7612 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/qr_qui.py
+-rw-r--r--   0        0        0     2854 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/__init__.py
+-rw-r--r--   0        0        0     4940 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/bytewords.py
+-rw-r--r--   0        0        0    11219 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/cbor_lite.py
+-rw-r--r--   0        0        0      179 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/constants.py
+-rw-r--r--   0        0        0      729 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/crc32.py
+-rw-r--r--   0        0        0     9747 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/fountain_decoder.py
+-rw-r--r--   0        0        0     4972 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/fountain_encoder.py
+-rw-r--r--   0        0        0     1604 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/fountain_utils.py
+-rw-r--r--   0        0        0     1568 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/random_sampler.py
+-rw-r--r--   0        0        0      491 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/ur.py
+-rw-r--r--   0        0        0     5091 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/ur_decoder.py
+-rw-r--r--   0        0        0     2016 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/ur_encoder.py
+-rw-r--r--   0        0        0     1638 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/utils.py
+-rw-r--r--   0        0        0     4422 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/xoshiro256.py
+-rw-r--r--   0        0        0     1076 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/LICENSE.md
+-rw-r--r--   0        0        0      318 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/README.md
+-rw-r--r--   0        0        0     1157 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/__init__.py
+-rw-r--r--   0        0        0     1582 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/bytes.py
+-rw-r--r--   0        0        0     1119 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/COPYING
+-rw-r--r--   0        0        0     1247 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/__init__.py
+-rw-r--r--   0        0        0     2165 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/data.py
+-rw-r--r--   0        0        0     6630 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/decoder.py
+-rw-r--r--   0        0        0     4831 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/encoder.py
+-rw-r--r--   0        0        0     1315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/__init__.py
+-rw-r--r--   0        0        0     2343 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/account.py
+-rw-r--r--   0        0        0     1845 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/bip39.py
+-rw-r--r--   0        0        0     1954 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/coin_info.py
+-rw-r--r--   0        0        0     2194 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/ec_key.py
+-rw-r--r--   0        0        0     8882 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/hd_key.py
+-rw-r--r--   0        0        0     3686 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/keypath.py
+-rw-r--r--   0        0        0     2425 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/multi_key.py
+-rw-r--r--   0        0        0     6339 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/output.py
+-rw-r--r--   0        0        0     1296 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/psbt.py
+-rw-r--r--   0        0        0     2291 2024-04-19 13:26:17.071784 bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/registry.py
+-rw-r--r--   0        0        0      779 2024-04-19 13:26:17.075784 bitcoin_qrreader-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 bitcoin_qrreader-0.8.3/PKG-INFO
```

### Comparing `bitcoin_qrreader-0.8.1/LICENSE` & `bitcoin_qrreader-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/README.md` & `bitcoin_qrreader-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/bitcoin_qr.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/bitcoin_qr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from abc import ABC, abstractmethod
-from os import fdopen
+import base64
+import enum
+import hashlib
+import json
+import logging
 import re
 import urllib.parse
-from typing import List, Optional, Tuple, Dict
+from abc import ABC, abstractmethod
 from decimal import Decimal
-import bdkpython as bdk
-import base64, json
-from .urtypes.crypto import PSBT as UR_PSBT
-from .urtypes.crypto import Output as US_OUTPUT
-from .ur.ur_decoder import URDecoder
-from .urtypes.bytes import Bytes as UR_BYTES
-import hashlib
+from os import fdopen
+from typing import Dict, List, Optional, Tuple
+
 import base58
-import logging
-import enum
+import bdkpython as bdk
 
 from .multipath_descriptor import MultipathDescriptor
 from .ur.fountain_encoder import CBOREncoder
 from .ur.ur import UR
+from .ur.ur_decoder import URDecoder
 from .ur.ur_encoder import UREncoder
+from .urtypes.bytes import Bytes as UR_BYTES
+from .urtypes.crypto import PSBT as UR_PSBT
+from .urtypes.crypto import Output as US_OUTPUT
 
 BITCOIN_BIP21_URI_SCHEME = "bitcoin"
 logger = logging.getLogger(__name__)
 
 
 def is_bitcoin_address(s, network: bdk.Network):
     try:
@@ -321,14 +323,15 @@
         return False
 
     for line in lines:
         try:
             obj = json.loads(line)
             # Check if all specified keys are present in the JSON object
             if not all(key in obj for key in keys):
+                logger.debug(f"Not all required keys {keys} are present in {obj}")
                 return False
         except json.JSONDecodeError:
             return False
 
     return True
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/bitcoin_qr_gui.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/bitcoin_qr_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from .qr_qui import VideoWidget
-from .bitcoin_qr import *
+import math
+
+import pygame
 from PyQt6 import QtWidgets
-import pygame, math
+
+from .bitcoin_qr import *
+from .qr_qui import VideoWidget
 
 
 class BitcoinVideoWidget(VideoWidget):
     def __init__(
         self,
         result_callback=None,
         close_on_result=True,
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/multipath_descriptor.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/multipath_descriptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import List, Optional
+
 import bdkpython as bdk
-from hwilib.descriptor import parse_descriptor, Descriptor, PubkeyProvider
+from hwilib.descriptor import Descriptor, PubkeyProvider, parse_descriptor
 
 logger = logging.getLogger(__name__)
 
 
 def get_all_pubkey_providers(hwi_descriptor: Descriptor) -> List[PubkeyProvider]:
     pubkey_providers = hwi_descriptor.pubkeys.copy()
     for subdescriptor in hwi_descriptor.subdescriptors:
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/qr_qui.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/qr_qui.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,52 @@
-import pygame
-import pygame.camera
-from PyQt6 import QtCore, QtWidgets, QtGui
-from pyzbar import pyzbar
+import logging
+
+logger = logging.getLogger(__name__)
+
+
 import time
-from PyQt6.QtCore import QEvent
+from typing import List
+
 import mss
 import numpy as np
-from PyQt6.QtCore import pyqtSignal
+import pygame
+import pygame.camera
+from PyQt6 import QtCore, QtGui, QtWidgets
+from PyQt6.QtCore import QEvent, pyqtSignal
+
+
+class BarcodeData:
+    def __init__(self, data, rect):
+        self.data = data  # The decoded text of the barcode
+        self.rect = rect  # The bounding rectangle of the barcode as a tuple (x, y, width, height)
+
+    def __repr__(self):
+        return f"BarcodeData(data={self.data}, rect={self.rect})"
 
 
 class VideoWidget(QtWidgets.QWidget):
     signal_qr_data_callback = pyqtSignal(object)
 
     def __init__(self, qr_data_callback=None, parent=None):
         super().__init__(parent)
+        self.cv2 = None
+        self.pyzbar = None
+        try:
+            # check if loading works
+            # it depend on zlib installed in the os
+            from pyzbar import pyzbar
+
+            self.pyzbar = pyzbar
+            logger.info("Load pyzbar successful")
+        except:
+            logger.info("Could not load pyzbar. Trying to load fallback cv2")
+            import cv2
+
+            self.cv2 = cv2
+
         self.is_screen_capture = False
         self.screen_capturer = mss.mss()
 
         self.label_image = QtWidgets.QLabel()
         self.qr_data_callback = qr_data_callback
         self.signal_qr_data_callback.connect(qr_data_callback)
 
@@ -63,15 +92,15 @@
                 temp_camera.start()
                 temp_camera.stop()
                 valid_cameras.append(camera)
             except SystemError:
                 continue
         return valid_cameras
 
-    def switch_camera(self, index):
+    def switch_camera(self, index: int):
         selected_camera = self.combo_cameras.currentText()
         if selected_camera == "Screen":
             self.is_screen_capture = True
             # Additional logic for initializing screen capture can be added here
         else:
             self.is_screen_capture = False
 
@@ -81,26 +110,52 @@
                 except:
                     pass
 
             self.capture = pygame.camera.Camera(self.cameras[index], (640, 480))
             self.capture.start()
             time.sleep(0.1)  # Add a short delay
 
-    def _numpy_to_surface(self, numpy_image):
+    def _numpy_to_surface(self, numpy_image: np.ndarray) -> pygame.Surface:
         # Convert numpy image (RGB) to pygame surface
         return pygame.surfarray.make_surface(numpy_image.transpose((1, 0, 2)))
 
-    def _surface_to_numpy(self, surface):
-        # Convert pygame surface to numpy array (RGB)
-        return pygame.surfarray.array3d(surface).transpose((1, 0, 2))
-
-    def _on_draw_surface(self, surface, barcode):
+    def _on_draw_surface(self, surface, barcode: BarcodeData):
         x, y, w, h = barcode.rect
         pygame.draw.rect(surface, (0, 255, 0), (x, y, w, h), 2)
 
+    def get_barcodes(self, array: np.ndarray) -> List[BarcodeData]:
+        if self.pyzbar:
+            decoded_codes = self.pyzbar.decode(array)
+            return [BarcodeData(data=decoded.data, rect=decoded.rect) for decoded in decoded_codes]
+        elif self.cv2:
+            array = self.cv2.transpose(array)
+            array = self.cv2.cvtColor(array, self.cv2.COLOR_RGB2BGR)
+            # Use OpenCV's QRCodeDetector to detect and decode the QR code.
+            detector = self.cv2.QRCodeDetector()
+            val, points, straight_qrcode = detector.detectAndDecode(array)
+
+            barcodes = []
+            if val:
+                # If a QR code is detected, 'val' contains the decoded text.
+                # 'points' contain the coordinates of the QR code corners.
+                if points is not None:
+                    # Convert points to a more manageable format
+                    points = points[0]  # Points are returned in a nested array.
+
+                    # Calculate the bounding rectangle using the points.
+                    y, x, w, h = self.cv2.boundingRect(points.astype(np.int32))
+                    rect = (x, y, w, h)  # Store the rectangle as a tuple
+
+                    barcode = BarcodeData(val.encode(), rect)
+                    barcodes.append(barcode)
+
+            return barcodes
+        else:
+            return []
+
     def update_frame(self):
 
         barcodes = []
         if self.is_screen_capture:
             with mss.mss() as sct:
                 monitor = sct.monitors[1]  # capture the first monitor
                 sct_img = sct.grab(monitor)
@@ -114,15 +169,15 @@
         else:
             try:
                 surface = self.capture.get_image()
             except:
                 # print("Could not get image")
                 return
 
-        barcodes = pyzbar.decode(pygame.surfarray.array3d(surface))
+        barcodes = self.get_barcodes(pygame.surfarray.array3d(surface))
         surface = pygame.transform.flip(surface, False, True)
         surface = pygame.transform.rotate(surface, -90)
 
         for barcode in barcodes:
             self._on_draw_surface(surface, barcode)
             # only show the 1. barcode
             break
@@ -130,15 +185,15 @@
         surface = pygame.transform.flip(surface, False, True)
         self.showSurface(surface, scale_to=(640, 480))
 
         for barcode in barcodes:
             self.signal_qr_data_callback.emit(barcode.data)
             break
 
-    def showSurface(self, surface, scale_to=(640, 480)):
+    def showSurface(self, surface: pygame.Surface, scale_to=(640, 480)):
 
         array3d = pygame.surfarray.array3d(surface)
         height, width, _ = array3d.shape
         bytes_per_line = 3 * width
         q_image = QtGui.QImage(array3d.data, width, height, bytes_per_line, QtGui.QImage.Format.Format_RGB888)
 
         # Convert QImage to QPixmap
@@ -164,18 +219,7 @@
 
         self.layout().addWidget(self.label_qr)
 
     def show_qr(self, qr_data):
         s = qr_data.decode("utf-8")
         print(s)
         self.label_qr.setText(s)
-
-
-if __name__ == "__main__":
-    import sys
-
-    app = QtWidgets.QApplication(sys.argv)
-
-    video_widget = DemoVideoWidget()
-    video_widget.show()
-
-    sys.exit(app.exec_())
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/LICENSE` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/bytewords.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/bytewords.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/cbor_lite.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/cbor_lite.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/crc32.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/crc32.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/fountain_decoder.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/fountain_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # fountain_decoder.py
 #
 # Copyright © 2020 Foundation Devices, Inc.
 # Licensed under the "BSD-2-Clause Plus Patent License"
 #
 
 from .fountain_utils import choose_fragments, contains, is_strict_subset, set_difference
-from .utils import join_bytes, crc32_int, xor_with, take_first
+from .utils import crc32_int, join_bytes, take_first, xor_with
 
 
 class InvalidPart(Exception):
     pass
 
 
 class InvalidChecksum(Exception):
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/fountain_encoder.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/fountain_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # fountain_encoder.py
 #
 # Copyright © 2020 Foundation Devices, Inc.
 # Licensed under the "BSD-2-Clause Plus Patent License"
 #
 
 import math
+
 from .cbor_lite import CBORDecoder, CBOREncoder
-from .fountain_utils import choose_fragments
-from .utils import split, crc32_int, xor_into, data_to_hex
 from .constants import MAX_UINT32, MAX_UINT64
+from .fountain_utils import choose_fragments
+from .utils import crc32_int, data_to_hex, split, xor_into
 
 
 class InvalidHeader(Exception):
     pass
 
 
 class Part:
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/fountain_utils.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/fountain_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # Licensed under the "BSD-2-Clause Plus Patent License"
 #
 
 from .random_sampler import RandomSampler
 from .utils import int_to_bytes
 from .xoshiro256 import Xoshiro256
 
+
 # Fisher-Yates shuffle
 def shuffled(items, rng):
     remaining = items
     result = []
     while len(remaining) > 0:
         index = rng.next_int(0, len(remaining) - 1)
         item = remaining.pop(index)
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/random_sampler.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/random_sampler.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/ur_decoder.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/ur_decoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 # ur_decoder.py
 #
 # Copyright © 2020 Foundation Devices, Inc.
 # Licensed under the "BSD-2-Clause Plus Patent License"
 #
 
-from .ur import UR
-from .fountain_encoder import Part as FountainEncoderPart
-from .fountain_decoder import FountainDecoder
 from .bytewords import *
+from .fountain_decoder import FountainDecoder
+from .fountain_encoder import Part as FountainEncoderPart
+from .ur import UR
 from .utils import drop_first, is_ur_type
 
 
 class InvalidScheme(Exception):
     pass
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/ur_encoder.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/ur_encoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # ur_encoder.py
 #
 # Copyright © 2020 Foundation Devices, Inc.
 # Licensed under the "BSD-2-Clause Plus Patent License"
 #
 
-from .fountain_encoder import FountainEncoder
 from .bytewords import *
+from .fountain_encoder import FountainEncoder
 
 
 class UREncoder:
     # Start encoding a (possibly) multi-part UR.
     def __init__(self, ur, max_fragment_len, first_seq_num=0, min_fragment_len=10):
         self.ur = ur
         self.fountain_encoder = FountainEncoder(ur.cbor, max_fragment_len, first_seq_num, min_fragment_len)
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/utils.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/utils.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/ur/xoshiro256.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/ur/xoshiro256.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     import uhashlib as hashlib
 except:
     try:
         import hashlib
     except:
         sys.exit("ERROR: No hashlib or uhashlib implementation found (required for sha256)")
 
-from ..ur.utils import string_to_bytes, int_to_bytes
 from ..ur.constants import MAX_UINT64
+from ..ur.utils import int_to_bytes, string_to_bytes
 
 # Original Info:
 # Written in 2018 by David Blackman and Sebastiano Vigna (vigna@acm.org)
 
 # To the extent possible under law, the author has dedicated all copyright
 # and related and neighboring rights to this software to the public domain
 # worldwide. This software is distributed without any warranty.
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/LICENSE.md` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/__init__.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from .registry import *
 from .bytes import *
+from .registry import *
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/bytes.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/bytes.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from ..urtypes import RegistryType, RegistryItem
+from ..urtypes import RegistryItem, RegistryType
 
 BYTES = RegistryType("bytes", None)
 
 
 class Bytes(RegistryItem):
     def __init__(self, data):
         super().__init__()
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/COPYING` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/COPYING`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/__init__.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/data.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/data.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/decoder.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/decoder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 # coding: utf-8
 
-import struct
 import math
+import struct
 
 from .data import DataItem, Undefined
 
 
 class InvalidCborError(Exception):
     pass
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/cbor/encoder.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/cbor/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # coding: utf-8
 
 import struct
 
 _str_type = type("")
 _bytes_type = type(b"")
 
-from .data import Tagging, Mapping, Undefined
+from .data import Mapping, Tagging, Undefined
 
 
 class EncoderError(Exception):
     pass
 
 
 class Encoder(object):
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/__init__.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/account.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from ...urtypes import RegistryType, RegistryItem
+from ...urtypes import RegistryItem, RegistryType
 from .output import Output
 
 CRYPTO_ACCOUNT = RegistryType("crypto-account", 311)
 
 
 class Account(RegistryItem):
     def __init__(self, master_fingerprint, output_descriptors):
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/bip39.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/bip39.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from ...urtypes import RegistryType, RegistryItem
+from ...urtypes import RegistryItem, RegistryType
 
 CRYPTO_BIP39 = RegistryType("crypto-bip39", 301)
 
 
 class BIP39(RegistryItem):
     def __init__(self, words, lang):
         super().__init__()
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/coin_info.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/coin_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from ...urtypes import RegistryType, RegistryItem
+from ...urtypes import RegistryItem, RegistryType
 
 CRYPTO_COIN_INFO = RegistryType("crypto-coin-info", 305)
 
 
 class CoinInfo(RegistryItem):
     def __init__(self, type, network):
         super().__init__()
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/ec_key.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/ec_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 import binascii
-from ...urtypes import RegistryType, RegistryItem
+
+from ...urtypes import RegistryItem, RegistryType
 
 CRYPTO_ECKEY = RegistryType("crypto-eckey", 306)
 
 
 class ECKey(RegistryItem):
     def __init__(self, data, curve, private_key):
         super().__init__()
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/hd_key.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/hd_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 import binascii
 import hashlib
-from ...urtypes import RegistryType, RegistryItem
+
+from ...urtypes import RegistryItem, RegistryType
 from ...urtypes.cbor import DataItem
 from .coin_info import CoinInfo
 from .keypath import Keypath
 
 CRYPTO_HDKEY = RegistryType("crypto-hdkey", 303)
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/keypath.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/keypath.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from ...urtypes import RegistryType, RegistryItem
+from ...urtypes import RegistryItem, RegistryType
 
 CRYPTO_KEYPATH = RegistryType("crypto-keypath", 304)
 
 
 class Keypath(RegistryItem):
     def __init__(self, components, source_fingerprint, depth):
         super().__init__()
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/multi_key.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/multi_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 from ...urtypes import RegistryItem
 from ...urtypes.cbor import DataItem
-from .hd_key import HDKey, CRYPTO_HDKEY
-from .ec_key import ECKey, CRYPTO_ECKEY
+from .ec_key import CRYPTO_ECKEY, ECKey
+from .hd_key import CRYPTO_HDKEY, HDKey
 
 
 class MultiKey(RegistryItem):
     def __init__(self, threshold, ec_keys, hd_keys):
         super().__init__()
         self.threshold = threshold
         self.ec_keys = ec_keys
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/output.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 import io
-from ...urtypes import RegistryType, RegistryItem
+
+from ...urtypes import RegistryItem, RegistryType
 from ...urtypes.cbor import DataItem
-from .multi_key import MultiKey
-from .hd_key import HDKey, CRYPTO_HDKEY
 from .ec_key import ECKey
+from .hd_key import CRYPTO_HDKEY, HDKey
+from .multi_key import MultiKey
 
 
 class ScriptExpression:
     def __init__(self, tag, expression):
         self.tag = tag
         self.expression = expression
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/crypto/psbt.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/crypto/psbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from ...urtypes import RegistryType, Bytes
+from ...urtypes import Bytes, RegistryType
 
 CRYPTO_PSBT = RegistryType("crypto-psbt", 310)
 
 
 class PSBT(Bytes):
     @classmethod
     def registry_type(cls):
```

### Comparing `bitcoin_qrreader-0.8.1/bitcoin_qrreader/urtypes/registry.py` & `bitcoin_qrreader-0.8.3/bitcoin_qrreader/urtypes/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 import io
-from ..urtypes.cbor import decoder, encoder, DataItem
+
+from ..urtypes.cbor import DataItem, decoder, encoder
 
 
 class RegistryType:
     def __init__(self, type, tag):
         self.type = type
         self.tag = tag
```

### Comparing `bitcoin_qrreader-0.8.1/pyproject.toml` & `bitcoin_qrreader-0.8.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 show_error_codes = true 
 disable_error_code = "assignment"
 
 
 
 [tool.poetry]
 name = "bitcoin-qrreader"
-version = "0.8.1"
+version = "0.8.3"
 authors = ["andreasgriffin <andreasgriffin@proton.me>"]
 license = "GPL-3.0"
 readme = "README.md"
 description = "A python bitcoin qr reader"
 homepage = "https://github.com/andreasgriffin/bitcoin-qrreader"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 pyqt6 = "^6.6.1"
 base58 = "2.1.1"
 bdkpython ="0.31.0"
 pygame ="2.5.0"
-pyzbar ="0.1.9"
 numpy = "^1.21.0"
 mss ="9.0.1"
 hwi = "2.3.1"
+opencv-python = "^4.9.0.80"
+pyzbar = "^0.1.9"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `bitcoin_qrreader-0.8.1/PKG-INFO` & `bitcoin_qrreader-0.8.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin-qrreader
-Version: 0.8.1
+Version: 0.8.3
 Summary: A python bitcoin qr reader
 Home-page: https://github.com/andreasgriffin/bitcoin-qrreader
 License: GPL-3.0
 Author: andreasgriffin
 Author-email: andreasgriffin@proton.me
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,17 +14,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: base58 (==2.1.1)
 Requires-Dist: bdkpython (==0.31.0)
 Requires-Dist: hwi (==2.3.1)
 Requires-Dist: mss (==9.0.1)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pygame (==2.5.0)
 Requires-Dist: pyqt6 (>=6.6.1,<7.0.0)
-Requires-Dist: pyzbar (==0.1.9)
+Requires-Dist: pyzbar (>=0.1.9,<0.2.0)
 Description-Content-Type: text/markdown
 
 # A python bitcoin qr reader
 
 * Recognizes (and classifies)
   * Addresses  (also BIP21 with amount)
   * Transactions (also base43 electrum encoding)
```

