# Comparing `tmp/bvhio-1.3.7.tar.gz` & `tmp/bvhio-1.3.8.tar.gz`

## Comparing `bvhio-1.3.7.tar` & `bvhio-1.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.3.7/.flake8
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.3.7/CITATION.cff
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.3.7/changelog.txt
--rw-r--r--   0        0        0    16571 2020-02-02 00:00:00.000000 bvhio-1.3.7/test.ipynb
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.3.7/.github/workflows/build_main.yml
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.3.7/.github/workflows/build_preview.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/__init__.py
--rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/lib/Parser.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/lib/bvh/BvhContainer.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/lib/bvh/BvhJoint.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/lib/bvh/__init__.py
--rw-r--r--   0        0        0    17687 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/lib/hierarchy/Joint.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/lib/hierarchy/__init__.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/tests/example.bvh
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/tests/test_bvh.py
--rw-r--r--   0        0        0    22186 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/tests/test_hierarchy.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/tests/test_io.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.3.7/bvhio/tests/utils.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bvhio-1.3.7/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.3.7/LICENSE
--rw-r--r--   0        0        0    18754 2020-02-02 00:00:00.000000 bvhio-1.3.7/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bvhio-1.3.7/pyproject.toml
--rw-r--r--   0        0        0    19387 2020-02-02 00:00:00.000000 bvhio-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.3.8/.flake8
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.3.8/CITATION.cff
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.3.8/changelog.txt
+-rw-r--r--   0        0        0    17292 2020-02-02 00:00:00.000000 bvhio-1.3.8/test.ipynb
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.3.8/.github/workflows/build_main.yml
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.3.8/.github/workflows/build_preview.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/__init__.py
+-rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/lib/Parser.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/lib/bvh/BvhContainer.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/lib/bvh/BvhJoint.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/lib/bvh/__init__.py
+-rw-r--r--   0        0        0    17687 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/lib/hierarchy/Joint.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/lib/hierarchy/__init__.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/tests/example.bvh
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/tests/test_bvh.py
+-rw-r--r--   0        0        0    22186 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/tests/test_hierarchy.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/tests/test_io.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.3.8/bvhio/tests/utils.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bvhio-1.3.8/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.3.8/LICENSE
+-rw-r--r--   0        0        0    19372 2020-02-02 00:00:00.000000 bvhio-1.3.8/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bvhio-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0    20005 2020-02-02 00:00:00.000000 bvhio-1.3.8/PKG-INFO
```

### Comparing `bvhio-1.3.7/test.ipynb` & `bvhio-1.3.8/test.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875202922077922%*

 * *Differences: {"'cells'": "{insert: [(10, OrderedDict([('cell_type', 'code'), ('execution_count', 9), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', ['import bvhio\\n', '\\n', "*

 * *            '\'# load data\\n\', "file1 = bvhio.readAsBvh(\'bvhio/tests/example.bvh\')\\n", "file2 '*

 * *            '= bvhio.readAsBvh(\'bvhio/tests/example.bvh\')\\n", \'\\n\', \'# get hierarchy of '*

 * *            "both files\\n', 'data1 = file1.Root.layout()\\n', 'data2 = file2.Root.layout()\\n', "*

 * *            "'\\n', '# app […]*

```diff
@@ -361,14 +361,40 @@
                 "# persists the current pose again as new pose.\n",
                 "# All keyframes between the first and this pose are linearly interpolated.\n",
                 "root.writePose(20, recursive=True)\n",
                 "\n",
                 "# store the animation\n",
                 "bvhio.writeHierarchy('test.bvh', root, 1/30, percision=4)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import bvhio\n",
+                "\n",
+                "# load data\n",
+                "file1 = bvhio.readAsBvh('bvhio/tests/example.bvh')\n",
+                "file2 = bvhio.readAsBvh('bvhio/tests/example.bvh')\n",
+                "\n",
+                "# get hierarchy of both files\n",
+                "data1 = file1.Root.layout()\n",
+                "data2 = file2.Root.layout()\n",
+                "\n",
+                "# append the animation data\n",
+                "for joint, index, _ in data1:\n",
+                "    joint.Keyframes.extend(data2[index][0].Keyframes)\n",
+                "\n",
+                "# update framecount to write all animation\n",
+                "file1.FrameCount += file2.FrameCount\n",
+                "\n",
+                "bvhio.writeBvh('test.bvh', file1, 4)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
@@ -379,15 +405,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.6"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "864323a39c18a1ade2bdf9707c04ff6c86bcf165d3ca262f89a74665bc096b3f"
             }
         }
```

### Comparing `bvhio-1.3.7/.github/workflows/build_main.yml` & `bvhio-1.3.8/.github/workflows/build_main.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/.github/workflows/build_preview.yml` & `bvhio-1.3.8/.github/workflows/build_preview.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/bvhio/lib/Parser.py` & `bvhio-1.3.8/bvhio/lib/Parser.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/bvhio/lib/bvh/BvhContainer.py` & `bvhio-1.3.8/bvhio/lib/bvh/BvhContainer.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/bvhio/lib/bvh/BvhJoint.py` & `bvhio-1.3.8/bvhio/lib/bvh/BvhJoint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/bvhio/lib/hierarchy/Joint.py` & `bvhio-1.3.8/bvhio/lib/hierarchy/Joint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/bvhio/tests/example.bvh` & `bvhio-1.3.8/bvhio/tests/example.bvh`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/bvhio/tests/test_bvh.py` & `bvhio-1.3.8/bvhio/tests/test_bvh.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/bvhio/tests/test_hierarchy.py` & `bvhio-1.3.8/bvhio/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/bvhio/tests/test_io.py` & `bvhio-1.3.8/bvhio/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/bvhio/tests/utils.py` & `bvhio-1.3.8/bvhio/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/LICENSE` & `bvhio-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.7/README.md` & `bvhio-1.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -302,14 +302,41 @@
 for joint, index, depth in root.layout():
     joint.Keyframes = [(frame * 100, key) for frame, key in joint.Keyframes]
 
 # persists the interpolations automatically
 bvhio.writeHierarchy('test.bvh', root, 1/30)
 ```
 
+
+### Merge BVH files
+```python
+
+# THIS WILL ONLY WORKs IF THE REST POSE IS THE SAME!
+# You cannot merge different skeletons / hierarchies.
+import bvhio
+
+# load data
+file1 = bvhio.readAsBvh('bvhio/tests/example.bvh')
+file2 = bvhio.readAsBvh('bvhio/tests/example.bvh')
+
+# get hierarchy of both files
+data1 = file1.Root.layout()
+data2 = file2.Root.layout()
+
+# append the animation to the end of the original one
+for joint, index, _ in data1:
+    joint.Keyframes.extend(data2[index][0].Keyframes)
+
+# update framecount to write all animation
+file1.FrameCount += file2.FrameCount
+
+bvhio.writeBvh('test.bvh', file1, 4)
+```
+
+
 ### Create/build animations from code
 ```python
 import bvhio
 
 # create custom hierarchy.
 root = bvhio.Joint('Root', (0,2,0)).setEuler((0,0,0)).attach(
     bvhio.Joint('UpperLegL', (+.3,2.1,0)).setEuler((0,0,180)).attach(
```

#### html2text {}

```diff
@@ -164,15 +164,23 @@
 bvhio.BvhContainer(bvhRoot, len(bvhRoot.Keyframes), 1/30)) ``` ### Interpolate
 between keyframes ```python import bvhio # load data root =
 bvhio.readAsHierarchy('bvhio/tests/example.bvh') # scales the frame id of the
 two given frames. # this will restult in the ids 0 and 100. # frames without
 keyframe are linearly interpolated. for joint, index, depth in root.layout():
 joint.Keyframes = [(frame * 100, key) for frame, key in joint.Keyframes] #
 persists the interpolations automatically bvhio.writeHierarchy('test.bvh',
-root, 1/30) ``` ### Create/build animations from code ```python import bvhio #
+root, 1/30) ``` ### Merge BVH files ```python # THIS WILL ONLY WORKs IF THE
+REST POSE IS THE SAME! # You cannot merge different skeletons / hierarchies.
+import bvhio # load data file1 = bvhio.readAsBvh('bvhio/tests/example.bvh')
+file2 = bvhio.readAsBvh('bvhio/tests/example.bvh') # get hierarchy of both
+files data1 = file1.Root.layout() data2 = file2.Root.layout() # append the
+animation to the end of the original one for joint, index, _ in data1:
+joint.Keyframes.extend(data2[index][0].Keyframes) # update framecount to write
+all animation file1.FrameCount += file2.FrameCount bvhio.writeBvh('test.bvh',
+file1, 4) ``` ### Create/build animations from code ```python import bvhio #
 create custom hierarchy. root = bvhio.Joint('Root', (0,2,0)).setEuler(
 (0,0,0)).attach( bvhio.Joint('UpperLegL', (+.3,2.1,0)).setEuler(
 (0,0,180)).attach( bvhio.Joint('LowerLegL', (+.3,1,0)).setEuler((0,0,180)) ),
 bvhio.Joint('UpperLegR', (-.3,2.1,0)).setEuler((0,0,180)).attach( bvhio.Joint
 ('LowerLegR', (-.3,1,0)).setEuler((0,0,180)) ), ) # sets current layout as rest
 pose root.writeRestPose(recursive=True) # change the pose of the hierarchy to
 save it alter as key frame # this will add a rotation to each leg joint for
```

### Comparing `bvhio-1.3.7/pyproject.toml` & `bvhio-1.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bvhio"
-version = "1.3.7"
+version = "1.3.8"
 authors = [ { name="Wasserwecken", email="author@example.com" }, ]
 description = "Read, write, edit and create .bvh files with hierarchical 3D transforms."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `bvhio-1.3.7/PKG-INFO` & `bvhio-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: bvhio
-Version: 1.3.7
+Version: 1.3.8
 Summary: Read, write, edit and create .bvh files with hierarchical 3D transforms.
 Project-URL: Homepage, https://github.com/Wasserwecken/bvhio
 Project-URL: Bug Tracker, https://github.com/Wasserwecken/bvhio/issues
 Author-email: Wasserwecken <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -319,14 +319,41 @@
 for joint, index, depth in root.layout():
     joint.Keyframes = [(frame * 100, key) for frame, key in joint.Keyframes]
 
 # persists the interpolations automatically
 bvhio.writeHierarchy('test.bvh', root, 1/30)
 ```
 
+
+### Merge BVH files
+```python
+
+# THIS WILL ONLY WORKs IF THE REST POSE IS THE SAME!
+# You cannot merge different skeletons / hierarchies.
+import bvhio
+
+# load data
+file1 = bvhio.readAsBvh('bvhio/tests/example.bvh')
+file2 = bvhio.readAsBvh('bvhio/tests/example.bvh')
+
+# get hierarchy of both files
+data1 = file1.Root.layout()
+data2 = file2.Root.layout()
+
+# append the animation to the end of the original one
+for joint, index, _ in data1:
+    joint.Keyframes.extend(data2[index][0].Keyframes)
+
+# update framecount to write all animation
+file1.FrameCount += file2.FrameCount
+
+bvhio.writeBvh('test.bvh', file1, 4)
+```
+
+
 ### Create/build animations from code
 ```python
 import bvhio
 
 # create custom hierarchy.
 root = bvhio.Joint('Root', (0,2,0)).setEuler((0,0,0)).attach(
     bvhio.Joint('UpperLegL', (+.3,2.1,0)).setEuler((0,0,180)).attach(
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bvhio Version: 1.3.7 Summary: Read, write, edit and
+Metadata-Version: 2.3 Name: bvhio Version: 1.3.8 Summary: Read, write, edit and
 create .bvh files with hierarchical 3D transforms. Project-URL: Homepage,
 https://github.com/Wasserwecken/bvhio Project-URL: Bug Tracker, https://
 github.com/Wasserwecken/bvhio/issues Author-email: Wasserwecken
 example.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy Requires-
 Dist: pyglm==2.7.0 Requires-Dist: spatial-transform==1.2.13 Description-
@@ -173,15 +173,23 @@
 bvhio.BvhContainer(bvhRoot, len(bvhRoot.Keyframes), 1/30)) ``` ### Interpolate
 between keyframes ```python import bvhio # load data root =
 bvhio.readAsHierarchy('bvhio/tests/example.bvh') # scales the frame id of the
 two given frames. # this will restult in the ids 0 and 100. # frames without
 keyframe are linearly interpolated. for joint, index, depth in root.layout():
 joint.Keyframes = [(frame * 100, key) for frame, key in joint.Keyframes] #
 persists the interpolations automatically bvhio.writeHierarchy('test.bvh',
-root, 1/30) ``` ### Create/build animations from code ```python import bvhio #
+root, 1/30) ``` ### Merge BVH files ```python # THIS WILL ONLY WORKs IF THE
+REST POSE IS THE SAME! # You cannot merge different skeletons / hierarchies.
+import bvhio # load data file1 = bvhio.readAsBvh('bvhio/tests/example.bvh')
+file2 = bvhio.readAsBvh('bvhio/tests/example.bvh') # get hierarchy of both
+files data1 = file1.Root.layout() data2 = file2.Root.layout() # append the
+animation to the end of the original one for joint, index, _ in data1:
+joint.Keyframes.extend(data2[index][0].Keyframes) # update framecount to write
+all animation file1.FrameCount += file2.FrameCount bvhio.writeBvh('test.bvh',
+file1, 4) ``` ### Create/build animations from code ```python import bvhio #
 create custom hierarchy. root = bvhio.Joint('Root', (0,2,0)).setEuler(
 (0,0,0)).attach( bvhio.Joint('UpperLegL', (+.3,2.1,0)).setEuler(
 (0,0,180)).attach( bvhio.Joint('LowerLegL', (+.3,1,0)).setEuler((0,0,180)) ),
 bvhio.Joint('UpperLegR', (-.3,2.1,0)).setEuler((0,0,180)).attach( bvhio.Joint
 ('LowerLegR', (-.3,1,0)).setEuler((0,0,180)) ), ) # sets current layout as rest
 pose root.writeRestPose(recursive=True) # change the pose of the hierarchy to
 save it alter as key frame # this will add a rotation to each leg joint for
```

