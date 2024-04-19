# Comparing `tmp/gym_jiminy_rllib-1.8.3-py3-none-any.whl.zip` & `tmp/gym_jiminy_rllib-1.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 25585 bytes, number of entries: 10
--rw-r--r--  2.0 unx      264 b- defN 24-Mar-07 12:04 gym_jiminy/rllib/__init__.py
--rw-r--r--  2.0 unx     3162 b- defN 24-Mar-07 12:04 gym_jiminy/rllib/callbacks.py
--rw-r--r--  2.0 unx    12290 b- defN 24-Mar-07 12:04 gym_jiminy/rllib/curriculum.py
--rw-r--r--  2.0 unx    28023 b- defN 24-Mar-07 12:04 gym_jiminy/rllib/ppo.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-07 12:04 gym_jiminy/rllib/py.typed
--rw-r--r--  2.0 unx    46328 b- defN 24-Mar-07 12:04 gym_jiminy/rllib/utilities.py
--rw-r--r--  2.0 unx     1022 b- defN 24-Mar-07 12:05 gym_jiminy_rllib-1.8.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-07 12:05 gym_jiminy_rllib-1.8.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Mar-07 12:05 gym_jiminy_rllib-1.8.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      839 b- defN 24-Mar-07 12:05 gym_jiminy_rllib-1.8.3.dist-info/RECORD
-10 files, 92031 bytes uncompressed, 24147 bytes compressed:  73.8%
+Zip file size: 25592 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/__init__.py
+-rw-r--r--  2.0 unx     3162 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/callbacks.py
+-rw-r--r--  2.0 unx    12290 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/curriculum.py
+-rw-r--r--  2.0 unx    28076 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/ppo.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/py.typed
+-rw-r--r--  2.0 unx    46328 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/utilities.py
+-rw-r--r--  2.0 unx      954 b- defN 24-Apr-19 21:52 gym_jiminy_rllib-1.8.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 21:52 gym_jiminy_rllib-1.8.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-19 21:52 gym_jiminy_rllib-1.8.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      838 b- defN 24-Apr-19 21:52 gym_jiminy_rllib-1.8.4.dist-info/RECORD
+10 files, 92015 bytes uncompressed, 24154 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: gym_jiminy/rllib/py.typed
 Comment: 
 
 Filename: gym_jiminy/rllib/utilities.py
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.3.dist-info/METADATA
+Filename: gym_jiminy_rllib-1.8.4.dist-info/METADATA
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.3.dist-info/WHEEL
+Filename: gym_jiminy_rllib-1.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.3.dist-info/top_level.txt
+Filename: gym_jiminy_rllib-1.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.3.dist-info/RECORD
+Filename: gym_jiminy_rllib-1.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_jiminy/rllib/ppo.py

```diff
@@ -158,21 +158,20 @@
     def _update_flattened_slice(data: torch.Tensor,
                                 shape: Tuple[int, ...],
                                 mirror_mat: torch.Tensor) -> torch.Tensor:
         """Mirror an array of flattened tensor using provided transformation
         matrix.
         """
         if len(shape) > 1:
-            data = data.reshape((-1, *shape)) \
-                       .swapaxes(1, 0) \
-                       .reshape((shape[0], -1))
+            assert len(shape) == 2, "shape > 2 is not supported for now."
+            data = data.reshape(
+                (-1, *shape)).swapaxes(1, 0).reshape((shape[0], -1))
             data_mirrored = mirror_mat @ data
-            return data_mirrored.reshape((shape[0], -1, shape[1])) \
-                                .swapaxes(1, 0) \
-                                .reshape((-1, *shape))
+            return data_mirrored.reshape(
+                (shape[0], -1, shape[1])).swapaxes(1, 0).reshape((-1, *shape))
         return torch.mm(data, mirror_mat)
 
     if isinstance(mirror_mat, dict):
         offset = 0
         value_mirrored = []
         for field, slice_mirror_mat in mirror_mat.items():
             field_shape = space.original_space[  # type: ignore[attr-defined]
@@ -265,15 +264,16 @@
     def get_default_config(cls) -> AlgorithmConfig:
         """Returns a default configuration for the algorithm.
         """
         return PPOConfig()
 
     @classmethod
     @override(_PPO)
-    def get_default_policy_class(cls, config: AlgorithmConfig
+    def get_default_policy_class(cls,
+                                 config: AlgorithmConfig
                                  ) -> Optional[Type[Policy]]:
         """Returns a default Policy class to use, given a config.
         """
         framework = config.framework_str
         if framework == "torch":
             return PPOTorchPolicy
         raise ValueError(f"The framework {framework} is not supported.")
@@ -369,14 +369,15 @@
         regularization.
         """
         view_requirements = super()._get_default_view_requirements()
         view_requirements["prev_obs"] = ViewRequirement(
             data_col=SampleBatch.OBS,
             space=self.observation_space,
             shift=-1,
+            batch_repeat_value=1,
             used_for_compute_actions=False,
             used_for_training=True)
         return view_requirements
 
     @override(_PPOTorchPolicy)
     def loss(self,
              model: ModelV2,
```

## Comparing `gym_jiminy_rllib-1.8.3.dist-info/METADATA` & `gym_jiminy_rllib-1.8.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-jiminy-rllib
-Version: 1.8.3
+Version: 1.8.4
 Summary: Specialized Reinforcement learning toolbox based on Ray RLlib for Gym Jiminy.
 Author: Alexis Duburcq
 Author-email: alexis.duburcq@gmail.com
 Maintainer: Alexis Duburcq
 License: MIT
 Keywords: reinforcement-learning robotics gym jiminy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,12 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<3.12
-Requires-Dist: gym-jiminy ~=1.8.3
-Requires-Dist: ray[default,rllib] ~=2.5.0
-Requires-Dist: async-timeout
-Requires-Dist: pydantic <2.0.0
+Requires-Dist: gym-jiminy ~=1.8.4
+Requires-Dist: ray[rllib] ~=2.9.0
 Requires-Dist: tensorboardX
 Requires-Dist: plotext >=5.0.0
```

