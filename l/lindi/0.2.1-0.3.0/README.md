# Comparing `tmp/lindi-0.2.1.tar.gz` & `tmp/lindi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lindi-0.2.1.tar", max compression
+gzip compressed data, was "lindi-0.3.0.tar", max compression
```

## Comparing `lindi-0.2.1.tar` & `lindi-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.2.1/LICENSE
--rw-r--r--   0        0        0     5169 2024-04-16 15:35:00.582419 lindi-0.2.1/README.md
--rw-r--r--   0        0        0    28733 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
--rw-r--r--   0        0        0      136 2024-03-21 11:16:09.352672 lindi-0.2.1/lindi/LindiH5ZarrStore/__init__.py
--rw-r--r--   0        0        0     2886 2024-04-04 18:56:02.142012 lindi-0.2.1/lindi/LindiH5ZarrStore/_util.py
--rw-r--r--   0        0        0     3710 2024-04-04 18:56:02.142012 lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py
--rw-r--r--   0        0        0     1045 2024-03-21 18:16:58.794258 lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py
--rw-r--r--   0        0        0        0 2024-03-21 18:16:58.794258 lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/__init__.py
--rw-r--r--   0        0        0     3236 2024-04-04 18:56:02.142012 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py
--rw-r--r--   0        0        0    12266 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyDataset.py
--rw-r--r--   0        0        0    18016 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyFile.py
--rw-r--r--   0        0        0     8485 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyGroup.py
--rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyLink.py
--rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyReference.py
--rw-r--r--   0        0        0     7868 2024-04-16 15:35:00.582419 lindi-0.2.1/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
--rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.2.1/lindi/LindiH5pyFile/__init__.py
--rw-r--r--   0        0        0      747 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
--rw-r--r--   0        0        0     1961 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
--rw-r--r--   0        0        0     5349 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/LindiH5pyFile/writers/__init__.py
--rw-r--r--   0        0        0     9558 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/LindiStagingStore/LindiStagingStore.py
--rw-r--r--   0        0        0     2915 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/LindiStagingStore/StagingArea.py
--rw-r--r--   0        0        0       76 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/LindiStagingStore/__init__.py
--rw-r--r--   0        0        0      286 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/conversion/__init__.py
--rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/conversion/_util.py
--rw-r--r--   0        0        0     5907 2024-04-04 18:56:02.146012 lindi-0.2.1/lindi/conversion/attr_conversion.py
--rw-r--r--   0        0        0    10819 2024-04-16 15:35:00.586419 lindi-0.2.1/lindi/conversion/create_zarr_dataset_from_h5_data.py
--rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.2.1/lindi/conversion/decode_references.py
--rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.2.1/lindi/conversion/h5_filters_to_codecs.py
--rw-r--r--   0        0        0     2041 2024-04-15 15:43:24.681869 lindi-0.2.1/lindi/conversion/h5_ref_to_zarr_attr.py
--rw-r--r--   0        0        0      936 2024-04-15 12:47:02.787743 lindi-0.2.1/lindi/conversion/nan_inf_ninf.py
--rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.2.1/lindi/conversion/reformat_json.py
--rw-r--r--   0        0        0      748 2024-04-16 15:35:20.118151 lindi-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5869 1970-01-01 00:00:00.000000 lindi-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-03-13 15:25:45.816228 lindi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5269 2024-04-19 19:44:06.440621 lindi-0.3.0/README.md
+-rw-r--r--   0        0        0    28820 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py
+-rw-r--r--   0        0        0      136 2024-03-21 11:16:09.352672 lindi-0.3.0/lindi/LindiH5ZarrStore/__init__.py
+-rw-r--r--   0        0        0     3112 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5ZarrStore/_util.py
+-rw-r--r--   0        0        0     3710 2024-04-04 18:56:02.142012 lindi-0.3.0/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py
+-rw-r--r--   0        0        0     1045 2024-03-21 18:16:58.794258 lindi-0.3.0/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py
+-rw-r--r--   0        0        0        0 2024-03-21 18:16:58.794258 lindi-0.3.0/lindi/LindiH5pyFile/FileSegmentReader/__init__.py
+-rw-r--r--   0        0        0     2242 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyAttributes.py
+-rw-r--r--   0        0        0    11685 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyDataset.py
+-rw-r--r--   0        0        0    15606 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyFile.py
+-rw-r--r--   0        0        0     6051 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyGroup.py
+-rw-r--r--   0        0        0      255 2024-03-21 11:16:09.352672 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyLink.py
+-rw-r--r--   0        0        0      478 2024-04-04 18:56:02.146012 lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyReference.py
+-rw-r--r--   0        0        0    10388 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py
+-rw-r--r--   0        0        0      327 2024-03-21 11:16:09.352672 lindi-0.3.0/lindi/LindiH5pyFile/__init__.py
+-rw-r--r--   0        0        0      528 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py
+-rw-r--r--   0        0        0     1941 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py
+-rw-r--r--   0        0        0     6651 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.0/lindi/LindiH5pyFile/writers/__init__.py
+-rw-r--r--   0        0        0    10625 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiStagingStore/LindiStagingStore.py
+-rw-r--r--   0        0        0     2915 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiStagingStore/StagingArea.py
+-rw-r--r--   0        0        0       76 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/LindiStagingStore/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:56:02.146012 lindi-0.3.0/lindi/conversion/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-04 18:56:02.146012 lindi-0.3.0/lindi/conversion/_util.py
+-rw-r--r--   0        0        0     5907 2024-04-18 21:52:00.325839 lindi-0.3.0/lindi/conversion/attr_conversion.py
+-rw-r--r--   0        0        0    10819 2024-04-19 19:44:06.440621 lindi-0.3.0/lindi/conversion/create_zarr_dataset_from_h5_data.py
+-rw-r--r--   0        0        0     1079 2024-04-15 13:56:49.245944 lindi-0.3.0/lindi/conversion/decode_references.py
+-rw-r--r--   0        0        0     2887 2024-04-15 13:02:34.168232 lindi-0.3.0/lindi/conversion/h5_filters_to_codecs.py
+-rw-r--r--   0        0        0     2041 2024-04-19 14:03:48.185150 lindi-0.3.0/lindi/conversion/h5_ref_to_zarr_attr.py
+-rw-r--r--   0        0        0      936 2024-04-18 21:52:00.325839 lindi-0.3.0/lindi/conversion/nan_inf_ninf.py
+-rw-r--r--   0        0        0      503 2024-04-15 12:44:19.013722 lindi-0.3.0/lindi/conversion/reformat_json.py
+-rw-r--r--   0        0        0      748 2024-04-19 19:44:21.692431 lindi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5969 1970-01-01 00:00:00.000000 lindi-0.3.0/PKG-INFO
```

### Comparing `lindi-0.2.1/LICENSE` & `lindi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/README.md` & `lindi-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: lindi
+Version: 0.3.0
+Summary: 
+Author: Jeremy Magland
+Author-email: jmagland@flatironinstitute.org
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: h5py (>=3.10.0,<4.0.0)
+Requires-Dist: numcodecs (>=0.12.1,<0.13.0)
+Requires-Dist: remfile (>=0.1.9,<0.2.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: zarr (>=2.16.1,<3.0.0)
+Description-Content-Type: text/markdown
+
 # LINDI - Linked Data Interface
 
 [![latest-release](https://img.shields.io/pypi/v/lindi.svg)](https://pypi.org/project/lindi)
 ![tests](https://github.com/neurodatawithoutborders/lindi/actions/workflows/integration_tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/neurodatawithoutborders/lindi/branch/main/graph/badge.svg?token=xxxx)](https://codecov.io/gh/neurodatawithoutborders/lindi)
 
 :warning: Please note, LINDI is currently under development and should not yet be used in practice.
@@ -10,15 +30,15 @@
 
 LINDI provides a JSON representation of NWB (Neurodata Without Borders) data where the large data chunks are stored separately from the main metadata. This enables efficient storage, composition, and sharing of NWB files on cloud systems such as [DANDI](https://www.dandiarchive.org/) without duplicating the large data blobs.
 
 LINDI provides:
 
 - A specification for representing arbitrary HDF5 files as Zarr stores. This handles scalar datasets, references, soft links, and compound data types for datasets.
 - A Zarr wrapper for remote or local HDF5 files (LindiH5ZarrStore).
-- A mechanism for creating .zarr.json (or .nwb.json) files that reference data chunks in external files, inspired by [kerchunk](https://github.com/fsspec/kerchunk).
+- A mechanism for creating .lindi.json (or .nwb.lindi.json) files that reference data chunks in external files, inspired by [kerchunk](https://github.com/fsspec/kerchunk).
 - An h5py-like interface for reading from and writing to these data sources that can be used with [pynwb](https://pynwb.readthedocs.io/en/stable/).
 - A mechanism for uploading and downloading these data sources to and from cloud storage, including DANDI.
 
 This project was inspired by [kerchunk](https://github.com/fsspec/kerchunk) and [hdmf-zarr](https://hdmf-zarr.readthedocs.io/en/latest/index.html) and depends on [zarr](https://zarr.readthedocs.io/en/stable/), [h5py](https://www.h5py.org/), [remfile](https://github.com/magland/remfile) and [numcodecs](https://numcodecs.readthedocs.io/en/stable/).
 
 ## Installation
 
@@ -31,21 +51,21 @@
 ```bash
 cd lindi
 pip install -e .
 ```
 
 ## Use cases
 
-* Represent a remote NWB/HDF5 file as a .nwb.json file.
-* Read a local or remote .nwb.json file using pynwb or other tools.
-* Edit a .nwb.json file using pynwb or other tools.
-* Add datasets to a .nwb.json file using a local staging area.
-* Upload a .nwb.json file to a cloud storage service such as DANDI.
+* Represent a remote NWB/HDF5 file as a .nwb.lindi.json file.
+* Read a local or remote .nwb.lindi.json file using pynwb or other tools.
+* Edit a .nwb.lindi.json file using pynwb or other tools.
+* Add datasets to a .nwb.lindi.json file using a local staging area.
+* Upload a .nwb.lindi.json file to a cloud storage service such as DANDI.
 
-### Represent a remote NWB/HDF5 file as a .nwb.json file
+### Represent a remote NWB/HDF5 file as a .nwb.lindi.json file
 
 ```python
 import json
 import pynwb
 import lindi
 
 # URL of the remote NWB file
@@ -54,91 +74,91 @@
 # Create a read-only Zarr store as a wrapper for the h5 file
 store = lindi.LindiH5ZarrStore.from_file(h5_url)
 
 # Generate a reference file system
 rfs = store.to_reference_file_system()
 
 # Save it to a file for later use
-with open("example.zarr.json", "w") as f:
+with open("example.lindi.json", "w") as f:
     json.dump(rfs, f, indent=2)
 
 # Create an h5py-like client from the reference file system
 client = lindi.LindiH5pyFile.from_reference_file_system(rfs)
 
 # Open using pynwb
 with pynwb.NWBHDF5IO(file=client, mode="r") as io:
     nwbfile = io.read()
     print(nwbfile)
 ```
 
-### Read a local or remote .nwb.json file using pynwb or other tools
+### Read a local or remote .nwb.lindi.json file using pynwb or other tools
 
 ```python
 import pynwb
 import lindi
 
-# URL of the remote .zarr.json file
+# URL of the remote .nwb.lindi.json file
 url = 'https://kerchunk.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
 
 # Load the h5py-like client for the reference file system
 client = lindi.LindiH5pyFile.from_reference_file_system(url)
 
 # Open using pynwb
 with pynwb.NWBHDF5IO(file=client, mode="r") as io:
     nwbfile = io.read()
     print(nwbfile)
 ```
 
-### Edit a .nwb.json file using pynwb or other tools
+### Edit a .nwb.lindi.json file using pynwb or other tools
 
 ```python
 import json
 import lindi
 
-# URL of the remote .zarr.json file
+# URL of the remote .nwb.lindi.json file
 url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
 
 # Load the h5py-like client for the reference file system
 # in read-write mode
 client = lindi.LindiH5pyFile.from_reference_file_system(url, mode="r+")
 
 # Edit an attribute
 client.attrs['new_attribute'] = 'new_value'
 
-# Save the changes to a new .nwb.json file
+# Save the changes to a new .nwb.lindi.json file
 rfs_new = client.to_reference_file_system()
-with open('new.nwb.json', 'w') as f:
+with open('new.nwb.lindi.json', 'w') as f:
     f.write(json.dumps(rfs_new, indent=2, sort_keys=True))
 ```
 
-### Add datasets to a .nwb.json file using a local staging area
+### Add datasets to a .nwb.lindi.json file using a local staging area
 
 ```python
 import lindi
 
-# URL of the remote .zarr.json file
+# URL of the remote .nwb.lindi.json file
 url = 'https://lindi.neurosift.org/dandi/dandisets/000939/assets/11f512ba-5bcf-4230-a8cb-dc8d36db38cb/zarr.json'
 
 # Load the h5py-like client for the reference file system
 # in read-write mode with a staging area
 with lindi.StagingArea.create(base_dir='lindi_staging') as staging_area:
     client = lindi.LindiH5pyFile.from_reference_file_system(
         url,
         mode="r+",
         staging_area=staging_area
     )
     # add datasets to client using pynwb or other tools
-    # upload the changes to the remote .nwb.json file
+    # upload the changes to the remote .nwb.lindi.json file
 ```
 
-### Upload a .nwb.json file to a cloud storage service such as DANDI
+### Upload a .nwb.lindi.json file to a cloud storage service such as DANDI
 
 See [this example](https://github.com/magland/lindi-dandi/blob/main/devel/lindi_test_2.py).
 
-
 ## For developers
 
 [Special Zarr annotations used by LINDI](docs/special_zarr_annotations.md)
 
 ## License
 
 See [LICENSE](LICENSE).
+
```

### Comparing `lindi-0.2.1/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py` & `lindi-0.3.0/lindi/LindiH5ZarrStore/LindiH5ZarrStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import json
 import base64
-from typing import Union, List, IO, Any, Dict, Literal
+from typing import Union, List, IO, Any, Dict
 from dataclasses import dataclass
 import numpy as np
 import zarr
 import remfile
 from zarr.storage import Store, MemoryStore
 import h5py
 from ._util import (
     _read_bytes,
     _get_chunk_byte_range,
     _get_byte_range_for_contiguous_dataset,
     _join,
-    _get_chunk_names_for_dataset
+    _get_chunk_names_for_dataset,
+    _write_rfs_to_file,
 )
 from ..conversion.attr_conversion import h5_to_zarr_attr
 from ..conversion.reformat_json import reformat_json
 from ..conversion.h5_filters_to_codecs import h5_filters_to_codecs
 from ..conversion.create_zarr_dataset_from_h5_data import create_zarr_dataset_from_h5_data
 from ..LindiH5pyFile.LindiReferenceFileSystemStore import LindiReferenceFileSystemStore
 
@@ -456,25 +457,25 @@
             return ret
         elif isinstance(item, h5py.Dataset):
             # Datasets do not have subdirectories
             return []
         else:
             return []
 
-    def to_file(self, file_name: str, *, file_type: Literal["zarr.json"] = "zarr.json"):
+    def write_reference_file_system(self, output_file_name: str):
         """Write a reference file system corresponding to this store to a file.
 
         This can then be loaded using LindiH5pyFile.from_reference_file_system(file_name)
         """
-        if file_type != "zarr.json":
-            raise Exception(f"Unsupported file type: {file_type}")
 
-        ret = self.to_reference_file_system()
-        with open(file_name, "w") as f:
-            json.dump(ret, f, indent=2)
+        if not output_file_name.endswith(".lindi.json"):
+            raise Exception("The output file name must end with .lindi.json")
+
+        rfs = self.to_reference_file_system()
+        _write_rfs_to_file(rfs=rfs, output_file_name=output_file_name)
 
     def to_reference_file_system(self) -> dict:
         """Create a reference file system corresponding to this store.
 
         This can then be loaded using LindiH5pyFile.from_reference_file_system(obj)
         """
         if self._h5f is None:
@@ -574,15 +575,16 @@
                             byte_offset,
                             byte_count,
                         ]
 
         # Process the groups recursively starting with the root group
         _process_group("", self._h5f)
 
-        LindiReferenceFileSystemStore.replace_meta_file_contents_with_dicts(ret)
+        LindiReferenceFileSystemStore.replace_meta_file_contents_with_dicts_in_rfs(ret)
+        LindiReferenceFileSystemStore.use_templates_in_rfs(ret)
         return ret
 
 
 class InlineArray:
     def __init__(self, h5_dataset: h5py.Dataset):
         self._additional_zarr_attributes = {}
         if h5_dataset.shape == ():
```

### Comparing `lindi-0.2.1/lindi/LindiH5ZarrStore/_util.py` & `lindi-0.3.0/lindi/LindiH5ZarrStore/_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import IO, List
+import json
 import numpy as np
 import h5py
 
 
 def _read_bytes(file: IO, offset: int, count: int):
     """Read a range of bytes from a file-like object."""
     file.seek(offset)
@@ -79,7 +80,14 @@
     else:
         names0 = _get_chunk_names_for_dataset(chunk_coords_shape[1:])
         names = []
         for i in range(chunk_coords_shape[0]):
             for name0 in names0:
                 names.append(f"{i}.{name0}")
         return names
+
+
+def _write_rfs_to_file(*, rfs: dict, output_file_name: str):
+    """Write a reference file system to a file.
+    """
+    with open(output_file_name, "w") as f:
+        json.dump(rfs, f, indent=2, sort_keys=True)
```

### Comparing `lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py` & `lindi-0.3.0/lindi/LindiH5pyFile/FileSegmentReader/DandiFileSegmentReader.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py` & `lindi-0.3.0/lindi/LindiH5pyFile/FileSegmentReader/FileSegmentReader.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyAttributes.py` & `lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyAttributes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Literal
 from .LindiH5pyReference import LindiH5pyReference
 from ..conversion.attr_conversion import zarr_to_h5_attr
 from ..conversion.nan_inf_ninf import decode_nan_inf_ninf
 from .writers.LindiH5pyAttributesWriter import LindiH5pyAttributesWriter
 
 _special_attribute_keys = [
     "_SCALAR",
@@ -10,82 +9,61 @@
     "_REFERENCE",
     "_EXTERNAL_ARRAY_LINK",
     "_SOFT_LINK",
 ]
 
 
 class LindiH5pyAttributes:
-    def __init__(self, attrs, attrs_type: Literal["h5py", "zarr"], readonly: bool):
+    def __init__(self, attrs, readonly: bool):
         self._attrs = attrs
-        self._attrs_type = attrs_type
         self._readonly = readonly
 
         if self._readonly:
             self._writer = None
         else:
             self._writer = LindiH5pyAttributesWriter(self)
 
     def get(self, key, default=None):
-        if self._attrs_type == "h5py":
-            return self._attrs.get(key, default)
-        elif self._attrs_type == "zarr":
-            try:
-                if key in _special_attribute_keys:
-                    raise KeyError
-                return self[key]
-            except KeyError:
-                return default
-        else:
-            raise ValueError(f"Unknown attrs_type: {self._attrs_type}")
+        try:
+            if key in _special_attribute_keys:
+                raise KeyError
+            return self[key]
+        except KeyError:
+            return default
 
     def __contains__(self, key):
-        if self._attrs_type == "h5py":
-            return key in self._attrs
-        elif self._attrs_type == "zarr":
-            if key in _special_attribute_keys:
-                return False
-            return key in self._attrs
-        else:
-            raise ValueError(f"Unknown attrs_type: {self._attrs_type}")
+        if key in _special_attribute_keys:
+            return False
+        return key in self._attrs
 
     def __getitem__(self, key):
         val = self._attrs[key]
-        if self._attrs_type == "h5py":
-            return val
-        elif self._attrs_type == "zarr":
-            if isinstance(val, dict) and "_REFERENCE" in val:
-                return LindiH5pyReference(val["_REFERENCE"])
-
-            # Convert special float values to actual floats (NaN, Inf, -Inf)
-            # Note that string versions of these values are not supported
-            val = decode_nan_inf_ninf(val)
+        if isinstance(val, dict) and "_REFERENCE" in val:
+            return LindiH5pyReference(val["_REFERENCE"])
 
-            return zarr_to_h5_attr(val)
-        else:
-            raise ValueError(f"Unknown attrs_type: {self._attrs_type}")
+        # Convert special float values to actual floats (NaN, Inf, -Inf)
+        # Note that string versions of these values are not supported
+        val = decode_nan_inf_ninf(val)
+
+        return zarr_to_h5_attr(val)
 
     def __setitem__(self, key, value):
         if self._readonly:
             raise ValueError("Cannot set items on read-only object")
         assert self._writer is not None
         self._writer.__setitem__(key, value)
 
     def __delitem__(self, key):
         raise KeyError("Cannot delete attributes on read-only object")
 
     def __iter__(self):
-        if self._attrs_type == "h5py":
-            return self._attrs.__iter__()
-        elif self._attrs_type == "zarr":
-            # Do not return special zarr attributes during iteration
-            for k in self._attrs:
-                if k not in _special_attribute_keys:
-                    yield k
-        else:
-            raise ValueError(f"Unknown attrs_type: {self._attrs_type}")
+        # Do not return special zarr attributes during iteration
+        for k in self._attrs:
+            if k not in _special_attribute_keys:
+                yield k
 
     def items(self):
         for k in self:
             yield k, self[k]
 
     def __len__(self):
         ct = 0
```

### Comparing `lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyDataset.py` & `lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyDataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Union, Any, Dict
+from typing import TYPE_CHECKING, Any, Dict
 import numpy as np
 import h5py
 import zarr
 import remfile
 
 from .LindiH5pyAttributes import LindiH5pyAttributes
 from .LindiH5pyReference import LindiH5pyReference
@@ -18,53 +18,47 @@
 # possibly multiple LindiH5pyFile objects. The key is the URL of the
 # external hdf5 file, and the value is the h5py.File object.
 # TODO: figure out how to close these clients
 _external_hdf5_clients: Dict[str, h5py.File] = {}
 
 
 class LindiH5pyDataset(h5py.Dataset):
-    def __init__(self, _dataset_object: Union[h5py.Dataset, zarr.Array], _file: "LindiH5pyFile"):
-        self._dataset_object = _dataset_object
+    def __init__(self, _zarr_array: zarr.Array, _file: "LindiH5pyFile"):
+        self._zarr_array = _zarr_array
         self._file = _file
         self._readonly = _file.mode not in ['r+']
 
         # see comment in LindiH5pyGroup
-        self._id = f'{id(self._file)}/{self._dataset_object.name}'
+        self._id = f'{id(self._file)}/{self._zarr_array.name}'
 
         # See if we have the _COMPOUND_DTYPE attribute, which signifies that
         # this is a compound dtype
-        if isinstance(_dataset_object, zarr.Array):
-            compound_dtype_obj = _dataset_object.attrs.get("_COMPOUND_DTYPE", None)
-            if compound_dtype_obj is not None:
-                assert isinstance(compound_dtype_obj, list)
-                # compound_dtype_obj is a list of tuples (name, dtype)
-                # where dtype == "<REFERENCE>" if it represents an HDF5 reference
-                for i in range(len(compound_dtype_obj)):
-                    if compound_dtype_obj[i][1] == '<REFERENCE>':
-                        compound_dtype_obj[i][1] = h5py.special_dtype(ref=h5py.Reference)
-                # If we have a compound dtype, then create the numpy dtype
-                self._compound_dtype = np.dtype(
-                    [
-                        (
-                            compound_dtype_obj[i][0],
-                            compound_dtype_obj[i][1]
-                        )
-                        for i in range(len(compound_dtype_obj))
-                    ]
-                )
-            else:
-                self._compound_dtype = None
+        compound_dtype_obj = _zarr_array.attrs.get("_COMPOUND_DTYPE", None)
+        if compound_dtype_obj is not None:
+            assert isinstance(compound_dtype_obj, list)
+            # compound_dtype_obj is a list of tuples (name, dtype)
+            # where dtype == "<REFERENCE>" if it represents an HDF5 reference
+            for i in range(len(compound_dtype_obj)):
+                if compound_dtype_obj[i][1] == '<REFERENCE>':
+                    compound_dtype_obj[i][1] = h5py.special_dtype(ref=h5py.Reference)
+            # If we have a compound dtype, then create the numpy dtype
+            self._compound_dtype = np.dtype(
+                [
+                    (
+                        compound_dtype_obj[i][0],
+                        compound_dtype_obj[i][1]
+                    )
+                    for i in range(len(compound_dtype_obj))
+                ]
+            )
         else:
             self._compound_dtype = None
 
         # Check whether this is a scalar dataset
-        if isinstance(_dataset_object, zarr.Array):
-            self._is_scalar = self._dataset_object.attrs.get("_SCALAR", False)
-        else:
-            self._is_scalar = self._dataset_object.ndim == 0
+        self._is_scalar = self._zarr_array.attrs.get("_SCALAR", False)
 
         # The self._write object handles all the writing operations
         from .writers.LindiH5pyDatasetWriter import LindiH5pyDatasetWriter  # avoid circular import
 
         if self._readonly:
             self._writer = None
         else:
@@ -75,112 +69,109 @@
         # see comment in LindiH5pyGroup
         return self._id
 
     @property
     def shape(self):  # type: ignore
         if self._is_scalar:
             return ()
-        return self._dataset_object.shape
+        return self._zarr_array.shape
 
     @property
     def size(self):
         if self._is_scalar:
             return 1
-        return self._dataset_object.size
+        return self._zarr_array.size
 
     @property
     def dtype(self):
         if self._compound_dtype is not None:
             return self._compound_dtype
-        ret = self._dataset_object.dtype
+        ret = self._zarr_array.dtype
         if ret.kind == 'O':
             if not ret.metadata:
                 # The following correction is needed because of
                 # this code in hdmf/backends/hdf5/h5tools.py:
                 # def _check_str_dtype(self, h5obj):
                 #     dtype = h5obj.dtype
                 #     if dtype.kind == 'O':
                 #         if dtype.metadata.get('vlen') == str and H5PY_3:
                 #             return StrDataset(h5obj, None)
                 #     return h5obj
                 # We cannot have a dtype with kind 'O' and no metadata
-                ret = np.dtype(str(ret), metadata={})
+                # There is also this section in pynwb validator.py
+                # if isinstance(received, np.dtype):
+                #     if received.char == 'O':
+                #         if 'vlen' in received.metadata:
+                #             received = received.metadata['vlen']
+                #         else:
+                #             raise ValueError("Unrecognized type: '%s'" % received)
+                #         received = 'utf' if received is str else 'ascii'
+                #     elif received.char == 'U':
+                #         received = 'utf'
+                #     elif received.char == 'S':
+                #         received = 'ascii'
+                #     else:
+                #         received = received.name
+                # ------------------------------------------
+                # I don't know how to figure out when vlen should be str or bytes
+                # but validate seems to work only when I put in vlen = bytes
+                #
+                vlen = bytes
+                ret = np.dtype(str(ret), metadata={'vlen': vlen})
         return ret
 
     @property
     def nbytes(self):
-        return self._dataset_object.nbytes
+        return self._zarr_array.nbytes
 
     @property
     def file(self):
         return self._file
 
     @property
     def name(self):
-        return self._dataset_object.name
+        return self._zarr_array.name
 
     @property
     def maxshape(self):
         # not sure what to return here, so let's return self.shape rather than self._h5py_dataset.maxshape
         # return self._h5py_dataset.maxshape
         return self.shape
 
     @property
     def ndim(self):
         if self._is_scalar:
             return 0
-        return self._dataset_object.ndim
+        return self._zarr_array.ndim
 
     @property
     def attrs(self):  # type: ignore
-        if isinstance(self._dataset_object, h5py.Dataset):
-            attrs_type = 'h5py'
-        elif isinstance(self._dataset_object, zarr.Array):
-            attrs_type = 'zarr'
-        else:
-            raise Exception(f'Unexpected dataset object type: {type(self._dataset_object)}')
-        return LindiH5pyAttributes(self._dataset_object.attrs, attrs_type=attrs_type, readonly=self._file.mode == 'r')
+        return LindiH5pyAttributes(self._zarr_array.attrs, readonly=self._file.mode == 'r')
 
     @property
     def fletcher32(self):
-        if isinstance(self._dataset_object, h5py.Dataset):
-            return self._dataset_object.fletcher32
-        elif isinstance(self._dataset_object, zarr.Array):
-            for f in self._dataset_object.filters:
-                if f.__class__.__name__ == 'Fletcher32':
-                    return True
-            return False
-        else:
-            raise Exception(f'Unexpected dataset object type: {type(self._dataset_object)}')
+        for f in self._zarr_array.filters:
+            if f.__class__.__name__ == 'Fletcher32':
+                return True
+        return False
 
     @property
     def chunks(self):
-        if isinstance(self._dataset_object, h5py.Dataset):
-            return self._dataset_object.chunks
-        elif isinstance(self._dataset_object, zarr.Array):
-            return self._dataset_object.chunks
-        else:
-            raise Exception(f'Unexpected dataset object type: {type(self._dataset_object)}')
+        return self._zarr_array.chunks
 
     def __repr__(self):  # type: ignore
         return f"<{self.__class__.__name__}: {self.name}>"
 
     def __str__(self):
         return f"<{self.__class__.__name__}: {self.name}>"
 
     def __getitem__(self, args, new_dtype=None):
-        if isinstance(self._dataset_object, h5py.Dataset):
-            ret = self._dataset_object.__getitem__(args, new_dtype)
-        elif isinstance(self._dataset_object, zarr.Array):
-            if new_dtype is not None:
-                raise Exception("new_dtype is not supported for zarr.Array")
-            ret = self._get_item_for_zarr(self._dataset_object, args)
-        else:
-            raise Exception(f"Unexpected type: {type(self._dataset_object)}")
-        return ret
+        if new_dtype is not None:
+            raise Exception("new_dtype is not supported for zarr.Array")
+        return self._get_item_for_zarr(self._zarr_array, args)
 
     def _get_item_for_zarr(self, zarr_array: zarr.Array, selection: Any):
         # First check whether this is an external array link
         external_array_link = zarr_array.attrs.get("_EXTERNAL_ARRAY_LINK", None)
         if external_array_link and isinstance(external_array_link, dict):
             link_type = external_array_link.get("link_type", None)
             if link_type == 'hdf5_dataset':
@@ -262,19 +253,19 @@
         self._ind = ind  # The index of the field in the compound dtype
         self._dtype = dtype  # The dtype of the field
         if self._dataset.ndim != 1:
             # For now we only support 1D datasets
             raise TypeError(
                 f"Compound field selection only implemented for 1D datasets, not {self._dataset.ndim}D"
             )
-        if not isinstance(self._dataset._dataset_object, zarr.Array):
+        if not isinstance(self._dataset._zarr_array, zarr.Array):
             raise TypeError(
-                f"Compound field selection only implemented for zarr.Array, not {type(self._dataset._dataset_object)}"
+                f"Compound field selection only implemented for zarr.Array, not {type(self._dataset._zarr_array)}"
             )
-        za = self._dataset._dataset_object
+        za = self._dataset._zarr_array
         self._zarr_array = za
         # Prepare the data in memory
         d = [za[i][self._ind] for i in range(len(za))]
         if self._dtype == h5py.Reference:
             # Convert to LindiH5pyReference
             # Every element in the selection should be a reference dict
             d = [LindiH5pyReference(x['_REFERENCE']) for x in d]
```

### Comparing `lindi-0.2.1/lindi/LindiH5pyFile/LindiH5pyFile.py` & `lindi-0.3.0/lindi/LindiH5pyFile/LindiH5pyFile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 from typing import Union, Literal
 import json
 import tempfile
 import urllib.request
 import h5py
 import zarr
 from zarr.storage import Store as ZarrStore
-from numcodecs.abc import Codec
 
 from .LindiH5pyGroup import LindiH5pyGroup
-from .LindiH5pyDataset import LindiH5pyDataset
 from .LindiH5pyAttributes import LindiH5pyAttributes
 from .LindiH5pyReference import LindiH5pyReference
 from .LindiReferenceFileSystemStore import LindiReferenceFileSystemStore
 
 from ..LindiStagingStore.StagingArea import StagingArea
 from ..LindiStagingStore.LindiStagingStore import LindiStagingStore
 
 
 class LindiH5pyFile(h5py.File):
-    def __init__(self, _file_object: Union[h5py.File, zarr.Group], *, _zarr_store: Union[ZarrStore, None] = None, _mode: Literal["r", "r+"] = "r"):
+    def __init__(self, _zarr_group: zarr.Group, *, _zarr_store: Union[ZarrStore, None] = None, _mode: Literal["r", "r+"] = "r"):
         """
         Do not use this constructor directly. Instead, use:
         from_reference_file_system, from_zarr_store, from_zarr_group,
         or from_h5py_file
         """
-        self._file_object = _file_object
+        self._zarr_group = _zarr_group
         self._zarr_store = _zarr_store
         self._mode: Literal['r', 'r+'] = _mode
-        self._the_group = LindiH5pyGroup(_file_object, self)
+        self._the_group = LindiH5pyGroup(_zarr_group, self)
 
         # see comment in LindiH5pyGroup
-        self._id = f'{id(self._file_object)}/'
+        self._id = f'{id(self._zarr_group)}/'
 
     @staticmethod
     def from_reference_file_system(rfs: Union[dict, str], mode: Literal["r", "r+"] = "r", staging_area: Union[StagingArea, None] = None):
         """
         Create a LindiH5pyFile from a reference file system.
 
         Parameters
         ----------
         rfs : Union[dict, str]
             The reference file system. This can be a dictionary or a URL or path
-            to a .zarr.json file.
+            to a .lindi.json file.
         mode : Literal["r", "r+"], optional
             The mode to open the file object in, by default "r". If the mode is
             "r", the file object will be read-only. If the mode is "r+", the
             file will be read-write. However, if the rfs is a string (URL or
             path), the file itself will not be modified on changes, but the
             internal in-memory representation will be modified. Use
             to_reference_file_system() to export the updated reference file
@@ -54,15 +52,15 @@
         if staging_area is not None:
             if mode not in ['r+']:
                 raise Exception("Staging area cannot be used in read-only mode")
 
         if isinstance(rfs, str):
             if rfs.startswith("http") or rfs.startswith("https"):
                 with tempfile.TemporaryDirectory() as tmpdir:
-                    filename = f"{tmpdir}/temp.zarr.json"
+                    filename = f"{tmpdir}/temp.lindi.json"
                     _download_file(rfs, filename)
                     with open(filename, "r") as f:
                         data = json.load(f)
                     assert isinstance(data, dict)  # prevent infinite recursion
                     return LindiH5pyFile.from_reference_file_system(data, mode=mode, staging_area=staging_area)
             else:
                 with open(rfs, "r") as f:
@@ -115,62 +113,40 @@
             The zarr store, internally set for use with
             to_reference_file_system().
 
         See from_zarr_store().
         """
         return LindiH5pyFile(zarr_group, _zarr_store=_zarr_store, _mode=mode)
 
-    @staticmethod
-    def from_h5py_file(h5py_file: h5py.File):
-        """
-        Create a LindiH5pyFile from an h5py file.
-
-        This is used mainly for testing and may be removed in the future.
-
-        Parameters
-        ----------
-        h5py_file : h5py.File
-            The h5py file.
-        """
-        return LindiH5pyFile(h5py_file)
-
     def to_reference_file_system(self):
         """
         Export the internal in-memory representation to a reference file system.
         In order to use this, the file object needs to have been created using
         from_reference_file_system().
         """
         if self._zarr_store is None:
             raise Exception("Cannot convert to reference file system without zarr store")
-        if not isinstance(self._zarr_store, LindiReferenceFileSystemStore):
+        zarr_store = self._zarr_store
+        if isinstance(zarr_store, LindiStagingStore):
+            zarr_store = zarr_store._base_store
+        if not isinstance(zarr_store, LindiReferenceFileSystemStore):
             raise Exception(f"Unexpected type for zarr store: {type(self._zarr_store)}")
-        rfs = self._zarr_store.rfs
+        rfs = zarr_store.rfs
         rfs_copy = json.loads(json.dumps(rfs))
-        LindiReferenceFileSystemStore.replace_meta_file_contents_with_dicts(rfs_copy)
+        LindiReferenceFileSystemStore.replace_meta_file_contents_with_dicts_in_rfs(rfs_copy)
+        LindiReferenceFileSystemStore.use_templates_in_rfs(rfs_copy)
         return rfs_copy
 
     @property
     def attrs(self):  # type: ignore
-        if isinstance(self._file_object, h5py.File):
-            attrs_type = 'h5py'
-        elif isinstance(self._file_object, zarr.Group):
-            attrs_type = 'zarr'
-        else:
-            raise Exception(f'Unexpected file object type: {type(self._file_object)}')
-        return LindiH5pyAttributes(self._file_object.attrs, attrs_type=attrs_type, readonly=self.mode == "r")
+        return LindiH5pyAttributes(self._zarr_group.attrs, readonly=self.mode == "r")
 
     @property
     def filename(self):
-        # This is not a string, but this is what h5py seems to do
-        if isinstance(self._file_object, h5py.File):
-            return self._file_object.filename
-        elif isinstance(self._file_object, zarr.Group):
-            return ''
-        else:
-            raise Exception(f"Unhandled type for file object: {type(self._file_object)}")
+        return ''
 
     @property
     def driver(self):
         raise Exception("Getting driver is not allowed")
 
     @property
     def mode(self):
@@ -192,44 +168,35 @@
         raise Exception("Getting swmr_mode is not allowed")
 
     def close(self):
         # Nothing was opened, so nothing needs to be closed
         pass
 
     def flush(self):
-        if isinstance(self._file_object, h5py.File):
-            return self._file_object.flush()
+        pass
 
     def __enter__(self):  # type: ignore
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def __str__(self):
-        return f'<LindiH5pyFile "{self._file_object}">'
+        return f'<LindiH5pyFile "{self._zarr_group}">'
 
     def __repr__(self):
-        return f'<LindiH5pyFile "{self._file_object}">'
+        return f'<LindiH5pyFile "{self._zarr_group}">'
 
     def __bool__(self):
         # This is called when checking if the file is open
-        if isinstance(self._file_object, h5py.File):
-            return self._file_object.__bool__()
-        elif isinstance(self._file_object, zarr.Group):
-            return True
-        else:
-            raise Exception(f"Unexpected type for file object: {type(self._file_object)}")
+        return True
 
     def __hash__(self):
         # This is called for example when using a file as a key in a dictionary
-        if isinstance(self._file_object, h5py.File):
-            return self._file_object.__hash__()
-        else:
-            return id(self)
+        return id(self)
 
     def copy(self, source, dest, name=None,
              shallow=False, expand_soft=False, expand_external=False,
              expand_refs=False, without_attrs=False):
         if shallow:
             raise Exception("shallow is not implemented for copy")
         if expand_soft:
@@ -254,38 +221,28 @@
         del grp[name.split('/')[-1]]
 
     # Group methods
     def __getitem__(self, name):  # type: ignore
         return self._get_item(name)
 
     def _get_item(self, name, getlink=False, default=None):
-        if isinstance(name, LindiH5pyReference) and isinstance(self._file_object, zarr.Group):
+        if isinstance(name, LindiH5pyReference):
             if getlink:
                 raise Exception("Getting link is not allowed for references")
-            zarr_group = self._file_object
+            zarr_group = self._zarr_group
             if name._source != '.':
                 raise Exception(f'For now, source of reference must be ".", got "{name._source}"')
             if name._source_object_id is not None:
                 if name._source_object_id != zarr_group.attrs.get("object_id"):
                     raise Exception(f'Mismatch in source object_id: "{name._source_object_id}" and "{zarr_group.attrs.get("object_id")}"')
             target = self[name._path]
             if name._object_id is not None:
                 if name._object_id != target.attrs.get("object_id"):
                     raise Exception(f'Mismatch in object_id: "{name._object_id}" and "{target.attrs.get("object_id")}"')
             return target
-        elif isinstance(name, h5py.Reference) and isinstance(self._file_object, h5py.File):
-            if getlink:
-                raise Exception("Getting link is not allowed for references")
-            x = self._file_object[name]
-            if isinstance(x, h5py.Group):
-                return LindiH5pyGroup(x, self)
-            elif isinstance(x, h5py.Dataset):
-                return LindiH5pyDataset(x, self)
-            else:
-                raise Exception(f"Unexpected type for resolved reference at path {name}: {type(x)}")
         # if it contains slashes, it's a path
         if isinstance(name, str) and "/" in name:
             parts = name.split("/")
             x = self._the_group
             for i, part in enumerate(parts):
                 if i == len(parts) - 1:
                     assert isinstance(x, LindiH5pyGroup)
@@ -356,28 +313,14 @@
     @property
     def staging_store(self):
         store = self._zarr_store
         if not isinstance(store, LindiStagingStore):
             return None
         return store
 
-    def create_dataset_with_zarr_compressor(
-        self,
-        name,
-        shape=None,
-        dtype=None,
-        data=None,
-        *,
-        compressor: Union[Codec, Literal['default']] = 'default',
-        **kwds
-    ):
-        if self._mode not in ['r+']:
-            raise Exception("Cannot create dataset in read-only mode")
-        return self._the_group.create_dataset_with_zarr_compressor(name, shape=shape, dtype=dtype, data=data, compressor=compressor, **kwds)
-
 
 def _download_file(url: str, filename: str) -> None:
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3"
     }
     req = urllib.request.Request(url, headers=headers)
     with urllib.request.urlopen(req) as response:
```

### Comparing `lindi-0.2.1/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py` & `lindi-0.3.0/lindi/LindiH5pyFile/LindiReferenceFileSystemStore.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,23 +30,41 @@
     (https://fsspec.github.io/kerchunk/spec.html), the reference file system is
     specified as a dictionary with a "refs" key. The value of "refs" is a
     dictionary where the keys are the names of the files and each value is
     either a string, a list, or a dict. If the value is a string, it is assumed
     to be the data of the file, which may be base64 encoded (see below). If the
     value is a list, it is assumed to have three elements: the URL of the file
     (or path of a local file), the byte offset of the data within the file, and
-    the byte length of the data. If the value is a dict, it represents a json
-    file, and the content of the file is the json representation of the dict.
+    the byte length of the data. Note that we do not permit the case of a list
+    of a single (url) element supported by fsspec, because it is good to be able
+    to know the size of the chunks without making a request to the file. If the
+    value is a dict, it represents a json file, and the content of the file is
+    the json representation of the dict.
 
     If the value for a file is a string, it may be prefixed with "base64:". If
     it is, the string is assumed to be base64 encoded and is decoded before
     being returned. Otherwise, the string is utf-8 encoded and returned as is.
     Note that a file that actually begins with "base64:" should be represented
     by a base64 encoded string, to avoid ambiguity.
 
+    We also support the use of templates as in fsspec, but do not support the
+    full jinja2 templating. There may be an optional "templates" key in the
+    dictionary, which is a dictionary of template strings. For example,
+    {
+        "templates": {"u1": "https://some/url", "u2": "https://some/other/url"},
+        "refs": {
+            ... "/some/key/0": [
+                "{{u1}}" 0, 100
+            ],
+            ...
+        }
+    }
+    In this case, the "{{u1}}" will be replaced with the value of the "u1"
+    template string.
+
     It is okay for rfs to be modified outside of this class, and the changes
     will be reflected immediately in the store. This can be used by experimental
     tools such as lindi-cloud.
     """
     def __init__(self, rfs: dict, mode: Literal["r", "r+"] = "r+"):
         """
         Create a LindiReferenceFileSystemStore.
@@ -76,14 +94,20 @@
                 if not isinstance(v[1], int):
                     raise Exception(f"Problem with {k}: second element must be an int")
                 if not isinstance(v[2], int):
                     raise Exception(f"Problem with {k}: third element must be an int")
             else:
                 raise Exception(f"Problem with {k}: value must be a string or a list")
 
+        # validate templates
+        if "templates" in rfs:
+            for k, v in rfs["templates"].items():
+                if not isinstance(v, str):
+                    raise Exception(f"Problem with templates: value for {k} must be a string")
+
         self.rfs = rfs
         self.mode = mode
 
     # These methods are overridden from MutableMapping
     def __getitem__(self, key: str):
         if key not in self.rfs["refs"]:
             raise KeyError(key)
@@ -97,14 +121,17 @@
             return json.dumps(x).encode("utf-8")
         elif isinstance(x, list):
             if len(x) != 3:
                 raise Exception("list must have 3 elements")  # pragma: no cover
             url = x[0]
             offset = x[1]
             length = x[2]
+            if '{{' in url and 'templates' in self.rfs:
+                for k, v in self.rfs["templates"].items():
+                    url = url.replace("{{" + k + "}}", v)
             val = _read_bytes_from_url(url, offset, length)
             return val
         else:
             # should not happen given checks in __init__, but self.rfs is mutable
             # and contains mutable lists
             raise Exception(f"Problem with {key}: value {x} must be a string or a list")
 
@@ -142,26 +169,57 @@
     def is_listable(self):
         return True
 
     def is_erasable(self):
         return False
 
     @staticmethod
-    def replace_meta_file_contents_with_dicts(rfs: dict) -> None:
+    def replace_meta_file_contents_with_dicts_in_rfs(rfs: dict) -> None:
         """
         Utility function for replacing the contents of the .zattrs, .zgroup, and
         .zarray files in an rfs with the json representation of the contents.
         """
         # important to use the LindiReferenceFileSystemStore here because then we
         # can resolve any base64 encoded values, etc when converting them to dicts
         store = LindiReferenceFileSystemStore(rfs)
         for k, v in rfs['refs'].items():
             if k.endswith('.zattrs') or k.endswith('.zgroup') or k.endswith('.zarray') or k.endswith('zarr.json'):  # note: zarr.json is for zarr v3
                 rfs['refs'][k] = json.loads(store[k].decode('utf-8'))
 
+    @staticmethod
+    def use_templates_in_rfs(rfs: dict) -> None:
+        """
+        Utility for replacing URLs in an rfs with template strings. Only URLs
+        that occur 5 or more times are replaced with template strings. The
+        templates are added to the "templates" key of the rfs. The template
+        strings are of the form "{{u1}}", "{{u2}}", etc.
+        """
+        url_counts: Dict[str, int] = {}
+        for k, v in rfs['refs'].items():
+            if isinstance(v, list):
+                url = v[0]
+                if '{{' not in url:
+                    url_counts[url] = url_counts.get(url, 0) + 1
+        urls_with_many_occurrences = sorted([url for url, count in url_counts.items() if count >= 5])
+        new_templates = rfs.get('templates', {})
+        template_names_for_urls: Dict[str, str] = {}
+        for url in urls_with_many_occurrences:
+            i = 1
+            while f'u{i}' in new_templates:
+                i += 1
+            new_templates[f'u{i}'] = url
+            template_names_for_urls[url] = f'u{i}'
+        if new_templates:
+            rfs['templates'] = new_templates
+        for k, v in rfs['refs'].items():
+            if isinstance(v, list):
+                url = v[0]
+                if url in template_names_for_urls:
+                    v[0] = '{{' + template_names_for_urls[url] + '}}'
+
 
 # Keep a global cache of file segment readers that apply to all instances of
 # LindiReferenceFileSystemStore. The key is the URL of the file.
 _file_segment_readers: Dict[str, FileSegmentReader] = {}
 
 
 def _read_bytes_from_url(url: str, offset: int, length: int):
```

### Comparing `lindi-0.2.1/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py` & `lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyAttributesWriter.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,11 @@
 
 
 class LindiH5pyAttributesWriter:
     def __init__(self, p: 'LindiH5pyAttributes'):
         self.p = p
 
     def __setitem__(self, key, value):
+        from ...conversion.attr_conversion import h5_to_zarr_attr  # avoid circular import
         if self.p._readonly:
             raise KeyError("Cannot set attributes on read-only object")
-        if self.p._attrs_type == "h5py":
-            self.p._attrs[key] = value
-        elif self.p._attrs_type == "zarr":
-            from ...conversion.attr_conversion import h5_to_zarr_attr  # avoid circular import
-            self.p._attrs[key] = h5_to_zarr_attr(value, h5f=None)
-        else:
-            raise ValueError(f"Unknown attrs_type: {self.p._attrs_type}")
+        self.p._attrs[key] = h5_to_zarr_attr(value, h5f=None)
```

### Comparing `lindi-0.2.1/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py` & `lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyDatasetWriter.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 
 
 class LindiH5pyDatasetWriter:
     def __init__(self, p: 'LindiH5pyDataset'):
         self.p = p
 
     def __setitem__(self, args, val):
-        if isinstance(self.p._dataset_object, h5py.Dataset):
-            self.p._dataset_object.__setitem__(args, val)
-        elif isinstance(self.p._dataset_object, zarr.Array):
-            self._set_item_for_zarr(self.p._dataset_object, args, val)
+        if isinstance(self.p._zarr_array, h5py.Dataset):
+            self.p._zarr_array.__setitem__(args, val)
+        elif isinstance(self.p._zarr_array, zarr.Array):
+            self._set_item_for_zarr(self.p._zarr_array, args, val)
         else:
-            raise Exception(f"Unexpected type: {type(self.p._dataset_object)}")
+            raise Exception(f"Unexpected type: {type(self.p._zarr_array)}")
 
     def _set_item_for_zarr(self, zarr_array: zarr.Array, selection: Any, val: Any):
         if self.p._compound_dtype is not None:
             raise Exception("Setting compound dataset is not implemented")
         if self.p.ndim == 0:
             if selection != ():
                 raise TypeError(f'Cannot slice a scalar dataset with {selection}')
```

### Comparing `lindi-0.2.1/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py` & `lindi-0.3.0/lindi/LindiH5pyFile/writers/LindiH5pyGroupWriter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-from typing import TYPE_CHECKING, Union, Literal
+from typing import TYPE_CHECKING
 import h5py
 import numpy as np
 import zarr
+import numcodecs
 from numcodecs.abc import Codec
 
 from ..LindiH5pyDataset import LindiH5pyDataset
 from ..LindiH5pyReference import LindiH5pyReference
 
 if TYPE_CHECKING:
     from ..LindiH5pyGroup import LindiH5pyGroup  # pragma: no cover
 
 from ...conversion.create_zarr_dataset_from_h5_data import create_zarr_dataset_from_h5_data
 
+_compression_not_specified_ = object()
+
 
 class LindiH5pyGroupWriter:
     def __init__(self, p: 'LindiH5pyGroup'):
         self.p = p
 
     def create_group(self, name, track_order=None):
         from ..LindiH5pyGroup import LindiH5pyGroup  # avoid circular import
         if track_order is not None:
             raise Exception("track_order is not supported (I don't know what it is)")
-        if isinstance(self.p._group_object, h5py.Group):
+        if isinstance(self.p._zarr_group, h5py.Group):
             return LindiH5pyGroup(
-                self.p._group_object.create_group(name), self.p._file
+                self.p._zarr_group.create_group(name), self.p._file
             )
-        elif isinstance(self.p._group_object, zarr.Group):
+        elif isinstance(self.p._zarr_group, zarr.Group):
             return LindiH5pyGroup(
-                self.p._group_object.create_group(name), self.p._file
+                self.p._zarr_group.create_group(name), self.p._file
             )
         else:
-            raise Exception(f'Unexpected group object type: {type(self.p._group_object)}')
+            raise Exception(f'Unexpected group object type: {type(self.p._zarr_group)}')
 
     def require_group(self, name):
         if name in self.p:
             ret = self.p[name]
             if not isinstance(ret, LindiH5pyGroup):
                 raise Exception(f'Expected a group at {name} but got {type(ret)}')
             return ret
@@ -42,33 +45,59 @@
 
     def create_dataset(
         self,
         name,
         shape=None,
         dtype=None,
         data=None,
-        *,
-        _zarr_compressor: Union[Codec, Literal['default']] = 'default',
         **kwds
     ):
         chunks = None
+        compression = _compression_not_specified_
+        compression_opts = None
         for k, v in kwds.items():
             if k == 'chunks':
                 chunks = v
+            elif k == 'compression':
+                compression = v
+            elif k == 'compression_opts':
+                compression_opts = v
             else:
                 raise Exception(f'Unsupported kwds in create_dataset: {k}')
 
-        if isinstance(self.p._group_object, h5py.Group):
+        if compression is _compression_not_specified_:
+            _zarr_compressor = 'default'
+            if compression_opts is not None:
+                raise Exception('compression_opts is only supported when compression is provided')
+        elif isinstance(compression, Codec):
+            _zarr_compressor = compression
+            if compression_opts is not None:
+                raise Exception('compression_opts is not supported when compression is provided as a Codec')
+        elif isinstance(compression, str):
+            if compression == 'gzip':
+                if compression_opts is None:
+                    level = 4  # default for h5py
+                elif isinstance(compression_opts, int):
+                    level = compression_opts
+                else:
+                    raise Exception(f'Unexpected type for compression_opts: {type(compression_opts)}')
+                _zarr_compressor = numcodecs.GZip(level=level)
+            else:
+                raise Exception(f'Compression {compression} is not supported')
+        else:
+            raise Exception(f'Unexpected type for compression: {type(compression)}')
+
+        if isinstance(self.p._zarr_group, h5py.Group):
             if _zarr_compressor != 'default':
                 raise Exception('zarr_compressor is not supported when _group_object is h5py.Group')
             return LindiH5pyDataset(
                 self._group_object.create_dataset(name, shape=shape, dtype=dtype, data=data, chunks=chunks),  # type: ignore
                 self.p._file
             )
-        elif isinstance(self.p._group_object, zarr.Group):
+        elif isinstance(self.p._zarr_group, zarr.Group):
             if isinstance(data, list):
                 data = np.array(data)
             if shape is None:
                 if data is None:
                     raise Exception('shape or data must be provided')
                 if isinstance(data, np.ndarray):
                     shape = data.shape
@@ -78,27 +107,27 @@
                 if data is None:
                     raise Exception('dtype or data must be provided')
                 if isinstance(data, np.ndarray):
                     dtype = data.dtype
                 else:
                     dtype = np.dtype(type(data))
             ds = create_zarr_dataset_from_h5_data(
-                zarr_parent_group=self.p._group_object,
+                zarr_parent_group=self.p._zarr_group,
                 name=name,
                 label=(self.p.name or '') + '/' + name,
                 h5_chunks=chunks,
                 h5_shape=shape,
                 h5_dtype=dtype,
                 h5_data=data,
                 h5f=None,
                 zarr_compressor=_zarr_compressor
             )
             return LindiH5pyDataset(ds, self.p._file)
         else:
-            raise Exception(f'Unexpected group object type: {type(self.p._group_object)}')
+            raise Exception(f'Unexpected group object type: {type(self.p._zarr_group)}')
 
     def require_dataset(self, name, shape, dtype, exact=False, **kwds):
         if name in self.p:
             ret = self.p[name]
             if not isinstance(ret, LindiH5pyDataset):
                 raise Exception(f'Expected a dataset at {name} but got {type(ret)}')
             if ret.shape != shape:
@@ -110,28 +139,28 @@
                 if not np.can_cast(ret.dtype, dtype):
                     raise Exception(f'Cannot cast dtype {ret.dtype} to {dtype}')
             return ret
         return self.create_dataset(name, *(shape, dtype), **kwds)
 
     def __setitem__(self, name, obj):
         if isinstance(obj, h5py.SoftLink):
-            if isinstance(self.p._group_object, h5py.Group):
-                self.p._group_object[name] = obj
-            elif isinstance(self.p._group_object, zarr.Group):
+            if isinstance(self.p._zarr_group, h5py.Group):
+                self.p._zarr_group[name] = obj
+            elif isinstance(self.p._zarr_group, zarr.Group):
                 grp = self.p.create_group(name)
-                grp._group_object.attrs['_SOFT_LINK'] = {
+                grp._zarr_group.attrs['_SOFT_LINK'] = {
                     'path': obj.path
                 }
             else:
-                raise Exception(f'Unexpected group object type: {type(self.p._group_object)}')
+                raise Exception(f'Unexpected group object type: {type(self.p._zarr_group)}')
         else:
             raise Exception(f'Unexpected type for obj in __setitem__: {type(obj)}')
 
     def __delitem__(self, name):
-        del self.p._group_object[name]
+        del self.p._zarr_group[name]
 
     @property
     def ref(self):
         return LindiH5pyReference({
             'object_id': self.p.attrs.get('object_id', None),
             'path': self.p.name,
             'source': '.',
```

### Comparing `lindi-0.2.1/lindi/LindiStagingStore/LindiStagingStore.py` & `lindi-0.3.0/lindi/LindiStagingStore/LindiStagingStore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Callable
 import json
 import tempfile
 import os
 from zarr.storage import Store as ZarrStore
 from ..LindiH5pyFile.LindiReferenceFileSystemStore import LindiReferenceFileSystemStore
 from .StagingArea import StagingArea, _random_str
+from ..LindiH5ZarrStore._util import _write_rfs_to_file
 
 
-# Accepts a string path to a file, stores it somewhere, and returns a string URL
+# Accepts a string path to a file, uploads (or copies) it somewhere, and returns a string URL
 # (or local path)
-StoreFileFunc = Callable[[str], str]
+UploadFileFunc = Callable[[str], str]
 
 
 class LindiStagingStore(ZarrStore):
     """
     A Zarr store that allows supplementing a base LindiReferenceFileSystemStore
     where the large data blobs are stored in a staging area. After writing new
     data to the store, the data blobs can be consolidated into larger files and
@@ -92,29 +93,29 @@
             offset,
             size
         ]
 
     def upload(
         self,
         *,
-        on_store_blob: StoreFileFunc,
-        on_store_main: StoreFileFunc,
+        on_upload_blob: UploadFileFunc,
+        on_upload_main: UploadFileFunc,
         consolidate_chunks: bool = True
     ):
         """
         Consolidate the chunks in the staging area, upload them to a storage
         system, updating the references in the base store, and then upload the
         updated reference file system .json file.
 
         Parameters
         ----------
-        on_store_blob : StoreFileFunc
-            A function that takes a string path to a blob file, stores it
+        on_upload_blob : StoreFileFunc
+            A function that takes a string path to a blob file, uploads or copies it
             somewhere, and returns a string URL (or local path).
-        on_store_main : StoreFileFunc
+        on_upload_main : StoreFileFunc
             A function that takes a string path to the main .json file, stores
             it somewhere, and returns a string URL (or local path).
         consolidate_chunks : bool
             If True (the default), consolidate the chunks in the staging area
             before uploading.
 
         Returns
@@ -123,29 +124,29 @@
             The URL (or local path) of the uploaded reference file system .json
             file.
         """
         if consolidate_chunks:
             self.consolidate_chunks()
         rfs = self._base_store.rfs
         rfs = json.loads(json.dumps(rfs))  # deep copy
-        LindiReferenceFileSystemStore.replace_meta_file_contents_with_dicts(rfs)
-        blob_mapping = _upload_directory_of_blobs(self._staging_area.directory, on_store_blob=on_store_blob)
+        LindiReferenceFileSystemStore.replace_meta_file_contents_with_dicts_in_rfs(rfs)
+        blob_mapping = _upload_directory_of_blobs(self._staging_area.directory, on_upload_blob=on_upload_blob)
         for k, v in rfs['refs'].items():
             if isinstance(v, list) and len(v) == 3:
                 url1 = v[0]
                 if url1.startswith(self._staging_area.directory + '/'):
                     url2 = blob_mapping.get(url1, None)
                     if url2 is None:
                         raise ValueError(f"Could not find url in blob mapping: {url1}")
                     rfs['refs'][k][0] = url2
         with tempfile.TemporaryDirectory() as tmpdir:
-            rfs_fname = f"{tmpdir}/rfs.json"
-            with open(rfs_fname, 'w') as f:
-                json.dump(rfs, f, indent=2, sort_keys=True)
-            return on_store_main(rfs_fname)
+            rfs_fname = f"{tmpdir}/rfs.lindi.json"
+            LindiReferenceFileSystemStore.use_templates_in_rfs(rfs)
+            _write_rfs_to_file(rfs=rfs, output_file_name=rfs_fname)
+            return on_upload_main(rfs_fname)
 
     def consolidate_chunks(self):
         """
         Consolidate the chunks in the staging area.
 
         This method is called by `upload` if `consolidate_chunks` is True.
         """
@@ -167,14 +168,17 @@
             ]
             if len(files) <= 1:
                 continue
             refs_keys_for_this_dir = refs_keys_by_reference_parent_path.get(root, [])
             if len(refs_keys_for_this_dir) <= 1:
                 continue
 
+            # sort so that the files are in order 0.0.0, 0.0.1, 0.0.2, ...
+            files = _sort_by_chunk_key(files)
+
             print(f'Consolidating {len(files)} files in {root}')
 
             offset = 0
             offset_maps = {}
             consolidated_id = _random_str(8)
             consolidated_index = 0
             max_size_of_consolidated_file = 1024 * 1024 * 1024  # 1 GB, a good size for cloud bucket files
@@ -202,17 +206,41 @@
                 consolidated_fname, new_offset = offset_maps[filename]
                 rfs['refs'][key] = [consolidated_fname, new_offset + old_offset, old_size]
             # remove the old files
             for fname in files:
                 os.remove(f"{root}/{fname}")
 
 
+def _sort_by_chunk_key(files: list) -> list:
+    # first verify that all the files have the same number of parts
+    num_parts = None
+    for fname in files:
+        parts = fname.split('.')
+        if num_parts is None:
+            num_parts = len(parts)
+        elif len(parts) != num_parts:
+            raise ValueError(f"Files have different numbers of parts: {files}")
+    # Verify that all the parts are integers
+    for fname in files:
+        parts = fname.split('.')
+        for p in parts:
+            try:
+                int(p)
+            except ValueError:
+                raise ValueError(f"File part is not an integer: {fname}")
+
+    def _chunk_key(fname: str) -> tuple:
+        parts = fname.split('.')
+        return tuple(int(p) for p in parts)
+    return sorted(files, key=_chunk_key)
+
+
 def _upload_directory_of_blobs(
     staging_dir: str,
-    on_store_blob: StoreFileFunc
+    on_upload_blob: UploadFileFunc
 ) -> dict:
     """
     Upload all the files in a directory to a storage system and return a mapping
     from the original file paths to the URLs of the uploaded files.
     """
     all_files = []
     for root, dirs, files in os.walk(staging_dir):
@@ -220,15 +248,15 @@
             full_fname = f"{root}/{fname}"
             all_files.append(full_fname)
     blob_mapping = {}
     for i, full_fname in enumerate(all_files):
         relative_fname = full_fname[len(staging_dir):]
         size_bytes = os.path.getsize(full_fname)
         print(f'Uploading blob {i + 1} of {len(all_files)} {relative_fname} ({_format_size_bytes(size_bytes)})')
-        blob_url = on_store_blob(full_fname)
+        blob_url = on_upload_blob(full_fname)
         blob_mapping[full_fname] = blob_url
     return blob_mapping
 
 
 def _format_size_bytes(size_bytes: int) -> str:
     if size_bytes < 1024:
         return f"{size_bytes} bytes"
```

### Comparing `lindi-0.2.1/lindi/LindiStagingStore/StagingArea.py` & `lindi-0.3.0/lindi/LindiStagingStore/StagingArea.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/lindi/conversion/attr_conversion.py` & `lindi-0.3.0/lindi/conversion/attr_conversion.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/lindi/conversion/create_zarr_dataset_from_h5_data.py` & `lindi-0.3.0/lindi/conversion/create_zarr_dataset_from_h5_data.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/lindi/conversion/decode_references.py` & `lindi-0.3.0/lindi/conversion/decode_references.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/lindi/conversion/h5_filters_to_codecs.py` & `lindi-0.3.0/lindi/conversion/h5_filters_to_codecs.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/lindi/conversion/h5_ref_to_zarr_attr.py` & `lindi-0.3.0/lindi/conversion/h5_ref_to_zarr_attr.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/lindi/conversion/nan_inf_ninf.py` & `lindi-0.3.0/lindi/conversion/nan_inf_ninf.py`

 * *Files identical despite different names*

### Comparing `lindi-0.2.1/pyproject.toml` & `lindi-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lindi"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = [
     "Jeremy Magland <jmagland@flatironinstitute.org>",
     "Ryan Ly <rly@lbl.gov>",
     "Oliver Ruebel <oruebel@lbl.gov>"
 ]
 readme = "README.md"
```

