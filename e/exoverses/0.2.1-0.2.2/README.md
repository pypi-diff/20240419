# Comparing `tmp/exoverses-0.2.1.tar.gz` & `tmp/exoverses-0.2.2.tar.gz`

## Comparing `exoverses-0.2.1.tar` & `exoverses-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 exoverses-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 exoverses-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 exoverses-0.2.1/README.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 exoverses-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 exoverses-0.2.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 exoverses-0.2.1/.github/workflows/release-please.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/disk.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/planet.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/star.py
--rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/system.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/universe.py
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/data/mamajek_rhk.csv
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/__init__.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/planet.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/star.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/system.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/universe.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/disk.py
--rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/planet.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/star.py
--rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/system.py
--rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/universe.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/fit/__init__.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/fit/planet.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/fit/system.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/util/__init__.py
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/util/misc.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 exoverses-0.2.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 exoverses-0.2.1/LICENSE
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 exoverses-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 exoverses-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 exoverses-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 exoverses-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 exoverses-0.2.2/README.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 exoverses-0.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 exoverses-0.2.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 exoverses-0.2.2/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/base/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/base/disk.py
+-rw-r--r--   0        0        0     9852 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/base/planet.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/base/star.py
+-rw-r--r--   0        0        0    15499 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/base/system.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/base/universe.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/data/mamajek_rhk.csv
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exosims/__init__.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exosims/planet.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exosims/star.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exosims/system.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exosims/universe.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exovista/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exovista/disk.py
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exovista/planet.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exovista/star.py
+-rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exovista/system.py
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/exovista/universe.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/fit/__init__.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/fit/planet.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/fit/system.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/util/__init__.py
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 exoverses-0.2.2/src/exoverses/util/misc.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 exoverses-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 exoverses-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 exoverses-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 exoverses-0.2.2/PKG-INFO
```

### Comparing `exoverses-0.2.1/.pre-commit-config.yaml` & `exoverses-0.2.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: trailing-whitespace
       - id: name-tests-test
       - id: end-of-file-fixer
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.3.7
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
   - repo: https://github.com/compilerla/conventional-pre-commit
```

### Comparing `exoverses-0.2.1/CHANGELOG.md` & `exoverses-0.2.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [0.2.2](https://github.com/CoreySpohn/exoverses/compare/v0.2.1...v0.2.2) (2024-04-19)
+
+
+### Bug Fixes
+
+* **main:** Improved the has_planets property, better planet classification string ([cf71a73](https://github.com/CoreySpohn/exoverses/commit/cf71a735a772c310f315c38b366d14c75f66de1f))
+
 ## [0.2.1](https://github.com/CoreySpohn/exoverses/compare/v0.2.0...v0.2.1) (2024-04-03)
 
 
 ### Bug Fixes
 
 * **main:** Remove usage of deprecated open_text importlib.resources method ([4e77086](https://github.com/CoreySpohn/exoverses/commit/4e77086b372a0a02d4ce9608b8e0b151aa7fa86c))
```

### Comparing `exoverses-0.2.1/README.md` & `exoverses-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/.github/workflows/publish-to-pypi.yml` & `exoverses-0.2.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/.github/workflows/release-please.yml` & `exoverses-0.2.2/.github/workflows/release-please.yml`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/base/planet.py` & `exoverses-0.2.2/src/exoverses/base/planet.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
 
         # # index of planet temp. cold,warm,hot
         L_types = ["Very Hot", "Hot", "Warm", "Cold", "Very Cold"]
         specific_L_bins = L_bins[Rp_bin, :]
         L_bin = np.digitize(Lp, specific_L_bins) - 1
         L_bin = max(0, min(L_bin, len(L_types) - 1))
         L_type = L_types[L_bin]
-        self.subtype = f"{Rp_type} {L_type}"
+        self.subtype = f"{L_type} {Rp_type.lower()}"
 
         # Determine if the planet is Earth-like
         # Reverse luminosity scaling
         a = self.a.to("AU").value / np.sqrt(self.star.luminosity.to("Lsun").value)
 
         lower_a = 0.95
         upper_a = 1.67
```

### Comparing `exoverses-0.2.1/src/exoverses/base/star.py` & `exoverses-0.2.2/src/exoverses/base/star.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/base/system.py` & `exoverses-0.2.2/src/exoverses/base/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
             f"Planets:\n{self.get_p_df()}"
         )
 
     @property
     def name(self):
         return self.star.name
 
+    @property
+    def has_planets(self):
+        return len(self.planets) > 0
+
     def planet_cleanup(self):
         self.pInds = np.arange(len(self.planets))
         # Sort the planets in the system by semi-major axis
         a_vals = [planet.a.value for planet in self.planets]
         self.planets = np.array(self.planets)[np.argsort(a_vals)].tolist()
         self.pInds = self.pInds[np.argsort(a_vals)]
 
@@ -64,39 +68,42 @@
             return [getattr(planet, attr).value for planet in self.planets] * getattr(
                 self.planets[0], attr
             ).unit
         else:
             return [getattr(planet, attr) for planet in self.planets]
 
     def get_p_df(self):
-        patts = [
-            "K",
-            "T",
-            "secosw",
-            "sesinw",
-            "T_c",
-            "a",
-            "e",
-            "inc",
-            "W",
-            "w",
-            "M0",
-            "t0",
-            "mass",
-            "radius",
-        ]
-        p_df = pd.DataFrame()
-        for att in patts:
-            pattr = self.getpattr(att)
-            if type(pattr) == u.Quantity:
-                p_df[att] = pattr.value
-            else:
-                p_df[att] = pattr
+        if self.has_planets:
+            patts = [
+                "K",
+                "T",
+                "secosw",
+                "sesinw",
+                "T_c",
+                "a",
+                "e",
+                "inc",
+                "W",
+                "w",
+                "M0",
+                "t0",
+                "mass",
+                "radius",
+            ]
+            p_df = pd.DataFrame()
+            for att in patts:
+                pattr = self.getpattr(att)
+                if type(pattr) == u.Quantity:
+                    p_df[att] = pattr.value
+                else:
+                    p_df[att] = pattr
 
-        return p_df
+            return p_df
+        else:
+            return "No planets in system."
 
     def propagate_rv(self, times):
         """
         Propagates system at all times given and returns the radial velocity
 
         """
         # Get unique time values, multiple instruments can be scheduled to
```

### Comparing `exoverses-0.2.1/src/exoverses/data/mamajek_rhk.csv` & `exoverses-0.2.2/src/exoverses/data/mamajek_rhk.csv`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/exosims/planet.py` & `exoverses-0.2.2/src/exoverses/exosims/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/exosims/star.py` & `exoverses-0.2.2/src/exoverses/exosims/star.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/exosims/system.py` & `exoverses-0.2.2/src/exoverses/exosims/system.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/exosims/universe.py` & `exoverses-0.2.2/src/exoverses/exosims/universe.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/exovista/disk.py` & `exoverses-0.2.2/src/exoverses/exovista/disk.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/exovista/planet.py` & `exoverses-0.2.2/src/exoverses/exovista/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/exovista/star.py` & `exoverses-0.2.2/src/exoverses/exovista/star.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/exovista/system.py` & `exoverses-0.2.2/src/exoverses/exovista/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,25 +101,27 @@
                 _E = _E[0] * u.rad
                 planet.M0 = (
                     (_E.value - planet.e * np.sin(_E)) % (2 * np.pi) * u.rad
                 ).to(u.deg)
                 planet.solve_dependent_params()
                 planet.classify_planet()
         if filter:
+            # TODO: Make this more flexible
+            # Keep only the planets that are Earth-like
             earth_ind = self.getpattr("is_earth")
-            K_vals = self.getpattr("K")
-            max_K = K_vals.max()
-            max_earth_K = self.getpattr("K")[np.argwhere(earth_ind).ravel()]
+            # K_vals = self.getpattr("K")
+            # max_K = K_vals.max()
+            # max_earth_K = self.getpattr("K")[np.argwhere(earth_ind).ravel()]
             # Remove all planets with K values larger than the largest K value of the Earth
             # except the larget K value
-            to_remove = np.argwhere(
-                (K_vals > max_earth_K.max()) & (K_vals != max_K)
-            ).ravel()
+            # to_remove = np.argwhere(
+            #     (K_vals > max_earth_K.max()) & (K_vals != max_K)
+            # ).ravel()
             self.planets = [
-                self.planets[i] for i in range(len(self.planets)) if i not in to_remove
+                self.planets[i] for i in range(len(self.planets)) if earth_ind[i]
             ]
             self.planet_cleanup()
 
     def spec_flux_densities(self, wavelengths, times):
         """
         Calculate the spectral flux density of the system at the given times and
         wavelengths
```

### Comparing `exoverses-0.2.1/src/exoverses/exovista/universe.py` & `exoverses-0.2.2/src/exoverses/exovista/universe.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,17 @@
 
 
 class ExovistaUniverse(Universe):
     """
     Class for the whole exoVista universe
     """
 
-    def __init__(self, path, target_list, convert=False, cache=False):
+    def __init__(
+        self, path, target_list, convert=False, cache=False, initial_epoch=2000
+    ):
         """
         Args:
             path (str or Path):
                 Location of all the system files. Should be something like "data/1/"
         """
         self.type = "ExoVista"
         if cache:
@@ -98,20 +100,21 @@
         self.names = [system.star.name for system in self.systems]
 
         super().__init__()
 
 
 def generate_systems(targetlist, path, workers=12):
     settings = Settings.Settings(timemax=10.0, output_dir=path)
+    settings.emax = 0.1
 
     stars, nexozodis = load_stars.load_stars(targetlist, from_master=True)
     print("\n{0:d} stars in model ranges.".format(len(stars)))
 
     planets, albedos = generate_planets.generate_planets(
-        stars, settings, force_earth=True
+        stars, settings, force_earth=False
     )
     disks, compositions = generate_disks.generate_disks(
         stars, planets, settings, nexozodis=nexozodis
     )
     print("Generating scenes. (This may take a while.)")
 
     cores = min(workers, os.cpu_count())
```

### Comparing `exoverses-0.2.1/src/exoverses/fit/planet.py` & `exoverses-0.2.2/src/exoverses/fit/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/fit/system.py` & `exoverses-0.2.2/src/exoverses/fit/system.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/src/exoverses/util/misc.py` & `exoverses-0.2.2/src/exoverses/util/misc.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/.gitignore` & `exoverses-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/LICENSE` & `exoverses-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/pyproject.toml` & `exoverses-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.1/PKG-INFO` & `exoverses-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: exoverses
-Version: 0.2.1
+Version: 0.2.2
 Summary: A unified interface for the various tools that create universes for exoplanet simulations
 Project-URL: Homepage, https://github.com/CoreySpohn/exoverses
 Project-URL: Issues, https://github.com/CoreySpohn/exoverses/issues
 Author-email: Corey Spohn <corey.a.spohn@nasa.gov>
 License: MIT License
         
         Copyright (c) 2023 CoreySpohn
```

