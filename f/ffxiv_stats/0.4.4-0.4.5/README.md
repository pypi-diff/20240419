# Comparing `tmp/ffxiv_stats-0.4.4.tar.gz` & `tmp/ffxiv_stats-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffxiv_stats-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ffxiv_stats-0.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ffxiv_stats-0.4.4.tar` & `ffxiv_stats-0.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      106 2023-12-24 23:30:17.666831 ffxiv_stats-0.4.4/.gitignore
--rw-r--r--   0        0        0    11558 2023-08-06 18:15:32.993652 ffxiv_stats-0.4.4/LICENSE
--rw-r--r--   0        0        0     4996 2024-02-04 04:04:49.060347 ffxiv_stats-0.4.4/README.md
--rw-r--r--   0        0        0   262348 2024-02-04 03:52:04.000902 ffxiv_stats-0.4.4/examples/deterministic-rotations.ipynb
--rw-r--r--   0        0        0    51264 2023-11-03 01:32:29.636143 ffxiv_stats-0.4.4/examples/smn-rotation-comparison/fryte-results.csv
--rw-r--r--   0        0        0   501435 2023-11-03 01:32:29.639995 ffxiv_stats-0.4.4/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb
--rw-r--r--   0        0        0    20959 2023-11-03 01:32:29.641016 ffxiv_stats-0.4.4/examples/smn-rotation-comparison/smn-rotation.csv
--rw-r--r--   0        0        0  1620366 2024-02-04 03:52:04.014901 ffxiv_stats-0.4.4/examples/stochastic-rotations.ipynb
--rw-r--r--   0        0        0      441 2024-04-14 19:52:38.808900 ffxiv_stats-0.4.4/ffxiv_stats/__init__.py
--rw-r--r--   0        0        0    30195 2024-04-14 19:51:14.746010 ffxiv_stats-0.4.4/ffxiv_stats/jobs.py
--rw-r--r--   0        0        0      299 2023-12-24 23:30:17.668826 ffxiv_stats-0.4.4/ffxiv_stats/modifiers.py
--rw-r--r--   0        0        0    47554 2024-02-07 03:43:11.874269 ffxiv_stats-0.4.4/ffxiv_stats/moments.py
--rw-r--r--   0        0        0     6564 2024-02-04 03:52:04.023903 ffxiv_stats-0.4.4/ffxiv_stats/rate.py
--rw-r--r--   0        0        0      593 2024-01-10 06:09:20.789049 ffxiv_stats-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 ffxiv_stats-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      106 2023-12-24 23:30:17.666831 ffxiv_stats-0.4.5/.gitignore
+-rw-r--r--   0        0        0    11558 2023-08-06 18:15:32.993652 ffxiv_stats-0.4.5/LICENSE
+-rw-r--r--   0        0        0     4996 2024-02-04 04:04:49.060347 ffxiv_stats-0.4.5/README.md
+-rw-r--r--   0        0        0   262348 2024-02-04 03:52:04.000902 ffxiv_stats-0.4.5/examples/deterministic-rotations.ipynb
+-rw-r--r--   0        0        0    51264 2023-11-03 01:32:29.636143 ffxiv_stats-0.4.5/examples/smn-rotation-comparison/fryte-results.csv
+-rw-r--r--   0        0        0   501435 2023-11-03 01:32:29.639995 ffxiv_stats-0.4.5/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb
+-rw-r--r--   0        0        0    20959 2023-11-03 01:32:29.641016 ffxiv_stats-0.4.5/examples/smn-rotation-comparison/smn-rotation.csv
+-rw-r--r--   0        0        0  1620366 2024-02-04 03:52:04.014901 ffxiv_stats-0.4.5/examples/stochastic-rotations.ipynb
+-rw-r--r--   0        0        0      441 2024-04-18 22:52:03.334795 ffxiv_stats-0.4.5/ffxiv_stats/__init__.py
+-rw-r--r--   0        0        0    31488 2024-04-18 22:55:43.827417 ffxiv_stats-0.4.5/ffxiv_stats/jobs.py
+-rw-r--r--   0        0        0      299 2023-12-24 23:30:17.668826 ffxiv_stats-0.4.5/ffxiv_stats/modifiers.py
+-rw-r--r--   0        0        0    47554 2024-02-07 03:43:11.874269 ffxiv_stats-0.4.5/ffxiv_stats/moments.py
+-rw-r--r--   0        0        0     6564 2024-02-04 03:52:04.023903 ffxiv_stats-0.4.5/ffxiv_stats/rate.py
+-rw-r--r--   0        0        0      593 2024-01-10 06:09:20.789049 ffxiv_stats-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 ffxiv_stats-0.4.5/PKG-INFO
```

### Comparing `ffxiv_stats-0.4.4/LICENSE` & `ffxiv_stats-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/README.md` & `ffxiv_stats-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/examples/deterministic-rotations.ipynb` & `ffxiv_stats-0.4.5/examples/deterministic-rotations.ipynb`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/examples/smn-rotation-comparison/fryte-results.csv` & `ffxiv_stats-0.4.5/examples/smn-rotation-comparison/fryte-results.csv`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb` & `ffxiv_stats-0.4.5/examples/smn-rotation-comparison/smn-rotation-analysis.ipynb`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/examples/smn-rotation-comparison/smn-rotation.csv` & `ffxiv_stats-0.4.5/examples/smn-rotation-comparison/smn-rotation.csv`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/examples/stochastic-rotations.ipynb` & `ffxiv_stats-0.4.5/examples/stochastic-rotations.ipynb`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/ffxiv_stats/jobs.py` & `ffxiv_stats-0.4.5/ffxiv_stats/jobs.py`

 * *Files 11% similar despite different names*

```diff
@@ -300,15 +300,15 @@
                             )
                             / 1000
                         )
                         * self.f_auto()
                     )
                     / 100
                 )
-                * self.trait
+                * self.auto_trait
             )
             / 100
         )
         return auto_d2
 
     def direct_d2(self, potency, ap_adjust=0):
         """
@@ -682,58 +682,95 @@
             self.atk_mod = 195
         if level == 80:
             self.atk_mod = 165
 
         pass
 
 
-# class PhysicalRanged(BaseStats):
-#     def __init__(self, mind, intelligence, vitality, strength, dexterity, det,
-#                  skill_speed, spell_speed, tenacity, crit_stat, dh_stat, weapon_damage, delay, level=90) -> None:
-#         """
-#         Set physical ranged-specific stats with this class like main stat, traits, etc.
-
-#         inputs:
-#         mind - int, mind stat
-#         intelligence - int, intelligence stat
-#         vitality - int, vitality stat
-#         strength, - int, strength stat
-#         dexterity - int, strength stat
-#         det - int, determination stat
-#         skill_speed - int, skill speed stat
-#         spell_speed - int, spell speed stat
-#         tenacity - tenacity stat
-#         crit_stat - critical hit stat
-#         dh_stat - direct hit rate stat
-#         weapon_damage - weapon damage stat
-#         delay - weapon delay stat
-#         """
-#         super().__init__(dexterity, 120, dexterity, mind, intelligence, vitality, strength, dexterity, det,
-#                          tenacity, crit_stat, dh_stat, skill_speed, skill_speed, weapon_damage, delay, level=90)
-
-#         self.add_role('Physical Ranged')
-
-#         self.skill_speed = skill_speed
-#         self.spell_speed = spell_speed
-#         pass
+class PhysicalRanged(BaseStats):
+    def __init__(
+        self,
+        dexterity: int,
+        det: int,
+        skill_speed: int,
+        crit_stat: int,
+        dh_stat: int,
+        weapon_damage: int,
+        delay: float,
+        pet_attack_power: int = None,
+        pet_attack_power_scalar: float = 1.,
+        pet_attack_power_offset: int = -61,
+        pet_job_attribute: int = 100,
+        pet_atk_mod: int = 195,
+        level: int = 90,
+    ) -> None:
+        """Set stats specific to Physical Ranged.
+
+        Args:
+            dexterity (int): Dexterity stat.
+            det (int): Determination stat.
+            skill_speed (int): Skill Speed stat.
+            crit_stat (int): Critical Hit Stat
+            dh_stat (int): Direct Hit Rate stat.
+            weapon_damage (int): Weapon Damage stat.
+            delay (float): Weapon Delay stat.
+            pet_attack_power (int, optional): Pet attack power, Dexterity stat with no party bonus. Defaults to None.
+            pet_attack_power_scalar (float, optional): Pet attack power scalar, set to EW value for Automaton Queen. Defaults to 1..
+            pet_attack_power_offset (int, optional): Pet attack power offset. Set to EW value for Automaton Queen. Defaults to -61.
+            pet_job_attribute (int, optional): Pet job attribute, set to EW value for Automaton Queen. Defaults to 100.
+            pet_atk_mod (int, optional): Pet attack modifier, same as player. Defaults to 195.
+            level (int, optional): Player level. Defaults to 90.
+        """
+        super().__init__(
+            attack_power=dexterity,
+            trait=120,
+            main_stat=dexterity,
+            strength=330,
+            det=det,
+            crit_stat=crit_stat,
+            dh_stat=dh_stat,
+            dot_speed_stat=skill_speed,
+            auto_speed_stat=skill_speed,
+            weapon_damage=weapon_damage,
+            delay=delay,
+            pet_attack_power=pet_attack_power,
+            pet_attack_power_scalar=pet_attack_power_scalar,
+            pet_attack_power_offset=pet_attack_power_offset,
+            pet_job_attribute=pet_job_attribute,
+            pet_atk_mod=pet_atk_mod,
+            level=level,
+        )
+
+        self.add_role("Physical Ranged")
+
+        self.auto_trait = 100
+        self.dot_speed_stat = skill_speed
+        self.auto_speed_stat = skill_speed
+
+        if level == 90:
+            self.atk_mod = 195
+        if level == 80:
+            self.atk_mod = 165
+
+        pass
 
 
 class Melee(BaseStats):
     def __init__(
         self,
         main_stat: int,
         det: int,
         skill_speed: int,
         crit_stat: int,
         dh_stat: int,
         weapon_damage: int,
         delay: float,
         job: str,
         pet_attack_power: int = None,
-        pet_attack_power_scalar: float = 1.,
+        pet_attack_power_scalar: float = 1.0,
         pet_attack_power_offset: int = 0,
         pet_job_attribute: int = 100,
         pet_atk_mod: int = 195,
         level: int = 90,
     ) -> None:
         """
         Set melee-specific stats with this class like main stat, traits, etc.
@@ -783,15 +820,17 @@
             self.atk_mod = 195
         if level == 80:
             self.atk_mod = 165
 
         self.job = job
 
         if job not in ("Monk", "Dragoon", "Reaper", "Ninja", "Samurai"):
-            raise ValueError("Invalid job, accepted values are {'Monk', 'Dragoon', 'Reaper', 'Ninja', 'Samurai'}")
+            raise ValueError(
+                "Invalid job, accepted values are {'Monk', 'Dragoon', 'Reaper', 'Ninja', 'Samurai'}"
+            )
 
         if job in ("Monk", "Ninja"):
             self.job_attribute = 110
         # But why
         elif job == "Samurai":
             self.job_attribute = 112
         else:
```

### Comparing `ffxiv_stats-0.4.4/ffxiv_stats/moments.py` & `ffxiv_stats-0.4.5/ffxiv_stats/moments.py`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/ffxiv_stats/rate.py` & `ffxiv_stats-0.4.5/ffxiv_stats/rate.py`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/pyproject.toml` & `ffxiv_stats-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ffxiv_stats-0.4.4/PKG-INFO` & `ffxiv_stats-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffxiv_stats
-Version: 0.4.4
+Version: 0.4.5
 Summary: Compute damage variability in the critically acclaimed MMORPG Final Fantasy XIV.
 Author-email: Acerola Paracletus <ffxivacerola@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: numpy >= 1.20.2
 Requires-Dist: matplotlib >= 3.4.2
```

