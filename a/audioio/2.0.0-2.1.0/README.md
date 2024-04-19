# Comparing `tmp/audioio-2.0.0.tar.gz` & `tmp/audioio-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioio-2.0.0.tar", last modified: Sun Feb 11 20:11:28 2024, max compression
+gzip compressed data, was "audioio-2.1.0.tar", last modified: Fri Apr 19 21:28:46 2024, max compression
```

## Comparing `audioio-2.0.0.tar` & `audioio-2.1.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-02-11 20:11:28.866289 audioio-2.0.0/
--rw-r--r--   0 benda     (1001) benda     (1001)    35141 2017-11-13 15:43:33.000000 audioio-2.0.0/LICENSE
--rw-r--r--   0 benda     (1001) benda     (1001)     3222 2024-02-11 20:11:28.866289 audioio-2.0.0/PKG-INFO
--rw-rw-r--   0 benda     (1001) benda     (1001)    13690 2024-02-11 20:09:07.000000 audioio-2.0.0/README.md
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-02-11 20:11:28.846288 audioio-2.0.0/audioio/
--rw-rw-r--   0 benda     (1001) benda     (1001)     1672 2024-02-11 20:09:07.000000 audioio-2.0.0/audioio/__init__.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    15155 2024-02-11 20:09:07.000000 audioio-2.0.0/audioio/audioconverter.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    57889 2024-02-11 20:09:07.000000 audioio-2.0.0/audioio/audioloader.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     3041 2024-02-11 20:09:07.000000 audioio-2.0.0/audioio/audiomarkers.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    22793 2024-02-11 20:09:07.000000 audioio-2.0.0/audioio/audiometadata.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    30588 2024-02-11 20:09:07.000000 audioio-2.0.0/audioio/audiomodules.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     3873 2024-01-31 08:47:24.000000 audioio-2.0.0/audioio/audiotools.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    31140 2024-02-03 22:04:12.000000 audioio-2.0.0/audioio/audiowriter.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    44372 2024-01-29 08:32:02.000000 audioio-2.0.0/audioio/playaudio.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    60166 2024-02-11 20:09:07.000000 audioio-2.0.0/audioio/riffmetadata.py
--rw-rw-r--   0 benda     (1001) benda     (1001)      287 2024-02-11 20:09:07.000000 audioio-2.0.0/audioio/version.py
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-02-11 20:11:28.866289 audioio-2.0.0/audioio.egg-info/
--rw-r--r--   0 benda     (1001) benda     (1001)     3222 2024-02-11 20:11:28.000000 audioio-2.0.0/audioio.egg-info/PKG-INFO
--rw-r--r--   0 benda     (1001) benda     (1001)      704 2024-02-11 20:11:28.000000 audioio-2.0.0/audioio.egg-info/SOURCES.txt
--rw-r--r--   0 benda     (1001) benda     (1001)        1 2024-02-11 20:11:28.000000 audioio-2.0.0/audioio.egg-info/dependency_links.txt
--rw-r--r--   0 benda     (1001) benda     (1001)      147 2024-02-11 20:11:28.000000 audioio-2.0.0/audioio.egg-info/entry_points.txt
--rw-r--r--   0 benda     (1001) benda     (1001)        6 2024-02-11 20:11:28.000000 audioio-2.0.0/audioio.egg-info/requires.txt
--rw-r--r--   0 benda     (1001) benda     (1001)        8 2024-02-11 20:11:28.000000 audioio-2.0.0/audioio.egg-info/top_level.txt
--rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-02-11 20:11:28.866289 audioio-2.0.0/setup.cfg
--rw-rw-r--   0 benda     (1001) benda     (1001)     3749 2024-02-11 20:09:07.000000 audioio-2.0.0/setup.py
-drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-02-11 20:11:28.866289 audioio-2.0.0/tests/
--rw-rw-r--   0 benda     (1001) benda     (1001)     4342 2024-02-11 20:09:07.000000 audioio-2.0.0/tests/test_audioconverter.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    12137 2024-01-29 08:32:02.000000 audioio-2.0.0/tests/test_audioloader.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     3307 2024-02-11 20:09:07.000000 audioio-2.0.0/tests/test_audiomarkers.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    11131 2024-02-11 20:09:07.000000 audioio-2.0.0/tests/test_audiometadata.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     1863 2024-01-29 08:32:02.000000 audioio-2.0.0/tests/test_audiomodules.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     4170 2024-02-02 18:29:09.000000 audioio-2.0.0/tests/test_audiotools.py
--rw-rw-r--   0 benda     (1001) benda     (1001)    13580 2024-02-11 20:09:07.000000 audioio-2.0.0/tests/test_audiowriter.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     5145 2024-01-06 10:32:15.000000 audioio-2.0.0/tests/test_playaudio.py
--rw-rw-r--   0 benda     (1001) benda     (1001)     9806 2024-02-04 20:58:02.000000 audioio-2.0.0/tests/test_riffmetadata.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-19 21:28:46.704173 audioio-2.1.0/
+-rw-r--r--   0 benda     (1001) benda     (1001)    35141 2017-11-13 15:43:33.000000 audioio-2.1.0/LICENSE
+-rw-r--r--   0 benda     (1001) benda     (1001)    55888 2024-04-19 21:28:46.704173 audioio-2.1.0/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)    14069 2024-04-17 08:26:59.000000 audioio-2.1.0/README.md
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1623 2024-04-19 21:28:16.000000 audioio-2.1.0/pyproject.toml
+-rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-19 21:28:46.704173 audioio-2.1.0/setup.cfg
+-rw-rw-r--   0 benda     (1001) benda     (1001)       38 2024-04-19 21:28:16.000000 audioio-2.1.0/setup.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-19 21:28:46.596170 audioio-2.1.0/src/
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-19 21:28:46.600170 audioio-2.1.0/src/audioio/
+-rw-rw-r--   0 benda     (1001) benda     (1001)     2205 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/__init__.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    16977 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/audioconverter.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    62105 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/audioloader.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3061 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/audiomarkers.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    59778 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/audiometadata.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    30609 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/audiomodules.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3879 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/audiotools.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    32361 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/audiowriter.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    44675 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/playaudio.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    64150 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/riffmetadata.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)      287 2024-04-19 21:28:16.000000 audioio-2.1.0/src/audioio/version.py
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-19 21:28:46.704173 audioio-2.1.0/src/audioio.egg-info/
+-rw-r--r--   0 benda     (1001) benda     (1001)    55888 2024-04-19 21:28:46.000000 audioio-2.1.0/src/audioio.egg-info/PKG-INFO
+-rw-rw-r--   0 benda     (1001) benda     (1001)      787 2024-04-19 21:28:46.000000 audioio-2.1.0/src/audioio.egg-info/SOURCES.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)        1 2024-04-19 21:28:46.000000 audioio-2.1.0/src/audioio.egg-info/dependency_links.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)      147 2024-04-19 21:28:46.000000 audioio-2.1.0/src/audioio.egg-info/entry_points.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)       12 2024-04-19 21:28:46.000000 audioio-2.1.0/src/audioio.egg-info/requires.txt
+-rw-rw-r--   0 benda     (1001) benda     (1001)        8 2024-04-19 21:28:46.000000 audioio-2.1.0/src/audioio.egg-info/top_level.txt
+drwxrwxr-x   0 benda     (1001) benda     (1001)        0 2024-04-19 21:28:46.688173 audioio-2.1.0/tests/
+-rw-rw-r--   0 benda     (1001) benda     (1001)     4505 2024-04-15 20:06:04.000000 audioio-2.1.0/tests/test_audioconverter.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    14119 2024-04-15 20:07:21.000000 audioio-2.1.0/tests/test_audioloader.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     3169 2024-04-15 19:47:14.000000 audioio-2.1.0/tests/test_audiomarkers.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    26441 2024-04-15 20:06:20.000000 audioio-2.1.0/tests/test_audiometadata.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     1741 2024-04-15 19:47:47.000000 audioio-2.1.0/tests/test_audiomodules.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     4248 2024-04-15 19:48:22.000000 audioio-2.1.0/tests/test_audiotools.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)    13259 2024-04-16 07:47:23.000000 audioio-2.1.0/tests/test_audiowriter.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     5148 2024-04-15 20:09:21.000000 audioio-2.1.0/tests/test_playaudio.py
+-rw-rw-r--   0 benda     (1001) benda     (1001)     9746 2024-04-15 20:02:38.000000 audioio-2.1.0/tests/test_riffmetadata.py
```

### Comparing `audioio-2.0.0/LICENSE` & `audioio-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audioio-2.0.0/README.md` & `audioio-2.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,37 +11,34 @@
 ![pullrequests open](https://img.shields.io/github/issues-pr/janscience/audioio.svg)
 ![pullrequests closed](https://img.shields.io/github/issues-pr-closed/janscience/audioio.svg)
 -->
 
 # AudioIO 
 
 Platform independent interfacing of numpy arrays of floats with audio
-files and devices.
+files and devices for scientific data analysis.
 
 [Documentation](https://bendalab.github.io/audioio) |
 [API Reference](https://bendalab.github.io/audioio/api)
 
-The AudioIO modules try to use whatever audio packages are installed
-on your system to achieve their tasks. AudioIO, however, adds own code
-for handling metadata and marker lists.
-
 
 ## Features
 
-- Audio data are always *numpy arrays of floats* (`np.float64`) with values ranging between -1 and 1 ...
-- ... independent of how the data are stored in an audio file.
-- [`load_audio()`](https://bendalab.github.io/audioio/api/audioloader.html#audioio.audioloader.load_audio) function for loading a whole audio file.
-- *Blockwise random-access* loading of large audio files ([`class AudioLoader`](https://bendalab.github.io/audioio/api/audioloader.html#audioio.audioloader.AudioLoader)).
-- [`blocks()`](https://bendalab.github.io/audioio/api/audioloader.html#audioio.audioloader.blocks) generator for iterating over blocks of data with optional overlap.
-- [`write_audio()`](https://bendalab.github.io/audioio/api/audiowriter.html#audioio.audiowriter.write_audio) function for writing data, metadata, and markers to an audio file. 
-- Read [`metadata()`](https://bendalab.github.io/audioio/api/audioloader.html#audioio.audioloader.metadata) as nested dictionaries of key-value pairs.
+- Audio data are always numpy arrays of floats with values ranging between -1 and 1 independent of how the data are stored in an audio file.
+- [`load_audio()`](https://bendalab.github.io/audioio/api/audioloader.html#audioio.audioloader.load_audio) function for loading data of a whole audio file at once.
+- Blockwise, random-access loading of large audio files ([`class AudioLoader`](https://bendalab.github.io/audioio/api/audioloader.html#audioio.audioloader.AudioLoader)).
+- Read arbitrary [`metadata()`](https://bendalab.github.io/audioio/api/audioloader.html#audioio.audioloader.metadata) as nested dictionaries of key-value pairs. Supported RIFF chunks are [INFO lists](https://www.recordingblogs.com/wiki/list-chunk-of-a-wave-file), [BEXT](https://tech.ebu.ch/docs/tech/tech3285.pdf), [iXML](http://www.gallery.co.uk/ixml/), and [GUANO](https://github.com/riggsd/guano-spec). 
 - Read [`markers()`](https://bendalab.github.io/audioio/api/audioloader.html#audioio.audioloader.markers), i.e. cue points with spans, labels, and descriptions.
-- Platform independent, synchronous (blocking) and asynchronous (non blocking) playback of numpy arrays  via [`play()`](https://bendalab.github.io/audioio/api/playaudio.html#audioio.playaudio.play).
-- Automatic resampling of data for playback to match supported sampling rates.
-- Detailed and *platform specific installation instructions* (pip, conda, Debian and RPM based Linux packages, homebrew for MacOS) for all supported audio packages ([audiomodules](https://bendalab.github.io/audioio/api/audiomodules.html)).
+- [`write_audio()`](https://bendalab.github.io/audioio/api/audiowriter.html#audioio.audiowriter.write_audio) function for writing data, metadata, and markers to an audio file. 
+- Platform independent, synchronous (blocking) and asynchronous (non blocking) playback of numpy arrays  via [`play()`](https://bendalab.github.io/audioio/api/playaudio.html#audioio.playaudio.play) with automatic resampling to match supported sampling rates.
+- Detailed and platform specific installation instructions (pip, conda, Debian and RPM based Linux packages, homebrew for MacOS) for all supported audio packages (see [audiomodules](https://bendalab.github.io/audioio/api/audiomodules.html)).
+
+The AudioIO modules try to use whatever audio packages are installed
+on your system to achieve their tasks. AudioIO, however, adds own code
+for handling metadata and marker lists.
 
 
 ## Installation
 
 AudioIO is available at [PyPi](https://pypi.org/project/audioio/). Simply run:
 ```
 pip install audioio
@@ -283,14 +280,20 @@
 which ones are recommended to install, and how to install them.
 
 See API documentation of the
 [`audiomodules`](https://bendalab.github.io/audioio/api/audiomodules.html)
 module for details.
 
 
+## Used by
+
+- [thunderfish](https://github.com/bendalab/thunderfish): Algorithms and programs for analysing electric field recordings of weakly electric fish.
+- [audian](https://github.com/bendalab/audian): Python-based GUI for viewing and analyzing recordings of animal vocalizations.
+
+
 ## Alternatives
 
 All the audio modules AudioIO is using.
 
 Reading and writing audio files:
 
 - [wave](https://docs.python.org/3.8/library/wave.html): simple wave file interface of the python standard library.
```

### Comparing `audioio-2.0.0/audioio/audioconverter.py` & `audioio-2.1.0/src/audioio/audioconverter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Command line script for converting, downsampling, renaming and merging audio files.
 
 ```sh
 audioconverter -o test.wav test.mp3
 ```
 converts 'test.mp3' to 'test.wav'.
 
-The script reads all input files with `audioloader.load_audio()`,
+The script reads all input files with `audioio.audioloader.load_audio()`,
 combines the audio and marker data and writes them along with the
-metadata to an output file using `audiowriter.write_audio()`.
+metadata to an output file using `audioio.audiowriter.write_audio()`.
 
 Thus, all formats supported by these functions and the installed
 python audio modules are available. This implies that MP3 files can be
 read via the [audioread](https://github.com/beetbox/audioread) module,
 and they can be written via [pydub](https://github.com/jiaaro/pydub).
 Many other input and output file formats are supported by the [sndfile
 library](http://www.mega-nerd.com/libsndfile/), provided the
@@ -50,16 +50,17 @@
   -h, --help    show this help message and exit
   --version     show program's version number and exit
   -v            print debug output
   -l            list supported file formats and encodings
   -f FORMAT     audio format of output file
   -e ENCODING   audio encoding of output file
   -s SCALE      scale the data by factor SCALE
-  -u [THRESH]   unwrap clipped data with threshold (default is 0.5) and divide by two
-  -U [THRESH]   unwrap clipped data with threshold (default is 0.5) and clip
+  -u [THRESH]   unwrap clipped data with threshold relative to maximum of input range (default is 0.5) and divide by
+                two
+  -U [THRESH]   unwrap clipped data with threshold relative to maximum of input range (default is 0.5) and clip
   -d FAC        downsample by integer factor
   -c CHANNELS   comma and dash separated list of channels to be saved (first channel is 0)
   -a KEY=VALUE  add key-value pairs to metadata. Keys can have section names separated by "."
   -r KEY        remove keys from metadata. Keys can have section names separated by "."
   -n NUM        merge NUM input files into one output file
   -o OUTPATH    path or filename of output file. Metadata keys enclosed in curly braces will be replaced by their
                 values from the input file
@@ -71,17 +72,18 @@
 
 import os
 import sys
 import argparse
 import numpy as np
 from scipy.signal import decimate
 from .version import __version__, __year__
-from .audioloader import load_audio, metadata, markers
+from .audioloader import load_audio, markers, AudioLoader
 from .audiometadata import flatten_metadata, unflatten_metadata
 from .audiometadata import add_metadata, remove_metadata, cleanup_metadata
+from .audiometadata import bext_history_str, add_history
 from .audiometadata import update_gain, add_unwrap
 from .audiotools import unwrap
 from .audiowriter import available_formats, available_encodings
 from .audiowriter import format_from_extension, write_audio
 
 
 def add_arguments(parser):
@@ -100,19 +102,19 @@
     parser.add_argument('-f', dest='data_format', default=None, type=str,
                         metavar='FORMAT', help='audio format of output file')
     parser.add_argument('-e', dest='encoding', default=None, type=str,
                         help='audio encoding of output file')
     parser.add_argument('-s', dest='scale', default=1, type=float,
                         help='scale the data by factor SCALE')
     parser.add_argument('-u', dest='unwrap', default=0, type=float,
-                        metavar='THRESH', const=0.5, nargs='?',
-                        help='unwrap clipped data with threshold (default is 0.5) and divide by two')
+                        metavar='THRESH', const=1.5, nargs='?',
+                        help='unwrap clipped data with threshold relative to maximum of input range (default is 0.5) and divide by two')
     parser.add_argument('-U', dest='unwrap_clip', default=0, type=float,
-                        metavar='THRESH', const=0.5, nargs='?',
-                        help='unwrap clipped data with threshold (default is 0.5) and clip')
+                        metavar='THRESH', const=1.5, nargs='?',
+                        help='unwrap clipped data with threshold relative to maximum of input range (default is 0.5) and clip')
     parser.add_argument('-d', dest='decimate', default=1, type=int,
                         metavar='FAC',
                         help='downsample by integer factor')
     parser.add_argument('-c', dest='channels', default='', type=str,
                         help='comma and dash separated list of channels to be saved (first channel is 0)')
     parser.add_argument('-a', dest='md_list', action='append', default=[],
                         type=str, metavar='KEY=VALUE',
@@ -243,15 +245,15 @@
             outfile = os.path.splitext(outfile)[0] + os.extsep + data_format.lower()
         else:
             data_format = format_from_ext(outfile)
     return outfile, data_format
 
 
 def modify_data(data, samplingrate, metadata, channels, scale,
-                unwrap_clip, unwrap_thresh, decimate_fac):
+                unwrap_clip, unwrap_thresh, ampl_max, unit, decimate_fac):
     """ Modify audio data and add modifications to metadata.
 
     Parameters
     ----------
     data: 2-D array of float
         The data to be written into the output file.
     samplingrate: float
@@ -259,20 +261,24 @@
     metadata: nested dict
         Metadata.
     channels: list of int
         List of channels to be selected from the data.
     scale: float
         Scaling factor to be applied to the data.
     unwrap_clip: float
-        If larger than zero, unwrap the data using this as a threshold,
-        and clip the data at +-1.
+        If larger than zero, unwrap the data using this as a threshold
+        relative to `ampl_max`, and clip the data at +-`ampl_max`.
     unwrap_thresh: float
-        If larger than zero, unwrap the data using this as a threshold,
-        and downscale the data by a factor of two. Also update the gain
-        in the metadata.
+        If larger than zero, unwrap the data using this as a threshold
+        relative to `ampl_max`, and downscale the data by a factor of two.
+        Also update the gain in the metadata.
+    ampl_max: float
+        Maximum amplitude of the input range.
+    unit: str
+        Unit of the input range.
     decimate_fac: int
         Downsample the data by this factor.
 
     Returns
     -------
     """
     # select channels:
@@ -280,23 +286,23 @@
         data = data[:,channels]
     # scale data:
     if scale != 1:
         data *= scale
         update_gain(metadata, 1/scale)
     # fix data:
     if unwrap_clip > 1e-3:
-        unwrap(data, unwrap_clip)
-        data[data > 1] = 1
-        data[data < -1] = -1
-        add_unwrap(metadata, unwrap_clip, 1.0)
+        unwrap(data, unwrap_clip, ampl_max)
+        data[data > +ampl_max] = +ampl_max
+        data[data < -ampl_max] = -ampl_max
+        add_unwrap(metadata, unwrap_clip*ampl_max, ampl_max, unit)
     elif unwrap_thresh > 1e-3:
-        unwrap(data, unwrap_thresh)
+        unwrap(data, unwrap_thresh, ampl_max)
         data *= 0.5
         update_gain(metadata, 0.5)
-        add_unwrap(metadata, unwrap_thresh, 0.0)
+        add_unwrap(metadata, unwrap_thresh*ampl_max, 0.0, unit)
     # decimate:
     if decimate_fac > 1:
         data = decimate(data, decimate_fac, axis=0)
         samplingrate /= decimate_fac
     return data, samplingrate
 
 
@@ -339,14 +345,16 @@
     if len(cargs) == 0:
         cargs = None
     args = parser.parse_args(cargs)
     
     channels = parse_channels(args.channels)
     
     if args.list_formats:
+        if args.data_format is None and len(args.file) > 0:
+            args.data_format = args.file[0]
         list_formats_encodings(args.data_format)
         return
 
     if len(args.file) == 0 or len(args.file[0]) == 0:
         print('! need to specify at least one input file !')
         sys.exit(-1)
 
@@ -362,21 +370,38 @@
                                             format_from_extension)
         if not check_format(data_format):
             sys.exit(-1)
         if os.path.realpath(infile) == os.path.realpath(outfile):
             print(f'! cannot convert "{infile}" to itself !')
             sys.exit(-1)
         # read in audio:
-        data, samplingrate = load_audio(infile)
-        md = metadata(infile)
-        locs, labels = markers(infile)
+        pre_history = None
+        try:
+            with AudioLoader(infile) as sf:
+                data = sf[:,:]
+                samplingrate = sf.samplerate
+                md = sf.metadata()
+                locs, labels = sf.markers()
+                pre_history = bext_history_str(sf.encoding,
+                                               sf.samplerate,
+                                               sf.channels,
+                                               sf.filepath)
+                if sf.encoding is not None and args.encoding is None:
+                    args.encoding = sf.encoding
+        except FileNotFoundError:
+            print(f'file "{infile}" not found!')
+            sys.exit(-1)
         if args.verbose > 1:
             print(f'loaded audio file "{infile}"')
         for infile in args.file[i0+1:i0+nmerge]:
-            xdata, xrate = load_audio(infile)
+            try:
+                xdata, xrate = load_audio(infile)
+            except FileNotFoundError:
+                print(f'file "{infile}" not found!')
+                sys.exit(-1)
             if abs(samplingrate - xrate) > 1:
                 print('! cannot merge files with different sampling rates !')
                 print(f'    file "{args.file[i0]}" has {samplingrate:.0f}Hz')
                 print(f'    file "{infile}" has {xrate:.0f}Hz')
                 sys.exit(-1)
             if xdata.shape[1] != data.shape[1]:
                 print('! cannot merge files with different numbers of channels !')
@@ -388,24 +413,36 @@
             locs = np.vstack((locs, xlocs))
             labels = np.vstack((labels, xlabels))
             if args.verbose > 1:
                 print(f'loaded audio file "{infile}"')
         data, samplingrate = modify_data(data, samplingrate, md,
                                          channels, args.scale,
                                          args.unwrap_clip,
-                                         args.unwrap, args.decimate)
+                                         args.unwrap, 1.0, '',
+                                         args.decimate)
         add_metadata(md, args.md_list, '.')
         if len(args.remove_keys) > 0:
             remove_metadata(md, args.remove_keys, '.')
             cleanup_metadata(md)
         outfile = format_outfile(outfile, md)
+        # history:
+        hkey = 'CodingHistory'
+        if 'BEXT' in md:
+            hkey = 'BEXT.' + hkey
+        history = bext_history_str(args.encoding, samplingrate,
+                                   data.shape[1], outfile)
+        add_history(md, history, hkey, pre_history)
         # write out audio:
-        write_audio(outfile, data, samplingrate,
-                    md, locs, labels,
-                    format=data_format, encoding=args.encoding)
+        try:
+            write_audio(outfile, data, samplingrate,
+                        md, locs, labels,
+                        format=data_format, encoding=args.encoding)
+        except PermissionError:
+            print(f'failed to write "{outfile}": permission denied!')
+            sys.exit(-1)
         # message:
         if args.verbose > 1:
             print(f'wrote "{outfile}"')
         elif args.verbose:
             print(f'converted audio file "{infile}" to "{outfile}"')
```

### Comparing `audioio-2.0.0/audioio/audioloader.py` & `audioio-2.1.0/src/audioio/audioloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 """Loading data, metadata, and markers from audio files.
 
 - `load_audio()`: load a whole audio file at once.
 - `metadata()`: read metadata of an audio file.
 - `markers()`: read markers of an audio file.
+- `BufferArray()`: random access to 2D data of which only a part is held in memory.
 - `AudioLoader`: read data from audio files in chunks.
 - `blocks()`: generator for blockwise processing of array data.
 
 The read in data are always numpy arrays of floats ranging between -1 and 1.
 The arrays are 2-D arrays with first axis time and second axis channel,
 even for single channel data.
 
 If an audio file cannot be loaded, you might need to install
 additional packages.  See
 [installation](https://bendalab.github.io/audioio/installation) for
 further instructions.
 
 For a demo run the module as:
 ```
-python -m audioio.audioloader audiofile.wav
+python -m src.audioio.audioloader audiofile.wav
 ```
 """
  
 import sys
 import warnings
 import os.path
 import numpy as np
 from .audiomodules import *
 from .riffmetadata import metadata_riff, markers_riff
+from .audiometadata import update_gain, add_unwrap
 from .audiotools import unwrap
 
 
-def load_wave(filepath, verbose=0):
+def load_wave(filepath):
     """Load wav file using the wave module from pythons standard libray.
     
     Documentation
     -------------
     https://docs.python.org/3.8/library/wave.html
 
     Parameters
     ----------
     filepath: string
         The full path and name of the file to load.
-    verbose: int
-        Not used.
 
     Returns
     -------
     data: array
         All data traces as an 2-D numpy array, first dimension is time, second is channel
     rate: float
         The sampling rate of the data in Hertz.
@@ -66,34 +66,32 @@
     buffer = wf.readframes(nframes)
     factor = 2.0**(sampwidth*8-1)
     if sampwidth == 1:
         dtype = 'u1'
         buffer = np.frombuffer(buffer, dtype=dtype).reshape(-1, nchannels)
         data = buffer.astype('d')/factor - 1.0
     else:
-        dtype = 'i%d' % sampwidth
+        dtype = f'i{sampwidth}' 
         buffer = np.frombuffer(buffer, dtype=dtype).reshape(-1, nchannels)
         data = buffer.astype('d')/factor
     wf.close()
     return data, float(rate)
 
     
-def load_ewave(filepath, verbose=0):
+def load_ewave(filepath):
     """Load wav file using ewave module.
 
     Documentation
     -------------
     https://github.com/melizalab/py-ewave
 
     Parameters
     ----------
     filepath: string
         The full path and name of the file to load.
-    verbose: int
-        Not used.
 
     Returns
     -------
     data: array
         All data traces as an 2-D numpy array, first dimension is time, second is channel.
     rate: float
         The sampling rate of the data in Hertz.
@@ -115,28 +113,26 @@
         buffer = wf.read()
         data = ewave.rescale(buffer, 'float')
     if len(data.shape) == 1:
         data = np.reshape(data,(-1, 1))
     return data, float(rate)
 
     
-def load_wavfile(filepath, verbose=0):
+def load_wavfile(filepath):
     """Load wav file using scipy.io.wavfile.
 
     Documentation
     -------------
     http://docs.scipy.org/doc/scipy/reference/io.html
     Does not support blocked read.
     
     Parameters
     ----------
     filepath: string
         The full path and name of the file to load.
-    verbose: int
-        If larger than zero show detailed error/warning messages.
 
     Returns
     -------
     data: array
         All data traces as an 2-D numpy array, first dimension is time, second is channel.
     rate: float
         The sampling rate of the data in Hertz.
@@ -147,44 +143,40 @@
         The scipy.io module is not installed
     *
         Loading of the data failed
     """
     if not audio_modules['scipy.io.wavfile']:
         raise ImportError
 
-    if verbose < 2:
-        warnings.filterwarnings("ignore")
+    warnings.filterwarnings("ignore")
     rate, data = wavfile.read(filepath)
-    if verbose < 2:
-        warnings.filterwarnings("always")
+    warnings.filterwarnings("always")
     if data.dtype == np.uint8:
         data = data / 128.0 - 1.0
     elif np.issubdtype(data.dtype, np.signedinteger):
         data = data / (2.0**(data.dtype.itemsize*8-1))
     else:
         data = data.astype(np.float64, copy=False)
     if len(data.shape) == 1:
         data = np.reshape(data,(-1, 1))
     return data, float(rate)
 
 
-def load_soundfile(filepath, verbose=0):
+def load_soundfile(filepath):
     """Load audio file using SoundFile (based on libsndfile).
 
     Documentation
     -------------
     http://pysoundfile.readthedocs.org
     http://www.mega-nerd.com/libsndfile
 
     Parameters
     ----------
     filepath: string
         The full path and name of the file to load.
-    verbose: int
-        Not used.
 
     Returns
     -------
     data: array
         All data traces as an 2-D numpy array, first dimension is time, second is channel.
     rate: float
         The sampling rate of the data in Hertz.
@@ -203,27 +195,25 @@
     rate = 0.0
     with soundfile.SoundFile(filepath, 'r') as sf:
         rate = sf.samplerate
         data = sf.read(frames=-1, dtype='float64', always_2d=True)
     return data, float(rate)
 
 
-def load_wavefile(filepath, verbose=0):
+def load_wavefile(filepath):
     """Load audio file using wavefile (based on libsndfile).
 
     Documentation
     -------------
     https://github.com/vokimon/python-wavefile
 
     Parameters
     ----------
     filepath: string
         The full path and name of the file to load.
-    verbose: int
-        Not used.
 
     Returns
     -------
     data: array
         All data traces as an 2-D numpy array, first dimension is time, second is channel.
     rate: float
         The sampling rate of the data in Hertz.
@@ -238,27 +228,25 @@
     if not audio_modules['wavefile']:
         raise ImportError
 
     rate, data = wavefile.load(filepath)
     return data.astype(np.float64, copy=False).T, float(rate)
 
 
-def load_audioread(filepath, verbose=0):
+def load_audioread(filepath):
     """Load audio file using audioread.
 
     Documentation
     -------------
     https://github.com/beetbox/audioread
 
     Parameters
     ----------
     filepath: string
         The full path and name of the file to load.
-    verbose: int
-        Not used.
 
     Returns
     -------
     data: array
         All data traces as an 2-D numpy array, first dimension is time, second is channel.
     rate: float
         The sampling rate of the data in Hertz.
@@ -290,24 +278,24 @@
             data[index:index+n,:] = fulldata[:n,:]
             index += n
     return data/(2.0**15-1.0), float(rate)
 
 
 audio_loader_funcs = (
     ('soundfile', load_soundfile),
-    ('audioread', load_audioread),
     ('wave', load_wave),
     ('wavefile', load_wavefile),
     ('ewave', load_ewave),
-    ('scipy.io.wavfile', load_wavfile)
+    ('scipy.io.wavfile', load_wavfile),
+    ('audioread', load_audioread),
     )
-"""List of implemented load functions.
+"""List of implemented load() functions.
 
 Each element of the list is a tuple with the module's name and its
-load function.
+load() function.
 
 """    
 
 
 def load_audio(filepath, verbose=0):
     """Call this function to load all channels of audio data from a file.
     
@@ -351,82 +339,78 @@
     plt.show()
     ```
     """
     # check values:
     if filepath is None or len(filepath) == 0:
         raise ValueError('input argument filepath is empty string!')
     if not os.path.isfile(filepath):
-        raise FileNotFoundError('file "%s" not found' % filepath)
+        raise FileNotFoundError(f'file "{filepath}" not found')
     if os.path.getsize(filepath) <= 0:
-        raise EOFError('file "%s" is empty (size=0)!' % filepath)
+        raise EOFError(f'file "{filepath}" is empty (size=0)!')
 
     # load an audio file by trying various modules:
-    success = False
     not_installed = []
+    errors = [f'failed to load data from file "{filepath}":']
     for lib, load_file in audio_loader_funcs:
         if not audio_modules[lib]:
             if verbose > 1:
-                print('unable to load data from file "%s" using %s module: module not available' %
-                      (filepath, lib))
+                print(f'unable to load data from file "{filepath}" using {lib} module: module not available')
             not_installed.append(lib)
             continue
         try:
-            data, rate = load_file(filepath, verbose)
+            data, rate = load_file(filepath)
             if len(data) > 0:
-                success = True
                 if verbose > 0:
-                    print('loaded data from file "%s" using %s module' %
-                          (filepath, lib))
+                    print(f'loaded data from file "{filepath}" using {lib} module')
                     if verbose > 1:
-                        print('  sampling rate: %g Hz' % rate)
-                        print('  channels     : %d' % data.shape[1])
-                        print('  data values  : %d' % len(data))
-                break
+                        print(f'  sampling rate: {rate:g} Hz')
+                        print(f'  channels     : {data.shape[1]}')
+                        print(f'  frames       : {len(data)}')
+                return data, rate
         except Exception as e:
-            pass
-    if not success:
-        need_install = ""
-        if len(not_installed) > 0:
-            need_install = " You may need to install one of the " + \
-              ', '.join(not_installed) + " packages."
-        raise IOError('failed to load data from file "%s".%s' %
-                      (filepath, need_install))
-    return data, rate
+            errors.append(f'  {lib} failed: {str(e)}')
+            if verbose > 1:
+                print(errors[-1])
+    if len(not_installed) > 0:
+        errors.append('\n  You may need to install one of the ' + \
+          ', '.join(not_installed) + ' packages.')
+    raise IOError('\n'.join(errors))
+    return np.zeros(0), 0.0
 
 
 def metadata(filepath, store_empty=False):
-    """ Read metadata of an audio file.
+    """Read metadata of an audio file.
 
     Parameters
     ----------
     filepath: string or file handle
         The audio file from which to read metadata.
     store_empty: bool
         If `False` do not return meta data with empty values.
 
     Returns
     -------
     meta_data: nested dict
         Meta data contained in the audio file.  Keys of the nested
-        dictionaries are always strings.  If the corresponding
-        values are dictionaries, then the key is the section name
-        of the metadata contained in the dictionary. All other
-        types of values are values for the respective key. In
-        particular they are strings. But other
-        simple types like ints or floats are also allowed.
-        See `audioio.audiometadata` module for available functions
-        to work with such metadata.
+        dictionaries are always strings.  If the corresponding values
+        are dictionaries, then the key is the section name of the
+        metadata contained in the dictionary. All other types of
+        values are values for the respective key. In particular they
+        are strings. But other types like for example ints or floats
+        are also allowed.  See `audioio.audiometadata` module for
+        available functions to work with such metadata.
 
     Examples
     --------
     ```
     from audioio import metadata, print_metadata
     md = metadata('data.wav')
     print_metadata(md)
     ```
+
     """
     try:
         return metadata_riff(filepath, store_empty)
     except ValueError: # not a RIFF file
         return {}
 
 
@@ -518,15 +502,15 @@
         for x in blocks(data, 100*nfft, nfft//2):
             f, t, Sxx = spectrogram(x, fs=data.samplerate,
                                     nperseg=nfft, noverlap=nfft//2)
     ```
 
     """
     if noverlap >= block_size:
-        raise ValueError('noverlap=%d larger than block_size=%d' % (noverlap, block_size))
+        raise ValueError(f'noverlap={noverlap} larger than block_size={block_size}')
     if stop is None:
         stop = len(data)
     m = block_size - noverlap
     n = (stop-start-noverlap)//m
     if n == 0:
         yield data[start:stop]
     else:
@@ -557,14 +541,16 @@
     set the following member variables, followed by a call to
     `_init_buffer()`:
     ```
     self.samplerate      # number of frames per second
     self.channels        # number of channels per frame
     self.frames          # total number of frames
     self.shape = (self.frames, self.channels)        
+    self.ndim            # number of dimensions: always 2 (frames and channels)
+    self.size            # total number of samples: frames times channels
     self.buffersize      # number of frames the buffer should hold
     self.backsize        # number of frames kept for moving back
     self._init_buffer()
     ```
     
     Parameters
     ----------
@@ -579,14 +565,16 @@
         The number of channels.
     frames: int
         The number of frames. Same as `len()`.
     shape: tuple
         Frames and channels of the data.
     ndim: int
         Number of dimensions: always 2 (frames and channels).
+    size: int
+        Total number of samples: frames times channels.
     offset: int
         Index of first frame in the current buffer.
     buffer: array of floats
         The curently available data.
     ampl_min: float
         Minimum amplitude the data supports.
     ampl_max: float
@@ -594,15 +582,14 @@
 
     Methods
     -------
     - `len()`: Number of frames.
     - `__getitem__`: Access data.
     - `update_buffer()`: Update the buffer for a range of frames.
     - `load_buffer()`: Load a range of frames into a buffer.
-    - `set_unwrap()`: Set parameters for unwrapping clipped data.
 
     Notes
     -----
     Access via `__getitem__` or `__next__` is slow!
     Even worse, using numpy functions on this class first converts
     it to a numpy array - that is something we actually do not want!
     We should subclass directly from numpy.ndarray .
@@ -614,23 +601,26 @@
     
     def __init__(self, verbose=0):
         self.samplerate = 0.0
         self.channels = 0
         self.frames = 0
         self.shape = (0, 0)
         self.ndim = 2
+        self.size = 0
         self.ampl_min = -1.0
         self.ampl_max = +1.0
         self.offset = 0
         self.buffersize = 0
         self.backsize = 0
-        self.buffer = np.zeros((0,0))
+        self.buffer = np.zeros((0, 0))
         self.unwrap = False
-        self.unwrap_thresh = 0.5
+        self.unwrap_thresh = 0.0
         self.unwrap_clips = False
+        self.unwrap_ampl = 1.0
+        self.unwrap_downscale = True
         self.verbose = verbose
 
     def __enter__(self):
         return self
         
     def __exit__(self, ex_type, ex_value, tb):
         self.__del__()
@@ -644,16 +634,16 @@
         return self
 
     def __next__(self):
         self.iter_counter += 1
         if self.iter_counter >= self.frames:
             raise StopIteration
         else:
-            self.update_buffer(self.iter_counter, self.iter_counter+1)
-            return self.buffer[self.iter_counter-self.offset,:]
+            self.update_buffer(self.iter_counter, self.iter_counter + 1)
+            return self.buffer[self.iter_counter - self.offset,:]
 
     def __getitem__(self, key):
         """Access data of the audio file."""
         if type(key) is tuple:
             index = key[0]
         else:
             index = key
@@ -717,28 +707,27 @@
             Index of the last frame for the buffer.
         """
         if start < self.offset or stop > self.offset + self.buffer.shape[0]:
             offset, size = self._read_indices(start, stop)
             r_offset, r_size = self._recycle_buffer(offset, size)
             self.offset = offset
             # load buffer content from file, this is backend specific:
-            self.load_buffer(r_offset, r_size,
-                             self.buffer[r_offset-self.offset:
-                                         r_offset+r_size-self.offset,:])
+            data = self.buffer[r_offset-self.offset:
+                               r_offset-self.offset+r_size,:]
+            self.load_buffer(r_offset, r_size, data)
             if self.unwrap:
-                data = self.buffer[r_offset-self.offset:r_offset+r_size-self.offset,:]
                 # TODO: handle edge effects!
-                unwrap(data, self.unwrap_thresh)
+                unwrap(data, self.unwrap_thresh, self.unwrap_ampl)
                 if self.unwrap_clips:
                     data[data > self.ampl_max] = self.ampl_max
                     data[data < self.ampl_min] = self.ampl_min
+                elif self.unwrap_down_scale:
+                    data *= 0.5
             if self.verbose > 1:
-                print('  loaded %d frames from %d up to %d'
-                      % (self.buffer.shape[0], self.offset,
-                         self.offset+self.buffer.shape[0]))
+                print(f'  loaded {self.buffer.shape[0]} frames from {self.offset} up to {self.offset+self.buffer.shape[0]}')
 
     def _read_indices(self, start, stop):
         """Compute position and size for next read from file.
 
         This takes buffersize and backsize into account.
 
         Parameters
@@ -767,15 +756,15 @@
                 offset = 0
             if offset + size > self.frames:
                 offset = self.frames - size
                 if offset < 0:
                     offset = 0
                     size = self.frames - offset
         if self.verbose > 2:
-            print('  request %6d frames at %d-%d' % (size, offset, offset+size))
+            print(f'  request {size:6d} frames at {offset}-{offset+size}')
         return offset, size
 
     def _recycle_buffer(self, offset, size):
         """Recycle buffer contents and return indices for data to be loaded from file.
 
         Move already existing parts of the buffer to their new position (as
         returned by _read_indices() ) and return position and size of
@@ -811,54 +800,28 @@
             m = self.buffer.shape[0]
             buffer = self.buffer[-i:m-i+n,:]
             allocate_buffer(size)
             self.buffer[:n,:] = buffer
             r_offset += n
             r_size -= n
             if self.verbose > 2:
-                print('  recycle %6d frames from %d-%d of the old %d-sized buffer to the front at %d-%d (%d-%d in buffer)'
-                       % (n, self.offset+m-i, self.offset+m-i+n, m, offset, offset+n, 0, n))
+                print(f'  recycle {n:6d} frames from {self.offset+m-i}-{self.offset+m-i+n} of the old {m}-sized buffer to the front at {offset}-{offset+n} ({0}-{n} in buffer)')
         elif ( offset + size > self.offset and
             offset + size <= self.offset + self.buffer.shape[0] ):
             n = offset + size - self.offset
             m = self.buffer.shape[0]
             buffer = self.buffer[:n,:]
             allocate_buffer(size)
             self.buffer[-n:,:] = buffer
             r_size -= n
             if self.verbose > 2:
-                print('  recycle %6d frames from %d-%d of the old %d-sized buffer to the end at %d-%d (%d-%d in buffer)'
-                       % (n, self.offset, self.offset+n, m, offset+size-n, offset+size, size-n, size))
+                print(f'  recycle {n:6d} frames from {self.offset}-{self.offset+n} of the old {m}-sized buffer to the end at {offset+size-n}-{offset+size} ({size-n}-{size} in buffer)')
         else:
             allocate_buffer(size)
         return r_offset, r_size
-
-    def set_unwrap(self, thresh, clips=False):
-        """Set parameters for unwrapping clipped data.
-
-        See unwrap() function from the audioio package.
-
-        Parameters
-        ----------
-        thresh: float
-            Threshold for detecting wrapped data.
-            If zero, do not unwrap.
-        clips: bool
-            If True, then clip the unwrapped data properly.
-            Otherwise, unwrap the data and double the
-            minimum and maximum data range
-            (self.ampl_min and self.ampl_max).
-        """
-        self.unwrap_thresh = thresh
-        self.unwrap_clips = clips
-        self.unwrap = thresh > 1e-3
-        if self.unwrap and not self.unwrap_clips:
-            self.ampl_min *= 2
-            self.ampl_max *= 2
-
             
 class AudioLoader(BufferArray):
     """Buffered reading of audio data for random access of the data in the file.
     
     The class allows for reading very large audio files that do not
     fit into memory.
     An AudioLoader instance can be used like a huge read-only numpy array, i.e.
@@ -872,15 +835,15 @@
     all available audio modules until it succeeds (first line). It
     then reads data from the file as necessary for the requested data
     (second line).
 
     Reading sequentially through the file is always possible. Some
     modules, however, (e.g. audioread, needed for mp3 files) can only
     read forward. If previous data are requested, then the file is read
-    from the beginning. This slows down access to previous data
+    from the beginning again. This slows down access to previous data
     considerably. Use the `backsize` argument of the open function to
     make sure some data are loaded into the buffer before the requested
     frame. Then a subsequent access to the data within backsize `seconds`
     before that frame can still be handled without the need to reread
     the file from the beginning.
 
     Usage
@@ -939,47 +902,54 @@
         Name of the file.
     buffersize: float
         Size of internal buffer in seconds.
     backsize: float
         Part of the buffer to be loaded before the requested start index in seconds.
     verbose: int
         If larger than zero show detailed error/warning messages.
+    store_empty: bool
+        If `False` do not return meta data with empty values.
 
     Attributes
     ----------
     filepath: str
         Path and name of the file.
     samplerate: float
         The sampling rate of the data in seconds.
     channels: int
         The number of channels.
     frames: int
         The number of frames in the file. Same as `len()`.
+    format: str or None
+        Format of the audio file.
+    encoding: str or None
+        Encoding/subtype of the audio file.
     shape: tuple
         Frames and channels of the data.
     offset: int
         Index of first frame in the current buffer.
     buffer: array of floats
         The curently available data from the file.
     ampl_min: float
         Minimum amplitude the file format supports.
-        Mostly -1.0, but -2.0 when unwrapping the data.
+        Always -1.0 for audio data.
     ampl_max: float
         Maximum amplitude the file format supports.
-        Mostly +1.0, but +2.0 when unwrapping the data.
+        Always +1.0 for audio data.
 
     Methods
     -------
     - `len()`: Number of frames.
     - `open()`: Open an audio file by trying available audio modules.
     - `open_*()`: Open an audio file with the respective audio module.
     - `__getitem__`: Access data of the audio file.
     - `update_buffer()`: Update the internal buffer for a range of frames.
     - `load_buffer()`: Load a range of frames into a buffer.
     - `blocks()`: Generator for blockwise processing of AudioLoader data.
+    - `format_dict()`: technical infos about how the data are stored.
     - `metadata()`: Metadata stored along with the audio data.
     - `markers()`: Markers stored along with the audio data.
     - `set_unwrap()`: Set parameters for unwrapping clipped data.
     - `close()`: Close the file.
 
     Notes
     -----
@@ -989,21 +959,38 @@
     We should subclass directly from numpy.ndarray .
     For details see http://docs.scipy.org/doc/numpy/user/basics.subclassing.html
     When subclassing, there is an offset argument, that might help to
     speed up `__getitem__` .
 
     """
     
-    def __init__(self, filepath=None, buffersize=10.0, backsize=0.0, verbose=0):
+    def __init__(self, filepath=None, buffersize=10.0, backsize=0.0,
+                 verbose=0, **meta_kwargs):
         super().__init__(verbose)
+        self.format = None
+        self.encoding = None
+        self._metadata = None
+        self._locs = None
+        self._labels = None
+        self._load_metadata = metadata
+        self._load_markers = markers
+        self._metadata_kwargs = meta_kwargs
         self.filepath = None
         self.sf = None
         self.close = self._close
         if filepath is not None:
             self.open(filepath, buffersize, backsize, verbose)
+            
+    numpy_encodings = {np.dtype(np.int64): 'PCM_64',
+                       np.dtype(np.int32): 'PCM_32',
+                       np.dtype(np.int16): 'PCM_16',
+                       np.dtype(np.single): 'FLOAT',
+                       np.dtype(np.double): 'DOUBLE'}
+    """ Map numpy dtypes to encodings.
+    """
 
     def _close(self):
         pass
 
     def __del__(self):
         self.close()
 
@@ -1042,37 +1029,65 @@
             for x in data.blocks(100*nfft, nfft//2):
                 f, t, Sxx = spectrogram(x, fs=data.samplerate,
                                         nperseg=nfft, noverlap=nfft//2)
         ```
         """
         return blocks(self, block_size, noverlap, start, stop)
 
-    def metadata(self, store_empty=False):
-        """Read metadata of the audio file.
+    def format_dict(self):
+        """ Technical infos about how the data are stored in the file.
+
+        Returns
+        -------
+        fmt: dict
+            Dictionary with filepath, format, encoding, samplingrate,
+            channels, frames, and duration of the audio file as strings.
+
+        """
+        fmt = dict(filepath=self.filepath)
+        if self.format is not None:
+            fmt['format'] = self.format
+        if self.encoding is not None:
+            fmt['encoding'] = self.encoding
+        fmt.update(dict(samplingrate=f'{self.samplerate:.0f}Hz',
+                        channels=self.channels,
+                        frames=self.frames,
+                        duration=f'{self.frames/self.samplerate:.3f}s'))
+        return fmt
+        
+    def metadata(self):
+        """Metadata of the audio file.
 
         Parameters
         ----------
         store_empty: bool
             If `False` do not add meta data with empty values.
 
         Returns
         -------
         meta_data: nested dict
+
             Meta data contained in the audio file.  Keys of the nested
             dictionaries are always strings.  If the corresponding
             values are dictionaries, then the key is the section name
             of the metadata contained in the dictionary. All other
             types of values are values for the respective key. In
-            particular they are strings. But other
-            simple types like ints or floats are also allowed.
-            See `audioio.audiometadata` module for available functions
-            to work with such metadata.
-        """
-        return metadata(self.filepath, store_empty)
+            particular they are strings. But other types like for
+            example ints or floats are also allowed.  See
+            `audioio.audiometadata` module for available functions to
+            work with such metadata.
 
+        """
+        if self._metadata is None:
+            if self._load_metadata is None:
+                self._metadata = {}
+            else:
+                self._metadata = self._load_metadata(self.filepath,
+                                                     **self._metadata_kwargs)
+        return self._metadata
 
     def markers(self):
         """Read markers of the audio file.
 
         See `audioio.audiomarkers` module for available functions
         to work with markers.
 
@@ -1081,16 +1096,67 @@
         locs: 2-D array of ints
             Marker positions (first column) and spans (second column)
             for each marker (rows).
         labels: 2-D array of string objects
             Labels (first column) and texts (second column)
             for each marker (rows).
         """
-        return markers(self.filepath)
-    
+        if self._locs is None:
+            if self._load_markers is None:
+                self._locs = np.zeros((0, 2), dtype=int)
+                self._labels = np.zeros((0, 2), dtype=object)
+            else:
+                self._locs, self._labels = self._load_markers(self.filepath)
+        return self._locs, self._labels 
+
+    def set_unwrap(self, thresh, clips=False, down_scale=True, unit=''):
+        """Set parameters for unwrapping clipped data.
+
+        See unwrap() function from the audioio package.
+
+        Parameters
+        ----------
+        thresh: float
+            Threshold for detecting wrapped data relative to self.unwrap_ampl
+            which is initially set to self.ampl_max.
+            If zero, do not unwrap.
+        clips: bool
+            If True, then clip the unwrapped data properly.
+            Otherwise, unwrap the data and double the
+            minimum and maximum data range
+            (self.ampl_min and self.ampl_max).
+        down_scale: bool
+            If not `clip`, then downscale the signal by a factor of two,
+            in order to keep the range between -1 and 1.
+        unit: str
+            Unit of the data.
+        """
+        self.unwrap_ampl = self.ampl_max
+        self.unwrap_thresh = thresh
+        self.unwrap_clips = clips
+        self.unwrap_down_scale = down_scale
+        self.unwrap = thresh > 1e-3
+        if self.unwrap:
+            if self.unwrap_clips:
+                add_unwrap(self.metadata(),
+                           self.unwrap_thresh*self.unwrap_ampl,
+                           self.unwrap_ampl, unit)
+            elif down_scale:
+                update_gain(self.metadata(), 0.5)
+                add_unwrap(self.metadata(),
+                           0.5*self.unwrap_thresh*self.unwrap_ampl,
+                           0.0, unit)
+            else:
+                self.ampl_min *= 2
+                self.ampl_max *= 2
+                add_unwrap(self.metadata(),
+                           self.unwrap_thresh*self.unwrap_ampl,
+                           0.0, unit)
+
+                
     # wave interface:        
     def open_wave(self, filepath, buffersize=10.0, backsize=0.0, verbose=0):
         """Open audio file for reading using the wave module.
 
         Note: we assume that setpos() and tell() use integer numbers!
 
         Parameters
@@ -1107,36 +1173,41 @@
         Raises
         ------
         ImportError
             The wave module is not installed
         """
         self.verbose = verbose
         if self.verbose > 0:
-            print('open_wave(filepath) with filepath=%s' % filepath)
+            print(f'open_wave(filepath) with filepath={filepath}')
         if not audio_modules['wave']:
             self.samplerate = 0.0
             self.channels = 0
             self.frames = 0
+            self.size = 0
             self.shape = (0, 0)
             self.offset = 0
             raise ImportError
         if self.sf is not None:
             self._close_wave()
         self.sf = wave.open(filepath, 'r')
         self.filepath = filepath
         self.samplerate = float(self.sf.getframerate())
+        self.format = 'WAV'
         sampwidth = self.sf.getsampwidth()
         if sampwidth == 1:
             self.dtype = 'u1'
+            self.encoding = 'PCM_U8'
         else:
-            self.dtype = 'i%d' % sampwidth
+            self.dtype = f'i{sampwidth}' 
+            self.encoding = f'PCM_{sampwidth*8}'
         self.factor = 1.0/(2.0**(sampwidth*8-1))
         self.channels = self.sf.getnchannels()
         self.frames = self.sf.getnframes()
         self.shape = (self.frames, self.channels)
+        self.size = self.frames * self.channels
         self.buffersize = int(buffersize*self.samplerate)
         self.backsize = int(backsize*self.samplerate)
         self._init_buffer()
         self.close = self._close_wave
         self.load_buffer = self._load_buffer_wave
         # read 1 frame to determine the unit of the position values:
         self.p0 = self.sf.tell()
@@ -1190,30 +1261,34 @@
         Raises
         ------
         ImportError
             The ewave module is not installed.
         """
         self.verbose = verbose
         if self.verbose > 0:
-            print('open_ewave(filepath) with filepath=%s' % filepath)
+            print(f'open_ewave(filepath) with filepath={filepath}')
         if not audio_modules['ewave']:
             self.samplerate = 0.0
             self.channels = 0
             self.frames = 0
             self.shape = (0, 0)
+            self.size = 0
             self.offset = 0
             raise ImportError
         if self.sf is not None:
             self._close_ewave()
         self.sf = ewave.open(filepath, 'r')
         self.filepath = filepath
         self.samplerate = float(self.sf.sampling_rate)
         self.channels = self.sf.nchannels
         self.frames = self.sf.nframes
         self.shape = (self.frames, self.channels)
+        self.size = self.frames * self.channels
+        self.format = 'WAV' # or WAVEX?
+        self.encoding = self.numpy_encodings[self.sf.dtype]
         self.buffersize = int(buffersize*self.samplerate)
         self.backsize = int(backsize*self.samplerate)
         self._init_buffer()
         self.close = self._close_ewave
         self.load_buffer = self._load_buffer_ewave
         return self
 
@@ -1259,34 +1334,39 @@
         Raises
         ------
         ImportError
             The SoundFile module is not installed
         """
         self.verbose = verbose
         if self.verbose > 0:
-            print('open_soundfile(filepath) with filepath=%s' % filepath)
+            print(f'open_soundfile(filepath) with filepath={filepath}')
         if not audio_modules['soundfile']:
             self.samplerate = 0.0
             self.channels = 0
             self.frames = 0
             self.shape = (0, 0)
+            self.size = 0
             self.offset = 0
             raise ImportError
         if self.sf is not None:
             self._close_soundfile()
         self.sf = soundfile.SoundFile(filepath, 'r')
         self.filepath = filepath
         self.samplerate = float(self.sf.samplerate)
         self.channels = self.sf.channels
         self.frames = 0
+        self.size = 0
         if self.sf.seekable():
             self.frames = self.sf.seek(0, soundfile.SEEK_END)
             self.sf.seek(0, soundfile.SEEK_SET)
         # TODO: if not seekable, we cannot handle that file!
         self.shape = (self.frames, self.channels)
+        self.size = self.frames * self.channels
+        self.format = self.sf.format
+        self.encoding = self.sf.subtype
         self.buffersize = int(buffersize*self.samplerate)
         self.backsize = int(backsize*self.samplerate)
         self._init_buffer()
         self.close = self._close_soundfile
         self.load_buffer = self._load_buffer_soundfile
         return self
 
@@ -1330,30 +1410,43 @@
         Raises
         ------
         ImportError
             The wavefile module is not installed
         """
         self.verbose = verbose
         if self.verbose > 0:
-            print('open_wavefile(filepath) with filepath=%s' % filepath)
+            print(f'open_wavefile(filepath) with filepath={filepath}')
         if not audio_modules['wavefile']:
             self.samplerate = 0.0
             self.channels = 0
             self.frames = 0
             self.shape = (0, 0)
+            self.size = 0
             self.offset = 0
             raise ImportError
         if self.sf is not None:
             self._close_wavefile()
         self.sf = wavefile.WaveReader(filepath)
         self.filepath = filepath
         self.samplerate = float(self.sf.samplerate)
         self.channels = self.sf.channels
         self.frames = self.sf.frames
         self.shape = (self.frames, self.channels)
+        self.size = self.frames * self.channels
+        # get format and encoding:
+        for attr in dir(wavefile.Format):
+            v = getattr(wavefile.Format, attr)
+            if isinstance(v, int):
+                if v & wavefile.Format.TYPEMASK > 0 and \
+                   (self.sf.format & wavefile.Format.TYPEMASK) == v:
+                    self.format = attr
+                if v & wavefile.Format.SUBMASK > 0 and \
+                   (self.sf.format & wavefile.Format.SUBMASK) == v:
+                    self.encoding = attr
+        # init buffer:
         self.buffersize = int(buffersize*self.samplerate)
         self.backsize = int(backsize*self.samplerate)
         self._init_buffer()
         self.close = self._close_wavefile
         self.load_buffer = self._load_buffer_wavefile
         return self
 
@@ -1402,30 +1495,32 @@
         Raises
         ------
         ImportError
             The audioread module is not installed
         """
         self.verbose = verbose
         if self.verbose > 0:
-            print('open_audio_read(filepath) with filepath=%s' % filepath)
+            print(f'open_audioread(filepath) with filepath={filepath}')
         if not audio_modules['audioread']:
             self.samplerate = 0.0
             self.channels = 0
             self.frames = 0
             self.shape = (0, 0)
+            self.size = 0
             self.offset = 0
             raise ImportError
         if self.sf is not None:
             self._close_audioread()
         self.sf = audioread.audio_open(filepath)
         self.filepath = filepath
         self.samplerate = float(self.sf.samplerate)
         self.channels = self.sf.channels
         self.frames = int(np.ceil(self.samplerate*self.sf.duration))
         self.shape = (self.frames, self.channels)
+        self.size = self.frames * self.channels
         self.buffersize = int(buffersize*self.samplerate)
         self.backsize = int(backsize*self.samplerate)
         self._init_buffer()
         self.read_buffer = np.zeros((0,0))
         self.read_offset = 0
         self.close = self._close_audioread
         self.load_buffer = self._load_buffer_audioread
@@ -1462,16 +1557,15 @@
             i = 0
             n = r_offset + r_size - self.read_offset
             if n > r_size:
                 i += n - r_size
                 n = r_size
             buffer[self.read_offset+i-r_offset:self.read_offset+i+n-r_offset,:] = self.read_buffer[i:i+n,:] / (2.0**15-1.0)
             if self.verbose > 2:
-                print('  recycle %6d frames from the front of the read buffer at %d-%d (%d-%d in buffer)'
-                       % (n, self.read_offset, self.read_offset+n, self.read_offset-self.offset, self.read_offset-self.offset+n))
+                print(f'  recycle {n:6d} frames from the front of the read buffer at {self.read_offset}-{self.read_offset+n} ({self.read_offset-self.offset}-{self.read_offset-self.offset+n} in buffer)')
             r_size -= n
             if r_size <= 0:
                 return
         # go back to beginning of file:
         if r_offset < self.read_offset:
             if self.verbose > 2:
                 print('  rewind')
@@ -1488,60 +1582,56 @@
                     fbuffer = self.sf_iter.next()
                 else:
                     fbuffer = next(self.sf_iter)
             except StopIteration:
                 self.read_buffer = np.zeros((0,0))
                 buffer[:,:] = 0.0
                 if self.verbose > 1:
-                    print('  caught StopIteration, padded buffer with %d zeros' % r_size)
+                    print(f'  caught StopIteration, padded buffer with {r_size} zeros')
                 break
             self.read_buffer = np.frombuffer(fbuffer, dtype='<i2').reshape(-1, self.channels)
             if self.verbose > 2:
-                print('  read forward by %d frames' % self.read_buffer.shape[0])
+                print(f'  read forward by {self.read_buffer.shape[0]} frames')
         # recycle file data:
         if ( self.read_offset + self.read_buffer.shape[0] > r_offset
              and self.read_offset <= r_offset ):
             i = r_offset - self.read_offset
             n = self.read_offset + self.read_buffer.shape[0] - r_offset
             if n > r_size:
                 n = r_size
             buffer[:n,:] = self.read_buffer[i:i+n,:] / (2.0**15-1.0)
             if self.verbose > 2:
-                print('  recycle %6d frames from the end of the read buffer at %d-%d to %d-%d (%d-%d in buffer)'
-                       % (n, self.read_offset, self.read_offset + self.read_buffer.shape[0],
-                          r_offset, r_offset+n, r_offset-self.offset, r_offset+n-self.offset))
+                print(f'  recycle {n:6d} frames from the end of the read buffer at {self.read_offset}-{self.read_offset + self.read_buffer.shape[0]} to {r_offset}-{r_offset+n} ({r_offset-self.offset}-{r_offset+n-self.offset} in buffer)')
             b_offset += n
             r_offset += n
             r_size -= n
         # read data:
         if self.verbose > 2 and r_size > 0:
-            print('  read    %6d frames at %d-%d (%d-%d in buffer)'
-                   % (r_size, r_offset, r_offset+r_size, r_offset-self.offset, r_offset+r_size-self.offset))
+            print(f'  read    {r_size:6d} frames at {r_offset}-{r_offset+r_size} ({r_offset-self.offset}-{r_offset+r_size-self.offset} in buffer)')
         while r_size > 0:
             self.read_offset += self.read_buffer.shape[0]
             try:
                 if hasattr(self.sf_iter, 'next'):
                     fbuffer = self.sf_iter.next()
                 else:
                     fbuffer = next(self.sf_iter)
             except StopIteration:
                 self.read_buffer = np.zeros((0,0))
                 buffer[b_offset:,:] = 0.0
                 if self.verbose > 1:
-                    print('  caught StopIteration, padded buffer with %d zeros' % r_size)
+                    print(f'  caught StopIteration, padded buffer with {r_size} zeros')
                 break
             self.read_buffer = np.frombuffer(fbuffer, dtype='<i2').reshape(-1, self.channels)
             n = self.read_buffer.shape[0]
             if n > r_size:
                 n = r_size
             if n > 0:
                 buffer[b_offset:b_offset+n,:] = self.read_buffer[:n,:] / (2.0**15-1.0)
                 if self.verbose > 2:
-                    print('    read  %6d frames to %d-%d (%d-%d in buffer)'
-                          % (n, r_offset, r_offset+n, r_offset-self.offset, r_offset+n-self.offset))
+                    print(f'    read  {n:6d} frames to {r_offset}-{r_offset+n} ({r_offset-self.offset}-{r_offset+n-self.offset} in buffer)')
                 b_offset += n
                 r_offset += n
                 r_size -= n
 
                                 
     def open(self, filepath, buffersize=10.0, backsize=0.0, verbose=0):
         """Open audio file for reading.
@@ -1566,57 +1656,59 @@
         EOFError
             File size of `filepath` is zero.
         IOError
             Failed to load data.
         """
         self.buffer = np.array([])
         self.samplerate = 0.0
-        if len(filepath) == 0:
+        if not filepath:
             raise ValueError('input argument filepath is empty string!')
         if not os.path.isfile(filepath):
-            raise FileNotFoundError('file "%s" not found' % filepath)
+            raise FileNotFoundError(f'file "{filepath}" not found')
         if os.path.getsize(filepath) <= 0:
-            raise EOFError('file "%s" is empty (size=0)!' % filepath)
+            raise EOFError(f'file "{filepath}" is empty (size=0)!')
         # list of implemented open functions:
-        audio_open = [
-            ['soundfile', self.open_soundfile],
-            ['audioread', self.open_audioread],
-            ['wave', self.open_wave],
-            ['wavefile', self.open_wavefile],
-            ['ewave', self.open_ewave]
-            ]
+        audio_open_funcs = (
+            ('soundfile', self.open_soundfile),
+            ('wave', self.open_wave),
+            ('wavefile', self.open_wavefile),
+            ('ewave', self.open_ewave),
+            ('audioread', self.open_audioread),
+            )
         # open an audio file by trying various modules:
-        success = False
         not_installed = []
-        for lib, open_file in audio_open:
+        errors = [f'failed to load data from file "{filepath}":']
+        for lib, open_file in audio_open_funcs:
             if not audio_modules[lib]:
                 if verbose > 1:
-                    print('failed to load data from file "%s" using %s module' %
-                          (filepath, lib))
+                    print(f'unable to load data from file "{filepath}" using {lib} module: module not available')
                 not_installed.append(lib)
                 continue
             try:
                 open_file(filepath, buffersize, backsize, verbose-1)
                 if self.frames > 0:
-                    success = True
                     if verbose > 0:
-                        print('opened audio file "%s" using %s' % (filepath, lib))
+                        print(f'opened audio file "{filepath}" using {lib}')
                         if verbose > 1:
-                            print('  sampling rate: %g Hz' % self.samplerate)
-                            print('  data values  : %d' % self.frames)
-                    break
+                            if self.format is not None:
+                                print(f'  format       : {self.format}')
+                            if self.encoding is not None:
+                                print(f'  encoding     : {self.encoding}')
+                            print(f'  sampling rate: {self.samplerate} Hz')
+                            print(f'  channels     : {self.channels}')
+                            print(f'  frames       : {self.frames}')
+                    return self
             except Exception as e:
-                    pass
-        if not success:
-            need_install = ""
-            if len(not_installed) > 0:
-                need_install = " You may need to install one of the " + \
-                  ', '.join(not_installed) + " packages."
-            raise IOError('failed to load data from file "%s".%s' %
-                          (filepath, need_install))
+                errors.append(f'  {lib} failed: {str(e)}')
+                if verbose > 1:
+                    print(errors[-1])
+        if len(not_installed) > 0:
+            errors.append('\n  You may need to install one of the ' + \
+              ', '.join(not_installed) + ' packages.')
+        raise IOError('\n'.join(errors))
         return self
 
     
 def demo(file_path, plot):
     """Demo of the audioloader functions.
 
     Parameters
@@ -1635,26 +1727,26 @@
 
     if audio_modules['soundfile'] and audio_modules['audioread']:
         print('')
         print("cross check:")
         data1, rate1 = load_soundfile(file_path)
         data2, rate2 = load_audioread(file_path)
         n = min((len(data1), len(data2)))
-        print("rms difference is %g" % np.std(data1[:n]-data2[:n]))
+        print(f"rms difference is {np.std(data1[:n]-data2[:n])}")
         if plot:
             plt.plot(np.arange(len(data1))/rate1, data1[:,0])
             plt.plot(np.arange(len(data2))/rate2, data2[:,0])
             plt.show()
     
     print('')
     print("try AudioLoader:")
     with AudioLoader(file_path, 4.0, 1.0, 1) as data:
-        print('samplerate: %g' % data.samplerate)
-        print('channels: %d %d' % (data.channels, data.shape[1]))
-        print('frames: %d %d' % (len(data), data.shape[0]))
+        print(f'samplerate: {data.samplerate:0f}Hz')
+        print(f'channels: {data.channels} {data.shape[1]}')
+        print(f'frames: {len(data)} {data.shape[0]}')
         nframes = int(1.5*data.samplerate)
         # check access:
         print('check random single frame access')
         for inx in np.random.randint(0, len(data), 1000):
             if np.any(np.abs(full_data[inx] - data[inx]) > 2.0**(-14)):
                 print('single random frame access failed', inx, full_data[inx], data[inx])
         print('check random frame slice access')
@@ -1667,22 +1759,22 @@
                 print('frame slice access forward failed', inx)
         print('check frame slice access backward')
         for inx in range(len(data)-nframes, 0, -10):
             if np.any(np.abs(full_data[inx:inx+nframes] - data[inx:inx+nframes]) > 2.0**(-14)):
                 print('frame slice access backward failed', inx)
         # forward:
         for i in range(0, len(data), nframes):
-            print('forward %d-%d' % (i, i+nframes))
+            print(f'forward {i}-{i+nframes}')
             x = data[i:i+nframes,0]
             if plot:
                 plt.plot((i+np.arange(len(x)))/rate, x)
                 plt.show()
         # and backwards:
         for i in reversed(range(0, len(data), nframes)):
-            print('backward %d-%d' % (i, i+nframes))
+            print(f'backward {i}-{i+nframes}')
             x = data[i:i+nframes,0]
             if plot:
                 plt.plot((i+np.arange(len(x)))/rate, x)
                 plt.show()
 
 
 def main(*args):
@@ -1698,15 +1790,15 @@
     help = False
     plot = False
     file_path = None
     mod = False
     for arg in args:
         if mod:
             if not select_module(arg):
-                print('can not select module %s that is not installed' % arg)
+                print(f'can not select module {arg} that is not installed')
                 return
             mod = False
         elif arg == '-h':
             help = True
             break
         elif arg == '-p':
             plot = True
@@ -1715,15 +1807,15 @@
         else:
             file_path = arg
             break
 
     if help:
         print('')
         print('Usage:')
-        print('  python -m audioio.audioloader [-m <module>] [-p] <audio/file.wav>')
+        print('  python -m src.audioio.audioloader [-m <module>] [-p] <audio/file.wav>')
         print('  -m: audio module to be used')
         print('  -p: plot loaded data')
         return
 
     if plot:
         import matplotlib.pyplot as plt
```

### Comparing `audioio-2.0.0/audioio/audiomarkers.py` & `audioio-2.1.0/src/audioio/audiomarkers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Working with marker lists.
 
 Markers are used to mark specific positions or regions in the audio
-data.  Each marker has a position, a span, a label, and a text.
-Position, and span are handled with 1-D or 2-D arrays of ints, where
-each row is a marker and the columns are position and optional
+data.  Each marker has a position (cue, event), a span, a label, and a
+text.  Position, and span are handled with 1-D or 2-D arrays of ints,
+where each row is a marker and the columns are position and optional
 span. Labels and texts come in another 1-D or 2-D array of objects
 pointing to strings. Again, rows are the markers, first column are the
 labels, and second column the optional texts. Try to keep the labels
 short, and use text for longer descriptions.
 
 - `write_markers()`: write markers to a text file or stream.
 - `print_markers()`: write markers to standard output.
@@ -49,32 +49,32 @@
     has_text = False
     if labels is not None and len(labels) > 0:
         has_labels = True
         if labels.ndim == 1:
             labels = labels.reshape(-1, 1)
         has_text = labels.shape[1] > 1
     # table header:
-    fh.write(f'{prefix}{"position":8}')
+    fh.write(f'{prefix}{"position":10}')
     if has_span:
-        fh.write(f'{sep}{"span":6}')
+        fh.write(f'{sep}{"span":8}')
     if has_labels:
         fh.write(f'{sep}{"label":10}')
     if has_text:
         fh.write(f'{sep}{"text"}')
     fh.write('\n')
     # table data:
     for i in range(len(locs)):
-        fh.write(f'{prefix}{locs[i,0]:8}')
+        fh.write(f'{prefix}{locs[i,0]:10}')
         if has_span:
-            fh.write(f'{sep}{locs[i,1]:6}')
+            fh.write(f'{sep}{locs[i,1]:8}')
         if has_labels:
             fh.write(f'{sep}{labels[i,0]:10}')
         if has_text:
             fh.write(f'{sep}{labels[i,1]}')
-    fh.write('\n')
+        fh.write('\n')
     if own_file:
         fh.close()
 
         
 def print_markers(locs, labels=None, sep=' ', prefix=''):
     """Write markers to standard output.
```

### Comparing `audioio-2.0.0/audioio/audiomodules.py` & `audioio-2.1.0/src/audioio/audiomodules.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 - `list_modules()`: print list of all supported modules and their installation status.
 - `missing_modules()`: missing audio modules that are recommended to be installed.
 - `missing_modules_instructions()`: print installation instructions for missing but useful audio modules.
 - `installation_instruction()`: instructions on how to install a specific audio module.
 - `main()`: command line program for listing installation status of audio modules.
 
 
-## Script
+## Command line script
 
 Run this module as a script
 ```sh
-> python -m audioio.auidomodules
+> python -m src.audioio.auidomodules
 ```
 or, when the audioio package is installed on your system, simply run
 ```sh
 > audiomodules
 ```
 for an overview of audio packages, their installation status, and recommendations on
 how to install further audio packages. The output looks like this:
@@ -767,15 +767,15 @@
 
 
 def main(*args):
     """ Command line program for listing installation status of audio modules.
 
     Run this module as a script
     ```
-    > python -m audioio.auidomodules
+    > python -m src.audioio.auidomodules
     ```
     or, when the audioio package is installed on your system, simply run
     ```sh
     > audiomodules
     ```
     for an overview of audio packages, their installation status, and recommendations on
     how to install further audio packages.
```

### Comparing `audioio-2.0.0/audioio/audiotools.py` & `audioio-2.1.0/src/audioio/audiotools.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         return decorator_jit
     prange = range
 
 
 def despike(data, thresh=1.0, n=1):
     """Remove spikes. 
 
-    If single data points stick out by more than a threshold, they are
+    If `n` data points stick out by more than a threshold, they are
     replaced by the mean of the two directly preceeding and succeeding
     data points.
 
     Parameters
     ----------
     data: 1D or 2D ndarray
         Data to be fixed in place.
@@ -69,53 +69,52 @@
                       ((diff[:-k] < -thresh) & (diff[k:] > thresh))
                 # replace with weighted average of neighbors:
                 for j in range(1, k+1):
                     data[j:-k-1+j][sel] = ((k+1-j)*data[:-1-k][sel] + \
                                            j*data[1+k:][sel])/(k+1)
 
 
-def unwrap(data, thresh=1.5):
+def unwrap(data, thresh=1.5, ampl_max=1.0):
     """Unwrap clipped data that are folded into the available data range.
 
     In some amplifiers/ADCs clipped data appear on the opposite side
     of the input range. This function tries to undo this wrapping.
     
     Parameters
     ----------
     data: 1D or 2D ndarray of floats
         Data to be fixed in place.
     thresh: float
         Minimum difference between succeeding data points required
-        for initiating unwrapping.
+        for initiating unwrapping relative to ampl_max.
+    ampl_max: float
+        Maximum amplitude of the input range.
     """
 
     @jit(nopython=True)
-    def unwrap_trace(data, delta):
-        thresh = delta - 1.0
+    def unwrap_trace(data, thresh, ampl_max):
         step = 0.0
         for i in range(1, len(data)):
             cstep = 0.0
             dd = data[i] - data[i-1]
             if data[i] >= 0:
-                if abs(dd - 2.0) < abs(dd):
-                    cstep = -2.0
+                if abs(dd - 2.0*ampl_max) < abs(dd):
+                    cstep = -2.0*ampl_max
             if data[i] <= 0:
-                if abs(dd + 2.0) < abs(dd + cstep):
-                    cstep = +2.0
-            #if step != cstep and (cstep == 0.0 or \
-            #                      (abs(data[i-1]) > thresh and \
-            #                       abs(dd) > delta)):
-            if step != cstep and (cstep == 0.0 or abs(dd) > delta):
+                if abs(dd + 2.0*ampl_max) < abs(dd + cstep):
+                    cstep = +2.0*ampl_max
+            if step != cstep and (cstep == 0.0 or abs(dd) > thresh):
                 step = cstep
             data[i] += step
         
     @jit(nopython=True, parallel=True)
-    def unwrap_traces(data, thresh):
+    def unwrap_traces(data, thresh, ampl_max):
         for c in prange(data.shape[1]):
-            unwrap_trace(data[:,c], thresh)
+            unwrap_trace(data[:,c], thresh, ampl_max)
 
     if not has_numba:
         warnings.warn('unwrap() requires numba to work')
+    thresh *= ampl_max
     if data.ndim > 1:
-        unwrap_traces(data, thresh)
+        unwrap_traces(data, thresh, ampl_max)
     else:
-        unwrap_trace(data, thresh)
+        unwrap_trace(data, thresh, ampl_max)
```

### Comparing `audioio-2.0.0/audioio/audiowriter.py` & `audioio-2.1.0/src/audioio/audiowriter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Writing numpy arrays of floats to audio files.
+"""Write numpy arrays of floats to audio files.
 
 - `write_audio()`: write audio data to file.
 - `available_formats()`: audio file formats supported by any of the installed audio modules.
 - `available_encodings()`: encodings of an audio file format supported by any of the installed audio modules.
 - `format_from_extension()`: deduce audio file format from file extension.
 
 The data to be written are 1-D or 2-D numpy arrays of floats ranging
@@ -11,15 +11,15 @@
 For support of more audio formats, you might need to install
 additional packages.
 See [installation](https://bendalab.github.io/audioio/installation)
 for further instructions.
 
 For a demo, run the script as:
 ```
-python -m audioio.audiowriter
+python -m src.audioio.audiowriter
 ```
 
 """
 
 import os
 import sys
 import subprocess
@@ -90,15 +90,15 @@
     elif format.upper() != 'WAV':
         return []
     else:
         return ['PCM_32', 'PCM_16', 'PCM_U8']
 
 
 def write_wave(filepath, data, samplerate, metadata=None, locs=None,
-               labels=None, format=None, encoding=None):
+               labels=None, format=None, encoding=None, marker_hint='cue'):
     """Write audio data using the wave module from pythons standard libray.
     
     Documentation
     -------------
     https://docs.python.org/3.8/library/wave.html
 
     Parameters
@@ -120,14 +120,17 @@
         Labels (first column) and texts (optional second column)
         for each marker (rows).
     format: string or None
         File format, only 'WAV' is supported.
     encoding: string or None
         Encoding of the data: 'PCM_32', 'PCM_16', or 'PCM_U8'.
         If None or empty string use 'PCM_16'.
+    marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
 
     Raises
     ------
     ImportError
         The wave module is not installed.
     *
         Writing of the data failed.
@@ -168,15 +171,15 @@
         buffer = np.floor((data+1.0) * factor).astype(dtype)
         buffer[data >= 1.0] = 2*factor - 1
     else:
         buffer = np.floor(data * factor).astype(dtype)
         buffer[data >= 1.0] = factor - 1
     wf.writeframes(buffer.tobytes())
     wf.close()
-    append_riff(filepath, metadata, locs, labels)
+    append_riff(filepath, metadata, locs, labels, samplerate, marker_hint)
 
 
 def formats_ewave():
     """Audio file formats supported by the ewave module.
 
     Returns
     -------
@@ -207,15 +210,15 @@
     elif format.upper() != 'WAV' and format.upper() != 'WAVEX':
         return []
     else:
         return ['PCM_64', 'PCM_32', 'PCM_16', 'FLOAT', 'DOUBLE']
 
 
 def write_ewave(filepath, data, samplerate, metadata=None, locs=None,
-                labels=None, format=None, encoding=None):
+                labels=None, format=None, encoding=None, marker_hint='cue'):
     """Write audio data using the ewave module from pythons standard libray.
 
     Documentation
     -------------
     https://github.com/melizalab/py-ewave
 
     Parameters
@@ -237,14 +240,17 @@
         Labels (first column) and texts (optional second column)
         for each marker (rows).
     format: string or None
         File format, only 'WAV' and 'WAVEX' are supported.
     encoding: string or None
         Encoding of the data: 'PCM_64', 'PCM_32', PCM_16', 'FLOAT', 'DOUBLE'
         If None or empty string use 'PCM_16'.
+    marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
 
     Raises
     ------
     ImportError
         The ewave module is not installed.
     *
         Writing of the data failed.
@@ -275,15 +281,15 @@
     channels = 1
     if len(data.shape) > 1:
         channels = data.shape[1]
 
     with ewave.open(filepath, 'w', sampling_rate=int(samplerate),
                     dtype=ewave_encodings[encoding], nchannels=channels) as wf:
         wf.write(data, scale=True)
-    append_riff(filepath, metadata, locs, labels)
+    append_riff(filepath, metadata, locs, labels, samplerate, marker_hint)
 
 
 def formats_wavfile():
     """Audio file formats supported by the scipy.io.wavfile module.
 
     Returns
     -------
@@ -314,15 +320,16 @@
     elif format.upper() != 'WAV':
         return []
     else:
         return ['PCM_U8', 'PCM_16', 'PCM_32', 'PCM_64', 'FLOAT', 'DOUBLE']
 
 
 def write_wavfile(filepath, data, samplerate, metadata=None,
-                  locs=None, labels=None, format=None, encoding=None):
+                  locs=None, labels=None, format=None, encoding=None,
+                  marker_hint='cue'):
     """Write audio data using the scipy.io.wavfile module.
     
     Documentation
     -------------
     http://docs.scipy.org/doc/scipy/reference/io.html
 
     Parameters
@@ -344,14 +351,17 @@
         Labels (first column) and texts (optional second column)
         for each marker (rows).
     format: string or None
         File format, only 'WAV' is supported.
     encoding: string or None
         Encoding of the data: 'PCM_64', 'PCM_32', PCM_16', 'PCM_U8', 'FLOAT', 'DOUBLE'
         If None or empty string use 'PCM_16'.
+    marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
 
     Raises
     ------
     ImportError
         The wavfile module is not installed.
     ValueError
         File format or encoding not supported.
@@ -388,15 +398,15 @@
     elif dtype[0] == 'i':
         factor = 2**(sampwidth*8-1)
         buffer = np.floor(data * factor).astype(dtype)
         buffer[data >= 1.0] = factor - 1
     else:
         buffer = data.astype(dtype, copy=False)
     wavfile.write(filepath, int(samplerate), buffer)
-    append_riff(filepath, metadata, locs, labels)
+    append_riff(filepath, metadata, locs, labels, samplerate, marker_hint)
 
 
 def formats_soundfile():
     """Audio file formats supported by the SoundFile module.
 
     Returns
     -------
@@ -425,15 +435,16 @@
     if not audio_modules['soundfile']:
         return []
     else:
         return sorted(list(soundfile.available_subtypes(format)))
 
 
 def write_soundfile(filepath, data, samplerate, metadata=None,
-                    locs=None, labels=None, format=None, encoding=None):
+                    locs=None, labels=None, format=None, encoding=None,
+                    marker_hint='cue'):
     """Write audio data using the SoundFile module (based on libsndfile).
     
     Documentation
     -------------
     http://pysoundfile.readthedocs.org
 
     Parameters
@@ -455,14 +466,17 @@
         Labels (first column) and texts (optional second column)
         for each marker (rows).
     format: string or None
         File format.
     encoding: string or None
         Encoding of the data.
         If None or empty string use 'PCM_16'.
+    marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
 
     Raises
     ------
     ImportError
         The SoundFile module is not installed.
     *
         Writing of the data failed.
@@ -480,15 +494,15 @@
     if not encoding:
         encoding = 'PCM_16'
     encoding = encoding.upper()
     
     soundfile.write(filepath, data, int(samplerate), format=format,
                     subtype=encoding)
     try:
-        append_riff(filepath, metadata, locs, labels)
+        append_riff(filepath, metadata, locs, labels, samplerate, marker_hint)
     except ValueError:
         pass
 
 
 def formats_wavefile():
     """Audio file formats supported by the wavefile module.
 
@@ -533,15 +547,16 @@
              and v & wavefile.Format.SUBMASK > 0
              and v != wavefile.Format.SUBMASK ):
             encodings.append(attr)
     return sorted(encodings)
 
     
 def write_wavefile(filepath, data, samplerate, metadata=None,
-                   locs=None, labels=None, format=None, encoding=None):
+                   locs=None, labels=None, format=None, encoding=None,
+                   marker_hint='cue'):
     """Write audio data using the wavefile module (based on libsndfile).
     
     Documentation
     -------------
     https://github.com/vokimon/python-wavefile
 
     Parameters
@@ -563,14 +578,17 @@
         Labels (first column) and texts (optional second column)
         for each marker (rows).
     format: string or None
         File format as in wavefile.Format.
     encoding: string or None
         Encoding of the data as in wavefile.Format.
         If None or empty string use 'PCM_16'.
+    marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
 
     Raises
     ------
     ImportError
         The wavefile module is not installed.
     ValueError
         File format or encoding not supported.
@@ -607,15 +625,15 @@
     else:
         data = data.reshape((-1, 1))
     with wavefile.WaveWriter(filepath, channels=channels,
                              samplerate=int(samplerate),
                              format=format_value|encoding_value) as w:
         w.write(data.T)
     try:
-        append_riff(filepath, metadata, locs, labels)
+        append_riff(filepath, metadata, locs, labels, samplerate, marker_hint)
     except ValueError:
         pass
 
 
 def formats_pydub():
     """Audio file formats supported by the Pydub module.
 
@@ -683,15 +701,15 @@
                 encoding = cols[1]
                 if encoding in pydub_encodings:
                     encoding = pydub_encodings[encoding]
                 encodings.append(encoding.upper())
     return encodings
 
 def write_pydub(filepath, data, samplerate, metadata=None, locs=None,
-                labels=None, format=None, encoding=None):
+                labels=None, format=None, encoding=None, marker_hint='cue'):
     """Write audio data using the Pydub module.
     
     Documentation
     -------------
     https://github.com/jiaaro/pydub
 
     Parameters
@@ -713,14 +731,17 @@
         Labels (first column) and texts (optional second column)
         for each marker (rows).
     format: string or None
         File format, everything ffmpeg or avtools are supporting.
     encoding: string or None
         Encoding of the data.
         If None or empty string use 'PCM_16'.
+    marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
 
     Raises
     ------
     ImportError
         The Pydub module is not installed.
     *
         Writing of the data failed.
@@ -757,30 +778,30 @@
     if len(data.shape) > 1:
         channels = data.shape[1]
     int_data = (data*(2**31-1)).astype(np.int32)
     sound = pydub.AudioSegment(int_data.ravel(), sample_width=4,
                                frame_rate=samplerate, channels=channels)
     sound.export(filepath, format=format.lower(), codec=encoding)
     try:
-        append_riff(filepath, metadata, locs, labels)
+        append_riff(filepath, metadata, locs, labels, samplerate, marker_hint)
     except ValueError:
         pass
     
 
 audio_formats_funcs = (
     ('soundfile', formats_soundfile),
     ('wavefile', formats_wavefile),
     ('wave', formats_wave),
     ('ewave', formats_ewave),
     ('scipy.io.wavfile', formats_wavfile),
     ('pydub', formats_pydub)
     )
-""" List of implemented formats functions.
+""" List of implemented formats() functions.
 
-Each element of the list is a tuple with the module's name and the formats function.
+Each element of the list is a tuple with the module's name and the formats() function.
 """
 
 
 def available_formats():
     """Audio file formats supported by any of the installed audio modules.
 
     Returns
@@ -807,17 +828,17 @@
     ('soundfile', encodings_soundfile),
     ('wavefile', encodings_wavefile),
     ('wave', encodings_wave),
     ('ewave', encodings_ewave),
     ('scipy.io.wavfile', encodings_wavfile),
     ('pydub', encodings_pydub)
     )
-""" List of implemented encodings functions.
+""" List of implemented encodings() functions.
 
-Each element of the list is a tuple with the module's name and the encodings function.
+Each element of the list is a tuple with the module's name and the encodings() function.
 """
 
 
 def available_encodings(format):
     """Encodings of an audio file format supported by any of the installed audio modules.
 
     Parameters
@@ -830,47 +851,43 @@
     encodings: list of strings
         List of supported encodings as strings.
 
     Example
     -------
     ```
     >>> from audioio import available_encodings
-    >>> e = available_encodings()
+    >>> e = available_encodings('WAV')
     >>> printf(e)
-    ['AAC', 'AC3', ..., 'PCM_16', 'PCM_24', 'PCM_32', ..., 'WAVPACK', 'WMAV1', 'WMAV2']
+    ['ALAW', 'DOUBLE', 'FLOAT', 'G721_32', 'GSM610', 'IMA_ADPCM', 'MS_ADPCM', 'PCM_16', 'PCM_24', 'PCM_32', 'PCM_U8', 'ULAW']
     ```
     """
-    got_sndfile = False
-    encodings = set()
     for module, encodings_func in audio_encodings_funcs:
-        if got_sndfile and module == 'scipy.io.wavfile':
-            continue
         encs = encodings_func(format)
-        encodings |= set(encs)
-        if module in ['soundfile', 'wavefile'] and len(encs) > 0:
-            got_sndfile = True
-    return sorted(list(encodings))
+        if len(encs) > 0:
+            return encs
+    return []
 
 
 audio_writer_funcs = (
     ('soundfile', write_soundfile),
     ('wavefile', write_wavefile),
     ('wave', write_wave),
     ('ewave', write_ewave),
     ('scipy.io.wavfile', write_wavfile),
     ('pydub', write_pydub)
     )
-""" List of implemented write functions.
+""" List of implemented write() functions.
 
-Each element of the list is a tuple with the module's name and the write function.
+Each element of the list is a tuple with the module's name and the write() function.
 """
 
 
 def write_audio(filepath, data, samplerate, metadata=None, locs=None,
-                labels=None, format=None, encoding=None, verbose=0):
+                labels=None, format=None, encoding=None, marker_hint='cue',
+                verbose=0):
     """Write audio data, metadata, and marker to file.
 
     Parameters
     ----------
     filepath: string
         Full path and name of the file to write.
     data: 1-D or 2-D array of floats
@@ -889,14 +906,17 @@
         for each marker (rows).
     format: string or None
         File format. If None deduce file format from filepath.
         See `available_formats()` for possible values.
     encoding: string or None
         Encoding of the data. See `available_encodings()` for possible values.
         If None or empty string use 'PCM_16'.
+    marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
     verbose: int
         If >0 show detailed error/warning messages.
 
     Raises
     ------
     ValueError
         `filepath` is empty string.
@@ -923,37 +943,38 @@
 
     # write audio with metadata and markers:
     if not format:
         format = format_from_extension(filepath)
     if format == 'WAV' and (metadata is not None or locs is not None):
         try:
             audioio_write_wave(filepath, data, samplerate, metadata,
-                               locs, labels, encoding)
+                               locs, labels, encoding, marker_hint)
             return
         except ValueError:
             pass
     # write audio file by trying available modules:
+    errors = [f'failed to write data to file "{filepath}":']
     for lib, write_file in audio_writer_funcs:
         if not audio_modules[lib]:
             continue
         try:
             write_file(filepath, data, samplerate, metadata, locs,
-                       labels, format, encoding)
+                       labels, format, encoding, marker_hint)
             success = True
             if verbose > 0:
                 print('wrote data to file "%s" using %s module' %
                       (filepath, lib))
                 if verbose > 1:
                     print('  sampling rate: %g Hz' % samplerate)
                     print('  channels     : %d' % (data.shape[1] if len(data.shape) > 1 else 1))
                     print('  frames       : %d' % len(data))
             return
         except Exception as e:
-            pass
-    raise IOError('failed to write data to file "%s"' % filepath)
+            errors.append(f'  {lib} failed: {str(e)}')
+    raise IOError('\n'.join(errors))
 
 
 def demo(file_path, channels=2, encoding=''):
     """Demo of the audiowriter functions.
 
     Parameters
     ----------
@@ -1010,15 +1031,15 @@
             break
     if file_path is None:
         file_path = 'test.wav'
 
     if help:
         print('')
         print('Usage:')
-        print('  python -m audioio.audiowriter [-m module] [-n channels] [<filename>] [<encoding>]')
+        print('  python -m src.audioio.audiowriter [-m module] [-n channels] [<filename>] [<encoding>]')
         return
 
     demo(file_path, channels=channels, encoding=encoding)
 
 
 if __name__ == "__main__":
     main(*sys.argv[1:])
```

### Comparing `audioio-2.0.0/audioio/playaudio.py` & `audioio-2.1.0/src/audioio/playaudio.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,24 @@
 
 You might need to install additional packages for better audio output.
 See [installation](https://bendalab.github.io/audioio/installation)
 for further instructions.
 
 For a demo, run the script as:
 ```
-python -m audioio.playaudio
+python -m src.audioio.playaudio
 ```
 
 """
 
 from sys import platform
 import os
 import warnings
 import numpy as np
+from scipy.signal import decimate
 from time import sleep
 from io import BytesIO
 from multiprocessing import Process
 from .audiomodules import *
 
 
 handle = None
@@ -147,15 +148,15 @@
         Time for fading in in seconds.
     """
     if len(data) < 4:
         return
     nr = min(int(np.round(fadetime*rate)), len(data)//2) 
     x = np.arange(float(nr))/float(nr) # 0 to pi/2
     y = np.sin(0.5*np.pi*x)**2.0
-    if len(data.shape) > 1:
+    if data.ndim > 1:
         data[:nr, :] *= y[:, None]
     else:
         data[:nr] *= y
 
         
 def fade_out(data, rate, fadetime):
     """Fade out a signal in place.
@@ -176,15 +177,15 @@
         Time for fading out in seconds.
     """
     if len(data) < 4:
         return
     nr = min(int(np.round(fadetime*rate)), len(data)//2) 
     x = np.arange(float(nr))/float(nr) + 1.0 # pi/2 to pi
     y = np.sin(0.5*np.pi*x)**2.0
-    if len(data.shape) > 1:
+    if data.ndim > 1:
         data[-nr:, :] *= y[:, None]
     else:
         data[-nr:] *= y
 
 
 def fade(data, rate, fadetime):
     """Fade in and out a signal in place.
@@ -293,22 +294,20 @@
         """
         if self.handle is None:
             self.open()
         else:
             self.stop()
         self.rate = rate
         self.channels = 1
-        if len(data.shape) > 1:
+        if data.ndim > 1:
             self.channels = data.shape[1]
         # convert data:
         rawdata = data - np.mean(data, axis=0)
         if scale is None:
-            maxd = np.abs(np.max(rawdata))
-            mind = np.abs(np.min(rawdata))
-            scale = 1.0/max((mind, maxd))
+            scale = 1.0/np.max(np.abs(rawdata))
         rawdata *= scale
         self.data = np.floor(rawdata*(2**15-1)).astype(np.int16, order='C')
         self.index = 0
         self._do_play(blocking)
 
     def beep(self, duration=0.5, frequency=880.0, amplitude=0.5, rate=44100.0,
              fadetime=0.05, blocking=True):
@@ -354,37 +353,49 @@
         # # final click for testing (mono only):
         # data = np.hstack((data, np.sin(2.0*np.pi*1000.0*time[0:int(np.ceil(4.0*rate/1000.0))])))
         # play:
         self.play(data, rate, scale=1.0, blocking=blocking)
 
     def _down_sample(self, channels, scale=1):
         """Sample the data down and adapt maximum channel number."""
-        if type(scale) == int:
-            if len(self.data.shape) > 1:
-                self.data = np.asarray(self.data[::scale, :channels], order='C')
+        iscale = 1
+        rscale = scale
+        if isinstance(scale, int):
+            iscale = scale
+            rscale = 1.0
+        elif scale > 2:
+            iscale = int(np.floor(scale))
+            rscale = scale/iscale
+        
+        if iscale > 1:
+            data = decimate(self.data, iscale, axis=0)
+            if self.data.ndim > 1:
+                self.data = np.asarray(data[:,:channels],
+                                       dtype=np.int16, order='C')
             else:
-                self.data = np.asarray(self.data[::scale], order='C')
-        else:
+                self.data = np.asarray(data, dtype=np.int16, order='C')
+            if self.verbose > 0:
+                print(f'decimated sampling rate from {self.rate:.1f}Hz down to {self.rate/iscale:.1f}Hz')
+            self.rate /= iscale
+
+        if rscale != 1.0:
             dt0 = 1.0/self.rate
-            dt1 = scale/self.rate
+            dt1 = rscale/self.rate
             old_time = np.arange(len(self.data))*dt0
             new_time = np.arange(0.0, old_time[-1]+0.5*dt0, dt1)
-            if len(self.data.shape) > 1:
+            if self.data.ndim > 1:
                 data = np.zeros((len(new_time), channels), order='C')
                 for c in range(channels):
-                    data[:, c] = np.interp(new_time, old_time, self.data[:, c])
+                    data[:,c] = np.interp(new_time, old_time, self.data[:,c])
             else:
                 data = np.interp(new_time, old_time, self.data)
-            if self.data.dtype == data.dtype and flags['C_CONTIGUOUS']:
-                self.data = data
-            else:
-                self.data = np.asarray(data, dtype=self.data.dtype, order='C')
-        if self.verbose > 0:
-            print(f'adapted sampling rate from {self.rate:.1f}Hz down to {self.rate/scale:.1f}Hz')
-        self.rate /= scale
+            self.data = np.asarray(data, dtype=self.data.dtype, order='C')
+            if self.verbose > 0:
+                print(f'adapted sampling rate from {self.rate:.1f}Hz to {self.rate/rscale:.1f}Hz')
+            self.rate /= rscale
         self.channels = channels
 
     def __del__(self):
         """Terminate the audio module."""
         self.close()
 
     def __enter__(self):
@@ -463,15 +474,15 @@
         if not self.run:
             flag = pyaudio.paComplete
         if self.index < len(self.data):
             out_data = self.data[self.index:self.index+frames]
             self.index += len(out_data)
             # zero padding:
             if len(out_data) < frames:
-                if len(self.data.shape) > 1:
+                if self.data.ndim > 1:
                     out_data = np.vstack((out_data,
                       np.zeros((frames-len(out_data), self.channels), dtype=np.int16)))
                 else:
                     out_data = np.hstack((out_data, np.zeros(frames-len(out_data), dtype=np.int16)))
             return (out_data, flag)
         else:
             # we need to play more to make sure everything is played!
@@ -639,33 +650,33 @@
     def _callback_sounddevice(self, out_data, frames, time_info, status):
         """Callback for sounddevice for supplying output with data."""
         if status:
             print(status)
         if self.index < len(self.data):
             ndata = len(self.data) - self.index
             if ndata >= frames :
-                if len(self.data.shape) <= 1:
+                if self.data.ndim <= 1:
                     out_data[:,0] = self.data[self.index:self.index+frames]
                 else:
                     out_data[:, :] = self.data[self.index:self.index+frames, :]
                 self.index += frames
             else:
-                if len(self.data.shape) <= 1:
+                if self.data.ndim <= 1:
                     out_data[:ndata, 0] = self.data[self.index:]
                     out_data[ndata:, 0] = np.zeros(frames-ndata, dtype=np.int16)
                 else:
                     out_data[:ndata, :] = self.data[self.index:, :]
                     out_data[ndata:, :] = np.zeros((frames-ndata, self.channels),
                                                    dtype=np.int16)
                 self.index += frames
         else:
             # we need to play more to make sure everything is played!
             # This is because of an ALSA bug and might be fixed in newer versions,
             # see http://music.columbia.edu/pipermail/portaudio/2012-May/013959.html
-            if len(self.data.shape) <= 1:
+            if self.data.ndim <= 1:
                 out_data[:, 0] = np.zeros(frames, dtype=np.int16)
             else:
                 out_data[:, :] = np.zeros((frames, self.channels), dtype=np.int16)
             self.index += frames
             if self.index >= len(self.data) + 2*self.latency:
                 raise sounddevice.CallbackStop
         if not self.run:
@@ -1299,15 +1310,15 @@
             mod = True
         else:
             break
 
     if help:
         print('')
         print('Usage:')
-        print('  python -m audioio.playaudio [-m <module>]')
+        print('  python -m src.audioio.playaudio [-m <module>]')
         print('  -m: audio module to be used')
         return
         
     demo()
 
             
 if __name__ == "__main__":
```

### Comparing `audioio-2.0.0/audioio/riffmetadata.py` & `audioio-2.1.0/src/audioio/riffmetadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,25 +19,22 @@
 list keys, but these keys are restricted to four characters and the
 INFO list chunk does also not allow for hierarchical metadata. The
 other metadata chunks, in particular the BEXT chunk, cannot be
 extended. With standard chunks, not all types of metadata can be
 stored.
 
 The [GUANO (Grand Unified Acoustic Notation
-Ontology)](https://github.com/riggsd/guano-spec), designed for bat
-acoustic recordings, has some standard ontologies that are of much
-more interest in scientific context, and also allows for
-extensions. This seems to be a good solution for some settings.
-
-Here, we add support for a novel odML chunk, that allows to store
-nested dictionaries of key-value pairs without any restrictions on the
-keys. The primary goal of the [odML data
-model](https://doi.org/10.3389/fninf.2011.00016) is to facilitate the
-immediate storage of all available metadata without the need to update
-an XML schema or terminology first.
+Ontology)](https://github.com/riggsd/guano-spec), primarily designed
+for bat acoustic recordings, has some standard ontologies that are of
+much more interest in scientific context.  In addition, GUANO allows
+for extensions with arbitray nested keys and string encoded values.
+In that respect it is a well defined and easy to handle serialization
+of the [odML data model](https://doi.org/10.3389/fninf.2011.00016).
+We use GUANO to write all metadata that do not fit into the INFO, BEXT
+or IXML chunks into a WAVE file.
 
 To interface the various ways to store and read metadata of RIFF
 files, the `riffmetadata` module simply uses nested dictionaries.  The
 keys are always strings. Values are strings or integers for key-value
 pairs. Value strings can also be numbers followed by a unit. Values
 can also be dictionaries for defining subsections of key-value
 pairs. The dictionaries can be nested to arbitrary depth.
@@ -46,22 +43,22 @@
 chunk. It checks for a key "INFO" with a flat dictionary of key value
 pairs. It then translates all keys of this dictionary using the
 `info_tags` mapping. If all the resulting keys have no more than four
 characters and there are no subsections, then an INFO list chunk is
 written. If no "INFO" key exists, then with the same procedure all
 elements of the provided metadata are checked for being valid INFO
 tags, and on success an INFO list chunk is written. Then, in similar
-ways, `write_wave()` tries to assemble valid BEXT, iXML, and GUANO
-chunks, based on the tags in `bext_tags` abd `ixml_tags`. All
-remaining metadata are then stored in an ODML chunk.
-
-When reading metadata from a RIFF file, INFO, BEXT, iXML, and GUANO
-chunks are returned as subsections with the respective keys. Metadata
-from an odML chunk are stored directly in the metadata dictionary
-without marking them as odML.
+ways, `write_wave()` tries to assemble valid BEXT and iXML chunks,
+based on the tags in `bext_tags` abd `ixml_tags`. All remaining
+metadata are then stored in an GUANO chunk.
+
+When reading metadata from a RIFF file, INFO, BEXT and iXML chunks are
+returned as subsections with the respective keys. Metadata from an
+GUANO chunk are stored directly in the metadata dictionary without
+marking them as GUANO.
 
 ## Markers
 
 A number of different chunk types exist for handling markers or cues
 that mark specific events or regions in the audio data. In the end,
 each marker has a position, a span, a label, and a text.  Position,
 and span are handled with 1-D or 2-D arrays of ints, where each row is
@@ -84,38 +81,39 @@
 - `append_riff()`: append metadata and markers to an existing RIFF file.
 
 ## Helper functions for reading RIFF and WAVE files
 
 - `read_chunk_tags()`: read tags of all chunks contained in a RIFF file.
 - `read_riff_header()`: read and check the RIFF file header.
 - `skip_chunk()`: skip over unknown RIFF chunk.
+- `read_format_chunk()`: read format chunk.
 - `read_info_chunks()`: read in meta data from info list chunk.
 - `read_bext_chunk()`: read in metadata from the broadcast-audio extension chunk.
 - `read_ixml_chunk()`: read in metadata from an IXML chunk.
 - `read_guano_chunk()`: read in metadata from a GUANO chunk.
-- `read_odml_chunk()`: read in metadata from an odml chunk.
-- `read_cue_chunk()`: read in marker ids and positions from cue chunk.
+- `read_cue_chunk()`: read in marker positions from cue chunk.
 - `read_playlist_chunk()`: read in marker spans from playlist chunk.
 - `read_adtl_chunks()`: read in associated data list chunks.
+- `read_lbl_chunk()`: read in marker positions, spans, labels, and texts from lbl chunk.
 
 ## Helper functions for writing RIFF and WAVE files
 
 - `write_riff_chunk()`: write RIFF file header.
 - `write_filesize()`: write the file size into the RIFF file header.
 - `write_chunk_name()`: change the name of a chunk.
 - `write_format_chunk()`: write format chunk.
 - `write_data_chunk()`: write data chunk.
 - `write_info_chunk()`: write metadata to LIST INFO chunk.
 - `write_bext_chunk()`: write metadata to BEXT chunk.
 - `write_ixml_chunk()`: write metadata to iXML chunk.
 - `write_guano_chunk()`: write metadata to GUANO chunk.
-- `write_odml_chunk()`: write metadata to ODML chunk.
 - `write_cue_chunk()`: write marker positions to cue chunk.
 - `write_playlist_chunk()`: write marker spans to playlist chunk.
 - `write_adtl_chunks()`: write associated data list chunks.
+- `write_lbl_chunk()`: write marker positions, spans, labels, and texts to lbl chunk.
 
 ## Demo
 
 - `demo()`: print metadata and marker list of RIFF/WAVE file.
 - `main()`: call demo with command line arguments.
 
 ## Descriptions of the RIFF/WAVE file format
@@ -136,15 +134,15 @@
 import io
 import os
 import sys
 import warnings
 import struct
 import numpy as np
 import xml.etree.ElementTree as ET
-from .audiometadata import flatten_metadata, unflatten_metadata
+from .audiometadata import flatten_metadata, unflatten_metadata, find_key
 
 
 info_tags = dict(AGES='Rated',
                  CMNT='Comment',
                  CODE='EncodedBy',
                  COMM='Comments',
                  DIRC='Directory',
@@ -473,14 +471,39 @@
         sf.seek(size, os.SEEK_CUR)
     if file_pos is None:
         sf.close()
     else:
         sf.seek(file_pos, os.SEEK_SET)
     return tags
     
+
+def read_format_chunk(sf):
+    """Read format chunk.
+
+    Parameters
+    ----------
+    sf: stream
+        File stream for reading FMT chunk.
+
+    Returns
+    -------
+    channels: int
+        Number of channels.
+    samplerate: float
+        Sampling rate (frames per time) in Hertz.
+    bits: int
+        Bit resolution.
+    """
+    size = struct.unpack('<I', sf.read(4))[0]
+    size += size % 2
+    ccode, channels, samplerate, byterate, blockalign, bits = struct.unpack('<HHIIHH', sf.read(16))
+    if size > 16:
+        sf.read(size - 16)
+    return channels, float(samplerate), bits
+
             
 def read_info_chunks(sf, store_empty):
     """Read in meta data from info list chunk.
 
     The variable `info_tags` is used to map the 4 character tags to
     human readable key names.
 
@@ -501,18 +524,24 @@
     """
     md = {}
     list_size = struct.unpack('<I', sf.read(4))[0]
     list_type = sf.read(4).decode('latin-1').upper()
     list_size -= 4
     if list_type == 'INFO':
         while list_size >= 8:
-            key = sf.read(4).decode('latin-1').rstrip(' \x00')
+            key = sf.read(4).decode('ascii').rstrip(' \x00')
             size = struct.unpack('<I', sf.read(4))[0]
             size += size % 2
-            value = sf.read(size).decode('latin-1').rstrip(' \x00')
+            bs = sf.read(size)
+            x = np.frombuffer(bs, dtype=np.uint8)
+            if np.sum((x >= 0x80) & (x <= 0x9f)) > 0:
+                s = bs.decode('windows-1252')
+            else:
+                s = bs.decode('latin1')
+            value = s.rstrip(' \x00\x02')
             list_size -= 8 + size
             if key in info_tags:
                 key = info_tags[key]
             if value or store_empty:
                 md[key] = value
     if list_size > 0:  # finish or skip
         sf.seek(list_size, os.SEEK_CUR)
@@ -549,58 +578,58 @@
         - 'UMID': unique material identifier.
         - 'LoudnessValue': integrated loudness value.
         - 'LoudnessRange':  loudness range.
         - 'MaxTruePeakLevel': maximum true peak value in dBTP.
         - 'MaxMomentaryLoudness': highest value of the momentary loudness level.
         - 'MaxShortTermLoudness': highest value of the short-term loudness level.
         - 'Reserved': 180 bytes reserved for extension.
-        - 'CodingHistory': description of coding processed applied to the audio data.
+        - 'CodingHistory': description of coding processed applied to the audio data, with comma separated subfields: "A=" coding algorithm, e.g. PCM, "F=" sampling rate in Hertz, "B=" bit-rate for MPEG files, "W=" word length in bits, "M=" mono, stereo, dual-mono, joint-stereo, "T=" free text. 
     """
     md = {}
     size = struct.unpack('<I', sf.read(4))[0]
     size += size % 2
-    s = sf.read(256).decode('latin-1').rstrip(' \x00')
+    s = sf.read(256).decode('ascii').strip(' \x00')
     if s or store_empty:
         md['Description'] = s
-    s = sf.read(32).decode('latin-1').rstrip(' \x00')
+    s = sf.read(32).decode('ascii').strip(' \x00')
     if s or store_empty:
         md['Originator'] = s
-    s = sf.read(32).decode('latin-1').rstrip(' \x00')
+    s = sf.read(32).decode('ascii').strip(' \x00')
     if s or store_empty:
         md['OriginatorReference'] = s
-    s = sf.read(10).decode('latin-1').rstrip(' \x00')
+    s = sf.read(10).decode('ascii').strip(' \x00')
     if s or store_empty:
         md['OriginationDate'] = s
-    s = sf.read(8).decode('latin-1').rstrip(' \x00')
+    s = sf.read(8).decode('ascii').strip(' \x00')
     if s or store_empty:
         md['OriginationTime'] = s
     reference, version = struct.unpack('<QH', sf.read(10))
     if reference > 0 or store_empty:
         md['TimeReference'] = reference
     if version > 0 or store_empty:
         md['Version'] = version
-    s = sf.read(64).decode('latin-1').rstrip(' \x00')
+    s = sf.read(64).decode('ascii').strip(' \x00')
     if s or store_empty:
         md['UMID'] = s
     lvalue, lrange, peak, momentary, shortterm = struct.unpack('<hhhhh', sf.read(10))
     if lvalue > 0 or store_empty:
         md['LoudnessValue'] = lvalue
     if lrange > 0 or store_empty:
         md['LoudnessRange'] = lrange
     if peak > 0 or store_empty:
         md['MaxTruePeakLevel'] = peak
     if momentary > 0 or store_empty:
         md['MaxMomentaryLoudness'] = momentary
     if shortterm > 0 or store_empty:
         md['MaxShortTermLoudness'] = shortterm
-    s = sf.read(180).decode('latin-1').rstrip(' \x00')
+    s = sf.read(180).decode('ascii').strip(' \x00')
     if s or store_empty:
         md['Reserved'] = s
     size -= 256 + 32 + 32 + 10 + 8 + 8 + 2 + 64 + 10 + 180
-    s = sf.read(size).decode('latin-1').rstrip(' \x00\n\r')
+    s = sf.read(size).decode('ascii').strip(' \x00\n\r')
     if s or store_empty:
         md['CodingHistory'] = s
     return md
 
 
 def read_ixml_chunk(sf, store_empty=True):
     """Read in metadata from an IXML chunk.
@@ -639,106 +668,64 @@
     root = ET.fromstring(xmls)
     md = {root.tag: parse_ixml(root, store_empty)}
     if len(md) == 1 and 'BWFXML' in md:
         md = md['BWFXML']
     return md
 
 
-def read_odml_chunk(sf, store_empty=True):
-    """Read in metadata from an odml chunk.
-
-    For storing any type of nested key-value pairs we define a new 
-    odml chunk holding the metadata as XML according to the odML data model.
-    For a description of odML see https://doi.org/10.3389/fninf.2011.00016 and
-    https://github.com/G-Node/python-odml
-    
-    Parameters
-    ----------
-    sf: stream
-        File stream of RIFF file.
-    store_empty: bool
-        If `False` do not add meta data with empty values.
-
-    Returns
-    -------
-    metadata: nested dict
-        Dictionary with key-value pairs.
-    """
-
-    def parse_odml(element, store_empty=True):
-        md = {}
-        for e in element:
-            if e.tag == 'Section':
-                md[e.attrib['name']] = parse_odml(e, store_empty)
-            elif e.tag == 'Property':
-                v = ''
-                if len(e) > 0 and e[0].tag == 'Value' and 'value' in e[0].attrib:
-                    v = e[0].attrib['value']
-                if len(v) > 0 or store_empty:
-                    md[e.attrib['name']] = v
-        return md
-
-    size = struct.unpack('<I', sf.read(4))[0]
-    size += size % 2
-    xmls = sf.read(size).decode('latin-1').rstrip(' \x00')
-    root = ET.fromstring(xmls)
-    md = {root.tag: parse_odml(root, store_empty)}
-    if len(md) == 1 and 'odML' in md:
-        md = md['odML']
-    return md
-
-
-def read_guano_chunk(sf, store_empty=True):
+def read_guano_chunk(sf):
     """Read in metadata from a GUANO chunk.
 
     GUANO is the Grand Unified Acoustic Notation Ontology, an
     extensible, open format for embedding metadata within bat acoustic
     recordings. See https://github.com/riggsd/guano-spec for details.
+
+    The GUANO specification allows for the inclusion of arbitrary
+    nested keys and string encoded values. In that respect it is a
+    well defined and easy to handle serialization of the [odML data
+    model](https://doi.org/10.3389/fninf.2011.00016).
     
     Parameters
     ----------
     sf: stream
         File stream of RIFF file.
-    store_empty: bool
-        If `False` do not add meta data with empty values.
 
     Returns
     -------
     metadata: nested dict
         Dictionary with key-value pairs.
+
     """
     md = {}
     size = struct.unpack('<I', sf.read(4))[0]
     size += size % 2
     for line in io.StringIO(sf.read(size).decode('utf-8')):
         ss = line.split(':')
         if len(ss) > 1:
-            md[ss[0].strip()] = ss[1].strip().replace(r'\n', '\n')
-        elif store_empty:
-            md[ss[0].strip()] = ''
+            md[ss[0].strip()] = ':'.join(ss[1:]).strip().replace(r'\n', '\n')
     return unflatten_metadata(md, '|')
 
     
 def read_cue_chunk(sf):
-    """Read in marker ids and positions from cue chunk.
+    """Read in marker positions from cue chunk.
     
     See https://www.recordingblogs.com/wiki/cue-chunk-of-a-wave-file
 
     Parameters
     ----------
     sf: stream
         File stream of RIFF file.
 
     Returns
     -------
     locs: 2-D array of ints
         Each row is a marker with unique identifier in the first column,
         position in the second column, and span in the third column.
         The cue chunk does not encode spans, so the third column is
-        initilazied with zeros.
+        initialized with zeros.
     """
     locs = []
     size, n = struct.unpack('<II', sf.read(8))
     for c in range(n):
         cpid, cppos = struct.unpack('<II', sf.read(8))
         datachunkid = sf.read(4).decode('latin-1').rstrip(' \x00').upper()
         chunkstart, blockstart, offset = struct.unpack('<III', sf.read(12))
@@ -833,14 +820,79 @@
                 sf.read(size)
             list_size -= 12 + size
     if list_size > 0:  # finish or skip
         sf.seek(list_size, os.SEEK_CUR)
     return labels
 
 
+def read_lbl_chunk(sf, samplerate):
+    """Read in marker positions, spans, labels, and texts from lbl chunk.
+    
+    The proprietary LBL chunk is specific to wave files generated by
+    [AviSoft](www.avisoft.com) products.
+
+    The labels (first column of `labels`) have special meanings.
+    Markers with a span (a section label in the terminology of
+    AviSoft) can be arranged in three levels when displayed:
+
+    - "M": layer 1, the top level section
+    - "N": layer 2, sections below layer 1
+    - "O": layer 3, sections below layer 2
+    - "P": total, section start and end are displayed with two vertical lines.
+
+    All other labels mark single point labels with a time and a
+    frequency (that we here discard). See also
+    https://www.avisoft.com/Help/SASLab/menu_main_tools_labels.htm
+    
+    Parameters
+    ----------
+    sf: stream
+        File stream of RIFF file.
+    samplerate: float
+        Sampling rate of the data in Hertz.
+
+    Returns
+    -------
+    locs: 2-D array of ints
+        Each row is a marker with unique identifier (simply integers
+        enumerating the markers) in the first column, position in the
+        second column, and span in the third column.
+    labels: 2-D array of string objects
+        Labels (first column) and texts (second column) for
+        each marker (rows).
+
+    """
+    size = struct.unpack('<I', sf.read(4))[0]
+    nn = size // 65
+    locs = np.zeros((nn, 3), dtype=int)
+    labels = np.zeros((nn, 2), dtype=object)
+    n = 0
+    for c in range(nn):
+        line = sf.read(65).decode('ascii')
+        fields = line.split('\t')
+        if len(fields) >= 4:
+            labels[n,0] = fields[3].strip()
+            labels[n,1] = fields[2].strip()
+            start_idx = int(np.round(float(fields[0].strip('\x00'))*samplerate))
+            end_idx = int(np.round(float(fields[1].strip('\x00'))*samplerate))
+            locs[n,0] = n
+            locs[n,1] = start_idx
+            if labels[n,0] in 'MNOP':
+                locs[n,2] = end_idx - start_idx
+            else:
+                locs[n,2] = 0
+            n += 1
+        else:
+            # the first 65 bytes are a title string that applies to
+            # the whole wave file that can be set from the AVISoft
+            # software. The recorder leave this empty.
+            pass
+    return locs[:n,:], labels[:n,:]
+
+
 def metadata_riff(filepath, store_empty=False):
     """Read metadata from a RIFF/WAVE file.
 
     Parameters
     ----------
     filepath: string or file handle
         The RIFF file.
@@ -854,16 +906,15 @@
         dictionaries are always strings.  If the corresponding
         values are dictionaries, then the key is the section name
         of the metadata contained in the dictionary. All other
         types of values are values for the respective key. In
         particular they are strings, or list of strings. But other
         simple types like ints or floats are also allowed.
         First level contains sections of meta data
-        (e.g. keys 'INFO', 'BEXT', 'IXML', 'GUANO', values are
-        dictionaries).
+        (e.g. keys 'INFO', 'BEXT', 'IXML', values are dictionaries).
 
     Raises
     ------
     ValueError
         Not a RIFF file.
 
     Examples
@@ -896,19 +947,15 @@
             if len(md) > 0:
                 meta_data['BEXT'] = md
         elif chunk == 'IXML':
             md = read_ixml_chunk(sf, store_empty)
             if len(md) > 0:
                 meta_data['IXML'] = md
         elif chunk == 'GUAN':
-            md = read_guano_chunk(sf, store_empty)
-            if len(md) > 0:
-                meta_data['GUANO'] = md
-        elif chunk == 'ODML':
-            md = read_odml_chunk(sf, store_empty)
+            md = read_guano_chunk(sf)
             if len(md) > 0:
                 meta_data.update(md)
         else:
             skip_chunk(sf)
     if file_pos is None:
         sf.close()
     else:
@@ -951,25 +998,30 @@
     sf = filepath
     file_pos = None
     if hasattr(filepath, 'read'):
         file_pos = sf.tell()
         sf.seek(0, os.SEEK_SET)
     else:
         sf = open(filepath, 'rb')
+    samplerate = None
     locs = np.zeros((0, 3), dtype=int)
     labels = np.zeros((0, 2), dtype=object)
     fsize = read_riff_header(sf)
     while (sf.tell() < fsize - 8):
         chunk = sf.read(4).decode('latin-1').upper()
-        if chunk == 'CUE ':
+        if chunk == 'FMT ':
+            samplerate = read_format_chunk(sf)[1]
+        elif chunk == 'CUE ':
             locs = read_cue_chunk(sf)
         elif chunk == 'PLST':
             read_playlist_chunk(sf, locs)
         elif chunk == 'LIST':
             labels = read_adtl_chunks(sf, locs, labels)
+        elif chunk == 'LBL ':
+            locs, labels = read_lbl_chunk(sf, samplerate)
         else:
             skip_chunk(sf)
     if file_pos is None:
         sf.close()
     else:
         sf.seek(file_pos, os.SEEK_SET)
     # sort markers according to their position:
@@ -1142,15 +1194,15 @@
     -------
     n: int
         Number of bytes written to the stream.
     keys_written: list of str
         Keys written to the INFO chunk.
 
     """
-    if metadata is None or len(metadata) == 0:
+    if not metadata:
         return 0, []
     is_info = False
     if 'INFO' in metadata:
         metadata = metadata['INFO']
         is_info = True
     tags = {v: k for k, v in info_tags.items()}
     n = 0
@@ -1158,15 +1210,15 @@
         kn = tags.get(k, k)
         if len(kn) > 4:
             if is_info:
                 warnings.warn(f'no 4-character info tag for key "{k}" found.')
             return 0, []
         if isinstance(metadata[k], dict):
             if is_info:
-                warnings.warn(f'value of info tag for key "{k}" must be a string.')
+                warnings.warn(f'value of key "{k}" in INFO chunk cannot be a dictionary.')
             return 0, []
         v = str(metadata[k])
         n += 8 + len(v) + len(v) % 2
     df.write(b'LIST')
     df.write(struct.pack('<I', n + 4))
     df.write(b'INFO')
     keys_written = []
@@ -1203,43 +1255,45 @@
     -------
     n: int
         Number of bytes written to the stream.
     keys_written: list of str
         Keys written to the BEXT chunk.
 
     """
-    if metadata is None or len(metadata) == 0 or not 'BEXT' in metadata:
+    if not metadata or not 'BEXT' in metadata:
         return 0, []
     metadata = metadata['BEXT']
     for k in metadata:
         if not k in bext_tags:
             warnings.warn(f'no bext tag for key "{k}" found.')
             return 0, []
     n = 0
     for k in bext_tags:
         n += bext_tags[k]
-    ch = metadata.get('CodingHistory', '').encode('latin-1')
-    nch = len(ch) + len(ch) % 2 + 2
+    ch = metadata.get('CodingHistory', '').encode('ascii')
+    if len(ch) >= 2 and ch[-2:] != '\r\n':
+        ch += b'\r\n'
+    nch = len(ch) + len(ch) % 2
     n += nch
     df.write(b'BEXT')
     df.write(struct.pack('<I', n))
     for k in bext_tags:
         bn = bext_tags[k]
         if bn == 2:
             v = metadata.get(k, '0')
             df.write(struct.pack('<H', int(v)))
         elif bn == 8 and k == 'TimeReference':
             v = metadata.get(k, '0')
             df.write(struct.pack('<Q', int(v)))
         elif bn == 0:
             df.write(ch)
-            df.write(b'\n\r' + bytes(nch - len(ch) - 2))
+            df.write(bytes(nch - len(ch)))
         else:
-            v = metadata.get(k, '').encode('latin-1')
-            df.write(v + bytes(bn - len(v)))
+            v = metadata.get(k, '').encode('ascii')
+            df.write(v[:bn] + bytes(bn - len(v)))
     return 8 + n, ['BEXT']
 
 
 def write_ixml_chunk(df, metadata, keys_written=None):
     """Write metadata to iXML chunk.
 
     If `metadata` contains an IXML key with valid IXML tags (one of
@@ -1278,19 +1332,19 @@
     def build_xml(node, metadata):
         kw = []
         for k in metadata:
             e = ET.SubElement(node, k)
             if isinstance(metadata[k], dict):
                 build_xml(e, metadata[k])
             else:
-                e.text = str(metadata[k]).replace('\n', '.')
+                e.text = str(metadata[k])
             kw.append(k)
         return kw
 
-    if metadata is None or len(metadata) == 0:
+    if not metadata:
         return 0, []
     md = metadata
     if keys_written:
         md = {k: metadata[k] for k in metadata if not k in keys_written}
     if len(md) == 0:
         return 0, []
     has_ixml = False
@@ -1309,121 +1363,70 @@
     df.write(b'IXML')
     df.write(struct.pack('<I', len(bs)))
     df.write(bs)
     return 8 + len(bs), ['IXML'] if has_ixml else kw
 
 
 def write_guano_chunk(df, metadata, keys_written=None):
-    """Write GUANO metadata to guan chunk.
+    """Write metadata to guan chunk.
 
     GUANO is the Grand Unified Acoustic Notation Ontology, an
     extensible, open format for embedding metadata within bat acoustic
     recordings. See https://github.com/riggsd/guano-spec for details.
 
-    If `metadata` contains a GUANO key, then the content of this key
-    is written as a GUANO chunk.
+    The GUANO specification allows for the inclusion of arbitrary
+    nested keys and string encoded values. In that respect it is a
+    well defined and easy to handle serialization of the [odML data
+    model](https://doi.org/10.3389/fninf.2011.00016).
+
+    This will write *all* metadata that are not in `keys_written`.
 
     Parameters
     ----------
     df: stream
-        File stream for writing odml chunk.
+        File stream for writing guano chunk.
     metadata: nested dict
         Metadata as key-value pairs. Values can be strings, integers,
         or dictionaries.
     keys_written: list of str
         Keys that have already written to INFO, BEXT, IXML chunk.
 
     Returns
     -------
     n: int
         Number of bytes written to the stream.
     keys_written: list of str
-        Keys written to the GUANO chunk: `['GUANO']`.
+        Top-level keys written to the GUANO chunk.
 
     """
-    if metadata is None or len(metadata) == 0:
+    if not metadata:
         return 0, []
-    if not 'GUANO' in metadata:
+    md = metadata
+    if keys_written:
+        md = {k: metadata[k] for k in metadata if not k in keys_written}
+    if len(md) == 0:
         return 0, []
-    fmd = flatten_metadata(metadata['GUANO'], True, '|')
+    fmd = flatten_metadata(md, True, '|')
     for k in fmd:
-        fmd[k] = fmd[k].replace('\n', r'\n')
-    # TODO make sure we have 'GUANO|Version' at the beginning
+        if isinstance(fmd[k], str):
+            fmd[k] = fmd[k].replace('\n', r'\n')
     sio = io.StringIO()
+    m, k = find_key(md, 'GUANO.Version')
+    if k is None:
+       sio.write('GUANO|Version:1.0\n')
     for k in fmd:
        sio.write(f'{k}:{fmd[k]}\n')
     bs = sio.getvalue().encode('utf-8')
     if len(bs) % 2 == 1:
-        bs += bytes(1)
+        bs += b' '
     n = len(bs)
     df.write(b'guan')
     df.write(struct.pack('<I', n))
     df.write(bs)
-    return n, ['GUANO']
-
-
-def write_odml_chunk(df, metadata, keys_written=None):
-    """Write metadata to ODML chunk.
-
-    For storing any type of nested key-value pairs we define a new 
-    odml chunk holding the metadata as XML according to the odML data model.
-    For odML see https://doi.org/10.3389/fninf.2011.00016 and
-    https://github.com/G-Node/python-odml
-
-    This will write *all* metadata that are not in `keys_written`.
-
-    Parameters
-    ----------
-    df: stream
-        File stream for writing odml chunk.
-    metadata: nested dict
-        Metadata as key-value pairs. Values can be strings, integers,
-        or dictionaries.
-    keys_written: list of str
-        Keys that have already written to INFO, BEXT, IXML, GUANO chunk.
-
-    Returns
-    -------
-    n: int
-        Number of bytes written to the stream.
-    keys_written: list of str
-        Keys written to the IXML chunk.
-    """
-    def build_odml(node, metadata):
-        kw = []
-        for k in metadata:
-            if isinstance(metadata[k], dict):
-                sec = ET.SubElement(node, 'Section')
-                sec.attrib = dict(name=k)
-                build_odml(sec, metadata[k])
-            else:
-                prop = ET.SubElement(node, 'Property')
-                prop.attrib = dict(name=k)
-                value = ET.SubElement(prop, 'Value')
-                value.attrib = dict(value=str(metadata[k]).replace('\n', '.'))
-            kw.append(k)
-        return kw
-
-    if metadata is None or len(metadata) == 0:
-        return 0, []
-    md = metadata
-    if keys_written:
-        md = {k: metadata[k] for k in metadata if not k in keys_written}
-    if len(md) == 0:
-        return 0, []
-    root = ET.Element('odML')
-    kw = build_odml(root, md)
-    bs = bytes(ET.tostring(root, xml_declaration=True,
-                           short_empty_elements=False))
-    if len(bs) % 2 == 1:
-        bs += bytes(1)
-    df.write(b'odml')
-    df.write(struct.pack('<I', len(bs)))
-    df.write(bs)
-    return 8 + len(bs), kw
+    return n, list(md)
 
 
 def write_cue_chunk(df, locs):
     """Write marker positions to cue chunk.
 
     See https://www.recordingblogs.com/wiki/cue-chunk-of-a-wave-file
 
@@ -1543,14 +1546,90 @@
                     df.write(b'ltxt')
                     df.write(struct.pack('<III', 20 + n, i, span))
                     df.write(struct.pack('<IHHHH', 0, 0, 0, 0, 0))
                     df.write(f'{t:<{n}s}'.encode('latin-1'))
     return 8 + size
 
 
+def write_lbl_chunk(df, locs, labels, samplerate):
+    """Write marker positions, spans, labels, and texts to lbl chunk.
+    
+    The proprietary LBL chunk is specific to wave files generated by
+    [AviSoft](www.avisoft.com) products.
+
+    The labels (first column of `labels`) have special meanings.
+    Markers with a span (a section label in the terminology of
+    AviSoft) can be arranged in three levels when displayed:
+
+    - "M": layer 1, the top level section
+    - "N": layer 2, sections below layer 1
+    - "O": layer 3, sections below layer 2
+    - "P": total, section start and end are displayed with two vertical lines.
+
+    All other labels mark single point labels with a time and a
+    frequency (that we here discard). See also
+    https://www.avisoft.com/Help/SASLab/menu_main_tools_labels.htm
+
+    If a marker has a span, and its label is not one of "M", "N", "O", or "P",
+    then its label is set to "M".
+    If a marker has no span, and its label is one of "M", "N", "O", or "P",
+    then its label is set to "a".
+
+    Parameters
+    ----------
+    df: stream
+        File stream for writing lbl chunk.
+    locs: None or 2-D array of ints
+        Positions (first column) and spans (optional second column)
+        for each marker (rows).
+    labels: None or 2-D array of string objects
+        Labels (first column) and texts (second column) for each marker (rows).
+    samplerate: float
+        Sampling rate of the data in Hertz.
+
+    Returns
+    -------
+    n: int
+        Number of bytes written to the stream.
+
+    """
+    if locs is None or len(locs) == 0:
+        return 0
+    size = (1 + len(locs)) * 65
+    df.write(b'LBL ')
+    df.write(struct.pack('<I', size))
+    # first empty entry (this is ment to be a title for the whole wave file):
+    df.write(b' ' * 63)
+    df.write(b'\r\n')
+    for k in range(len(locs)):
+        t0 = locs[k,0]/samplerate
+        t1 = t0
+        t1 += locs[k,1]/samplerate
+        ls = 'M' if locs[k,1] > 0 else 'a'
+        ts = ''
+        if labels is not None and len(labels) > k:
+            ls = labels[k,0]
+            if ls != 0 and len(ls) > 0:
+                ls = ls[0]
+                if ls in 'MNOP':
+                    if locs[k,1] == 0:
+                        ls = 'a'
+                else:
+                    if locs[k,1] > 0:
+                        ls = 'M'
+            ts = labels[k,1]
+            if ts == 0:
+                ts = ''
+        df.write(struct.pack('<14sc', f'{t0:e}'.encode('ascii'), b'\t'))
+        df.write(struct.pack('<14sc', f'{t1:e}'.encode('ascii'), b'\t'))
+        bs = f'{ts:31s}\t{ls}\r\n'.encode('ascii')
+        df.write(bs)
+    return 8 + size
+
+
 def append_metadata_riff(df, metadata):
     """Append metadata chunks to RIFF file.
 
     You still need to update the filesize by calling
     `write_filesize()`.
 
     Parameters
@@ -1564,15 +1643,15 @@
     Returns
     -------
     n: int
         Number of bytes written to the stream.
     tags: list of str
         Tag names of chunks written to audio file.
     """
-    if metadata is None or len(metadata) == 0:
+    if not metadata:
         return 0, []
     n = 0
     tags = []
     # metadata INFO chunk:
     nc, kw = write_info_chunk(df, metadata)
     if nc > 0:
         tags.append('LIST-INFO')
@@ -1585,29 +1664,25 @@
     kw.extend(bkw)
     # metadata IXML chunk:
     nc, xkw = write_ixml_chunk(df, metadata, kw)
     if nc > 0:
         tags.append('IXML')
     n += nc
     kw.extend(xkw)
-    # metadata GUANO chunk:
-    nc, bkw = write_guano_chunk(df, metadata)
+    # write remaining metadata to GUANO chunk:
+    nc, _ = write_guano_chunk(df, metadata, kw)
     if nc > 0:
         tags.append('GUAN')
     n += nc
     kw.extend(bkw)
-    # write remaining metadata to odML chunk:
-    nc, _ = write_odml_chunk(df, metadata, kw)
-    if nc > 0:
-        tags.append('ODML')
-    n += nc
     return n, tags
 
 
-def append_markers_riff(df, locs, labels=None):
+def append_markers_riff(df, locs, labels=None, samplerate=None,
+                        marker_hint='cue'):
     """Append marker chunks to RIFF file.
 
     You still need to update the filesize by calling
     `write_filesize()`.
 
     Parameters
     ----------
@@ -1615,14 +1690,20 @@
         File stream for writing metadata chunks.
     locs: None or 1-D or 2-D array of ints
         Marker positions (first column) and spans (optional second column)
         for each marker (rows).
     labels: None or 1-D or 2-D array of string objects
         Labels (first column) and texts (optional second column)
         for each marker (rows).
+    samplerate: float
+        Sampling rate of the data in Hertz, needed for storing markers
+        in seconds.
+    marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
 
     Returns
     -------
     n: int
         Number of bytes written to the stream.
     tags: list of str
         Tag names of chunks written to audio file.
@@ -1632,50 +1713,57 @@
     ValueError
         Encoding not supported.
     IndexError
         `locs` and `labels` differ in len.
     """
     if locs is None or len(locs) == 0:
         return 0, []
-    if not locs is None and not labels is None and \
-       len(locs) > 0 and len(labels) > 0 and len(labels) != len(locs):
+    if labels is not None and len(labels) > 0 and len(labels) != len(locs):
         raise IndexError(f'locs and labels must have same number of elements.')
     # make locs and labels 2-D:
     if not locs is None and locs.ndim == 1:
         locs = locs.reshape(-1, 1)
     if not labels is None and labels.ndim == 1:
         labels = labels.reshape(-1, 1)
     # sort markers according to their position:
-    if not locs is None and len(locs) > 0:
-        idxs = np.argsort(locs[:,0])
-        locs = locs[idxs,:]
-        if not labels is None and len(labels) > 0:
-            labels = labels[idxs,:]
+    idxs = np.argsort(locs[:,0])
+    locs = locs[idxs,:]
+    if not labels is None and len(labels) > 0:
+        labels = labels[idxs,:]
     n = 0
     tags = []
-    # write marker positions:
-    nc = write_cue_chunk(df, locs)
-    if nc > 0:
-        tags.append('CUE ')
-    n += nc
-    # write marker spans:
-    nc = write_playlist_chunk(df, locs)
-    if nc > 0:
-        tags.append('PLST')
-    n += nc
-    # write marker labels:
-    nc = write_adtl_chunks(df, locs, labels)
-    if nc > 0:
-        tags.append('LIST-ADTL')
-    n += nc
+    if marker_hint.lower() == 'cue':
+        # write marker positions:
+        nc = write_cue_chunk(df, locs)
+        if nc > 0:
+            tags.append('CUE ')
+        n += nc
+        # write marker spans:
+        nc = write_playlist_chunk(df, locs)
+        if nc > 0:
+            tags.append('PLST')
+        n += nc
+        # write marker labels:
+        nc = write_adtl_chunks(df, locs, labels)
+        if nc > 0:
+            tags.append('LIST-ADTL')
+        n += nc
+    elif marker_hint.lower() == 'lbl':
+        # write avisoft labels:
+        nc = write_lbl_chunk(df, locs, labels, samplerate)
+        if nc > 0:
+            tags.append('LBL ')
+        n += nc
+    else:
+        raise ValueError(f'marker_hint "{marker_hint}" not supported for storing markers')
     return n, tags
 
 
 def write_wave(filepath, data, samplerate, metadata=None, locs=None,
-               labels=None, encoding=None):
+               labels=None, encoding=None, marker_hint='cue'):
     """Write time series, metadata and markers to a WAVE file.
 
     Only 16 or 32bit PCM encoding is supported.
 
     Parameters
     ----------
     filepath: string
@@ -1693,15 +1781,18 @@
         for each marker (rows).
     labels: None or 1-D or 2-D array of string objects
         Labels (first column) and texts (optional second column)
         for each marker (rows).
     encoding: string or None
         Encoding of the data: 'PCM_32' or 'PCM_16'.
         If None or empty string use 'PCM_16'.
- 
+     marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
+
     Raises
     ------
     ValueError
         Encoding not supported.
     IndexError
         `locs` and `labels` differ in len.
 
@@ -1732,32 +1823,33 @@
     bits = 0
     if encoding == 'PCM_16':
         bits = 16
     elif encoding == 'PCM_32':
         bits = 32
     else:
         raise ValueError(f'file encoding {encoding} not supported')
-    if not locs is None and not labels is None and \
-       len(locs) > 0 and len(labels) > 0 and len(labels) != len(locs):
+    if locs is not None and len(locs) > 0 and \
+       labels is not None and len(labels) > 0 and len(labels) != len(locs):
         raise IndexError(f'locs and labels must have same number of elements.')
     # write WAVE file:
     with open(filepath, 'wb') as df:
         write_riff_chunk(df)
         if data.ndim == 1:
             write_format_chunk(df, 1, len(data), samplerate, bits)
         else:
             write_format_chunk(df, data.shape[1], data.shape[0],
                                samplerate, bits)
         append_metadata_riff(df, metadata)
-        append_markers_riff(df, locs, labels)
         write_data_chunk(df, data, bits)
+        append_markers_riff(df, locs, labels, samplerate, marker_hint)
         write_filesize(df)
 
 
-def append_riff(filepath, metadata=None, locs=None, labels=None):
+def append_riff(filepath, metadata=None, locs=None, labels=None,
+                samplerate=None, marker_hint='cue'):
     """Append metadata and markers to an existing RIFF file.
 
     Parameters
     ----------
     filepath: string
         Full path and name of the file to write.
     metadata: None or nested dict
@@ -1765,14 +1857,20 @@
         or dictionaries.
     locs: None or 1-D or 2-D array of ints
         Marker positions (first column) and spans (optional second column)
         for each marker (rows).
     labels: None or 1-D or 2-D array of string objects
         Labels (first column) and texts (optional second column)
         for each marker (rows).
+    samplerate: float
+        Sampling rate of the data in Hertz, needed for storing markers
+        in seconds.
+    marker_hint: str
+        - 'cue': store markers in cue and and adtl chunks.
+        - 'lbl': store markers in avisoft lbl chunk.
 
     Returns
     -------
     n: int
         Number of bytes written to the stream.
  
     Raises
@@ -1788,28 +1886,28 @@
     
     md = dict(Artist='underscore_')    # metadata
     append_riff('audio/file.wav', md)  # append them to existing audio file
     ```
     """
     if not filepath:
         raise ValueError('no file specified!')
-    if not locs is None and not labels is None and \
-       len(locs) > 0 and len(labels) > 0 and len(labels) != len(locs):
+    if locs is not None and len(locs) > 0 and \
+       labels is not None and len(labels) > 0 and len(labels) != len(locs):
         raise IndexError(f'locs and labels must have same number of elements.')
     # check RIFF file:
     chunks = read_chunk_tags(filepath)
     # append to RIFF file:
     n = 0
     with open(filepath, 'r+b') as df:
         tags = []
         df.seek(0, os.SEEK_END)
         nc, tgs = append_metadata_riff(df, metadata)
         n += nc
         tags.extend(tgs)
-        nc, tgs = append_markers_riff(df, locs, labels)
+        nc, tgs = append_markers_riff(df, locs, labels, samplerate, marker_hint)
         n += nc
         tags.extend(tgs)
         write_filesize(df)
         # blank out already existing chunks:
         for tag in chunks:
             if tag in tags:
                 if '-' in tag:
@@ -1831,15 +1929,15 @@
     def print_meta_data(meta_data, level=0):
         for sk in meta_data:
             md = meta_data[sk]
             if isinstance(md, dict):
                 print(f'{"":<{level*4}}{sk}:')
                 print_meta_data(md, level+1)
             else:
-                v = str(md).replace('\n', '.')
+                v = str(md).replace('\n', '.').replace('\r', '.')
                 print(f'{"":<{level*4}s}{sk:<20s}: {v}')
         
     # read meta data:
     meta_data = metadata_riff(filepath, store_empty=False)
     
     # print meta data:
     print()
@@ -1868,15 +1966,15 @@
     ----------
     args: list of strings
         Command line arguments as returned by sys.argv[1:]
     """
     if len(args) > 0 and (args[0] == '-h' or args[0] == '--help'):
         print()
         print('Usage:')
-        print('  python -m audioio.riffmetadata [--help] <audio/file.wav>')
+        print('  python -m src.audioio.riffmetadata [--help] <audio/file.wav>')
         print()
         return
 
     if len(args) > 0:
         demo(args[0])
     else:
         rate = 44100
```

### Comparing `audioio-2.0.0/audioio.egg-info/SOURCES.txt` & `audioio-2.1.0/src/audioio.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
-audioio/__init__.py
-audioio/audioconverter.py
-audioio/audioloader.py
-audioio/audiomarkers.py
-audioio/audiometadata.py
-audioio/audiomodules.py
-audioio/audiotools.py
-audioio/audiowriter.py
-audioio/playaudio.py
-audioio/riffmetadata.py
-audioio/version.py
-audioio.egg-info/PKG-INFO
-audioio.egg-info/SOURCES.txt
-audioio.egg-info/dependency_links.txt
-audioio.egg-info/entry_points.txt
-audioio.egg-info/requires.txt
-audioio.egg-info/top_level.txt
+src/audioio/__init__.py
+src/audioio/audioconverter.py
+src/audioio/audioloader.py
+src/audioio/audiomarkers.py
+src/audioio/audiometadata.py
+src/audioio/audiomodules.py
+src/audioio/audiotools.py
+src/audioio/audiowriter.py
+src/audioio/playaudio.py
+src/audioio/riffmetadata.py
+src/audioio/version.py
+src/audioio.egg-info/PKG-INFO
+src/audioio.egg-info/SOURCES.txt
+src/audioio.egg-info/dependency_links.txt
+src/audioio.egg-info/entry_points.txt
+src/audioio.egg-info/requires.txt
+src/audioio.egg-info/top_level.txt
 tests/test_audioconverter.py
 tests/test_audioloader.py
 tests/test_audiomarkers.py
 tests/test_audiometadata.py
 tests/test_audiomodules.py
 tests/test_audiotools.py
 tests/test_audiowriter.py
```

### Comparing `audioio-2.0.0/tests/test_audioconverter.py` & `audioio-2.1.0/tests/test_audioconverter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nose.tools import assert_equal, assert_greater, assert_greater_equal, assert_less, assert_raises
+import pytest
 import os
 import shutil
 import numpy as np
 import audioio.audioloader as al
 import audioio.audiowriter as aw
 import audioio.audioconverter as ac
 
@@ -22,24 +22,39 @@
 def test_main():
     filename = 'test.wav'
     filename1 = 'test1.wav'
     destfile = 'test2'
     destpath = 'test3'
     os.mkdir(destpath)
     write_audio_file(filename)
-    assert_raises(SystemExit, ac.main, '-h')
-    assert_raises(SystemExit, ac.main, '--help')
-    assert_raises(SystemExit, ac.main, '--version')
+    with pytest.raises(SystemExit):
+        ac.main()
+    with pytest.raises(SystemExit):
+        ac.main('-h')
+    with pytest.raises(SystemExit):
+        ac.main('--help')
+    with pytest.raises(SystemExit):
+        ac.main('--version')
     ac.main('-l')
     ac.main('-f', 'wav', '-l')
     ac.main('-f', 'wav', '-o', destfile, filename)
-    assert_raises(SystemExit, ac.main, '')
-    assert_raises(SystemExit, ac.main, '-f', 'xxx', '-l')
-    assert_raises(SystemExit, ac.main, '-f', 'xxx', '-o', destfile, filename)
-    assert_raises(SystemExit, ac.main, '-o', 'test.xxx', filename)
+    with pytest.raises(SystemExit):
+        ac.main('')
+    with pytest.raises(SystemExit):
+        ac.main('-f', 'xxx', '-l')
+    with pytest.raises(SystemExit):
+        ac.main('-f', 'xxx', '-o', destfile, filename)
+    with pytest.raises(SystemExit):
+        ac.main('-o', 'test.xxx', filename)
+    with pytest.raises(SystemExit):
+        ac.main('-f', 'xyz123', filename)
+    with pytest.raises(SystemExit):
+        ac.main(filename)
+    with pytest.raises(SystemExit):
+        ac.main('-o', filename, filename)
     ac.main('-o', destfile + '.wav', filename)
     ac.main('-f', 'wav', '-o', destfile, filename)
     ac.main('-u', '-f', 'wav', '-o', destfile, filename)
     ac.main('-u', '0.8', '-f', 'wav', '-o', destfile, filename)
     ac.main('-U', '0.8', '-f', 'wav', '-o', destfile, filename)
     ac.main('-s', '0.1', '-f', 'wav', '-o', destfile, filename)
     ac.main('-e', 'PCM_32', '-o', destfile + '.wav', filename)
@@ -49,48 +64,47 @@
         ac.main('-e', 'float', '-o', destfile + '.wav', filename)
     if 'OGG' in aw.available_formats():
         ac.main('-f', 'ogg', '-l')
         ac.main('-f', 'ogg', '-e', 'vorbis', '-o', destfile, filename)
         ac.main('-f', 'ogg', '-e', 'vorbis', filename)
         os.remove(filename.replace('.wav', '.ogg'))
         os.remove(destfile+'.ogg')
-    assert_raises(SystemExit, ac.main, '-f', 'xyz123', filename)
-    assert_raises(SystemExit, ac.main, filename)
-    assert_raises(SystemExit, ac.main, '-o', filename, filename)
-    assert_raises(SystemExit, ac.main)
     ac.main('-a', 'INFO.Artist=John Doe', '-o', destfile + '.wav', filename)
     ac.main('-r', 'Amplifier', '-o', destfile + '.wav', filename)
     write_audio_file(filename)
     write_audio_file(filename1, 4)
     ac.main('-c', '1', '-o', destfile + '.wav', filename1)
     ac.main('-c', '0-2', '-o', destfile + '.wav', filename1)
     ac.main('-c', '0-1,3', '-o', destfile + '.wav', filename1)
-    assert_raises(SystemExit, ac.main, '-o', destfile + '.wav', filename, filename1)
+    with pytest.raises(SystemExit):
+        ac.main('-o', destfile + '.wav', filename, filename1)
     write_audio_file(filename1, 2, 20000)
-    assert_raises(SystemExit, ac.main, '-o', destfile + '.wav', filename, filename1)
+    with pytest.raises(SystemExit):
+        ac.main('-o', destfile + '.wav', filename, filename1)
     write_audio_file(filename1)
-    assert_raises(SystemExit, ac.main, '-n', '1', '-o', destfile, filename, filename1)
+    with pytest.raises(SystemExit):
+        ac.main('-n', '1', '-o', destfile, filename, filename1)
     ac.main('-n', '1', '-f', 'wav', '-o', destfile, filename, filename1)
-    os.remove(os.path.join(destfile, filename))
-    os.remove(os.path.join(destfile, filename1))
-    os.rmdir(destfile)
+    shutil.rmtree(destfile)
     ac.main('-vv', '-o', destfile + '.wav', filename, filename1)
     xdata, xrate = al.load_audio(filename)
     n = len(xdata)
     xdata, xrate = al.load_audio(filename1)
     n += len(xdata)
     xdata, xrate = al.load_audio(destfile + '.wav')
-    assert_equal(len(xdata), n, 'len of merged files')
+    assert len(xdata) == n, 'len of merged files'
     md1 = al.metadata(filename)
+    md1['CodingHistory'] = 'A=PCM,F=44100,W=16,M=stereo,T=test.wav\nA=PCM,F=44100,W=16,M=stereo,T=test2.wav'
     md2 = al.metadata(destfile + '.wav')
-    assert_equal(md1, md2, 'metadata of merged files')
+    md2['CodingHistory'] = md2['CodingHistory'].replace('\r\n', '\n')
+    assert md1 == md2, 'metadata of merged files'
     ac.main('-d', '4', '-o', destfile + '.wav', filename)
     xdata, xrate = al.load_audio(filename)
     ydata, yrate = al.load_audio(destfile + '.wav')
-    assert_equal(len(ydata), len(xdata)//4, 'decimation data')
-    assert_equal(yrate*4, xrate, 'decimation rate')
+    assert len(ydata) == len(xdata)//4, 'decimation data'
+    assert yrate*4 == xrate, 'decimation rate'
     ac.main('-o', 'test{Num}.wav', filename)
     os.remove('test42.wav')
     os.remove(filename)
     os.remove(filename1)
     os.remove(destfile+'.wav')
     shutil.rmtree(destpath)
```

### Comparing `audioio-2.0.0/tests/test_audioloader.py` & `audioio-2.1.0/tests/test_audioloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nose.tools import assert_true, assert_false, assert_equal, assert_raises
+import pytest
 import os
 import numpy as np
 import audioio.audiowriter as aw
 import audioio.audioloader as al
 import audioio.audiomodules as am
 
 
@@ -28,26 +28,25 @@
         if lib in ['scipy.io.wavfile', 'pydub']:
             continue
         print('')
         print('check single frame access for module %s ...' % lib)
         am.select_module(lib)
         full_data, rate = al.load_audio(filename, verbose=4)
         with al.AudioLoader(filename, 5.0, 2.0, verbose=4) as data:
-            assert_false(np.any(np.abs(full_data[0] - data[0]) > tolerance), 'first frame access failed with %s module' % lib)
-            assert_false(np.any(np.abs(full_data[-1] - data[-1]) > tolerance), 'last frame access failed with %s module' % lib)
-            def access_end(n):
-                x = data[len(data)+n]
+            assert not np.any(np.abs(full_data[0] - data[0]) > tolerance), 'first frame access failed with %s module' % lib
+            assert not np.any(np.abs(full_data[-1] - data[-1]) > tolerance), 'last frame access failed with %s module' % lib
             for n in range(10):
-                assert_raises(IndexError, access_end, n)
+                with pytest.raises(IndexError):
+                    x = data[len(data)+n]
             failed = -1
             for inx in np.random.randint(-len(data), len(data), ntests):
                 if np.any(np.abs(full_data[inx] - data[inx]) > tolerance):
                     failed = inx
                     break
-            assert_true(failed < 0, 'single random frame access failed at index %d with %s module' % (failed, lib))
+            assert failed < 0, 'single random frame access failed at index %d with %s module' % (failed, lib)
     os.remove(filename)
     am.enable_module()
 
 
 def test_slice():
     am.enable_module()
     filename = 'test.wav'
@@ -59,25 +58,25 @@
             continue
         print('')
         print('random frame slice access for module %s' % lib)
         am.select_module(lib)
         full_data, rate = al.load_audio(filename, verbose=4)
         with al.AudioLoader(filename, 5.0, 2.0, verbose=4) as data:
             for n in range(5):
-                assert_false(np.any(np.abs(data[:n]-full_data[:n]) > tolerance), 'zero slice up to %d does not match' % n)
+                assert not np.any(np.abs(data[:n]-full_data[:n]) > tolerance), 'zero slice up to %d does not match' % n
             for n in range(1, 5):
-                assert_false(np.any(np.abs(data[:50:n]-full_data[:50:n]) > tolerance), 'step slice with step=%d does not match' % n)
+                assert not np.any(np.abs(data[:50:n]-full_data[:50:n]) > tolerance), 'step slice with step=%d does not match' % n
             for time in [0.1, 1.5, 2.0, 5.5, 8.0]:
                 nframes = int(time*data.samplerate)
                 failed = -1
                 for inx in np.random.randint(0, len(data)-nframes, ntests):
                     if np.any(np.abs(full_data[inx:inx+nframes] - data[inx:inx+nframes]) > tolerance):
                         failed = inx
                         break
-                assert_true(failed < 0, 'random frame slice access failed at index %d with nframes=%d and %s module' % (failed, nframes, lib))
+                assert failed < 0, 'random frame slice access failed at index %d with nframes=%d and %s module' % (failed, nframes, lib)
     os.remove(filename)
     am.enable_module()
 
 
 def test_forward():
     am.enable_module()
     filename = 'test.wav'
@@ -96,15 +95,15 @@
                 nframes = int(time*data.samplerate)
                 step = int(len(data)/nsteps)
                 failed = -1
                 for inx in range(0, len(data)-nframes, step):
                     if np.any(np.abs(full_data[inx:inx+nframes] - data[inx:inx+nframes]) > tolerance):
                         failed = inx
                         break
-                assert_true(failed < 0, 'frame slice access forward failed at index %d with nframes=%d and %s module' % (failed, nframes, lib))
+                assert failed < 0, 'frame slice access forward failed at index %d with nframes=%d and %s module' % (failed, nframes, lib)
     os.remove(filename)
     am.enable_module()
 
 
 def test_backward():
     am.enable_module()
     filename = 'test.wav'
@@ -124,15 +123,15 @@
                 step = int(len(data)/nsteps)
                 failed = -1
                 print('  check backward slice access...')
                 for inx in range(len(data)-nframes, 0, -step):
                     if np.any(np.abs(full_data[inx:inx+nframes] - data[inx:inx+nframes]) > tolerance):
                         failed = inx
                         break
-                assert_true(failed < 0, 'frame slice access backward failed at index %d with nframes=%d and %s module' % (failed, nframes, lib))
+                assert failed < 0, 'frame slice access backward failed at index %d with nframes=%d and %s module' % (failed, nframes, lib)
     os.remove(filename)
     am.enable_module()
 
 
 def test_negative():
     am.enable_module()
     filename = 'test.wav'
@@ -151,15 +150,15 @@
                 nframes = int(time*data.samplerate)
                 step = int(len(data)/nsteps)
                 failed = -1
                 for inx in range(0, len(data)-nframes, step):
                     if np.any(np.abs(full_data[-inx:-inx+nframes] - data[-inx:-inx+nframes]) > tolerance):
                         failed = -inx
                         break
-                assert_true(failed < 0, 'frame slice access backward with negative indices failed at index %d with nframes=%d and %s module' % (failed, nframes, lib))
+                assert failed < 0, 'frame slice access backward with negative indices failed at index %d with nframes=%d and %s module' % (failed, nframes, lib)
     os.remove(filename)
     am.enable_module()
 
 
 def test_multiple():
     am.enable_module()
     filename = 'test.wav'
@@ -184,117 +183,164 @@
                         offs = np.random.randint(len(data)-nframes)
                     failed = -1
                     for k in range(ntests):
                         inx = np.random.randint(0, nframes, n) + offs
                         if np.any(np.abs(full_data[inx] - data[inx]) > tolerance):
                             failed = 1
                             break
-                    assert_equal(failed, -1, ('multiple random frame access failed with %s module at indices ' % lib) + str(inx))
+                    assert failed == -1, ('multiple random frame access failed with %s module at indices ' % lib) + str(inx)
     os.remove(filename)
     am.enable_module()
 
 
 def test_modules():
     am.enable_module()
     filename = 'test.wav'
     write_audio_file(filename, 1.0)
     for lib, load_file in al.audio_loader_funcs:
         print(lib)
         am.disable_module(lib)
-        assert_raises(ImportError, load_file, filename)
+        with pytest.raises(ImportError):
+            load_file(filename)
         data = al.AudioLoader(verbose=4)
         load_funcs = {
             'soundfile': data.open_soundfile,
             'wavefile': data.open_wavefile,
             'audioread': data.open_audioread,
             'wave': data.open_wave,
             'ewave': data.open_ewave,
             }
         if lib not in load_funcs:
             continue
-        assert_raises(ImportError, load_funcs[lib], filename, 10.0, 2.0)
+        with pytest.raises(ImportError):
+            load_funcs[lib](filename, 10.0, 2.0)
         if am.select_module(lib):
             # check double opening:
             load_funcs[lib](filename)
             load_funcs[lib](filename)
             data.close()
     os.remove(filename)
     am.enable_module()
         
 
 def test_audio_files():
     am.enable_module()
-    assert_raises(ValueError, al.load_audio, '')
-    assert_raises(FileNotFoundError, al.load_audio, 'xxx.wav')
-    assert_raises(ValueError, al.AudioLoader, '')
-    assert_raises(FileNotFoundError, al.AudioLoader, 'xxx.wav')
+    with pytest.raises(ValueError):
+        al.load_audio('')
+    with pytest.raises(ValueError):
+        al.AudioLoader('')
+    with pytest.raises(FileNotFoundError):
+        al.load_audio('xxx.wav')
+    with pytest.raises(FileNotFoundError):
+        al.AudioLoader('xxx.wav')
     filename = 'test.wav'
     df = open(filename, 'w')
     df.close()
-    assert_raises(EOFError, al.load_audio, filename)
-    assert_raises(EOFError, al.AudioLoader, filename)
+    with pytest.raises(EOFError):
+        al.load_audio(filename)
+    with pytest.raises(EOFError):
+        al.AudioLoader(filename)
     os.remove(filename)
     write_audio_file(filename)
     am.disable_module()
-    assert_raises(IOError, al.load_audio, filename)
-    assert_raises(IOError, al.AudioLoader, filename)
+    with pytest.raises(IOError):
+        al.load_audio(filename)
+    with pytest.raises(IOError):
+        al.AudioLoader(filename)
     os.remove(filename)
     am.enable_module()
 
     
 def test_iter():
     am.enable_module()
     filename = 'test.wav'
     write_audio_file(filename, 1.0)
     full_data, rate = al.load_audio(filename)
     tolerance = 2.0**(-15)
     with al.AudioLoader(filename, 0.2) as data:
         for k, x in enumerate(data):
-            assert_false(np.any(np.abs(x-full_data[k]) > tolerance), 'iteration %d does not match' % k)
+            assert not np.any(np.abs(x-full_data[k]) > tolerance), 'iteration %d does not match' % k
 
         
 def test_blocks():
     am.enable_module()
     filename = 'test.wav'
     write_audio_file(filename)
     full_data, rate = al.load_audio(filename)
     tolerance = 2.0**(-15)
     for n in [5000, len(full_data)+100]:
         read_data = []
         with al.AudioLoader(filename) as data:
             for x in al.blocks(data, n, 10):
                 read_data.append(x[:-10].copy())
         read_data = np.vstack(read_data)
-        assert_equal(full_data.shape[0]-10, read_data.shape[0], 'len of blocked data differ from input data')
-        assert_equal(full_data.shape[1], read_data.shape[1], 'columns of blocked data differ from input data')
-        assert_false(np.any(np.abs(full_data[:-10] - read_data) > tolerance), 'blocks() failed')
+        assert full_data.shape[0]-10 == read_data.shape[0], 'len of blocked data differ from input data'
+        assert full_data.shape[1] == read_data.shape[1], 'columns of blocked data differ from input data'
+        assert not np.any(np.abs(full_data[:-10] - read_data) > tolerance), 'blocks() failed'
         read_data = []
         with al.AudioLoader(filename) as data:
             for x in data.blocks(n, 10):
                 read_data.append(x[:-10].copy())
         read_data = np.vstack(read_data)
-        assert_equal(full_data.shape[0]-10, read_data.shape[0], 'len of blocked data differ from input data')
-        assert_equal(full_data.shape[1], read_data.shape[1], 'columns of blocked data differ from input data')
-        assert_false(np.any(np.abs(full_data[:-10] - read_data) > tolerance), 'blocks() failed')
+        assert full_data.shape[0]-10 == read_data.shape[0], 'len of blocked data differ from input data'
+        assert full_data.shape[1] == read_data.shape[1], 'columns of blocked data differ from input data'
+        assert not np.any(np.abs(full_data[:-10] - read_data) > tolerance), 'blocks() failed'
 
-    def wrong_blocks(data):
-        for x in al.blocks(data, 10, 20):
+    with pytest.raises(ValueError):
+        for x in al.blocks(full_data, 10, 20):
             pass
-    assert_raises(ValueError, wrong_blocks, full_data)
 
 
 def test_unwrap():
+    duration = 0.1
     samplerate = 44100.0
-    t = np.arange(0.0, 1.0, 1.0/samplerate)
-    data = np.sin(2.0*np.pi*880.0*t) * t
-    al.unwrap(data)
-    data = data.reshape((-1, 1))
-    al.unwrap(data)
-    data = data.reshape((-1, 2))
-    al.unwrap(data)
+    channels = 4
+    t = np.arange(0.0, duration, 1.0/samplerate)
+    data = 1.5*np.sin(2.0*np.pi*880.0*t) * 2**15
+    data = data.astype(dtype=np.int16).astype(dtype=float)/2**15
+    data = data.astype(dtype=float)
+    filename = 'test.wav'
+    aw.write_wave(filename, data, samplerate, metadata={'Gain': '20mV'},
+                  encoding='PCM_16')
+
+    with al.AudioLoader(filename) as sf:
+        sf.set_unwrap(1.5, down_scale=False)
+        sdata = sf[:,:]
+        md = sf.metadata()['INFO']
+    assert md['UnwrapThreshold'] == '1.50', 'AudioLoader with unwrap adds metadata'
+    assert md['Gain'] == '20mV', 'AudioLoader with unwrap modifies gain'
+    assert len(sdata) == len(t), 'AudioLoader with unwrap keeps frames'
+    assert sdata.ndim == 2, 'AudioLoader with unwrap keeps two dimensions'
+    assert np.max(sdata) > 1.4, 'AudioLoader with unwrap expands beyond +1'
+    assert np.min(sdata) < -1.4, 'AudioLoader with unwrap expands below -1'
+
+    with al.AudioLoader(filename) as sf:
+        sf.set_unwrap(1.5)
+        sdata = sf[:,:]
+        md = sf.metadata()['INFO']
+    assert md['UnwrapThreshold'] == '0.75', 'AudioLoader with unwrap adds metadata'
+    assert md['Gain'] == '40.0mV', 'AudioLoader with unwrap modifies gain'
+    assert len(sdata) == len(t), 'AudioLoader with unwrap keeps frames'
+    assert sdata.ndim == 2, 'AudioLoader with unwrap keeps two dimensions'
+    assert np.max(sdata) <= 1.0, 'AudioLoader with unwrap downscales below +1'
+    assert np.min(sdata) >= -1.0, 'AudioLoader with unwrap downscales above -1'
+
+    with al.AudioLoader(filename) as sf:
+        sf.set_unwrap(1.5, clips=True)
+        sdata = sf[:,:]
+        md = sf.metadata()['INFO']
+    assert md['UnwrapThreshold'] == '1.50', 'AudioLoader with unwrap adds metadata'
+    assert md['UnwrapClippedAmplitude'] == '1.00', 'AudioLoader with unwrap adds metadata'
+    assert md['Gain'] == '20mV', 'AudioLoader with unwrap modifies gain'
+    assert len(sdata) == len(t), 'AudioLoader with unwrap keeps frames'
+    assert sdata.ndim == 2, 'AudioLoader with unwrap keeps two dimensions'
+    assert np.max(sdata) <= 1.0, 'AudioLoader with unwrap clips at +1'
+    assert np.min(sdata) >= -1.0, 'AudioLoader with unwrap clips at -1'
+    
+    os.remove(filename)
 
 
 def test_demo():
     am.enable_module()
     filename = 'test.wav'
     write_audio_file(filename, duration=5.0)
     al.demo(filename, False)
```

### Comparing `audioio-2.0.0/tests/test_audiomarkers.py` & `audioio-2.1.0/tests/test_audiomarkers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nose.tools import assert_true, assert_false, assert_equal, assert_raises
+import pytest
 import os
 import numpy as np
 import audioio.audioloader as al
 import audioio.audiowriter as aw
 import audioio.audiomarkers as am
 
 
@@ -27,56 +27,57 @@
     for i in range(len(labels)):
         labels[i,0] = chr(ord('a') + i % 26)
         labels[i,1] = chr(ord('A') + i % 26)*5
     filename = 'test.wav'
     
     aw.write_audio(filename, data, rate, None, locs)
     llocs, llabels = al.markers(filename)
-    assert_equal(len(llabels), 0, 'no labels')
-    assert_true(np.all(locs == llocs), 'same locs')
+    assert len(llabels) == 0, 'no labels'
+    assert np.all(locs == llocs), 'same locs'
     
     aw.write_audio(filename, data, rate, None, locs[:,0])
     llocs, llabels = al.markers(filename)
-    assert_equal(len(llabels), 0, 'no labels')
-    assert_true(np.all(locs[:,0] == llocs[:,0]), 'same locs')
+    assert len(llabels) == 0, 'no labels'
+    assert np.all(locs[:,0] == llocs[:,0]), 'same locs'
     
     aw.write_audio(filename, data, rate, None, locs, labels)
     llocs, llabels = al.markers(filename)
-    assert_true(np.all(locs == llocs), 'same locs')
-    assert_true(np.all(labels == llabels), 'same labels')
+    assert np.all(locs == llocs), 'same locs'
+    assert np.all(labels == llabels), 'same labels'
 
     with open(filename, 'rb') as sf:
         llocs, llabels = al.markers(sf)
-    assert_true(np.all(locs == llocs), 'same locs')
-    assert_true(np.all(labels == llabels), 'same labels')
+    assert np.all(locs == llocs), 'same locs'
+    assert np.all(labels == llabels), 'same labels'
     
-    assert_raises(IndexError, aw.write_audio, filename, data, rate,
-                  None, locs, labels[:-2,:])
+    with pytest.raises(IndexError):
+        aw.write_audio(filename, data, rate, None, locs,
+                       labels[:-2,:])
     
     aw.write_audio(filename, data, rate, None, locs, labels[:,0])
     llocs, llabels = al.markers(filename)
-    assert_true(np.all(locs == llocs), 'same locs')
-    assert_true(np.all(labels[:,0] == llabels[:,0]), 'same labels')
+    assert np.all(locs == llocs), 'same locs'
+    assert np.all(labels[:,0] == llabels[:,0]), 'same labels'
     
     aw.write_audio(filename, data, rate, None, locs[:,0], labels[:,0])
     llocs, llabels = al.markers(filename)
-    assert_true(np.all(locs[:,0] == llocs[:,0]), 'same locs')
-    assert_true(np.all(labels[:,0] == llabels[:,0]), 'same labels')
+    assert np.all(locs[:,0] == llocs[:,0]), 'same locs'
+    assert np.all(labels[:,0] == llabels[:,0]), 'same labels'
 
     labels = np.zeros((len(locs), 2), dtype=np.object_)
     aw.write_audio(filename, data, rate, None, locs, labels)
     llocs, llabels = al.markers(filename)
-    assert_true(np.all(locs == llocs), 'same locs')
-    assert_equal(len(llabels), 0, 'no labels')
+    assert np.all(locs == llocs), 'same locs'
+    assert len(llabels) == 0, 'no labels'
 
     locs[:,-1] = 0
     aw.write_audio(filename, data, rate, None, locs)
     llocs, llabels = al.markers(filename)
-    assert_equal(len(llabels), 0, 'no labels')
-    assert_true(np.all(locs == llocs), 'same locs')
+    assert len(llabels) == 0, 'no labels'
+    assert np.all(locs == llocs), 'same locs'
 
     os.remove(filename)
 
     filename = 'test.xyz'
     with open(filename, 'wb') as df:
         df.write(b'XYZ!')
     mmd = al.metadata(filename)
```

### Comparing `audioio-2.0.0/tests/test_audiomodules.py` & `audioio-2.1.0/tests/test_audiomodules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from nose.tools import assert_equal, assert_greater, assert_greater_equal, assert_raises
+import pytest
 import numpy as np
 import audioio.audiomodules as am
 
 
 def test_audiomodules():
     am.enable_module()
     funcs = ['all', 'fileio', 'device']
     for func in funcs:
         am.enable_module()
         print('')
         print('module lists for %s:' % func)
         inst_mods = am.installed_modules(func)
         print('installed:', len(inst_mods), inst_mods)
-        assert_greater(len(inst_mods), 0, 'no installed modules for %s' % func)
+        assert len(inst_mods) > 0, 'no installed modules for %s' % func
         avail_mods = am.available_modules(func)
         print('available:', len(avail_mods), avail_mods)
-        assert_equal(len(avail_mods), len(inst_mods), 'less available modules than installed modules for %s' % func)
+        assert len(avail_mods) == len(inst_mods), 'less available modules than installed modules for %s' % func
         unavail_mods = am.unavailable_modules(func)
         print('unavailable:', len(unavail_mods), unavail_mods)
-        assert_greater_equal(len(unavail_mods), 0, 'wrong number of unavailable modules for %s' % func)
+        assert len(unavail_mods) >= 0, 'wrong number of unavailable modules for %s' % func
         missing_mods = am.missing_modules(func)
         print('missing:', len(missing_mods), missing_mods)
-        assert_greater_equal(len(missing_mods), 0, 'wrong number of missing modules for %s' % func)
+        assert len(missing_mods) >= 0, 'wrong number of missing modules for %s' % func
         am.missing_modules_instructions(func)
         am.list_modules(func, False)
         am.list_modules(func, True)
 
     print()
     print('single module functions:')
     for module in am.audio_modules.keys():
         am.disable_module(module)
         am.enable_module(module)
         am.select_module(module)
         am.enable_module()
         inst = am.installation_instruction(module)
-        assert_greater(len(inst), 0, 'no installation instructions for module %s' % module)
+        assert len(inst) > 0, 'no installation instructions for module %s' % module
         am.list_modules(module, False)
         am.list_modules(module, True)
 
 
 def test_main():
     am.enable_module()
     am.main()
```

### Comparing `audioio-2.0.0/tests/test_audiotools.py` & `audioio-2.1.0/tests/test_audiotools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nose.tools import assert_true, assert_false, assert_equal
+import pytest
 import numpy as np
 import audioio.audiotools as at
 
 
 def test_despike():
     duration = 0.1
     samplerate = 44100.0
@@ -11,36 +11,36 @@
     data = 0.9*np.sin(2.0*np.pi*880.0*t)
     idx = np.random.randint(1, len(t)//10-20, 20)*10
     data[idx] += 1
     data[idx+25] -= 1
     
     sdata = data[:]
     at.despike(sdata, 0.5)
-    assert_equal(len(sdata), len(t), 'despike keeps frames')
-    assert_equal(sdata.ndim, 1, 'despike keeps single dimension')
-    assert_true(np.max(sdata) <= 1.0, 'despike does not expand beyond +1')
-    assert_true(np.min(sdata) >= -1.0, 'despike does not expand below -1')
+    assert len(sdata) == len(t), 'despike keeps frames'
+    assert sdata.ndim == 1, 'despike keeps single dimension'
+    assert np.max(sdata) <= 1.0, 'despike does not expand beyond +1'
+    assert np.min(sdata) >= -1.0, 'despike does not expand below -1'
 
     data = data.reshape((-1, 1))
     for k in range(data.shape[1], channels):
         data = np.hstack((data, data[:,0].reshape((-1, 1))/k))
 
     cdata = data.copy()
     at.despike(cdata, 0.5)
-    assert_equal(len(cdata), len(t), 'despike keeps frames')
-    assert_equal(cdata.shape[1], channels, 'despike keeps channels')
-    assert_true(np.max(cdata) <= 1.0, 'despike does not expand beyond +1')
-    assert_true(np.min(cdata) >= -1.0, 'despike does not expand below -1')
+    assert len(cdata) == len(t), 'despike keeps frames'
+    assert cdata.shape[1] == channels, 'despike keeps channels'
+    assert np.max(cdata) <= 1.0, 'despike does not expand beyond +1'
+    assert np.min(cdata) >= -1.0, 'despike does not expand below -1'
 
     at.has_numba = False
     at.despike(data, 0.5)
-    assert_equal(len(data), len(t), 'despike keeps frames')
-    assert_equal(data.shape[1], channels, 'despike keeps channels')
-    assert_true(np.max(data) <= 1.0, 'despike does not expand beyond +1')
-    assert_true(np.min(data) >= -1.0, 'despike does not expand below -1')
+    assert len(data) == len(t), 'despike keeps frames'
+    assert data.shape[1] == channels, 'despike keeps channels'
+    assert np.max(data) <= 1.0, 'despike does not expand beyond +1'
+    assert np.min(data) >= -1.0, 'despike does not expand below -1'
     at.has_numba = True
 
 
 def test_despike2():
     duration = 0.1
     samplerate = 44100.0
     channels = 4
@@ -50,64 +50,71 @@
     data[idx] += 1
     data[idx+1] += 1
     data[idx+25] -= 1
     data[idx+26] -= 1
     
     sdata = data[:]
     at.despike(sdata, 0.5, 2)
-    assert_equal(len(sdata), len(t), 'despike keeps frames')
-    assert_equal(sdata.ndim, 1, 'despike keeps single dimension')
-    assert_true(np.max(sdata) <= 1.0, 'despike does not expand beyond +1')
-    assert_true(np.min(sdata) >= -1.0, 'despike does not expand below -1')
+    assert len(sdata) == len(t), 'despike keeps frames'
+    assert sdata.ndim == 1, 'despike keeps single dimension'
+    assert np.max(sdata) <= 1.0, 'despike does not expand beyond +1'
+    assert np.min(sdata) >= -1.0, 'despike does not expand below -1'
 
     data = data.reshape((-1, 1))
     for k in range(data.shape[1], channels):
         data = np.hstack((data, data[:,0].reshape((-1, 1))/k))
 
     cdata = data.copy()
     at.despike(cdata, 0.5, 2)
-    assert_equal(len(cdata), len(t), 'despike keeps frames')
-    assert_equal(cdata.shape[1], channels, 'despike keeps channels')
-    assert_true(np.max(cdata) <= 1.0, 'despike does not expand beyond +1')
-    assert_true(np.min(cdata) >= -1.0, 'despike does not expand below -1')
+    assert len(cdata) == len(t), 'despike keeps frames'
+    assert cdata.shape[1] == channels, 'despike keeps channels'
+    assert np.max(cdata) <= 1.0, 'despike does not expand beyond +1'
+    assert np.min(cdata) >= -1.0, 'despike does not expand below -1'
 
     at.has_numba = False
     at.despike(data, 0.5, 2)
-    assert_equal(len(data), len(t), 'despike keeps frames')
-    assert_equal(data.shape[1], channels, 'despike keeps channels')
-    assert_true(np.max(data) <= 1.0, 'despike does not expand beyond +1')
-    assert_true(np.min(data) >= -1.0, 'despike does not expand below -1')
+    assert len(data) == len(t), 'despike keeps frames'
+    assert data.shape[1] == channels, 'despike keeps channels'
+    assert np.max(data) <= 1.0, 'despike does not expand beyond +1'
+    assert np.min(data) >= -1.0, 'despike does not expand below -1'
     at.has_numba = True
 
 
 def test_unwrap():
     duration = 0.1
     samplerate = 44100.0
     channels = 4
     t = np.arange(0.0, duration, 1.0/samplerate)
     data = 1.5*np.sin(2.0*np.pi*880.0*t) * 2**15
     data = data.astype(dtype=np.int16).astype(dtype=float)/2**15
-    sdata = data[:]
-
+    
+    sdata = data.copy()
     at.unwrap(sdata)
-    assert_equal(len(sdata), len(t), 'unwrap keeps frames')
-    assert_equal(sdata.ndim, 1, 'unwrap keeps single dimension')
-    assert_true(np.max(sdata) > 1.4, 'unwrap expands beyond +1')
-    assert_true(np.min(sdata) < -1.4, 'unwrap expands below -1')
+    assert len(sdata) == len(t), 'unwrap keeps frames'
+    assert sdata.ndim == 1, 'unwrap keeps single dimension'
+    assert np.max(sdata) > 1.4, 'unwrap expands beyond +1'
+    assert np.min(sdata) < -1.4, 'unwrap expands below -1'
+    
+    sdata = data * 120
+    at.unwrap(sdata, 1.5, 120)
+    assert len(sdata) == len(t), 'unwrap keeps frames'
+    assert sdata.ndim == 1, 'unwrap keeps single dimension'
+    assert np.max(sdata) > 1.4*120, 'unwrap expands beyond +1'
+    assert np.min(sdata) < -1.4*120, 'unwrap expands below -1'
 
     data = data.reshape((-1, 1))
     for k in range(data.shape[1], channels):
         data = np.hstack((data, data[:,0].reshape((-1, 1))/k))
 
     cdata = data.copy()
     at.unwrap(cdata)
-    assert_equal(len(cdata), len(t), 'unwrap keeps frames')
-    assert_equal(cdata.shape[1], channels, 'unwrap keeps channels')
-    assert_true(np.max(cdata) > 1.4, 'unwrap expands beyond +1')
-    assert_true(np.min(cdata) < -1.4, 'unwrap expands below -1')
+    assert len(cdata) == len(t), 'unwrap keeps frames'
+    assert cdata.shape[1] == channels, 'unwrap keeps channels'
+    assert np.max(cdata) > 1.4, 'unwrap expands beyond +1'
+    assert np.min(cdata) < -1.4, 'unwrap expands below -1'
 
     at.has_numba = False
     did = id(data)
     at.unwrap(data)
-    assert_equal(did, id(data), 'without numba unwrap does not touch the array')
+    assert did == id(data), 'without numba unwrap does not touch the array'
     at.has_numba = True
```

### Comparing `audioio-2.0.0/tests/test_audiowriter.py` & `audioio-2.1.0/tests/test_audiowriter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,54 @@
-from nose.tools import assert_true, assert_equal, assert_greater_equal, assert_less, assert_almost_equal, assert_raises
+import pytest
 import os
 import numpy as np
 import audioio.audiowriter as aw
 import audioio.audioloader as al
 import audioio.audiometadata as amd
 import audioio.audiomodules as am
 
 
 def test_formats_encodings():
     am.enable_module()
     min_formats = {'wave': 1, 'ewave': 2, 'scipy.io.wavfile': 1,
-                   'soundfile': 23, 'wavefile': 23, 'pydub': 10}
+                   'soundfile': 23, 'wavefile': 6, 'pydub': 10}
     for (module, formats_func), (m, encodings_func) in zip(aw.audio_formats_funcs, aw.audio_encodings_funcs):
         if aw.audio_modules[module]:
             min_f = min_formats[module]
             formats = formats_func()
-            assert_greater_equal(len(formats), min_f,
-                                 'formats_%s() did not return enough formats' % module.split('.')[-1])
+            assert len(formats) >= min_f, 'formats_%s() did not return enough formats' % module.split('.')[-1]
             for f in formats:
                 encodings = encodings_func(f)
-                assert_greater_equal(len(encodings), 1,
-                                     'encodings_%s() did not return enough encodings for format %s' % (module.split('.')[-1], f))
+                assert len(encodings) >= 1, 'encodings_%s() did not return enough encodings for format %s' % (module.split('.')[-1], f)
             encodings = encodings_func('xxx')
-            assert_equal(len(encodings), 0, 'encodings_%s() returned encodings for invalid format xxx' % module.split('.')[-1])
+            assert len(encodings) == 0, 'encodings_%s() returned encodings for invalid format xxx' % module.split('.')[-1]
             encodings = encodings_func('')
-            assert_equal(len(encodings), 0, 'encodings_%s() returned encodings for empty format xxx' % module.split('.')[-1])
+            assert len(encodings) == 0, 'encodings_%s() returned encodings for empty format xxx' % module.split('.')[-1]
 
     formats = aw.available_formats()
-    assert_greater_equal(len(formats), 1,
-                         'available_formats() did not return enough formats')
+    assert len(formats) >= 1, 'available_formats() did not return enough formats'
     for f in formats:
         encodings = aw.available_encodings(f)
-        assert_greater_equal(len(encodings), 1,
-                             'available_encodings() did not return enough encodings for format %s' % f)
+        assert len(encodings) >= 1, 'available_encodings() did not return enough encodings for format %s' % f
                 
 
 def test_write_read():
 
     def check(samplerate_write, data_write, samplerate_read, data_read, lib, encoding):
-        assert_almost_equal(samplerate_write, samplerate_read, 'samplerates differ for module %s with encoding %s' % (lib, encoding))
-        assert_equal(len(data_write), len(data_read), 'frames %d %d differ for module %s with encoding %s' % (len(data_write), len(data_read), lib, encoding))
-        assert_equal(len(data_write.shape), len(data_read.shape), 'shape len differs for module %s with encoding %s' % (lib, encoding))
-        assert_equal(len(data_read.shape), 2, 'shape differs from 2 for module %s with encoding %s' % (lib, encoding))
-        assert_equal(data_write.shape[0], data_read.shape[0], 'shape[0] differs for module %s with encoding %s' % (lib, encoding))
-        assert_equal(data_write.shape[1], data_read.shape[1], 'shape[1] differs for module %s with encoding %s' % (lib, encoding))
-        assert_equal(data_read.dtype, np.float64, 'read in data are not doubles for module %s with encoding %s' % (lib, encoding))
+        assert samplerate_write == pytest.approx(samplerate_read), 'samplerates differ for module %s with encoding %s' % (lib, encoding)
+        assert len(data_write) == len(data_read), 'frames %d %d differ for module %s with encoding %s' % (len(data_write), len(data_read), lib, encoding)
+        assert len(data_write.shape) == len(data_read.shape), 'shape len differs for module %s with encoding %s' % (lib, encoding)
+        assert len(data_read.shape) == 2, 'shape differs from 2 for module %s with encoding %s' % (lib, encoding)
+        assert data_write.shape[0] == data_read.shape[0], 'shape[0] differs for module %s with encoding %s' % (lib, encoding)
+        assert data_write.shape[1] == data_read.shape[1], 'shape[1] differs for module %s with encoding %s' % (lib, encoding)
+        assert data_read.dtype == np.float64, 'read in data are not doubles for module %s with encoding %s' % (lib, encoding)
         n = min([len(data_write), len(data_read)])
         max_error = np.max(np.abs(data_write[:n] - data_read[:n]))
         print('maximum error = %g' % max_error)
-        assert_less(max_error, 0.05, 'values differ for module %s with encoding %s by up to %g' % (lib, encoding, max_error))
+        assert max_error < 0.05, 'values differ for module %s with encoding %s by up to %g' % (lib, encoding, max_error)
         
     am.enable_module()
     # generate data:
     samplerate = 44100.0
     duration = 10.0
     t = np.arange(0.0, duration, 1.0/samplerate)
     data = np.sin(2.0*np.pi*880.0*t) * t/duration
@@ -137,16 +133,16 @@
             continue
         print('%s module...' % lib)
         am.select_module(lib)
         aw.write_audio(filename, data, samplerate)
         if lib == 'pydub':
             am.select_module('audioread')
         data_read, samplerate_read = al.load_audio(filename)
-        assert_equal(len(data_read.shape), 2, 'read in data must be a 2-D array')
-        assert_equal(data_read.shape[1], 1, 'read in data must be a 2-D array with one column')
+        assert len(data_read.shape) == 2, 'read in data must be a 2-D array'
+        assert data_read.shape[1] == 1, 'read in data must be a 2-D array with one column'
 
     print('2-D data one channel')
     filename = 'test.wav'
     samplerate = 44100.0
     duration = 10.0
     t = np.arange(0.0, duration, 1.0/samplerate)
     data = np.sin(2.0*np.pi*880.0*t) * t/duration
@@ -157,17 +153,17 @@
             continue
         print('%s module...' % lib)
         am.select_module(lib)
         aw.write_audio(filename, data, samplerate)
         if lib == 'pydub':
             am.select_module('audioread')
         data_read, samplerate_read = al.load_audio(filename)
-        assert_equal(len(data_read.shape), 2, 'read in data must be a 2-D array')
-        assert_equal(data_read.shape[1], 1, 'read in data must be a 2-D array with one column')
-        assert_equal(data_read.shape, data.shape, 'input and output data must have same shape')
+        assert len(data_read.shape) == 2, 'read in data must be a 2-D array'
+        assert data_read.shape[1] == 1, 'read in data must be a 2-D array with one column'
+        assert data_read.shape == data.shape, 'input and output data must have same shape'
 
     print('2-D data two channel')
     filename = 'test.wav'
     samplerate = 44100.0
     duration = 10.0
     t = np.arange(0.0, duration, 1.0/samplerate)
     data = np.sin(2.0*np.pi*880.0*t) * t/duration
@@ -178,17 +174,17 @@
             continue
         print('%s module...' % lib)
         am.select_module(lib)
         aw.write_audio(filename, data, samplerate)
         if lib == 'pydub':
             am.select_module('audioread')
         data_read, samplerate_read = al.load_audio(filename)
-        assert_equal(len(data_read.shape), 2, 'read in data must be a 2-D array')
-        assert_equal(data_read.shape[1], 2, 'read in data must be a 2-D array with two columns')
-        assert_equal(data_read.shape, data.shape, 'input and output data must have same shape')
+        assert len(data_read.shape) == 2, 'read in data must be a 2-D array'
+        assert data_read.shape[1] == 2, 'read in data must be a 2-D array with two columns'
+        assert data_read.shape == data.shape, 'input and output data must have same shape'
     am.enable_module()
 
 
 def test_write_read_modules():
     am.enable_module()
     # generate data:
     filename = 'test.wav'
@@ -197,43 +193,50 @@
     duration = 10.0
     t = np.arange(int(duration*samplerate))/samplerate
     data = np.sin(2.0*np.pi*880.0*t) * t/duration
     # test for wrong formats:
     for lib, write_func in aw.audio_writer_funcs:
         if not am.select_module(lib):
             continue
-        assert_raises(ValueError, write_func, '', data, samplerate)
-        assert_raises(ValueError, write_func, filename, data, samplerate, format='xxx')
+        with pytest.raises(ValueError):
+            write_func('', data, samplerate)
+        with pytest.raises(ValueError):
+            write_func(filename, data, samplerate, format='xxx')
         write_func(filename, data, samplerate, format='')
         os.remove(filename)
-        assert_raises(ValueError, write_func, filename, data, samplerate, encoding='xxx')
+        with pytest.raises(ValueError):
+            write_func(filename, data, samplerate, encoding='xxx')
         write_func(filename, data, samplerate, encoding='')
         os.remove(filename)
         am.enable_module()
-    assert_raises(ValueError, aw.write_audio, '', data, samplerate)
-    assert_raises(IOError, aw.write_audio, filename, data, samplerate, format='xxx')
+    with pytest.raises(ValueError):
+        aw.write_audio('', data, samplerate)
+    with pytest.raises(IOError):
+        aw.write_audio(filename, data, samplerate, format='xxx')
     aw.write_audio(filename, data, samplerate, format='')
     os.remove(filename)
-    assert_raises(IOError, aw.write_audio, filename, data, samplerate, encoding='xxx')
+    with pytest.raises(IOError):
+        aw.write_audio(filename, data, samplerate, encoding='xxx')
     aw.write_audio(filename, data, samplerate, encoding='')
     os.remove(filename)
     # test for not available modules:
     for lib, write_func in aw.audio_writer_funcs:
         am.disable_module(lib)
-        assert_raises(ImportError, write_func, filename, data, samplerate)
+        with pytest.raises(ImportError):
+            write_func(filename, data, samplerate)
         am.enable_module(lib)
     for lib, encodings_func in aw.audio_encodings_funcs:
         am.disable_module(lib)
         enc = encodings_func(format)
-        assert_equal(len(enc), 0, 'no encoding should be returned for disabled module %s' % lib)
+        assert len(enc) == 0, 'no encoding should be returned for disabled module %s' % lib
         am.enable_module(lib)
     for lib, formats_func in aw.audio_formats_funcs:
         am.disable_module(lib)
         formats = formats_func()
-        assert_equal(len(formats), 0, 'no format should be returned for disabled module %s' % lib)
+        assert len(formats) == 0, 'no format should be returned for disabled module %s' % lib
         am.enable_module(lib)
 
 
 def test_write_metadata():
     am.enable_module()
     # generate data:
     samplerate = 44100.0
@@ -245,55 +248,55 @@
     filename = 'test.wav'
     for lib, write_func in aw.audio_writer_funcs:
         if not am.select_module(lib):
             continue
         write_func(filename, data, samplerate, md)
         mmd = al.metadata(filename)
         os.remove(filename)
-        assert_equal(md, mmd, 'metadata for wavefiles')
+        assert md == mmd, 'metadata for wavefiles'
         am.enable_module()
     # test storage of metadata in ogg files:
     filename = 'test.ogg'
     for lib, write_func in aw.audio_writer_funcs:
         if lib == 'pydub':
             continue
         if not am.select_module(lib):
             continue
         if not 'OGG' in aw.available_formats():
             continue
         write_func(filename, data, samplerate, md, encoding='VORBIS')
         mmd = al.metadata(filename)
         os.remove(filename)
-        assert_equal(len(mmd), 0, 'metadata for ogg files')
+        assert len(mmd) == 0, 'metadata for ogg files'
         am.enable_module()
     # test storage of metadata in mp3 files:
     if am.audio_modules['pydub']:
         filename = 'test.mp3'
         aw.write_pydub(filename, data, samplerate, md)
         mmd = al.metadata(filename)
         os.remove(filename)
-        assert_equal(len(mmd), 0, 'metadata for mp3 files')
+        assert len(mmd) == 0, 'metadata for mp3 files'
         am.enable_module()
 
         
 def test_extensions():
     f = aw.format_from_extension(None)
-    assert_true(f is None, 'None filepath')
+    assert f is None, 'None filepath'
     f = aw.format_from_extension('file')
-    assert_true(f is None, 'filepath withouth extension')
+    assert f is None, 'filepath withouth extension'
     f = aw.format_from_extension('file.')
-    assert_true(f is None, 'filepath withouth extension')
+    assert f is None, 'filepath withouth extension'
     f = aw.format_from_extension('file.wave')
-    assert_equal(f, 'WAV', 'filepath with wave')
+    assert f == 'WAV', 'filepath with wave'
     f = aw.format_from_extension('file.wav')
-    assert_equal(f, 'WAV', 'filepath with wav')
+    assert f == 'WAV', 'filepath with wav'
     f = aw.format_from_extension('file.ogg')
-    assert_equal(f, 'OGG', 'filepath with wav')
+    assert f == 'OGG', 'filepath with wav'
     f = aw.format_from_extension('file.mpeg4')
-    assert_equal(f, 'MP4', 'filepath with wav')
+    assert f == 'MP4', 'filepath with wav'
 
 
 def test_demo():
     am.enable_module()
     filename = 'test.wav'
     aw.demo(filename)
     aw.demo(filename, channels=1)
```

### Comparing `audioio-2.0.0/tests/test_playaudio.py` & `audioio-2.1.0/tests/test_playaudio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nose.tools import assert_equal, assert_greater, assert_greater_equal, assert_less, assert_raises
+import pytest
 import time
 import numpy as np
 import audioio.playaudio as ap
 import audioio.audiomodules as am
 
 
 def test_beep():
@@ -99,37 +99,46 @@
             print(f'test_downsample() with {lib} ({ap.handle.lib}) module found no device.')
         ap.close()
         am.enable_module()
 
 
 def test_note2freq():
     fa = 460.0
-    assert_less(np.abs(ap.note2freq('a4', fa)-fa), 1e-6, 'wrong a4 frequency')
+    assert np.abs(ap.note2freq('a4', fa)-fa) < 1e-6, 'wrong a4 frequency'
     fp = 0.5*ap.note2freq('a0')
     for o in range(10):
         for n in 'cdefgab':
             note = '%s%d' % (n, o)
             f = ap.note2freq(note)
-            assert_greater(f, fp, 'frequency of %s should be greater than the one of previous note' % note)
+            assert f > fp, 'frequency of %s should be greater than the one of previous note' % note
             note = '%s#%d' % (n, o)
             fs = ap.note2freq(note)
-            assert_greater(fs, f, 'frequency of %s should be greater' % note)
+            assert fs > f, 'frequency of %s should be greater' % note
             note = '%sb%d' % (n, o)
             fb = ap.note2freq(note)
-            assert_less(fb, f, 'frequency of %s should be greater' % note)
+            assert fb < f, 'frequency of %s should be greater' % note
             fp = f
-    assert_raises(ValueError, ap.note2freq, 'h')
-    assert_raises(ValueError, ap.note2freq, 'da')
-    assert_raises(ValueError, ap.note2freq, 'dx#')
-    assert_raises(ValueError, ap.note2freq, 'd4#')
-    assert_raises(ValueError, ap.note2freq, 'd4x')
-    assert_raises(ValueError, ap.note2freq, 'd#4x')
-    assert_raises(ValueError, ap.note2freq, 'd-2')
-    assert_raises(ValueError, ap.note2freq, '')
-    assert_raises(ValueError, ap.note2freq, 0)
+    with pytest.raises(ValueError):
+        ap.note2freq('h')
+    with pytest.raises(ValueError):
+        ap.note2freq('da')
+    with pytest.raises(ValueError):
+        ap.note2freq('dx#')
+    with pytest.raises(ValueError):
+        ap.note2freq('d4#')
+    with pytest.raises(ValueError):
+        ap.note2freq('d4x')
+    with pytest.raises(ValueError):
+        ap.note2freq('d#4x')
+    with pytest.raises(ValueError):
+        ap.note2freq('d-2')
+    with pytest.raises(ValueError):
+        ap.note2freq('')
+    with pytest.raises(ValueError):
+        ap.note2freq(0)
 
 
 def test_demo():
     am.enable_module()
     try:
         ap.demo()
     except FileNotFoundError:
```

### Comparing `audioio-2.0.0/tests/test_riffmetadata.py` & `audioio-2.1.0/tests/test_riffmetadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nose.tools import assert_true, assert_false, assert_equal, assert_raises
+import pytest
 import os
 import numpy as np
 import audioio.riffmetadata as rm
 
 
 def generate_data():
     duration = 2.0
@@ -17,69 +17,75 @@
 
 
 def test_write():
     data, rate = generate_data()
     filename = 'test.wav'
     for encoding in ['PCM_16', 'PCM_32']:
         rm.write_wave(filename, data, rate, None, encoding=encoding)
-    assert_raises(ValueError, rm.write_wave, '', data, rate,
-                  None, encoding=encoding)
-    assert_raises(ValueError, rm.write_wave, filename, data, rate,
-                  None, encoding='XYZ')
+    with pytest.raises(ValueError):
+        rm.write_wave('', data, rate, None, encoding=encoding)
+    with pytest.raises(ValueError):
+        rm.write_wave(filename, data, rate, None, encoding='XYZ')
     with open(filename, 'wb') as df:
         rm.write_riff_chunk(df, 1000)
         rm.write_riff_chunk(df)
         rm.write_riff_chunk(df, 1000, '1234')
-        assert_raises(ValueError, rm.write_riff_chunk, df, 2000, tag='12345')
+        with pytest.raises(ValueError):
+            rm.write_riff_chunk(df, 2000, tag='12345')
         rm.write_chunk_name(df, 12, '1234')
-        assert_raises(ValueError, rm.write_chunk_name, df, 12, '123456')
+        with pytest.raises(ValueError):
+            rm.write_chunk_name(df, 12, '123456')
         n, t = rm.write_info_chunk(df, None)
-        assert_equal(n, 0, 'no info chunk')
-        assert_equal(len(t), 0, 'no info chunk')
+        assert n == 0, 'no info chunk'
+        assert len(t) == 0, 'no info chunk'
         n, t = rm.write_info_chunk(df, dict(INFO=dict(IART='John Doe', TITLX='TLDR')))
-        assert_equal(n, 0, 'no info chunk')
-        assert_equal(len(t), 0, 'no info chunk')
+        assert n == 0, 'no info chunk'
+        assert len(t) == 0, 'no info chunk'
         n, t = rm.write_bext_chunk(df, None)
-        assert_equal(n, 0, 'no bext chunk')
-        assert_equal(len(t), 0, 'no bext chunk')
+        assert n == 0, 'no bext chunk'
+        assert len(t) == 0, 'no bext chunk'
         n, t = rm.write_ixml_chunk(df, None)
-        assert_equal(n, 0, 'no ixml chunk')
-        assert_equal(len(t), 0, 'no ixml chunk')
-        n, t = rm.write_odml_chunk(df, None)
-        assert_equal(n, 0, 'no odml chunk')
-        assert_equal(len(t), 0, 'no odml chunk')
+        assert n == 0, 'no ixml chunk'
+        assert len(t) == 0, 'no ixml chunk'
+        n, t = rm.write_guano_chunk(df, None)
+        assert n == 0, 'no guano chunk'
+        assert len(t) == 0, 'no odml chunk'
         n = rm.write_cue_chunk(df, None)
-        assert_equal(n, 0, 'no cue chunk')
-        assert_raises(IndexError, rm.append_markers_riff, df, np.ones((4, 2)), np.zeros(3))
-    assert_raises(ValueError, rm.append_riff, '')
-    assert_raises(IndexError, rm.append_riff, filename, None, np.ones((4, 2)), np.zeros(3))
+        assert n == 0, 'no cue chunk'
+        with pytest.raises(IndexError):
+            rm.append_markers_riff(df, np.ones((4, 2)), np.zeros(3))
+    with pytest.raises(ValueError):
+        rm.append_riff('')
+    with pytest.raises(IndexError):
+        rm.append_riff(filename, None, np.ones((4, 2)), np.zeros(3))
     md = dict(Artist='John Doe')
     rm.append_riff(filename, md, np.ones((4, 2), dtype=int), np.zeros(4))
     rm.append_riff(filename, md, np.ones((4, 2), dtype=int), np.zeros(4))
     os.remove(filename)
 
 
 def test_read():
     data, rate = generate_data()
     md = dict(Artist='John Doe')
     filename = 'test.wav'
     rm.write_wave(filename, data, rate, md)
     with open(filename, 'rb') as sf:
         n = rm.read_riff_header(sf)
-        assert_true(n > 0, 'riff header')
+        assert n > 0, 'riff header'
     with open(filename, 'rb') as sf:
         n = rm.read_riff_header(sf, 'WAVE')
-        assert_true(n > 0, 'riff header')
+        assert n > 0, 'riff header'
     with open(filename, 'rb') as sf:
-        assert_raises(ValueError, rm.read_riff_header, sf, 'XYZ ')
+        with pytest.raises(ValueError):
+            rm.read_riff_header(sf, 'XYZ ')
     chunks = rm.read_chunk_tags(filename)
-    assert_equal(len(chunks), 3, 'chunk tags')
+    assert len(chunks) == 3, 'chunk tags'
     with open(filename, 'rb') as sf:
         chunks = rm.read_chunk_tags(sf)
-        assert_equal(len(chunks), 3, 'chunk tags')
+        assert len(chunks) == 3, 'chunk tags'
     os.remove(filename)
 
     
 def test_metadata():
     data, rate = generate_data()
     filename = 'test.wav'
     imd = dict(IENG='John Doe', ICRD='2024-01-24', RATE=9,
@@ -94,83 +100,71 @@
     omd = iimd.copy()
     omd['Production'] = bbmd
 
     # INFO:
     md = dict(INFO=imd)
     rm.write_wave(filename, data, rate, md)
     mdd = rm.metadata_riff(filename, False)
-    assert_true('INFO' in mdd, 'INFO section exists')
-    assert_equal(iimd, mdd['INFO'], 'INFO section matches')
+    assert 'INFO' in mdd, 'INFO section exists'
+    assert iimd == mdd['INFO'], 'INFO section matches'
     with open(filename, 'rb') as sf:
         mdd = rm.metadata_riff(sf, False)
-    assert_true('INFO' in mdd, 'INFO section exists')
-    assert_equal(iimd, mdd['INFO'], 'INFO section matches')
+    assert 'INFO' in mdd, 'INFO section exists'
+    assert iimd == mdd['INFO'], 'INFO section matches'
     md['INFO']['IENG'] = ''
     rm.write_wave(filename, data, rate, md)
     mdd = rm.metadata_riff(filename, True)
-    assert_true('INFO' in mdd, 'INFO section exists')
+    assert 'INFO' in mdd, 'INFO section exists'
     md['INFO']['IENG'] = 'John Doe'
 
     # BEXT:
     md = dict(BEXT=bmd)
     rm.write_wave(filename, data, rate, md)
     mdd = rm.metadata_riff(filename, False)
-    assert_true('BEXT' in mdd, 'BEXT section exists')
-    assert_equal(bmd, mdd['BEXT'], 'BEXT section matches')
+    assert 'BEXT' in mdd, 'BEXT section exists'
+    assert bmd == mdd['BEXT'], 'BEXT section matches'
     mdd = rm.metadata_riff(filename, True)
-    assert_true('BEXT' in mdd, 'BEXT section exists')
+    assert 'BEXT' in mdd, 'BEXT section exists'
 
     # IXML:
     md = dict(IXML=xmd)
     rm.write_wave(filename, data, rate, md)
     mdd = rm.metadata_riff(filename, False)
-    assert_true('IXML' in mdd, 'IXML section exists')
-    assert_equal(xmd, mdd['IXML'], 'IXML section matches')
+    assert 'IXML' in mdd, 'IXML section exists'
+    assert xmd == mdd['IXML'], 'IXML section matches'
     md['IXML']['Note'] = ''
     rm.write_wave(filename, data, rate, md)
     mdd = rm.metadata_riff(filename, True)
-    assert_true('IXML' in mdd, 'IXML section exists')
+    assert 'IXML' in mdd, 'IXML section exists'
     md['IXML']['Note'] = 'still testing'
 
     # GUANO:
-    md = dict(GUANO=iimd)
+    md = dict(GUANO=dict(**iimd))
     rm.write_wave(filename, data, rate, md)
     mdd = rm.metadata_riff(filename, False)
-    assert_true('GUANO' in mdd, 'GUANO section exists')
-    assert_equal(md, mdd, 'GUANO section matches')
-    md['GUANO']['Engineer'] = ''
-    rm.write_wave(filename, data, rate, md)
-    mdd = rm.metadata_riff(filename, True)
-    assert_true('GUANO' in mdd, 'GUANO section exists')
-    md['GUANO']['Engineer'] = 'John Doe'
-
-    # ODML:
-    md = dict(Recording=omd, Production=bbmd, Notes=xmd)
-    rm.write_wave(filename, data, rate, md)
-    mdd = rm.metadata_riff(filename, False)
-    assert_equal(md, mdd, 'ODML sections match')
+    assert md == mdd, 'GUANO section matches'
     
-    md = dict(INFO=imd, BEXT=bmd, IXML=xmd,
+    md = dict(INFO=iimd, BEXT=bmd, IXML=xmd,
               Recording=omd, Production=bmd, Notes=xmd)
     rm.write_wave(filename, data, rate, md)
     mdd = rm.metadata_riff(filename, False)
-    assert_true('INFO' in mdd, 'INFO section exists')
-    assert_equal(iimd, mdd['INFO'], 'INFO section matches')
-    assert_true('BEXT' in mdd, 'BEXT section exists')
-    assert_equal(bmd, mdd['BEXT'], 'BEXT section matches')
-    assert_true('IXML' in mdd, 'IXML section exists')
-    assert_equal(xmd, mdd['IXML'], 'IXML section matches')
-    assert_true('Recording' in mdd, 'Recording section exists')
-    assert_true('Production' in mdd, 'Recording section exists')
-    assert_true('Notes' in mdd, 'Recording section exists')
-    assert_equal(md['Notes'], mdd['Notes'], 'Notes section matches')
+    assert 'INFO' in mdd, 'INFO section exists'
+    assert iimd == mdd['INFO'], 'INFO section matches'
+    assert 'BEXT' in mdd, 'BEXT section exists'
+    assert bmd == mdd['BEXT'], 'BEXT section matches'
+    assert 'IXML' in mdd, 'IXML section exists'
+    assert xmd == mdd['IXML'], 'IXML section matches'
+    assert 'Recording' in mdd, 'Recording section exists'
+    assert 'Production' in mdd, 'Production section exists'
+    assert 'Notes' in mdd, 'Notes section exists'
+    assert md['Notes'] == mdd['Notes'], 'Notes section matches'
     md = dict(Recording=omd, Production='', Notes=xmd)
     rm.write_wave(filename, data, rate, md)
     mdd = rm.metadata_riff(filename, True)
-    assert_equal(len(mdd['Production']), 0, 'Empty Production value')
+    assert len(mdd['Production']) == 0, 'Empty Production value'
 
     # INFO:
     imd['SUBI'] = bmd
     md = dict(INFO=imd)
     rm.write_wave(filename, data, rate, md)
 
     # BEXT:
@@ -191,57 +185,69 @@
     for i in range(len(labels)):
         labels[i,0] = chr(ord('a') + i % 26)
         labels[i,1] = chr(ord('A') + i % 26)*5
     filename = 'test.wav'
     
     rm.write_wave(filename, data, rate, None, locs)
     llocs, llabels = rm.markers_riff(filename)
-    assert_equal(len(llabels), 0, 'no labels')
-    assert_true(np.all(locs == llocs), 'same locs')
+    assert len(llabels) == 0, 'no labels'
+    assert np.all(locs == llocs), 'same locs'
     
     rm.write_wave(filename, data, rate, None, locs[:,0])
     llocs, llabels = rm.markers_riff(filename)
-    assert_equal(len(llabels), 0, 'no labels')
-    assert_equal(len(llocs), len(locs), 'same number of locs')
-    assert_true(np.all(locs[:,0] == llocs[:,0]), 'same locs')
+    assert len(llabels) == 0, 'no labels'
+    assert len(llocs) == len(locs), 'same number of locs'
+    assert np.all(locs[:,0] == llocs[:,0]), 'same locs'
     
     rm.write_wave(filename, data, rate, None, locs, labels)
     llocs, llabels = rm.markers_riff(filename)
-    assert_true(np.all(locs == llocs), 'same locs')
-    assert_true(np.all(labels == llabels), 'same labels')
+    assert np.all(locs == llocs), 'same locs'
+    assert np.all(labels == llabels), 'same labels'
+    
+    rm.write_wave(filename, data, rate, None, locs, labels, marker_hint='cue')
+    llocs, llabels = rm.markers_riff(filename)
+    assert np.all(locs == llocs), 'same locs in cue lists'
+    assert np.all(labels == llabels), 'same labels in cue lists'
 
     with open(filename, 'rb') as sf:
         llocs, llabels = rm.markers_riff(sf)
-    assert_true(np.all(locs == llocs), 'same locs')
-    assert_true(np.all(labels == llabels), 'same labels')
+    assert np.all(locs == llocs), 'same locs'
+    assert np.all(labels == llabels), 'same labels'
+    
+    rm.write_wave(filename, data, rate, None, locs, labels, marker_hint='lbl')
+    llocs, llabels = rm.markers_riff(filename)
+    assert np.all(locs == llocs), 'same locs in lbl chunk'
+    assert np.all(labels[:,1] == llabels[:,1]), 'same texts in lbl chunk'
+    assert np.all(llabels[llocs[:,1] > 0,0] == 'M'), 'M labels in lbl chunk'
+    assert np.all(llabels[llocs[:,1] == 0,0] == labels[llocs[:,1] == 0,0]), 'same labels in lbl chunk'
     
-    assert_raises(IndexError, rm.write_wave, filename, data, rate,
-                  None, locs, labels[:-2,:])
+    with pytest.raises(IndexError):
+        rm.write_wave(filename, data, rate, None, locs, labels[:-2,:])
     
     rm.write_wave(filename, data, rate, None, locs, labels[:,0])
     llocs, llabels = rm.markers_riff(filename)
-    assert_true(np.all(locs == llocs), 'same locs')
-    assert_true(np.all(labels[:,0] == llabels[:,0]), 'same labels')
+    assert np.all(locs == llocs), 'same locs'
+    assert np.all(labels[:,0] == llabels[:,0]), 'same labels'
     
     rm.write_wave(filename, data, rate, None, locs[:,0], labels[:,0])
     llocs, llabels = rm.markers_riff(filename)
-    assert_true(np.all(locs[:,0] == llocs[:,0]), 'same locs')
-    assert_true(np.all(labels[:,0] == llabels[:,0]), 'same labels')
+    assert np.all(locs[:,0] == llocs[:,0]), 'same locs'
+    assert np.all(labels[:,0] == llabels[:,0]), 'same labels'
     
     labels = np.zeros((len(locs), 2), dtype=np.object_)
     rm.write_wave(filename, data, rate, None, locs, labels)
     llocs, llabels = rm.markers_riff(filename)
-    assert_true(np.all(locs == llocs), 'same locs')
-    assert_equal(len(llabels), 0, 'no labels')
+    assert np.all(locs == llocs), 'same locs'
+    assert len(llabels) == 0, 'no labels'
 
     locs[:,-1] = 0
     rm.write_wave(filename, data, rate, None, locs)
     llocs, llabels = rm.markers_riff(filename)
-    assert_equal(len(llabels), 0, 'no labels')
-    assert_true(np.all(locs == llocs), 'same locs')
+    assert len(llabels) == 0, 'no labels'
+    assert np.all(locs == llocs), 'same locs'
 
     os.remove(filename)
 
     
 def test_main():
     rm.main('-h')
     rm.main()
```

