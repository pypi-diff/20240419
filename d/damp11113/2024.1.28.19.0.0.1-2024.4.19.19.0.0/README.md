# Comparing `tmp/damp11113-2024.1.28.19.0.0.1.tar.gz` & `tmp/damp11113-2024.4.19.19.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damp11113-2024.1.28.19.0.0.1.tar", last modified: Sun Jan 28 12:01:30 2024, max compression
+gzip compressed data, was "damp11113-2024.4.19.19.0.0.tar", last modified: Fri Apr 19 08:47:44 2024, max compression
```

## Comparing `damp11113-2024.1.28.19.0.0.1.tar` & `damp11113-2024.4.19.19.0.0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-01-28 12:01:30.974080 damp11113-2024.1.28.19.0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-11-18 06:45:41.000000 damp11113-2024.1.28.19.0.0.1/LICENSE.rst
--rw-rw-rw-   0        0        0     2832 2024-01-28 12:01:30.974080 damp11113-2024.1.28.19.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1685 2024-01-28 11:50:38.000000 damp11113-2024.1.28.19.0.0.1/README.md
--rw-rw-rw-   0        0        0      115 2024-01-28 12:01:30.976086 damp11113-2024.1.28.19.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2078 2024-01-28 12:01:21.000000 damp11113-2024.1.28.19.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-28 12:01:30.923262 damp11113-2024.1.28.19.0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-28 12:01:30.955060 damp11113-2024.1.28.19.0.0.1/src/damp11113/
--rw-rw-rw-   0        0        0    34969 2023-12-24 19:38:01.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/DSP.py
--rw-rw-rw-   0        0        0     5251 2023-10-24 09:24:15.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/PyserHTTP.py
--rw-rw-rw-   0        0        0    27000 2024-01-20 11:37:59.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/PyserSSH.py
--rw-rw-rw-   0        0        0     3317 2023-12-09 09:35:23.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/__init__.py
--rw-rw-rw-   0        0        0    15730 2024-01-28 11:27:05.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/convert.py
--rw-rw-rw-   0        0        0     7130 2023-10-31 07:18:30.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/file.py
--rw-rw-rw-   0        0        0     9672 2024-01-09 10:30:45.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/format.py
--rw-rw-rw-   0        0        0     7070 2023-10-02 15:53:20.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/imageps.py
--rw-rw-rw-   0        0        0     8535 2024-01-28 11:47:04.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/info.py
--rw-rw-rw-   0        0        0     2955 2023-10-02 15:53:20.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/logic.py
--rw-rw-rw-   0        0        0    25011 2024-01-19 11:30:47.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/media.py
--rw-rw-rw-   0        0        0    11354 2023-11-20 15:59:46.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/minecraft.py
--rw-rw-rw-   0        0        0    12448 2024-01-19 10:15:03.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/network.py
--rw-rw-rw-   0        0        0     8701 2023-10-02 15:53:20.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/plusmata.py
--rw-rw-rw-   0        0        0    13228 2023-12-03 05:39:32.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/processbar.py
--rw-rw-rw-   0        0        0    11792 2024-01-28 11:19:50.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/pywindows.py
--rw-rw-rw-   0        0        0     4682 2023-10-07 12:58:00.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/randoms.py
--rw-rw-rw-   0        0        0    19380 2024-01-20 13:44:04.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-28 12:01:30.972075 damp11113-2024.1.28.19.0.0.1/src/damp11113.egg-info/
--rw-rw-rw-   0        0        0     2832 2024-01-28 12:01:30.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      669 2024-01-28 12:01:30.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       53 2024-01-28 12:01:30.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      292 2024-01-28 12:01:30.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-28 12:01:30.000000 damp11113-2024.1.28.19.0.0.1/src/damp11113.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 08:47:44.128771 damp11113-2024.4.19.19.0.0/
+-rw-rw-rw-   0        0        0     1092 2024-01-28 12:04:30.000000 damp11113-2024.4.19.19.0.0/LICENSE.rst
+-rw-rw-rw-   0        0        0     2886 2024-04-19 08:47:44.127772 damp11113-2024.4.19.19.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1685 2024-01-28 12:04:30.000000 damp11113-2024.4.19.19.0.0/README.md
+-rw-rw-rw-   0        0        0      115 2024-04-19 08:47:44.130277 damp11113-2024.4.19.19.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2098 2024-04-19 08:47:26.000000 damp11113-2024.4.19.19.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:47:44.071146 damp11113-2024.4.19.19.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:47:44.106093 damp11113-2024.4.19.19.0.0/src/damp11113/
+-rw-rw-rw-   0        0        0    36496 2024-03-18 05:47:49.000000 damp11113-2024.4.19.19.0.0/src/damp11113/DSP.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:47:44.123771 damp11113-2024.4.19.19.0.0/src/damp11113/OPFONMW/
+-rw-rw-rw-   0        0        0     3975 2024-03-25 17:00:51.000000 damp11113-2024.4.19.19.0.0/src/damp11113/OPFONMW/StepperLib.py
+-rw-rw-rw-   0        0        0      258 2024-04-08 14:21:20.000000 damp11113-2024.4.19.19.0.0/src/damp11113/OPFONMW/__init__.py
+-rw-rw-rw-   0        0        0    16272 2023-08-12 14:03:04.000000 damp11113-2024.4.19.19.0.0/src/damp11113/OPFONMW/dearpygui_animate.py
+-rw-rw-rw-   0        0        0    12399 2023-10-29 15:43:15.000000 damp11113-2024.4.19.19.0.0/src/damp11113/OPFONMW/ofdm_codec.py
+-rw-rw-rw-   0        0        0     5253 2024-04-07 08:09:44.000000 damp11113-2024.4.19.19.0.0/src/damp11113/PyserHTTP.py
+-rw-rw-rw-   0        0        0     3425 2024-04-19 08:45:06.000000 damp11113-2024.4.19.19.0.0/src/damp11113/__init__.py
+-rw-rw-rw-   0        0        0    16155 2024-02-25 06:15:10.000000 damp11113-2024.4.19.19.0.0/src/damp11113/convert.py
+-rw-rw-rw-   0        0        0     5929 2024-03-15 09:38:31.000000 damp11113-2024.4.19.19.0.0/src/damp11113/file.py
+-rw-rw-rw-   0        0        0    21496 2024-03-15 09:38:31.000000 damp11113-2024.4.19.19.0.0/src/damp11113/format.py
+-rw-rw-rw-   0        0        0     5309 2024-03-15 09:38:31.000000 damp11113-2024.4.19.19.0.0/src/damp11113/imageps.py
+-rw-rw-rw-   0        0        0     8535 2024-04-19 08:45:51.000000 damp11113-2024.4.19.19.0.0/src/damp11113/info.py
+-rw-rw-rw-   0        0        0     2955 2023-10-02 15:53:20.000000 damp11113-2024.4.19.19.0.0/src/damp11113/logic.py
+-rw-rw-rw-   0        0        0    25132 2024-03-17 02:51:35.000000 damp11113-2024.4.19.19.0.0/src/damp11113/media.py
+-rw-rw-rw-   0        0        0    11354 2024-03-15 09:38:31.000000 damp11113-2024.4.19.19.0.0/src/damp11113/minecraft.py
+-rw-rw-rw-   0        0        0     8585 2024-03-15 09:38:31.000000 damp11113-2024.4.19.19.0.0/src/damp11113/network.py
+-rw-rw-rw-   0        0        0    11074 2024-03-02 08:49:18.000000 damp11113-2024.4.19.19.0.0/src/damp11113/plusmata.py
+-rw-rw-rw-   0        0        0    13228 2023-12-03 05:39:32.000000 damp11113-2024.4.19.19.0.0/src/damp11113/processbar.py
+-rw-rw-rw-   0        0        0    10651 2024-03-15 09:43:53.000000 damp11113-2024.4.19.19.0.0/src/damp11113/pywindows.py
+-rw-rw-rw-   0        0        0     4451 2024-04-14 07:48:34.000000 damp11113-2024.4.19.19.0.0/src/damp11113/randoms.py
+-rw-rw-rw-   0        0        0    20748 2024-03-18 07:29:52.000000 damp11113-2024.4.19.19.0.0/src/damp11113/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:47:44.126773 damp11113-2024.4.19.19.0.0/src/damp11113.egg-info/
+-rw-rw-rw-   0        0        0     2886 2024-04-19 08:47:43.000000 damp11113-2024.4.19.19.0.0/src/damp11113.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      792 2024-04-19 08:47:43.000000 damp11113-2024.4.19.19.0.0/src/damp11113.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       53 2024-04-19 08:47:43.000000 damp11113-2024.4.19.19.0.0/src/damp11113.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      316 2024-04-19 08:47:43.000000 damp11113-2024.4.19.19.0.0/src/damp11113.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 08:47:43.000000 damp11113-2024.4.19.19.0.0/src/damp11113.egg-info/top_level.txt
```

### Comparing `damp11113-2024.1.28.19.0.0.1/LICENSE.rst` & `damp11113-2024.4.19.19.0.0/LICENSE.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-2023 damp11113
+Copyright (c) 2021-2024 damp11113
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `damp11113-2024.1.28.19.0.0.1/PKG-INFO` & `damp11113-2024.4.19.19.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damp11113
-Version: 2024.1.28.19.0.0.1
+Version: 2024.4.19.19.0.0
 Summary: A Utils library and Easy to using.
 Home-page: https://github.com/damp11113/damp11113-library
 Author: damp11113
 Author-email: damp51252@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
@@ -20,29 +20,31 @@
 Requires-Dist: libscrc
 Requires-Dist: PyAudio
 Requires-Dist: python-vlc
 Requires-Dist: ffmpeg-python
 Requires-Dist: yt-dlp
 Requires-Dist: youtube_dl
 Requires-Dist: pafy
-Requires-Dist: tqdm
+Requires-Dist: pafy2tqdm
 Requires-Dist: qrcode
 Requires-Dist: python-barcode
 Requires-Dist: pydub
 Requires-Dist: pyzbar
 Requires-Dist: mcstatus
 Requires-Dist: mcrcon
 Requires-Dist: paho-mqtt
 Requires-Dist: requests
 Requires-Dist: pymata-aio
-Requires-Dist: paramiko
 Requires-Dist: six
 Requires-Dist: key-generator
 Requires-Dist: PyQt5
 Requires-Dist: gTTS
+Requires-Dist: py-cpuinfo
+Requires-Dist: GPUtil
+Requires-Dist: playsound
 Requires-Dist: pywin32
 Requires-Dist: win32gui
 Requires-Dist: comtypes
 
 damp11113-library
 ===============
 A Utils library and Easy to use.
@@ -70,14 +72,14 @@
     pip install git+https://github.com/damp11113/damp11113-library.git
     
 License
 ===============
 
 MIT License
 
-Copyright (c) 2021-2022 damp11113
+Copyright (c) 2021-2024 damp11113
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `damp11113-2024.1.28.19.0.0.1/README.md` & `damp11113-2024.4.19.19.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     pip install git+https://github.com/damp11113/damp11113-library.git
     
 License
 ===============
 
 MIT License
 
-Copyright (c) 2021-2022 damp11113
+Copyright (c) 2021-2024 damp11113
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `damp11113-2024.1.28.19.0.0.1/setup.py` & `damp11113-2024.4.19.19.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,29 +18,32 @@
     "libscrc",
     "PyAudio",
     "python-vlc",
     "ffmpeg-python",
     "yt-dlp",
     "youtube_dl",
     "pafy",
+    "pafy2"
     "tqdm",
     "qrcode",
     "python-barcode",
     "pydub",
     "pyzbar",
     "mcstatus",
     "mcrcon",
     "paho-mqtt",
     "requests",
     "pymata-aio",
-    "paramiko",
     "six",
     "key-generator",
     "PyQt5",
     "gTTS",
+    "py-cpuinfo",
+    "GPUtil",
+    "playsound"
 ]
 
 # Windows-specific dependencies
 windows_dependencies = [
     "pywin32",
     "win32gui",
     "comtypes",
@@ -66,15 +69,15 @@
     # Exclude files for non-Windows platforms
     package_data = {
         '': exclude_files_windows,
     }
 
 setup(
     name='damp11113',
-    version='2024.1.28.19.0.0.1', # fix twine can't upload
+    version='2024.4.19.19.0.0',
     license='MIT',
     author='damp11113',
     author_email='damp51252@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/damp11113/damp11113-library',
     description="A Utils library and Easy to using.",
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/DSP.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/DSP.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 damp11113-library - A Utils library and Easy to use. For more info visit https://github.com/damp11113/damp11113-library/wiki
-Copyright (C) 2021-2023 damp11113 (MIT)
+Copyright (C) 2021-2024 damp11113 (MIT)
 
 Visit https://github.com/damp11113/damp11113-library
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
@@ -387,15 +387,19 @@
     q_normalized = q_channel / np.max(np.abs(q_channel))
 
     # Combine I and Q channels into stereo signal
     return np.column_stack((i_normalized, q_normalized))
 
 def getDBFS(audio_array, full_scale=1):
     # Calculate the RMS value of the audio data
-    rms = np.sqrt(np.mean(np.square(audio_array)))
+    rms = np.sqrt(np.mean(np.square(audio_array.astype(np.float32))))
+
+    # Ensure that rms is positive to avoid math domain error
+    if rms <= 0:
+        return float('-inf')  # Return negative infinity for dBFS
 
     # Calculate dBFS
     dbfs = 20 * math.log10(rms / full_scale)
 
     return dbfs
 
 def RTCompressor2(sample_data, Threshold=-20, Knee=10, Ratio=2, Attack=0.01, Release=0.1, Gain=1):
@@ -421,15 +425,14 @@
     gain_reduction[above_knee] -= (1 - (1 / Ratio)) * ((knee_width - 1) ** 2)
 
     # Apply makeup gain and gain reduction
     compressed_audio = sample_data / (10 ** (Gain / 20)) * (1 - gain_reduction)
 
     return compressed_audio
 
-
 def RTEqualizer(sample_data, bands, sample_rate=48000):
     # Check if sample_data is a numpy array, if not, convert it to one
     if not isinstance(sample_data, np.ndarray):
         sample_data = np.array(sample_data, dtype=np.float32)
 
     # Ensure the input audio data has the correct shape (n_samples, n_channels)
     if sample_data.ndim == 1:
@@ -931,7 +934,46 @@
                 roffle = np.sin(2 * np.pi * tone2 * np.arange(samples_per_bit) / samplerate)
                 byte_data = np.append(byte_data, roffle * 0.8)
             else:
                 sinewave = np.sin(2 * np.pi * tone1 * np.arange(samples_per_bit) / samplerate)
                 byte_data = np.append(byte_data, sinewave)
 
     return byte_data
+
+def preamble2(samplerate=48000, baudrate=100, tone1=1000, tone2=2000, hexcode=None):
+    if hexcode is None:
+        hexcode = 0xAB
+
+    # Convert hexadecimal integer to binary string
+    binary_string = bin(hexcode)[2:].zfill(8)
+
+    t = 1.0 / baudrate
+    samples_per_bit = int(t * samplerate)
+    byte_data = np.zeros(0)
+
+    for _ in range(0, 16):
+        for bit in binary_string:
+            if bit == '1':
+                roffle = np.sin(2 * np.pi * tone2 * np.arange(samples_per_bit) / samplerate)
+                byte_data = np.append(byte_data, roffle * 0.8)
+            else:
+                sinewave = np.sin(2 * np.pi * tone1 * np.arange(samples_per_bit) / samplerate)
+                byte_data = np.append(byte_data, sinewave)
+
+    return byte_data
+
+
+def mono2stereo(signal1, signal2):
+    # Check if both signals have the same length
+    if len(signal1) != len(signal2):
+        raise ValueError("Both signals must have the same length")
+
+    # Interleave the samples to create the stereo signal
+    stereo_signal = np.empty((len(signal1), 2), dtype=signal1.dtype)
+    stereo_signal[:, 0] = signal1
+    stereo_signal[:, 1] = signal2
+    return stereo_signal
+
+def stereo2mono(stereo_signal):
+    left_channel = stereo_signal[::2]
+    right_channel = stereo_signal[1::2]
+    return left_channel, right_channel
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/PyserHTTP.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/PyserHTTP.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import logging
 
 logger = logging.getLogger('PyserHTTP')
 
 class HTTPServer:
     def __init__(self):
         self.routes = {}
+
     def route(self, path, methods=['GET']):
         def decorator(func):
             self.routes[path] = {'handler': func, 'methods': methods}
             return func
 
         return decorator
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/__init__.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,40 +22,43 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import os
+import platform
 from .info import __version__
 
 try:
     os.environ["damp11113_load_all_module"]
 except:
     os.environ["damp11113_load_all_module"] = "YES"
 
 if os.environ["damp11113_load_all_module"] == "YES":
+    if platform.system() == "Windows":
+        from .pywindows import *
+        from .OPFONMW.dearpygui_animate import *
+        from .OPFONMW.ofdm_codec import *
+
     from .info import *
     from .file import *
     from .network import *
     from .randoms import *
     from .processbar import *
     from .media import *
-    from .pywindows import *
     from .convert import *
     from .imageps import *
     from .utils import *
     from .minecraft import *
     from .plusmata import *
     from .imageps import *
     from .DSP import *
-    from .OPFONMW.dearpygui_animate import *
     from .logic import *
 
-
 try:
     os.environ["damp11113_check_update"]
 except:
     os.environ["damp11113_check_update"] = "YES"
 
 if os.environ["damp11113_check_update"] == "YES":
     from pygments import console
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/convert.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 damp11113-library - A Utils library and Easy to use. For more info visit https://github.com/damp11113/damp11113-library/wiki
-Copyright (C) 2021-2023 damp11113 (MIT)
+Copyright (C) 2021-2024 damp11113 (MIT)
 
 Visit https://github.com/damp11113/damp11113-library
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
@@ -51,14 +51,28 @@
 def str2bin2(s):
     binary_strings = [format(num, '08b') for num in s]
     return ''.join(binary_strings)
 
 def bin2str(b):
     return ''.join(chr(int(b[i:i+8], 2)) for i in range(0, len(b), 8))
 
+def bytes2bin(data):
+    binary_string = ""
+    for byte in data:
+        binary_string += format(byte, '08b')  # Convert each byte to its binary representation with 8 bits
+    return binary_string
+
+def bin2bytes(binary_string):
+    bytes_data = bytearray()
+    for i in range(0, len(binary_string), 8):
+        byte = binary_string[i:i+8]
+        bytes_data.append(int(byte, 2))
+    return bytes(bytes_data)
+
+
 def list2str(list_):
     return '\n'.join(list_)
 
 def list2str2(list_):
     return ''.join(list_)
 
 def str2list(string):
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/file.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/file.py`

 * *Files 26% similar despite different names*

```diff
@@ -135,74 +135,14 @@
 def appendfileline(file, line, data):
     with open(file, 'r') as f:
         lines = f.readlines()
         lines[line] = data
         with open(file, 'a') as f:
             f.writelines(lines)
 
-#---------------------------------------open---------------------------------
-
-def openfile(ide, file):
-    os.system(f"{ide} {file}")
-
-#---------------------------------------run---------------------------------
-
-def runfile(file):
-    os.system(f"start {file}")
-
-def runpy(file):
-    os.system(f"python {file}")
-
-def runjs(file):
-    os.system(f"node {file}")
-
-def runjava(file):
-    os.system(f"java {file}")
-
-def runbash(file):
-    os.system(f"bash {file}")
-
-def runcpp(file):
-    os.system(f"g++ {file}")
-
-def runc(file):
-    os.system(f"gcc {file}")
-
-def runphp(file):
-    os.system(f"php {file}")
-
-def runruby(file):
-    os.system(f"ruby {file}")
-
-def rungo(file):
-    os.system(f"go {file}")
-
-def runperl(file):
-    os.system(f"perl {file}")
-
-def rundocker(file):
-    os.system(f"docker {file}")
-
-def runvim(file):
-    os.system(f"vim {file}")
-
-def runnano(file):
-    os.system(f"nano {file}")
-
-def rungedit(file):
-    os.system(f"gedit {file}")
-
-def runkate(file):
-    os.system(f"kate {file}")
-
-#--------------------------------------kill---------------------------------
-
-def kill(file):
-    os.system(f"taskkill /f /im {file}")
-
 #--------------------------------------zip----------------------------------
 
 def unzip(file, to):
     with zipfile.ZipFile(file, 'r') as zip_ref:
         zip_ref.extractall(to)
 
 def comzip(file, to):
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/info.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import os
 import time
 import psutil
 import cpuinfo
 import GPUtil
 from .utils import get_format_time3, TextFormatter
 
-__version__ = '2024.1.28.19.0.0' # 2023/1/28 | 19 file (no __init__.py) | --- function |
+__version__ = '2024.4.19.19.0.0' # 2023/4/19 | 19 file (no __init__.py) | --- function |
 
 def pyversion(fullpython=False, fullversion=False, tags=False, date=False, compiler=False, implementation=False, revision=False):
     if fullpython:
         return f'python {sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro} {sys.version_info.releaselevel} {platform.python_build()[0]} {platform.python_build()[1]} {platform.python_compiler()} {platform.python_implementation()} {platform.python_revision()}'
     if fullversion:
         return f'{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}'
     if tags:
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/logic.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/logic.py`

 * *Files identical despite different names*

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/media.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/media.py`

 * *Files 7% similar despite different names*

```diff
@@ -249,32 +249,14 @@
 
     def get_title(self):
         return self.ydl.extract_info(self.url, download=False)['title']
 
     def get_dec(self):
         return self.ydl.extract_info(self.url, download=False)['description']
 
-
-class ffmpeg_stream:
-    def __init__(self) -> None:
-        pass
-
-    def load(self, file_path):
-        self.stream = ffmpeg.input(file_path)
-        return f"Loaded {file_path}"
-
-    def write(self, file_path, acodec='mp4', ac=2, hz='44100', bitrate='320'):
-        ffmpeg.run(self.stream.output(file_path, acodec=acodec, ac=ac, ar=hz, **{'b:a': f'{bitrate}k'}))
-        return f"Writing {file_path}"
-
-    def streaming(self, url, acodec='mp4', ac=2, hz='44100', bitrate='320'):
-        ffmpeg.run(self.stream.output(url, acodec=acodec, ac=ac, ar=hz, **{'b:a': f'{bitrate}k'}))
-        return f"Streaming {url}"
-
-
 def clip2frames(clip_path, frame_path, currentframe=1, filetype='png'):
     try:
         clip = cv2.VideoCapture(clip_path)
         length = int(clip.get(cv2.CAP_PROP_FRAME_COUNT))
         progress = tqdm.tqdm(total=length, unit='frame')
         progress.set_description(f'set output to {frame_path}')
         if not os.path.exists(frame_path):
@@ -341,14 +323,48 @@
     res.save(output)
 
 def repixpil(pilarray, i_size):
     small_img = pilarray.resize(i_size, Image.BILINEAR)
     res = small_img.resize(pilarray.size, Image.NEAREST)
     return res
 
+
+def resziepil(image, max_width, max_height):
+    """
+    Resize an image to fit within a bounding box without cropping.
+
+    Args:
+    image (PIL.Image): The input image object.
+    max_width (int): Maximum width of the bounding box.
+    max_height (int): Maximum height of the bounding box.
+
+    Returns:
+    PIL.Image: The resized image object.
+    """
+    # Calculate new dimensions while preserving aspect ratio
+    width_ratio = max_width / image.width
+    height_ratio = max_height / image.height
+    min_ratio = min(width_ratio, height_ratio)
+    new_width = int(image.width * min_ratio)
+    new_height = int(image.height * min_ratio)
+
+    # Resize the image
+    resized_image = image.resize((new_width, new_height), Image.ANTIALIAS)
+
+    # Create a new image of the correct dimensions, with a white background
+    new_image = Image.new("RGB", (max_width, max_height), "white")
+
+    # Paste the resized image onto the new image, centered
+    x_offset = (max_width - new_width) // 2
+    y_offset = (max_height - new_height) // 2
+    new_image.paste(resized_image, (x_offset, y_offset))
+
+    # Return the resized image
+    return new_image
+
 def qrcodegen(text, showimg=False, save_path='./', filename='qrcode', filetype='png', version=1, box_size=10, border=5, fill_color="black", back_color="white", error_correction=qrcode.constants.ERROR_CORRECT_L, fit=True):
     qr = qrcode.QRCode(
         version=version,
         error_correction=error_correction,
         box_size=box_size,
         border=border,
     )
@@ -416,15 +432,14 @@
             LRGB = (L, R, G, B)
             im.putpixel((x, y), LRGB)
     im.save(opath)
 
 def PIL2DPG(pil_image):
     return CV22DPG(PIL2CV2(pil_image))
 
-
 def CV22DPG(cv2_array):
     try:
         if cv2_array is None or len(cv2_array.shape) < 3:
             print("Invalid or empty array received.")
             return None
 
         if len(cv2_array.shape) == 2:
@@ -445,42 +460,42 @@
     one_time : if you use once than it's True.
     country : TH
     money : money (if have)
     currency : THB
     """
     Version = "0002"+"01" # เวชั่นของ  PromptPay
     if one_time==True: # one_time คือ ต้องการให้โค้ดนี้ครั้งเดียวหรือไม่
-        one_time="010212" # 12 ใช้ครั้งเดียว
+        one_time = "010212" # 12 ใช้ครั้งเดียว
     else:
-        one_time="010211" # 11 ใช้ได้้หลายครั้ง
-    merchant_account_information="2937" # ข้อมูลผู้ขาย
-    merchant_account_information+="0016"+"A000000677010111" # หมายเลขแอปพลิเคชั่น PromptPay
-    if len(account)!=13: # ใช้บัญชีใช้เป็นเบอร์มือถือหรือไม่ ถ้าใช่ จำนวนจะไม่เท่ากับ 13
-        account=list(account)
-        merchant_account_information+="011300" # 01 หมายเลขโทรศัพท์ ความยาว 13 ขึ้นต้น 00
-        if country=="TH":
-            merchant_account_information+="66" # รหัสประเทศ 66 คือประเทศไทย
+        one_time = "010211" # 11 ใช้ได้้หลายครั้ง
+    merchant_account_information = "2937" # ข้อมูลผู้ขาย
+    merchant_account_information += "0016" + "A000000677010111" # หมายเลขแอปพลิเคชั่น PromptPay
+    if len(account) != 13: # ใช้บัญชีใช้เป็นเบอร์มือถือหรือไม่ ถ้าใช่ จำนวนจะไม่เท่ากับ 13
+        account = list(account)
+        merchant_account_information += "011300" # 01 หมายเลขโทรศัพท์ ความยาว 13 ขึ้นต้น 00
+        if country == "TH":
+            merchant_account_information += "66" # รหัสประเทศ 66 คือประเทศไทย
         del account[0] # ตัดเลข 0 หน้าเบอร์ออก
-        merchant_account_information+=''.join(account)
+        merchant_account_information += ''.join(account)
     else:
-        merchant_account_information+="02"+account.replace('-','') # กรณีที่ไม่รับมือถือ แสดงว่าเป็นเลขบัตรประชาชน
-    country="5802"+country # ประเทศ
-    if currency=="THB":
-        currency="5303"+"764" # "764"  คือเงินบาทไทย ตาม https://en.wikipedia.org/wiki/ISO_4217
-    if money!="": # กรณีกำหนดเงิน
-        check_money=money.split('.') # แยกจาก .
-        if len(check_money)==1 or len(check_money[1])==1: # กรณีที่ไม่มี . หรือ มีทศนิยมแค่หลักเดียว
-            money="54"+"0"+str(len(str(float(money)))+1)+str(float(money))+"0"
+        merchant_account_information += "02" + account.replace('-', '') # กรณีที่ไม่รับมือถือ แสดงว่าเป็นเลขบัตรประชาชน
+    country = "5802" + country # ประเทศ
+    if currency == "THB":
+        currency = "5303" + "764" # "764"  คือเงินบาทไทย ตาม https://en.wikipedia.org/wiki/ISO_4217
+    if money != "": # กรณีกำหนดเงิน
+        check_money = money.split('.') # แยกจาก .
+        if len(check_money) == 1 or len(check_money[1]) == 1: # กรณีที่ไม่มี . หรือ มีทศนิยมแค่หลักเดียว
+            money = "54" + "0" + str(len(str(float(money)))+1) + str(float(money)) + "0"
         else:
-            money="54"+"0"+str(len(str(float(money))))+str(float(money)) # กรณีที่มีทศนิยมครบ
-    check_sum=Version+one_time+merchant_account_information+country+currency+money+"6304" # เช็คค่า check sum
-    check_sum1=hex(libscrc.ccitt(check_sum.encode("ascii"),0xffff)).replace('0x','')
-    if len(check_sum1)<4: # # แก้ไขข้อมูล check_sum ไม่ครบ 4 หลัก
-        check_sum1=("0"*(4-len(check_sum1)))+check_sum1
-    check_sum+=check_sum1
+            money = "54" + "0" + str(len(str(float(money)))) + str(float(money)) # กรณีที่มีทศนิยมครบ
+    check_sum = Version + one_time + merchant_account_information + country + currency + money + "6304" # เช็คค่า check sum
+    check_sum1 = hex(libscrc.ccitt(check_sum.encode("ascii"), 0xffff)).replace('0x', '')
+    if len(check_sum1) < 4: # # แก้ไขข้อมูล check_sum ไม่ครบ 4 หลัก
+        check_sum1 = ("0" * (4 - len(check_sum1))) + check_sum1
+    check_sum += check_sum1
     return check_sum.upper() # upper ใช้คืนค่าสตริงเป็นตัวพิมพ์ใหญ่
 
 def change_color_bit(image, output, colorbit=64):
     img = Image.open(image)
     a = img.convert("P", palette=Image.ADAPTIVE, colors=colorbit)
     a.save(output)
 
@@ -550,14 +565,16 @@
     info = p.get_host_api_info_by_index(0)
     numdevices = info.get('deviceCount')
     for i in range(0, numdevices):
         if (p.get_device_info_by_host_api_device_index(0, i).get('maxInputChannels')) > 0:
             lis.append([i, p.get_device_info_by_host_api_device_index(0, i).get('name')])
     return lis
 
+# --------------------------------------------------------
+
 def EdgeDetection(cvarray):
     # Convert to graycsale
     img_gray = cv2.cvtColor(cvarray, cv2.COLOR_BGR2GRAY)
     # Blur the image for better edge detection
     img_blur = cv2.GaussianBlur(img_gray, (3, 3), 0)
     edges = cv2.Canny(image=img_blur, threshold1=100, threshold2=200)  # Canny Edge Detection
     return edges
@@ -632,48 +649,20 @@
                 cv2.rectangle(frame, (x, y), (x + w, y + h), fcolor, 2)
                 text = f"{self.classes[class_ids[i]]}: {confidences[i]:.2f}"
                 cv2.putText(frame, text, (x, y - 5), cv2.FONT_HERSHEY_SIMPLEX, 0.5, tcolor, 2)
                 info.append([self.classes[class_ids[i]], confidences[i], x, y, w, h])
 
         return frame, info
 
-def mp32pyaudio(file, convertpyaudio=False):
+def audiofile2pyaudio(file, format, codec, startat=0, convertpyaudio=False, arrayformat=np.int16):
     """
-    !!Warning, this conversion with this function is very loud. please turn down the volume. this function be beta!!
-
-    @param file: mp3 file, convertpyaudio=False
-    @return: data, sample_rate, audio_format, channels
-
-    ex.
-
-    data, sample_rate, audio_format, channels = mp32pyaudio(file_path, convertpyaudio=True)
-
-    # Create an instance of the PyAudio class
-    p = pyaudio.PyAudio()
-
-    # Open a PyAudio stream
-    stream = p.open(format=audio_format,
-                    channels=channels,
-                    rate=sample_rate,
-                    output=True)
-
-    audio_bytes = data.astype(np.float32).tobytes()
-
-    stream.write(audio_bytes)
-
+    data, sample_rate, audio_format, channels = audiofile2pyaudio(file_path, format="ogg", codec="opus", convertpyaudio=True)
     """
-
     # import file
-    audio = AudioSegment.from_mp3(file)
-
-    # get info
-    sample_rate = audio.frame_rate
-    audio_format = audio.sample_width
-    channels = audio.channels
-
-    # read samples
+    audio = AudioSegment.from_file(file, format, codec, start_second=startat)
+    # read samples to array
     audio_bytes = np.array(audio.get_array_of_samples())
+    # convert
     if convertpyaudio:
-        print("Please use int16")
-        audio_bytes = audio_bytes.astype(np.int16).reshape((-1, channels)).tobytes()
+        audio_bytes = audio_bytes.astype(arrayformat).reshape((-1, audio.channels)).tobytes()
 
-    return audio_bytes, sample_rate, audio_format, channels
+    return audio_bytes, audio.frame_rate, audio.sample_width, audio.channels
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/minecraft.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/minecraft.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 class install_exception(Exception):
     pass
 
 class rcon_exception(Exception):
     pass
 
 #------------------------server------------------------------
+
 class mcserver:
     def __init__(self, server='server.jar', java='java', ramuse='1024', nogui=True, noguipp=False):
         self.serverf = server
         self.java = java
         self.ramuse = ramuse
         self.nogui = nogui
         self.noguipp = noguipp
@@ -140,15 +141,14 @@
         # json to dict
         d = json.loads(js)
         # get skin url
         return d['timestamp']
     except Exception as e:
         raise uuid2name_exception(f"error: {e}")
 
-
 #----------------------mcstatus------------------------
 
 def mcstatusplayerparse(sample):
     listplayer = []
     for p in sample:
         listplayer.append(p.name)
     return listplayer
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/network.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/network.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,24 +24,21 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import socket
 import traceback
 from tqdm import tqdm
-import webbrowser
 import paho.mqtt.client as mqtt
 import time
 from .file import *
-import youtube_dl
-from .convert import bin2str, byte2str, str2bin
-import yt_dlp as youtube_dl2
+from .convert import byte2str
 import re
 import requests
-from .utils import get_size_unit, emb
+from .utils import emb
 from .processbar import LoadingProgress, steps5
 
 class vc_exception(Exception):
     pass
 
 class line_api_exception(Exception):
     pass
@@ -51,15 +48,14 @@
 
 class receive_exception(Exception):
     pass
 
 class send_exception(Exception):
     pass
 
-
 def youtube_search(search, firstresult=True):
     formatUrl = requests.get(f'https://www.youtube.com/results?search_query={search}')
     search_result = re.findall(r'watch\?v=(\S{11})', formatUrl.text)
 
     if firstresult:
         return f"https://www.youtube.com/watch?v={search_result[0]}"
     else:
@@ -72,28 +68,14 @@
     try:
         s.connect((ip, port))
         rech = f'{ip}:{port} is connected'
     except socket.error as e:
         raise ip_exeption(f'{ip}:{port} is disconnected')
     return rech
 
-attack_num = 0
-
-def http_ddos_attack(target): #beta
-    while True:
-        try:
-            d = requests.get(target)
-            global attack_num
-            attack_num += 1
-            print(f'[{attack_num}] {target} is connected')
-            d.close()
-        except:
-            print(f'[-] ddos attack is stop because {target} is disconnected')
-            pass
-
 #-------------------------download---------------------------
 
 def loadfile(url, filename):
     progress = LoadingProgress(desc=f'loading file from {url}', steps=steps5, unit="B", shortunitsize=1024, shortnum=True)
     progress.start()
     try:
         progress.desc = f'Downloading {filename} from {url}'
@@ -115,66 +97,16 @@
         progress.stop()
     except Exception as e:
         progress.status = "Error"
         progress.faill = f"[ ❌ ] Failed to download {filename} from {url} | " + str(e)
         progress.stopfail()
         emb(str(e), traceback.print_exc())
 
-def installpackage(package):
-    os.system(f'title install {package}')
-    os.system(f'pip install {package}')
-
-ydl_optss = {
-    'format': 'bestvideo[ext=mp4]+bestaudio[ext=m4a]/best[ext=mp4]/best',
-    'outtmpl': '%(title)s.%(ext)s'
-}
-
-def ytload(url, ydl_opts=ydl_optss):
-    try:
-        with youtube_dl.YoutubeDL(ydl_opts) as ydl:
-            ydl.download([url])
-    except:
-        print("ytload error")
-        pass
-
-def ytload2(url, ydl_opts=ydl_optss):
-    try:
-        with youtube_dl2.YoutubeDL(ydl_opts) as ydl:
-            ydl.download([url])
-    except:
-        print("ytload error")
-        pass
-#----------------------------read------------------------------
-
-def readtextweb(url):
-    try:
-        r = requests.get(url)
-        return r.text
-    except Exception as e:
-        print("read error", e)
-
-#-----------------------------open-----------------------------
-
-def openurl(url):
-    webbrowser.open(url)
-
 #-----------------------------send-----------------------------
 
-def sendtext(url, text):
-    try:
-        return requests.post(url, data=text).status_code
-    except Exception as e:
-        raise send_exception(f'send error: {e}')
-
-def sendfile(url, file):
-    try:
-        requests.post(url, files=file)
-    except Exception as e:
-        raise send_exception(f'send error: {e}')
-
 def mqtt_publish(topic, message, port=1883, host="localhost"):
     try:
         client = mqtt.Client()
         client.connect(host, port, 60)
         client.publish(topic, message)
         client.disconnect()
     except Exception as e:
@@ -196,24 +128,14 @@
         s.connect((host, port))
         s.sendall(bytes(message, "utf-8"))
         s.close()
         print(f"udp send to {host}:{port}")
     except Exception as e:
         raise send_exception(f'send error: {e}')
 
-def binary_send(host, port, message):
-    try:
-        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        s.connect((host, port))
-        s.sendall(bytes(str2bin(message), 'utf-8'))
-        s.close()
-        print(f"binary send to {host}:{port}")
-    except Exception as e:
-        raise send_exception(f'send error: {e}')
-
 def file_send(host, port, file, buffsize=4096, speed=0.0000001):
     try:
         filesize = sizefile(file)
         s = socket.socket()
         s.connect((host, port))
         s.send(f"{file}{filesize}".encode())
         progress_bar = tqdm(total=filesize, unit='B', unit_scale=True, desc=f'Sending {file}')
@@ -262,27 +184,14 @@
         data, addr = s.recvfrom(1024)
         s.close()
         print(f"udp receive from {host}:{port}")
         return byte2str(data)
     except Exception as e:
         raise receive_exception(f'receive error: {e}')
 
-def binary_receive(host, port):
-    try:
-        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        s.bind((host, port))
-        s.listen(1)
-        conn, addr = s.accept()
-        data = bin2str(conn.recv(1024))
-        conn.close()
-        print(f"binary receive from {host}:{port}")
-        return byte2str(data)
-    except Exception as e:
-        raise receive_exception(f'receive error: {e}')
-
 def file_receive(host, port, buffsize=4096, speed=0.0000001):
     try:
         s = socket.socket()
         s.bind((host, port))
         s.listen(5)
         conn, addr = s.accept()
         received = conn.recv(buffsize)
@@ -298,58 +207,14 @@
                 progress_bar.update(len(data))
                 time.sleep(speed)
         progress_bar.close()
         conn.close()
     except Exception as e:
         raise receive_exception(f'receive error: {e}')
 
-#-----------------------------run-----------------------------
-
-def runngrok(type, ip, port):
-    os.system(f"start ngrok {type} {ip}:{port}")
-
-#---------flask------------------
-
-def flask_run(url, port):
-    os.system(f"flask run --host {url} --port {port}")
-
-def flask_run_debug(url, port):
-    os.system(f"flask run --host {url} --port {port} --debug")
-
-def flask_run_ssl(url, port, cert, key):
-    os.system(f"flask run --host {url} --port {port} --ssl-cert {cert} --ssl-key {key}")
-
-def flask_run_debug_ssl(url, port, cert, key):
-    os.system(f"flask run --host {url} --port {port} --debug --ssl-cert {cert} --ssl-key {key}")
-
-#----webshell------------------
-
-def runwebshell(url):
-    os.system(f"webshell {url}")
-
-def runwebshell_debug(url):
-    os.system(f"webshell {url} --debug")
-
-def runwebshell_ssl(url, cert, key):
-    os.system(f"webshell {url} --ssl-cert {cert} --ssl-key {key}")
-
-def runwebshell_debug_ssl(url, cert, key):
-    os.system(f"webshell {url} --debug --ssl-cert {cert} --ssl-key {key}")
-
-#----------------------------kill-----------------------------
-
-def killngrok():
-    os.system("taskkill /f /im ngrok.exe")
-
-def killflask():
-    os.system("taskkill /f /im flask.exe")
-
-def killwebshell():
-    os.system("taskkill /f /im webshell.exe")
-
 #----------------------line-api------------------------
 
 class line_notify:
     def __init__(self, token):
         self.token = token
 
     def send(self, message):
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/plusmata.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/plusmata.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+import time
 
 from pymata_aio.pymata3 import PyMata3        # type: ignore
 from pymata_aio.constants import Constants    # type: ignore
 from PIL import Image
 
 # matrix led
 
@@ -237,8 +238,74 @@
             m = get_matrix(data, x, y)
             sprites[i] = make_sprite(m)
         self.sprites = sprites
 
     def get_sprite(self, ch):
         return self.sprites[ord(ch)]
 
-#----------------------------------------------------------------------------------------------------------------------
+#----------------------------------------------------------------------------------------------------------------------
+
+class StepperMotor5:
+    def __init__(self, board, motor_pins):
+        self.board = board
+        self.motor_pins = motor_pins
+        self.steps_sequence = [
+            [1, 0, 1, 0, 1],  # Step 0: 01101
+            [1, 0, 0, 0, 1],  # Step 1: 01001
+            [1, 0, 1, 1, 1],  # Step 2: 01011
+            [1, 0, 0, 1, 0],  # Step 3: 01010
+            [1, 1, 0, 1, 0],  # Step 4: 11010
+            [1, 0, 0, 1, 0],  # Step 5: 10010
+            [1, 1, 1, 1, 0],  # Step 6: 10110
+            [1, 0, 1, 0, 0],  # Step 7: 10100
+            [1, 0, 1, 0, 1],  # Step 8: 10101
+            [0, 0, 1, 0, 1]   # Step 9: 00101
+        ]
+        self.number_of_steps = len(self.steps_sequence)
+        self.step_delay = 0
+        self.set_speed(60)
+
+        # Set up pins for output
+        for pin in self.motor_pins:
+            self.board.digital[pin].mode = 1
+
+    def set_speed(self, speed):
+        self.step_delay = 60 * 1000 / self.number_of_steps / speed
+
+    def step(self, steps_to_move):
+        steps_left = abs(steps_to_move)
+        direction = 1 if steps_to_move > 0 else 0
+
+        while steps_left > 0:
+            for step in range(self.number_of_steps):
+                for i, pin in enumerate(self.motor_pins):
+                    self.board.digital[pin].write(self.steps_sequence[step][i])
+                time.sleep(self.step_delay / 1000.0)  # delay is in milliseconds
+            steps_left -= 1
+
+class StepperMotor4:
+    def __init__(self, board, step_pin, direction_pin):
+        self.board = board
+        self.step_pin = step_pin
+        self.direction_pin = direction_pin
+
+        self.board.digital[self.step_pin].mode = 1
+        self.board.digital[self.direction_pin].mode = 1
+
+        self.step_delay = 0
+        self.set_speed(60)
+
+    def set_speed(self, speed):
+        self.step_delay = 60 * 1000 / speed
+
+    def step(self, steps_to_move):
+        direction = 1 if steps_to_move > 0 else 0
+        steps_left = abs(steps_to_move)
+
+        self.board.digital[self.direction_pin].write(direction)
+
+        while steps_left > 0:
+            self.board.digital[self.step_pin].write(1)
+            time.sleep(self.step_delay / 1000.0)
+            self.board.digital[self.step_pin].write(0)
+            time.sleep(self.step_delay / 1000.0)
+            steps_left -= 1
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/processbar.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/processbar.py`

 * *Files identical despite different names*

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/pywindows.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/pywindows.py`

 * *Files 24% similar despite different names*

```diff
@@ -224,72 +224,17 @@
             self.destroy(self.hwnd, 0, 0, 0)
         elif 1024 <= id < 1024 + len(self.menu_options):
             self.menu_options[id - 1024][2](self)
 
     def loop(self):
         win32gui.PumpMessages()
 
-class color:
-    def __init__(self) -> None:
-        pass
-
-    def black(self):
-        os.system('color 0')
-    def blue(self):
-        os.system('color 1')
-    def green(self):
-        os.system('color 2')
-    def Aqua(self):
-        os.system('color 3')
-    def red(self):
-        os.system('color 4')
-    def purple(self):
-        os.system('color 5')
-    def yellow(self):
-        os.system('color 6')
-    def white(self):
-        os.system('color 7')
-    def gray(self):
-        os.system('color 8')
-    def lightblue(self):
-        os.system('color 9')
-    def lightgreen(self):
-        os.system('color a')
-    def lightaqua(self):
-        os.system('color b')
-    def lightred(self):
-        os.system('color c')
-    def lightpurple(self):
-        os.system('color d')
-    def lightyellow(self):
-        os.system('color e')
-    def lightwhite(self):
-        os.system('color f')
-
-def title(title):
-    os.system(f'title {title}')
-
-def pause():
-    os.system('pause')
-
-def cexit():
-    os.system('exit')
-
-def clear():
-    os.system('cls')
-
 def size(x, y):
     os.system('mode con: cols={} lines={}'.format(x, y))
 
-def echo(message='Hello world'):
-    os.system(f'echo {message}')
-
-def cmd(command='echo hello world!'):
-    return os.system(command)
-
 def setConsoleTitle(window_title_string, wait_for_change=False):
     os.system("title " + window_title_string)
     if (wait_for_change):
         matched_window = 0
         while (matched_window == 0):
             matched_window = win32gui.FindWindow(None, window_title_string)
             time.sleep(0.025)  # To not flood it too much...
@@ -299,7 +244,10 @@
 def setConsoleIcon(window_title, image_path):
     hwnd = win32gui.FindWindow(None, window_title)
     icon_flags = win32con.LR_LOADFROMFILE | win32con.LR_DEFAULTSIZE
     hicon = win32gui.LoadImage(None, image_path, win32con.IMAGE_ICON, 0, 0, icon_flags)
 
     win32gui.SendMessage(hwnd, win32con.WM_SETICON, win32con.ICON_SMALL, hicon)
     win32gui.SendMessage(hwnd, win32con.WM_SETICON, win32con.ICON_BIG, hicon)
+
+def mbox(title, text, style):
+    return ctypes.windll.user32.MessageBoxW(0, text, title, style)
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/randoms.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/randoms.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,22 +24,25 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import random
 import string
 import uuid
-from key_generator.key_generator import generate
 from .convert import list2str2
 
-
 def rannum(number1, number2):
     try:
-        output = random.randint(int(number1), int(number2))
-        return output
+        return random.randint(int(number1), int(number2))
+    except ValueError:
+        print("Please enter a number1 to number2")
+
+def rannumfloat(number1, number2):
+    try:
+        return random.uniform(number1, number2)
     except ValueError:
         print("Please enter a number1 to number2")
 
 def ranstr(charset):
     try:
         char_set = string.ascii_uppercase + string.digits
         output = ''.join(random.sample(char_set * int(charset), int(charset)))
@@ -48,69 +51,35 @@
         print("Please enter a number charset")
 
 def ranuuid(uuid_type='uuid1'):
     if uuid_type == "uuid1":
         return uuid.uuid1()
     elif uuid_type == "uuid4":
         return uuid.uuid4()
-
 def ranchoice(list):
     try:
         output = random.choice(list)
         return output
     except ValueError:
         print("Please enter a list")
 
-def ranchoices(list, number):
-    try:
-        output = random.choices(list, k=number)
-        return output
-    except ValueError:
-        print("Please enter a list")
-
 def ranshuffle(list):
     try:
         output = random.shuffle(list)
         return output
     except ValueError:
         print("Please enter a list")
 
-def ranuniform(number1, number2):
-    try:
-        output = random.uniform(number1, number2)
-        return output
-    except ValueError:
-        print("Please enter a number1 to number2")
-
-def ranrandint(number1, number2):
-    try:
-        output = random.randint(number1, number2)
-        return output
-    except ValueError:
-        print("Please enter a number1 to number2")
-
 def ranrandrange(number1, number2):
     try:
         output = random.randrange(number1, number2)
         return output
     except ValueError:
         print("Please enter a number1 to number2")
 
-def rankeygen(min, max, seed=None):
-    if seed is None:
-        try:
-            return generate(max_atom_len=max, min_atom_len=min).get_key()
-        except ValueError:
-            print("Please enter a key_type and key_length")
-    else:
-        try:
-            return generate(max_atom_len=max, min_atom_len=min, seed=seed).get_key()
-        except ValueError:
-            print("Please enter a key_type and key_length")
-
 def rancolor():
     """RGB"""
     return (rannum(1, 255), rannum(1, 255), rannum(1, 255))
 
 def rantextuplow(text):
     nct = list(text)
     ct = []
@@ -138,9 +107,31 @@
     # Flip the selected bits
     received_codeword = list(codeword)
     for index in error_indices:
         received_codeword[index] = '1' if received_codeword[index] == '0' else '0'
 
     return ''.join(received_codeword)
 
+
+def ranlossbytes(data, loss_percentage):
+    if not 0 <= loss_percentage <= 100:
+        raise ValueError("Loss percentage should be between 0 and 100")
+
+    num_bytes_to_drop = int(len(data) * (loss_percentage / 100))
+    indices_to_drop = random.sample(range(len(data)), num_bytes_to_drop)
+
+    result = bytearray()
+    for i, byte in enumerate(data):
+        if i not in indices_to_drop:
+            result.append(byte)
+
+    return bytes(result)
+
 def rannumlist(number1, number2, maxrange):
-    return [random.randint(number1, number2) for _ in range(maxrange)]
+    return [random.randint(number1, number2) for _ in range(maxrange)]
+
+def generate_binary_combinations(width):
+    binarys = []
+    total_combinations = 2 ** width
+    for i in range(total_combinations):
+        binarys.append(format(i, '0' + str(width) + 'b'))
+    return binarys
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113/utils.py` & `damp11113-2024.4.19.19.0.0/src/damp11113/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 damp11113-library - A Utils library and Easy to use. For more info visit https://github.com/damp11113/damp11113-library/wiki
-Copyright (C) 2021-2023 damp11113 (MIT)
+Copyright (C) 2021-2024 damp11113 (MIT)
 
 Visit https://github.com/damp11113/damp11113-library
 
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
@@ -107,16 +107,15 @@
 def typing(text, speed=0.3):
     for character in text:
         sys.stdout.write(character)
         sys.stdout.flush()
         time.sleep(speed)
 
 def timestamp():
-    now = datetime.now()
-    return datetime.timestamp(now)
+    return datetime.timestamp(datetime.now())
 
 def full_cpu(min=100, max=10000, speed=0.000000000000000001):
     _range = rannum(min, max)
     class thread_class(Thread):
         def __init__(self, name, _range):
             Thread.__init__(self)
             self.name = name
@@ -126,28 +125,14 @@
                 print(f'{self.name} is running')
     for i in range(_range):
         name = f'Thread {i}/{_range}'
         thread = thread_class(name, _range)
         thread.start()
         sleep(speed)
 
-def full_disk(min=100, max=10000,speed=0.000000000000000001):
-    ra = rannum(min, max)
-    for i in range(ra):
-        createfile('test.txt')
-        writefile2('test.txt', 'test')
-        readfile('test.txt')
-        removefile('test.txt')
-        sleep(speed)
-        print(f'{i}/{ra}')
-
-
-def mbox(title, text, style):
-    return ctypes.windll.user32.MessageBoxW(0, text, title, style)
-
 def tts(text, lang, play=True, name='tts.mp3', slow=False):
     tts = gTTS(text=text, lang=lang, slow=slow)
     tts.save(name)
     if play:
         playsound(name)
         removefile(name)
 
@@ -196,24 +181,14 @@
     retval = msg.exec_()
 
     if retval == 0:
         return True
     else:
         sys.exit()
 
-class Queue:
-    def __init__(self, queue):
-        self.queue = queue
-    def put(self, item):
-        self.queue.append(item)
-    def get(self):
-        r = self.queue[0]
-        self.queue.pop(0)
-        return r
-
 def get_size_unit(bytes):
     for unit in ['', 'K', 'M', 'G', 'T', 'P']:
         if bytes < 1024:
             return f"{bytes:.2f} {unit}B/s"
         bytes /= 1024
 
 def get_size_unit2(number, unitp, persec=True, unitsize=1024, decimal=True, space=" "):
@@ -236,14 +211,19 @@
 def textonumber(text):
     l = []
     tl = list(text)
     for i in tl:
         l.append(ord(i))
     return ''.join(str(v) for v in l)
 
+def numbertotext(numbers):
+    l = []
+    for i in range(0, len(numbers), 2):
+        l.append(chr(int(numbers[i:i+2])))
+    return ''.join(l)
 
 def Amap(x, in_min, in_max, out_min, out_max):
     try:
         return int((x - in_min) * (out_max - out_min) / (in_max - in_min) + out_min)
     except:
         return 0
 
@@ -297,15 +277,14 @@
     elif sec >= 60: # minutes
         m, s = divmod(sec, 60)
         h, m = divmod(m, 60)
         return f"{m}m {s}s"
     else:
         return f"{sec}s"
 
-
 def get_format_time2(sec):
     if sec >= 31557600: # years
         m, s = divmod(sec, 60)
         h, m = divmod(m, 60)
         d, h = divmod(h, 24)
         y, d = divmod(d, 365)
         return f"{y}y {d}d {str(h).zfill(2)}:{str(m).zfill(2)}:{str(sec).zfill(2)}"
@@ -382,22 +361,16 @@
         raise ValueError("n must be a positive integer.")
 
     chunks = [original_string[i:i+n] for i in range(0, len(original_string), n)]
     result = add_string.join(chunks)
     return result
 
 def findStringDifferencesInList(list1, list2):
-    # Convert the input lists to sets
-    set1 = set(list1)
-    set2 = set(list2)
-
     # Find the differences between the sets
-    difference = list(set1.symmetric_difference(set2))
-
-    return difference
+    return list(set(list1).symmetric_difference(set(list2)))
 
 def replaceEnterWithCrlf(input_string):
     if '\n' in input_string:
         input_string = input_string.replace('\n', '\r\n')
     return input_string
 
 def scrollTextBySteps(text, scrollstep, scrollspace=10):
@@ -559,14 +532,61 @@
         if target_text == "":
             formatted_text += text + TextFormatter.RESET
         else:
             formatted_text += text[:start_index] + text[start_index:end_index] + TextFormatter.RESET + text[end_index:]
 
         return formatted_text
 
+    @staticmethod
+    def format_text_truecolor(text, color=None, background=None, attributes=None, target_text=''):
+        formatted_text = ""
+        start_index = text.find(target_text)
+        end_index = start_index + len(target_text) if start_index != -1 else len(text)
+
+        if color:
+            formatted_text += f"\033[38;2;{color}m"
+
+        if background:
+            formatted_text += f"\033[48;2;{background}m"
+
+        if attributes in TextFormatter.TEXT_ATTRIBUTES:
+            formatted_text += TextFormatter.TEXT_ATTRIBUTES[attributes]
+
+        if target_text == "":
+            formatted_text += text + TextFormatter.RESET
+        else:
+            formatted_text += text[:start_index] + text[start_index:end_index] + TextFormatter.RESET + text[end_index:]
+
+        return formatted_text
+
+    @staticmethod
+    def interpolate_color(color1, color2, ratio):
+        """
+        Interpolates between two RGB colors.
+        """
+        r = int(color1[0] * (1 - ratio) + color2[0] * ratio)
+        g = int(color1[1] * (1 - ratio) + color2[1] * ratio)
+        b = int(color1[2] * (1 - ratio) + color2[2] * ratio)
+        return f"{r};{g};{b}"
+
+    @staticmethod
+    def format_gradient_text(text, color1, color2, attributes=None):
+        formatted_text = ""
+        gradient_length = len(text)
+        for i in range(gradient_length):
+            ratio = i / (gradient_length - 1)
+            interpolated_color = TextFormatter.interpolate_color(color1, color2, ratio)
+            formatted_text += f"\033[38;2;{interpolated_color}m{text[i]}"
+        formatted_text += TextFormatter.RESET
+
+        if attributes:
+            formatted_text = f"{TextFormatter.TEXT_ATTRIBUTES[attributes]}{formatted_text}"
+
+        return formatted_text
+
 def center_string(main_string, replacement_string):
     # Find the center index of the main string
     center_index = len(main_string) // 2
 
     # Calculate the start and end indices for replacing
     start_index = center_index - len(replacement_string) // 2
     end_index = start_index + len(replacement_string)
@@ -590,15 +610,15 @@
 
     mid_lower = len(lower_half) // 2
     mid_upper = len(upper_half) // 2
 
     q1 = lower_half[mid_lower] if len(lower_half) % 2 != 0 else (lower_half[mid_lower - 1] + lower_half[mid_lower]) / 2
     q3 = upper_half[mid_upper] if len(upper_half) % 2 != 0 else (upper_half[mid_upper - 1] + upper_half[mid_upper]) / 2
 
-    return q1, q2, q3
+    return min(data), q1, q2, q3, max(data)
 
 def limit_string_in_line(text, limit):
     lines = text.split('\n')
     new_lines = []
 
     for line in lines:
         words = line.split()
@@ -610,8 +630,11 @@
             else:
                 new_lines.append(new_line.strip())
                 new_line = word + ' '
 
         if new_line:
             new_lines.append(new_line.strip())
 
-    return '\n'.join(new_lines)
+    return '\n'.join(new_lines)
+
+def split_string_at_intervals(input_string, interval):
+    return [input_string[i:i+interval] for i in range(0, len(input_string), interval)]
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113.egg-info/PKG-INFO` & `damp11113-2024.4.19.19.0.0/src/damp11113.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damp11113
-Version: 2024.1.28.19.0.0.1
+Version: 2024.4.19.19.0.0
 Summary: A Utils library and Easy to using.
 Home-page: https://github.com/damp11113/damp11113-library
 Author: damp11113
 Author-email: damp51252@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
@@ -20,29 +20,31 @@
 Requires-Dist: libscrc
 Requires-Dist: PyAudio
 Requires-Dist: python-vlc
 Requires-Dist: ffmpeg-python
 Requires-Dist: yt-dlp
 Requires-Dist: youtube_dl
 Requires-Dist: pafy
-Requires-Dist: tqdm
+Requires-Dist: pafy2tqdm
 Requires-Dist: qrcode
 Requires-Dist: python-barcode
 Requires-Dist: pydub
 Requires-Dist: pyzbar
 Requires-Dist: mcstatus
 Requires-Dist: mcrcon
 Requires-Dist: paho-mqtt
 Requires-Dist: requests
 Requires-Dist: pymata-aio
-Requires-Dist: paramiko
 Requires-Dist: six
 Requires-Dist: key-generator
 Requires-Dist: PyQt5
 Requires-Dist: gTTS
+Requires-Dist: py-cpuinfo
+Requires-Dist: GPUtil
+Requires-Dist: playsound
 Requires-Dist: pywin32
 Requires-Dist: win32gui
 Requires-Dist: comtypes
 
 damp11113-library
 ===============
 A Utils library and Easy to use.
@@ -70,14 +72,14 @@
     pip install git+https://github.com/damp11113/damp11113-library.git
     
 License
 ===============
 
 MIT License
 
-Copyright (c) 2021-2022 damp11113
+Copyright (c) 2021-2024 damp11113
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `damp11113-2024.1.28.19.0.0.1/src/damp11113.egg-info/SOURCES.txt` & `damp11113-2024.4.19.19.0.0/src/damp11113.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE.rst
 README.md
 setup.cfg
 setup.py
 src/damp11113/DSP.py
 src/damp11113/PyserHTTP.py
-src/damp11113/PyserSSH.py
 src/damp11113/__init__.py
 src/damp11113/convert.py
 src/damp11113/file.py
 src/damp11113/format.py
 src/damp11113/imageps.py
 src/damp11113/info.py
 src/damp11113/logic.py
@@ -20,8 +19,12 @@
 src/damp11113/pywindows.py
 src/damp11113/randoms.py
 src/damp11113/utils.py
 src/damp11113.egg-info/PKG-INFO
 src/damp11113.egg-info/SOURCES.txt
 src/damp11113.egg-info/dependency_links.txt
 src/damp11113.egg-info/requires.txt
-src/damp11113.egg-info/top_level.txt
+src/damp11113.egg-info/top_level.txt
+src/damp11113/OPFONMW/StepperLib.py
+src/damp11113/OPFONMW/__init__.py
+src/damp11113/OPFONMW/dearpygui_animate.py
+src/damp11113/OPFONMW/ofdm_codec.py
```

