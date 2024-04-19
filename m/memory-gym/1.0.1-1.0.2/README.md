# Comparing `tmp/memory_gym-1.0.1.tar.gz` & `tmp/memory_gym-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_gym-1.0.1.tar", last modified: Mon Apr 15 07:31:04 2024, max compression
+gzip compressed data, was "memory_gym-1.0.2.tar", last modified: Fri Apr 19 12:32:22 2024, max compression
```

## Comparing `memory_gym-1.0.1.tar` & `memory_gym-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 07:31:04.347465 memory_gym-1.0.1/
--rw-rw-rw-   0        0        0     1091 2024-04-15 07:30:51.000000 memory_gym-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    30634 2024-04-15 07:31:04.346465 memory_gym-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    29854 2024-04-15 07:30:51.000000 memory_gym-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 07:31:04.325444 memory_gym-1.0.1/memory_gym/
--rw-rw-rw-   0        0        0     1896 2023-08-21 08:19:45.000000 memory_gym-1.0.1/memory_gym/__init__.py
--rw-rw-rw-   0        0        0    12630 2023-08-24 10:26:30.000000 memory_gym-1.0.1/memory_gym/character_controller.py
--rw-rw-rw-   0        0        0    21682 2024-01-28 12:49:20.000000 memory_gym-1.0.1/memory_gym/endless_mortar_mayhem.py
--rw-rw-rw-   0        0        0    23640 2024-01-28 12:50:23.000000 memory_gym-1.0.1/memory_gym/endless_mystery_path.py
--rw-rw-rw-   0        0        0    25755 2024-01-28 12:49:01.000000 memory_gym-1.0.1/memory_gym/endless_searing_spotlights.py
--rw-rw-rw-   0        0        0      328 2023-08-21 08:19:45.000000 memory_gym-1.0.1/memory_gym/environment.py
--rw-rw-rw-   0        0        0    21467 2024-01-28 12:50:13.000000 memory_gym-1.0.1/memory_gym/mortar_mayhem.py
--rw-rw-rw-   0        0        0    15608 2024-01-28 12:49:42.000000 memory_gym-1.0.1/memory_gym/mortar_mayhem_b.py
--rw-rw-rw-   0        0        0    15611 2024-01-28 12:49:51.000000 memory_gym-1.0.1/memory_gym/mortar_mayhem_b_grid.py
--rw-rw-rw-   0        0        0    21719 2024-01-28 12:39:18.000000 memory_gym-1.0.1/memory_gym/mortar_mayhem_grid.py
--rw-rw-rw-   0        0        0    15274 2024-01-28 12:51:19.000000 memory_gym-1.0.1/memory_gym/mystery_path.py
--rw-rw-rw-   0        0        0    15531 2024-01-28 12:50:07.000000 memory_gym-1.0.1/memory_gym/mystery_path_grid.py
--rw-rw-rw-   0        0        0    36457 2023-09-23 05:15:45.000000 memory_gym-1.0.1/memory_gym/pygame_assets.py
--rw-rw-rw-   0        0        0    28043 2024-03-19 07:17:52.000000 memory_gym-1.0.1/memory_gym/searing_spotlights.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:31:04.346465 memory_gym-1.0.1/memory_gym.egg-info/
--rw-rw-rw-   0        0        0    30634 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      640 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 07:31:04.000000 memory_gym-1.0.1/memory_gym.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 07:31:04.347465 memory_gym-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2274 2024-04-15 07:30:51.000000 memory_gym-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:32:22.819419 memory_gym-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-19 12:32:07.000000 memory_gym-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    30634 2024-04-19 12:32:22.818419 memory_gym-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    29854 2024-04-19 12:32:07.000000 memory_gym-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 12:32:22.788392 memory_gym-1.0.2/memory_gym/
+-rw-rw-rw-   0        0        0     1896 2023-08-21 08:19:45.000000 memory_gym-1.0.2/memory_gym/__init__.py
+-rw-rw-rw-   0        0        0    12630 2023-08-24 10:26:30.000000 memory_gym-1.0.2/memory_gym/character_controller.py
+-rw-rw-rw-   0        0        0    21652 2024-04-19 12:09:30.000000 memory_gym-1.0.2/memory_gym/endless_mortar_mayhem.py
+-rw-rw-rw-   0        0        0    23595 2024-04-19 11:57:46.000000 memory_gym-1.0.2/memory_gym/endless_mystery_path.py
+-rw-rw-rw-   0        0        0    25720 2024-04-19 11:58:44.000000 memory_gym-1.0.2/memory_gym/endless_searing_spotlights.py
+-rw-rw-rw-   0        0        0      328 2023-08-21 08:19:45.000000 memory_gym-1.0.2/memory_gym/environment.py
+-rw-rw-rw-   0        0        0    21426 2024-04-19 12:10:11.000000 memory_gym-1.0.2/memory_gym/mortar_mayhem.py
+-rw-rw-rw-   0        0        0    15610 2024-04-19 11:56:21.000000 memory_gym-1.0.2/memory_gym/mortar_mayhem_b.py
+-rw-rw-rw-   0        0        0    15613 2024-04-19 11:56:29.000000 memory_gym-1.0.2/memory_gym/mortar_mayhem_b_grid.py
+-rw-rw-rw-   0        0        0    21635 2024-04-19 12:09:57.000000 memory_gym-1.0.2/memory_gym/mortar_mayhem_grid.py
+-rw-rw-rw-   0        0        0    15236 2024-04-19 12:00:31.000000 memory_gym-1.0.2/memory_gym/mystery_path.py
+-rw-rw-rw-   0        0        0    15489 2024-04-19 12:00:15.000000 memory_gym-1.0.2/memory_gym/mystery_path_grid.py
+-rw-rw-rw-   0        0        0    36457 2023-09-23 05:15:45.000000 memory_gym-1.0.2/memory_gym/pygame_assets.py
+-rw-rw-rw-   0        0        0    28012 2024-04-19 12:12:32.000000 memory_gym-1.0.2/memory_gym/searing_spotlights.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:32:22.817418 memory_gym-1.0.2/memory_gym.egg-info/
+-rw-rw-rw-   0        0        0    30634 2024-04-19 12:32:22.000000 memory_gym-1.0.2/memory_gym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2024-04-19 12:32:22.000000 memory_gym-1.0.2/memory_gym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 12:32:22.000000 memory_gym-1.0.2/memory_gym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      640 2024-04-19 12:32:22.000000 memory_gym-1.0.2/memory_gym.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-04-19 12:32:22.000000 memory_gym-1.0.2/memory_gym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 12:32:22.000000 memory_gym-1.0.2/memory_gym.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 12:32:22.820420 memory_gym-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2274 2024-04-19 12:32:07.000000 memory_gym-1.0.2/setup.py
```

### Comparing `memory_gym-1.0.1/LICENSE` & `memory_gym-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `memory_gym-1.0.1/PKG-INFO` & `memory_gym-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-gym
-Version: 1.0.1
+Version: 1.0.2
 Summary: A gym that contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing Spotlights
 Home-page: https://github.com/MarcoMeter/drl-memory-gym
 Author: Marco Pleines
 Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
 Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
 Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial Observation
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: memory-gym Version: 1.0.1 Summary: A gym that
+Metadata-Version: 2.1 Name: memory-gym Version: 1.0.2 Summary: A gym that
 contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing
 Spotlights Home-page: https://github.com/MarcoMeter/drl-memory-gym Author:
 Marco Pleines Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
 Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
 Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial
 Observation Classifier: Programming Language :: Python :: 3 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `memory_gym-1.0.1/README.md` & `memory_gym-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `memory_gym-1.0.1/memory_gym/__init__.py` & `memory_gym-1.0.2/memory_gym/__init__.py`

 * *Files identical despite different names*

### Comparing `memory_gym-1.0.1/memory_gym/character_controller.py` & `memory_gym-1.0.2/memory_gym/character_controller.py`

 * *Files identical despite different names*

### Comparing `memory_gym-1.0.1/memory_gym/endless_mortar_mayhem.py` & `memory_gym-1.0.2/memory_gym/endless_mortar_mayhem.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from memory_gym.pygame_assets import Command, MortarArena
 from pygame._sdl2 import Window, Texture, Renderer
 
 SCALE = 0.25
 
 class EndlessMortarMayhemEnv(CustomEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 25,
     }
 
     default_reset_parameters = {
                 "max_steps": -1,
                 "agent_scale": 1.0 * SCALE,
                 "agent_speed": 12.0 * SCALE,
@@ -56,15 +56,15 @@
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
         super().__init__()
         
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -75,15 +75,15 @@
             pygame.event.set_allowed(None)
 
         # Init debug window
         self.debug_window = None      
 
         # Setup observation and action space
         self.action_space = spaces.MultiDiscrete([3, 3])
-        self.observation_space= sspaces.Box(
+        self.observation_space= spaces.Box(
                     low = 0,
                     high = 255,
                     shape = [self.screen_dim, self.screen_dim, 3],
                     dtype = np.uint8)
 
         # Optional information that is part of the returned info dictionary during reset and step
         # The absolute position (ground truth) of the agent is distributed using the info dictionary.
@@ -368,53 +368,52 @@
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
-            {np.ndarray} -- The rendered image of the environment.
+            {np.ndarray} -- The rendered image of the environment. Returns None if the render mode is set to "human".
         """
-        if self.render_mode is not None:
-            if self._command_visualization:
-                    fps = 3
-            else:
-                fps = EndlessMortarMayhemEnv.metadata["render_fps"]
+        if self.render_mode == "human":
+            # Create debug window if it doesn't exist yet
+            if self.debug_window is None:
+                self.debug_window = Window(size = (336, 336))
+                self.debug_window.show()
+                self.renderer = Renderer(self.debug_window)
             
-            if self.render_mode == "rgb_array":
-                self.clock.tick(fps)
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
-            elif self.render_mode == "debug_rgb_array":
-                # Create debug window if it doesn't exist yet
-                if self.debug_window is None:
-                    self.debug_window = Window(size = (336, 336))
-                    self.debug_window.show()
-                    self.renderer = Renderer(self.debug_window)
-                
-                self.debug_window.title = "seed " + str(self.current_seed)
-                self.clock.tick(fps)
-
-                debug_surface = self._build_debug_surface()
-                texture = Texture.from_surface(self.renderer, debug_surface)
-                texture.draw(dstrect=(0, 0))
-                self.renderer.present()
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(self.renderer.to_surface()).astype(np.uint8), 3))
+            self.debug_window.title = "seed " + str(self.current_seed)
+            
+            fps = EndlessMortarMayhemEnv.metadata["render_fps"]
+            if self._command_visualization:
+                fps = 3
+            self.clock.tick(fps)
+
+            debug_surface = self._build_debug_surface()
+            texture = Texture.from_surface(self.renderer, debug_surface)
+            texture.draw(dstrect=(0, 0))
+            self.renderer.present()
+        elif self.render_mode == "rgb_array":
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        elif self.render_mode == "debug_rgb_array":
+            debug_surface = self._build_debug_surface()
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(debug_surface).astype(np.uint8), 3))
 
     def close(self):
         """Close the environment."""
         if self.debug_window is not None:
             self.debug_window.destroy()
         pygame.quit()
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = EndlessMortarMayhemEnv(render_mode="debug_rgb_array")
+    env = EndlessMortarMayhemEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     vis_obs, reset_info = env.reset(seed = options.seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym/endless_mystery_path.py` & `memory_gym-1.0.2/memory_gym/endless_mystery_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from memory_gym.pygame_assets import EndlessMysteryPath, draw_column_tile_surface
 from pygame._sdl2 import Window, Texture, Renderer
 
 SCALE = 0.25
 
 class EndlessMysteryPathEnv(CustomEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 25,
     }
 
     default_reset_parameters = {
                 "max_steps": -1,
                 "agent_scale": 1.0 * SCALE,
                 "agent_speed": 12.0 * SCALE,
@@ -57,15 +57,15 @@
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
         super().__init__()
         
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -440,48 +440,48 @@
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
-            {np.ndarray} -- The rendered image of the environment.
+            {np.ndarray} -- The rendered image of the environment. Returns None if the render mode is set to "human".
         """
-        if self.render_mode is not None:
-            if self.render_mode == "rgb_array":
-                self.clock.tick(EndlessMysteryPathEnv.metadata["render_fps"])
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
-            elif self.render_mode == "debug_rgb_array":
-                # Create debug window if it doesn't exist yet
-                if self.debug_window is None:
-                    self.debug_window = Window(size = (336, 336))
-                    self.debug_window.show()
-                    self.renderer = Renderer(self.debug_window)
-                
-                self.debug_window.title = "seed " + str(self.current_seed)
-                self.clock.tick(EndlessMysteryPathEnv.metadata["render_fps"])
-
-                debug_surface = self._build_debug_surface()
-                texture = Texture.from_surface(self.renderer, debug_surface)
-                texture.draw(dstrect=(0, 0))
-                self.renderer.present()
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(self.renderer.to_surface()).astype(np.uint8), 3))
+        if self.render_mode == "human":
+            # Create debug window if it doesn't exist yet
+            if self.debug_window is None:
+                self.debug_window = Window(size = (336, 336))
+                self.debug_window.show()
+                self.renderer = Renderer(self.debug_window)
+            
+            self.debug_window.title = "seed " + str(self.current_seed)
+            self.clock.tick(EndlessMysteryPathEnv.metadata["render_fps"])
+
+            debug_surface = self._build_debug_surface()
+            texture = Texture.from_surface(self.renderer, debug_surface)
+            texture.draw(dstrect=(0, 0))
+            self.renderer.present()
+        elif self.render_mode == "rgb_array":
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        elif self.render_mode == "debug_rgb_array":
+            debug_surface = self._build_debug_surface()
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(debug_surface).astype(np.uint8), 3))
 
     def close(self):
         """Close the environment."""
         if self.debug_window is not None:
             self.debug_window.destroy()
         pygame.quit()
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = EndlessMysteryPathEnv(render_mode = "debug_rgb_array")
+    env = EndlessMysteryPathEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     vis_obs, reset_info = env.reset(seed = seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym/endless_searing_spotlights.py` & `memory_gym-1.0.2/memory_gym/endless_searing_spotlights.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from memory_gym.pygame_assets import Coin, GridPositionSampler, Spotlight, get_tiled_background_surface
 from pygame._sdl2 import Window, Texture, Renderer
 
 SCALE = 0.25
 
 class EndlessSearingSpotlightsEnv(CustomEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 25,
     }
 
     default_reset_parameters = {
                 # Spotlight parameters
                 "max_steps": -1,
                 "steps_per_coin": 160,
@@ -77,15 +77,15 @@
 
         Arguments:
             render_mode {str} -- The rendering mode for the environment. (default: None)
         """
         super().__init__()
         
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -498,42 +498,42 @@
             self.debug_window.destroy()
         pygame.quit()
 
     def render(self):
         """Render the environment.
 
         Returns:
-            {np.ndarray} -- The rendered image of the environment.
+            {np.ndarray} -- The rendered image of the environment. Returns None if the render mode is set to "human".
         """
-        if self.render_mode is not None:
-            if self.render_mode == "rgb_array":
-                self.clock.tick(EndlessSearingSpotlightsEnv.metadata["render_fps"])
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
-            elif self.render_mode == "debug_rgb_array":
-                # Create debug window if it doesn't exist yet
-                if self.debug_window is None:
-                    self.debug_window = Window(size = (336, 336))
-                    self.debug_window.show()
-                    self.renderer = Renderer(self.debug_window)
-
-                self.debug_window.title = "seed " + str(self.current_seed)
-                self.clock.tick(EndlessSearingSpotlightsEnv.metadata["render_fps"])
-
-                debug_surface = self._build_debug_surface()
-                texture = Texture.from_surface(self.renderer, debug_surface)
-                texture.draw(dstrect=(0, 0))
-                self.renderer.present()
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(self.renderer.to_surface()).astype(np.uint8), 3))
+        if self.render_mode == "human":
+            # Create debug window if it doesn't exist yet
+            if self.debug_window is None:
+                self.debug_window = Window(size = (336, 336))
+                self.debug_window.show()
+                self.renderer = Renderer(self.debug_window)
+            
+            self.debug_window.title = "seed " + str(self.current_seed)
+            self.clock.tick(EndlessSearingSpotlightsEnv.metadata["render_fps"])
+
+            debug_surface = self._build_debug_surface()
+            texture = Texture.from_surface(self.renderer, debug_surface)
+            texture.draw(dstrect=(0, 0))
+            self.renderer.present()
+        elif self.render_mode == "rgb_array":
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        elif self.render_mode == "debug_rgb_array":
+            debug_surface = self._build_debug_surface()
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(debug_surface).astype(np.uint8), 3))
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = EndlessSearingSpotlightsEnv(render_mode = "debug_rgb_array")
+    env = EndlessSearingSpotlightsEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     vis_obs, reset_info = env.reset(seed = options.seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym/mortar_mayhem.py` & `memory_gym-1.0.2/memory_gym/mortar_mayhem.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from memory_gym.pygame_assets import Command, MortarArena, calc_max_episode_steps
 from pygame._sdl2 import Window, Texture, Renderer
 
 SCALE = 0.25
 
 class MortarMayhemEnv(CustomEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 25,
     }
 
     default_reset_parameters = {
                 "agent_scale": 1.0 * SCALE,
                 "agent_speed": 12.0 * SCALE,
                 "arena_size": 5,
@@ -58,15 +58,15 @@
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
         super().__init__()
         
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -368,53 +368,52 @@
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
-            {np.ndarray} -- The rendered image of the environment.
+            {np.ndarray} -- The rendered image of the environment. Returns None if the render mode is set to "human".
         """
-        if self.render_mode is not None:
-            if self._command_visualization:
-                    fps = 4
-            else:
-                fps = MortarMayhemEnv.metadata["render_fps"]
+        if self.render_mode == "human":
+            # Create debug window if it doesn't exist yet
+            if self.debug_window is None:
+                self.debug_window = Window(size = (336, 336))
+                self.debug_window.show()
+                self.renderer = Renderer(self.debug_window)
             
-            if self.render_mode == "rgb_array":
-                self.clock.tick(fps)
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
-            elif self.render_mode == "debug_rgb_array":
-                # Create debug window if it doesn't exist yet
-                if self.debug_window is None:
-                    self.debug_window = Window(size = (336, 336))
-                    self.debug_window.show()
-                    self.renderer = Renderer(self.debug_window)
-                
-                self.debug_window.title = "seed " + str(self.current_seed)
-                self.clock.tick(fps)
-
-                debug_surface = self._build_debug_surface()
-                texture = Texture.from_surface(self.renderer, debug_surface)
-                texture.draw(dstrect=(0, 0))
-                self.renderer.present()
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(self.renderer.to_surface()).astype(np.uint8), 3))
+            self.debug_window.title = "seed " + str(self.current_seed)
+
+            fps = MortarMayhemEnv.metadata["render_fps"]
+            if self._command_visualization:
+                fps = 3
+            self.clock.tick(fps)
+
+            debug_surface = self._build_debug_surface()
+            texture = Texture.from_surface(self.renderer, debug_surface)
+            texture.draw(dstrect=(0, 0))
+            self.renderer.present()
+        elif self.render_mode == "rgb_array":
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        elif self.render_mode == "debug_rgb_array":
+            debug_surface = self._build_debug_surface()
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(debug_surface).astype(np.uint8), 3))
 
     def close(self):
         """Close the environment."""
         if self.debug_window is not None:
             self.debug_window.destroy()
         pygame.quit()
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = MortarMayhemEnv(render_mode="debug_rgb_array")
+    env = MortarMayhemEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     vis_obs, reset_info = env.reset(seed = options.seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym/mortar_mayhem_b.py` & `memory_gym-1.0.2/memory_gym/mortar_mayhem_b.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from memory_gym.mortar_mayhem import MortarMayhemEnv
 from memory_gym.pygame_assets import Command, MortarArena, calc_max_episode_steps
 
 SCALE = 0.25
 
 class MortarMayhemTaskBEnv(MortarMayhemEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 25,
     }
 
     default_reset_parameters = {
                 "agent_scale": 1.0 * SCALE,
                 "agent_speed": 12.0 * SCALE,
                 "arena_size": 5,
@@ -57,15 +57,15 @@
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
         super().__init__(render_mode)
 
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -288,15 +288,15 @@
         return {"visual_observation": vis_obs, "vector_observation": self._commands_one_hot}, reward, done, False, info
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = MortarMayhemTaskBEnv(render_mode = "debug_rgb_array")
+    env = MortarMayhemTaskBEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     obs, reset_info = env.reset(seed = options.seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym/mortar_mayhem_b_grid.py` & `memory_gym-1.0.2/memory_gym/mortar_mayhem_b_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from memory_gym.mortar_mayhem_grid import GridMortarMayhemEnv
 from memory_gym.pygame_assets import Command, MortarArena, calc_max_episode_steps
 
 SCALE = 0.25
 
 class GridMortarMayhemTaskBEnv(GridMortarMayhemEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 1,
     }
 
     default_reset_parameters = {
                 "agent_scale": 1.0 * SCALE,
                 "arena_size": 5,
                 "allowed_commands": 5,
@@ -56,15 +56,15 @@
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
         super().__init__(render_mode)
 
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -286,15 +286,15 @@
         return {"visual_observation": vis_obs, "vector_observation": self._commands_one_hot}, reward, done, False, info
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = GridMortarMayhemTaskBEnv(render_mode = "debug_rgb_array")
+    env = GridMortarMayhemTaskBEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     obs, reset_info = env.reset(seed = options.seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym/mortar_mayhem_grid.py` & `memory_gym-1.0.2/memory_gym/mortar_mayhem_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from memory_gym.pygame_assets import Command, MortarArena, calc_max_episode_steps
 from pygame._sdl2 import Window, Texture, Renderer
 
 SCALE = 0.25
 
 class GridMortarMayhemEnv(CustomEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 6,
     }
 
     default_reset_parameters = {
                 "agent_scale": 1.0 * SCALE,
                 "arena_size": 5,
                 "allowed_commands": 5,
@@ -57,15 +57,15 @@
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
         super().__init__()
         
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -374,53 +374,52 @@
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
-            {np.ndarray} -- The rendered image of the environment.
+            {np.ndarray} -- The rendered image of the environment. Returns None if the render mode is set to "human".
         """
-        if self.render_mode is not None:
-            if self._command_visualization:
-                    fps = GridMortarMayhemEnv.metadata["render_fps"]
-            else:
-                fps = GridMortarMayhemEnv.metadata["render_fps"]
+        if self.render_mode == "human":
+            # Create debug window if it doesn't exist yet
+            if self.debug_window is None:
+                self.debug_window = Window(size = (336, 336))
+                self.debug_window.show()
+                self.renderer = Renderer(self.debug_window)
             
-            if self.render_mode == "rgb_array":
-                self.clock.tick(fps)
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
-            elif self.render_mode == "debug_rgb_array":
-                # Create debug window if it doesn't exist yet
-                if self.debug_window is None:
-                    self.debug_window = Window(size = (336, 336))
-                    self.debug_window.show()
-                    self.renderer = Renderer(self.debug_window)
-                
-                self.debug_window.title = "seed " + str(self.current_seed)
-                self.clock.tick(fps)
-
-                debug_surface = self._build_debug_surface()
-                texture = Texture.from_surface(self.renderer, debug_surface)
-                texture.draw(dstrect=(0, 0))
-                self.renderer.present()
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(self.renderer.to_surface()).astype(np.uint8), 3))
+            self.debug_window.title = "seed " + str(self.current_seed)
+
+            fps = GridMortarMayhemEnv.metadata["render_fps"]
+            if self._command_visualization:
+                fps = 3
+            self.clock.tick(fps)
+
+            debug_surface = self._build_debug_surface()
+            texture = Texture.from_surface(self.renderer, debug_surface)
+            texture.draw(dstrect=(0, 0))
+            self.renderer.present()
+        elif self.render_mode == "rgb_array":
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        elif self.render_mode == "debug_rgb_array":
+            debug_surface = self._build_debug_surface()
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(debug_surface).astype(np.uint8), 3))
 
     def close(self):
         """Close the environment."""
         if self.debug_window is not None:
             self.debug_window.destroy()
         pygame.quit()
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = GridMortarMayhemEnv(render_mode = "debug_rgb_array")
+    env = GridMortarMayhemEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     vis_obs, reset_info = env.reset(seed = options.seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym/mystery_path.py` & `memory_gym-1.0.2/memory_gym/mystery_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from memory_gym.pygame_assets import MysteryPath
 from pygame._sdl2 import Window, Texture, Renderer
 
 SCALE = 0.25
 
 class MysteryPathEnv(CustomEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 25,
     }
 
     default_reset_parameters = {
                 "max_steps": 512,
                 "agent_scale": 1.0 * SCALE,
                 "agent_speed": 12.0 * SCALE,
@@ -54,15 +54,15 @@
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
         super().__init__()
         
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -275,48 +275,48 @@
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
-            {np.ndarray} -- The rendered image of the environment.
+            {np.ndarray} -- The rendered image of the environment. Returns None if the render mode is set to "human".
         """
-        if self.render_mode is not None:
-            if self.render_mode == "rgb_array":
-                self.clock.tick(MysteryPathEnv.metadata["render_fps"])
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
-            elif self.render_mode == "debug_rgb_array":
-                # Create debug window if it doesn't exist yet
-                if self.debug_window is None:
-                    self.debug_window = Window(size = (336, 336))
-                    self.debug_window.show()
-                    self.renderer = Renderer(self.debug_window)
-                
-                self.debug_window.title = "seed " + str(self.current_seed)
-                self.clock.tick(MysteryPathEnv.metadata["render_fps"])
-
-                debug_surface = self._build_debug_surface()
-                texture = Texture.from_surface(self.renderer, debug_surface)
-                texture.draw(dstrect=(0, 0))
-                self.renderer.present()
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(self.renderer.to_surface()).astype(np.uint8), 3))
+        if self.render_mode == "human":
+            # Create debug window if it doesn't exist yet
+            if self.debug_window is None:
+                self.debug_window = Window(size = (336, 336))
+                self.debug_window.show()
+                self.renderer = Renderer(self.debug_window)
+            
+            self.debug_window.title = "seed " + str(self.current_seed)
+            self.clock.tick(MysteryPathEnv.metadata["render_fps"])
+
+            debug_surface = self._build_debug_surface()
+            texture = Texture.from_surface(self.renderer, debug_surface)
+            texture.draw(dstrect=(0, 0))
+            self.renderer.present()
+        elif self.render_mode == "rgb_array":
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        elif self.render_mode == "debug_rgb_array":
+            debug_surface = self._build_debug_surface()
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(debug_surface).astype(np.uint8), 3))
 
     def close(self):
         """Close the environment."""
         if self.debug_window is not None:
             self.debug_window.destroy()
         pygame.quit()
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = MysteryPathEnv(render_mode = "debug_rgb_array")
+    env = MysteryPathEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     vis_obs, reset_info = env.reset(seed = seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym/mystery_path_grid.py` & `memory_gym-1.0.2/memory_gym/mystery_path_grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from memory_gym.pygame_assets import MysteryPath
 from pygame._sdl2 import Window, Texture, Renderer
 
 SCALE = 0.25
 
 class GridMysteryPathEnv(CustomEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 3,
     }
 
     default_reset_parameters = {
                 "max_steps": 128,
                 "agent_scale": 1.0 * SCALE,
                 "cardinal_origin_choice": [0, 1, 2, 3],
@@ -53,15 +53,15 @@
 
         Arguments:
             render_mode {str} -- The render mode for the environment. Default is None. (default: {None})
         """
         super().__init__()
         
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -276,48 +276,48 @@
 
         return vis_obs, reward, done, False, info
 
     def render(self):
         """Render the environment.
 
         Returns:
-            {np.ndarray} -- The rendered image of the environment.
+            {np.ndarray} -- The rendered image of the environment. Returns None if the render mode is set to "human".
         """
-        if self.render_mode is not None:
-            if self.render_mode == "rgb_array":
-                self.clock.tick(GridMysteryPathEnv.metadata["render_fps"])
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
-            elif self.render_mode == "debug_rgb_array":
-                # Create debug window if it doesn't exist yet
-                if self.debug_window is None:
-                    self.debug_window = Window(size = (336, 336))
-                    self.debug_window.show()
-                    self.renderer = Renderer(self.debug_window)
-                
-                self.debug_window.title = "seed " + str(self.current_seed)
-                self.clock.tick(GridMysteryPathEnv.metadata["render_fps"])
-
-                debug_surface = self._build_debug_surface()
-                texture = Texture.from_surface(self.renderer, debug_surface)
-                texture.draw(dstrect=(0, 0))
-                self.renderer.present()
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(self.renderer.to_surface()).astype(np.uint8), 3))
+        if self.render_mode == "human":
+            # Create debug window if it doesn't exist yet
+            if self.debug_window is None:
+                self.debug_window = Window(size = (336, 336))
+                self.debug_window.show()
+                self.renderer = Renderer(self.debug_window)
+            
+            self.debug_window.title = "seed " + str(self.current_seed)
+            self.clock.tick(GridMysteryPathEnv.metadata["render_fps"])
+
+            debug_surface = self._build_debug_surface()
+            texture = Texture.from_surface(self.renderer, debug_surface)
+            texture.draw(dstrect=(0, 0))
+            self.renderer.present()
+        elif self.render_mode == "rgb_array":
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        elif self.render_mode == "debug_rgb_array":
+            debug_surface = self._build_debug_surface()
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(debug_surface).astype(np.uint8), 3))
 
     def close(self):
         """Close the environment."""
         if self.debug_window is not None:
             self.debug_window.destroy()
         pygame.quit()
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = GridMysteryPathEnv(render_mode = "debug_rgb_array")
+    env = GridMysteryPathEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     vis_obs, reset_info = env.reset(seed = seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym/pygame_assets.py` & `memory_gym-1.0.2/memory_gym/pygame_assets.py`

 * *Files identical despite different names*

### Comparing `memory_gym-1.0.1/memory_gym/searing_spotlights.py` & `memory_gym-1.0.2/memory_gym/searing_spotlights.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from memory_gym.pygame_assets import Coin, Exit, GridPositionSampler, Spotlight, get_tiled_background_surface
 from pygame._sdl2 import Window, Texture, Renderer
 
 SCALE = 0.25
 
 class SearingSpotlightsEnv(CustomEnv):
     metadata = {
-        "render_modes": ["rgb_array", "debug_rgb_array"],
+        "render_modes": ["human", "rgb_array", "debug_rgb_array"],
         "render_fps": 25,
     }
 
     default_reset_parameters = {
                 # Spotlight parameters
                 "max_steps": 256,
                 "initial_spawns": 4,
@@ -86,15 +86,15 @@
 
         Arguments:
             render_mode {str} -- The rendering mode for the environment. (default: None)
         """
         super().__init__()
         
         self.render_mode = render_mode
-        if render_mode is None:
+        if render_mode != "human":
             os.putenv('SDL_VIDEODRIVER', 'fbcon')
             os.environ["SDL_VIDEODRIVER"] = "dummy"
         else:
             pygame.display.set_caption("Environment")
 
         # Init PyGame screen
         pygame.init()
@@ -119,15 +119,15 @@
         # Tiled background surface
         self.blue_background_surface = get_tiled_background_surface(self.screen, self.screen_dim, (0, 0, 255), SCALE)
         self.red_background_surface = get_tiled_background_surface(self.screen, self.screen_dim, (255, 0, 0), SCALE)
 
         # Spotlight surface
         self.spotlight_surface = pygame.Surface((self.screen_dim, self.screen_dim))
         self.spotlight_surface.fill(0)
-        self.spotlight_surface.set_colorkey((255, 0, 0, 0))
+        self.spotlight_surface.set_colorkey((255, 0, 0))
 
         # Agent boundaries
         self.walkable_rect = pygame.Rect(0, 16 * SCALE, self.screen_dim, self.screen_dim - 16 * SCALE)
 
         # Init grid spawner
         self.grid_sampler = GridPositionSampler(self.screen_dim)
         # self.grid_sampler = GridPositionSampler(self.screen_dim - 16 * SCALE, self.screen_dim // 24)
@@ -567,42 +567,42 @@
             self.debug_window.destroy()
         pygame.quit()
 
     def render(self):
         """Render the environment.
 
         Returns:
-            {np.ndarray} -- The rendered image of the environment.
+            {np.ndarray} -- The rendered image of the environment. Returns None if the render mode is set to "human".
         """
-        if self.render_mode is not None:
-            if self.render_mode == "rgb_array":
-                self.clock.tick(SearingSpotlightsEnv.metadata["render_fps"])
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
-            elif self.render_mode == "debug_rgb_array":
-                # Create debug window if it doesn't exist yet
-                if self.debug_window is None:
-                    self.debug_window = Window(size = (336, 336))
-                    self.debug_window.show()
-                    self.renderer = Renderer(self.debug_window)
-
-                self.debug_window.title = "seed " + str(self.current_seed)
-                self.clock.tick(SearingSpotlightsEnv.metadata["render_fps"])
-
-                debug_surface = self._build_debug_surface()
-                texture = Texture.from_surface(self.renderer, debug_surface)
-                texture.draw(dstrect=(0, 0))
-                self.renderer.present()
-                return np.fliplr(np.rot90(pygame.surfarray.array3d(self.renderer.to_surface()).astype(np.uint8), 3))
+        if self.render_mode == "human":
+            # Create debug window if it doesn't exist yet
+            if self.debug_window is None:
+                self.debug_window = Window(size = (336, 336))
+                self.debug_window.show()
+                self.renderer = Renderer(self.debug_window)
+            
+            self.debug_window.title = "seed " + str(self.current_seed)
+            self.clock.tick(SearingSpotlightsEnv.metadata["render_fps"])
+
+            debug_surface = self._build_debug_surface()
+            texture = Texture.from_surface(self.renderer, debug_surface)
+            texture.draw(dstrect=(0, 0))
+            self.renderer.present()
+        elif self.render_mode == "rgb_array":
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(pygame.display.get_surface()).astype(np.uint8), 3)) # pygame.surfarray.pixels3d(pygame.display.get_surface()).astype(np.uint8)
+        elif self.render_mode == "debug_rgb_array":
+            debug_surface = self._build_debug_surface()
+            return np.fliplr(np.rot90(pygame.surfarray.array3d(debug_surface).astype(np.uint8), 3))
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("--seed", type=int, help="The to be used seed for the environment's random number generator.", default=0)
     options = parser.parse_args()
 
-    env = SearingSpotlightsEnv(render_mode = "debug_rgb_array")
+    env = SearingSpotlightsEnv(render_mode = "human")
     reset_params = {}
     seed = options.seed
     vis_obs, reset_info = env.reset(seed = options.seed, options = reset_params)
     img = env.render()
     done = False
 
     while not done:
```

### Comparing `memory_gym-1.0.1/memory_gym.egg-info/PKG-INFO` & `memory_gym-1.0.2/memory_gym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-gym
-Version: 1.0.1
+Version: 1.0.2
 Summary: A gym that contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing Spotlights
 Home-page: https://github.com/MarcoMeter/drl-memory-gym
 Author: Marco Pleines
 Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
 Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
 Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial Observation
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: memory-gym Version: 1.0.1 Summary: A gym that
+Metadata-Version: 2.1 Name: memory-gym Version: 1.0.2 Summary: A gym that
 contains the memory benchmarks Mortar Mayhem, Mystery Maze and Searing
 Spotlights Home-page: https://github.com/MarcoMeter/drl-memory-gym Author:
 Marco Pleines Project-URL: Github, https://github.com/MarcoMeter/drl-memory-gym
 Project-URL: Bug Tracker, https://github.com/MarcoMeter/drl-memory-gym/issues
 Keywords: Deep Reinforcement Learning,gym,POMDP,Imperfect Information,Partial
 Observation Classifier: Programming Language :: Python :: 3 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
```

### Comparing `memory_gym-1.0.1/memory_gym.egg-info/SOURCES.txt` & `memory_gym-1.0.2/memory_gym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memory_gym-1.0.1/memory_gym.egg-info/entry_points.txt` & `memory_gym-1.0.2/memory_gym.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `memory_gym-1.0.1/setup.py` & `memory_gym-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,9 +45,9 @@
             "mortar_mayhem_grid=memory_gym.mortar_mayhem_grid:main",
             "mortar_mayhem_b_grid=memory_gym.mortar_mayhem_b_grid:main",
             "mystery_path=memory_gym.mystery_path:main",
             "endless_mystery_path=memory_gym.endless_mystery_path:main",
             "mystery_path_grid=memory_gym.mystery_path_grid:main",
             ],
       },
-      version="1.0.1",
+      version="1.0.2",
 )
```

