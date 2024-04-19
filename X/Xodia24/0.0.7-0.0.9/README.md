# Comparing `tmp/Xodia24-0.0.7.tar.gz` & `tmp/Xodia24-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xodia24-0.0.7.tar", last modified: Fri Apr 19 05:54:21 2024, max compression
+gzip compressed data, was "Xodia24-0.0.9.tar", last modified: Fri Apr 19 06:01:03 2024, max compression
```

## Comparing `Xodia24-0.0.7.tar` & `Xodia24-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 05:54:21.529616 Xodia24-0.0.7/
--rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     5854 2024-04-19 05:54:21.521612 Xodia24-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5075 2024-04-01 15:09:02.000000 Xodia24-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 05:54:21.521612 Xodia24-0.0.7/Xodia24.egg-info/
--rw-rw-rw-   0        0        0     5854 2024-04-19 05:54:20.000000 Xodia24-0.0.7/Xodia24.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-04-19 05:54:21.000000 Xodia24-0.0.7/Xodia24.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 05:54:20.000000 Xodia24-0.0.7/Xodia24.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-19 05:54:20.000000 Xodia24-0.0.7/Xodia24.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 05:54:20.000000 Xodia24-0.0.7/Xodia24.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 05:54:21.529616 Xodia24-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-04-19 05:50:18.000000 Xodia24-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:01:03.326712 Xodia24-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2024-04-01 14:18:58.000000 Xodia24-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     8044 2024-04-19 06:01:03.326712 Xodia24-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7225 2024-04-19 05:57:27.000000 Xodia24-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 06:01:03.277905 Xodia24-0.0.9/Xodia24/
+-rw-rw-rw-   0        0        0       21 2024-04-19 06:00:48.000000 Xodia24-0.0.9/Xodia24/__init__.py
+-rw-rw-rw-   0        0        0     3844 2024-04-19 05:35:28.000000 Xodia24-0.0.9/Xodia24/env.py
+-rw-rw-rw-   0        0        0      385 2024-04-01 13:45:24.000000 Xodia24-0.0.9/Xodia24/path.py
+drwxrwxrwx   0        0        0        0 2024-04-19 06:01:03.323140 Xodia24-0.0.9/Xodia24.egg-info/
+-rw-rw-rw-   0        0        0     8044 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-19 06:01:02.000000 Xodia24-0.0.9/Xodia24.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 06:01:03.326712 Xodia24-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2024-04-19 06:00:58.000000 Xodia24-0.0.9/setup.py
```

### Comparing `Xodia24-0.0.7/LICENSE` & `Xodia24-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Xodia24-0.0.7/PKG-INFO` & `Xodia24-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -15,25 +15,23 @@
 License-File: LICENSE
 Requires-Dist: gymnasium
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # Xodia24: PocketTank Environment
 
-<p  align="center">
-<img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0" width="400px">
+<p align="center">
+  <img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0" width="400px">
 </p>
-  
 
 Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid. The objective is to train a Reinforcement Learning (RL) agent to effectively control one of the tanks and shoot at the other tank using different actions such as adjusting power, angle, and moving the tank.
 
 ## Installation
 
 You can install Xodia24 via pip:
-
 ```
 pip install Xodia24
 ```
 
 ## Usage
 
 1. **Implementing the Custom Reward Function:**
@@ -43,63 +41,63 @@
    After implementing the custom reward function, you can train your RL model using this environment by interacting with it through the `step()` method. Provide actions to the tank and observe the resulting state, reward, and other information.
 
 Example:
 ```python
 # Import the environment
 from Xodia24.env import PocketTank
 
-
 # Train RL model using the environment
 # ...
 ```
 
-
-## Dependencies
-
-- `gymnasium`: A toolkit for developing and comparing reinforcement learning algorithms.
-- `numpy`: Library for numerical computations and array operations.
-- `matplotlib`: Library for creating plots and visualizations.
-
-## Implementation Note
-
-If the custom reward function is not implemented, the default behavior will set the reward to 0. It's essential to implement a meaningful reward function tailored to the specific problem requirements for effective training of the RL model.
-
-## Custom PocketTank Environment
-
-To implement a custom reward function and use it in the PocketTank environment, you can utilize the `CustomPocketTank` class. Below is a code template for `CustomPocketTank`:
+3. **Using the Custom PocketTank Environment:**
+   If you want to utilize a custom implementation of the PocketTank environment, you can create your subclass and override the necessary methods. Here's a sample implementation:
 
 ```python
-# custom_reward.py
+# custom_pocket_tank.py
 
-from Xodia24.env import PocketTank
+from Xodia24.pocket_tank import PocketTank
+from gymnasium import spaces
+import numpy as np
 
-# Import the PocketTank class and inherit from it to override the reward function
 class CustomPocketTank(PocketTank):
     def __init__(self):
         super().__init__()
-
-    # Override the reward function with your custom implementation
-    def reward(self, action, diff_distance):
+        """
+        Define a custom action space but only limit it
+        dont change actual crux or step function wont work
+         """
+        # Example 1
+		self.action_space  =  spaces.MultiDiscrete([100,90,1]) # This limit movement only hit from the current position
+		# Example 2
+		self.action_space  =  spaces.MultiDiscrete([100,45,3]) # Limit the angle
+		# Example 3
+		self.action_space  =  spaces.MultiDiscrete([60,90,3])# Limit the power of firing
+    def reward(self, diff_distance):
         """
         Custom reward function implementation.
 
         Args:
-            action (np.ndarray): Array representing the action taken by the agent.
             diff_distance (float): Difference in distance between the bullet and the target tank.
 
         Returns:
             float: Custom reward value based on the difference in distance.
         """
         # Implement your custom reward logic here
-        custom_reward = 0  # Modify this according to your requirements
+        custom_reward = 1.0 / (1.0 + diff_distance)  # Example: Inverse distance as reward
         return custom_reward
-
-# Train RL Model
 ```
 
+## Dependencies
+
+- `gymnasium`: A toolkit for developing and comparing reinforcement learning algorithms.
+- `numpy`: Library for numerical computations and array operations.
+- `matplotlib`: Library for creating plots and visualizations.
+
+
 ### Action Space
 
 The action space in the Xodia24 PocketTank environment refers to the set of possible actions that the reinforcement learning (RL) agent can take at each time step. In the tank battle scenario, the agent controls one of the tanks and has several actions available to it, including adjusting the power and angle of the tank's cannon and moving the tank across the 2D grid.
 
 #### Available Actions:
 - **Adjust Power**: The agent can adjust the power setting of the tank's cannon, determining the force with which the projectile is fired.
 - **Adjust Angle**: The agent can adjust the angle of the tank's cannon, controlling the direction in which the projectile is launched.
@@ -115,7 +113,49 @@
 - **Tank Positions**: The coordinates of both the agent-controlled tank and the opponent tank on the 2D grid.
 - **Terrain Information**: Information about the terrain features, such as obstacles or cover, that may affect the trajectory of the projectile.
 - **Projectile Position**: The current position of the projectile fired by the tanks.
 
 The observation space can be represented as a vector, matrix, or other data structure depending on the complexity of the environment and the information that needs to be conveyed to the agent.
 
 
+Here's the documentation for the reinforcement learning environment for the Pocket Tanks game, with updated information for the fourth bullet:
+
+
+## Bullet Types
+
+The tank has seven different types of bullets available, each with unique properties and effects. The tank has access to each bullet type an unlimited number of times.
+
+1. *Standard Shell*:
+    - *Description*: A classic projectile bullet that follows projectile motion.
+    - *Damage*: Deals 20 damage upon hitting the target.
+    - *Trajectory*: Parabolic trajectory determined by initial angle and velocity.
+
+2. *Triple Threat*:
+    - *Description*: A bullet that splits into three smaller bullets upon firing.
+    - *Damage*: Each of the three bullets deals 20 damage, similar to the Standard Shell.
+    - *Trajectory*: Parabolic trajectory similar to Standard Shell.
+
+3. *Long Shot*:
+    - *Description*: A bullet that deals more damage based on the distance it travels before hitting the ground.
+    - *Damage*: Damage increases as the distance traveled increases.
+    - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+
+4. *Heavy Impact*:
+    - *Description*: A high-damage bullet with limited range and velocity.
+    - *Damage*: Deals 40 damage upon hitting the target.
+    - *Trajectory*: Limited velocity and range compared to other bullets.
+
+5. *Blast Radius*:
+    - *Description*: A bullet that causes area damage within a radius of 100.
+    - *Damage*: Deals 10 damage in a radius of 100 around the impact point.
+    - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+
+6. *Healing Halo*:
+    - *Description*: A bullet that heals the tank upon impact.
+    - *Healing*: Heals the tank by 10 points upon hitting the ground or a target.
+    - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+
+7. *Boomerang Blast*:
+    - *Description*: A bullet that follows a unique trajectory resembling a boomerang.
+    - *Damage*: Deals 20 damage upon hitting the target.
+    - *Trajectory*: Follows a curved trajectory that slightly reverses direction, like a boomerang.
+
```

### Comparing `Xodia24-0.0.7/Xodia24.egg-info/PKG-INFO` & `Xodia24-0.0.9/Xodia24.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xodia24
-Version: 0.0.7
+Version: 0.0.9
 Summary: Python package providing a custom environment for simulating tank battles
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,reinforcement-learning,tank-battle
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -15,25 +15,23 @@
 License-File: LICENSE
 Requires-Dist: gymnasium
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 # Xodia24: PocketTank Environment
 
-<p  align="center">
-<img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0" width="400px">
+<p align="center">
+  <img src="https://i.ibb.co/P4nyZNv/Xodia-Logo-removebg-preview.png" alt="Xodia-Logo-removebg-preview" border="0" width="400px">
 </p>
-  
 
 Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid. The objective is to train a Reinforcement Learning (RL) agent to effectively control one of the tanks and shoot at the other tank using different actions such as adjusting power, angle, and moving the tank.
 
 ## Installation
 
 You can install Xodia24 via pip:
-
 ```
 pip install Xodia24
 ```
 
 ## Usage
 
 1. **Implementing the Custom Reward Function:**
@@ -43,63 +41,63 @@
    After implementing the custom reward function, you can train your RL model using this environment by interacting with it through the `step()` method. Provide actions to the tank and observe the resulting state, reward, and other information.
 
 Example:
 ```python
 # Import the environment
 from Xodia24.env import PocketTank
 
-
 # Train RL model using the environment
 # ...
 ```
 
-
-## Dependencies
-
-- `gymnasium`: A toolkit for developing and comparing reinforcement learning algorithms.
-- `numpy`: Library for numerical computations and array operations.
-- `matplotlib`: Library for creating plots and visualizations.
-
-## Implementation Note
-
-If the custom reward function is not implemented, the default behavior will set the reward to 0. It's essential to implement a meaningful reward function tailored to the specific problem requirements for effective training of the RL model.
-
-## Custom PocketTank Environment
-
-To implement a custom reward function and use it in the PocketTank environment, you can utilize the `CustomPocketTank` class. Below is a code template for `CustomPocketTank`:
+3. **Using the Custom PocketTank Environment:**
+   If you want to utilize a custom implementation of the PocketTank environment, you can create your subclass and override the necessary methods. Here's a sample implementation:
 
 ```python
-# custom_reward.py
+# custom_pocket_tank.py
 
-from Xodia24.env import PocketTank
+from Xodia24.pocket_tank import PocketTank
+from gymnasium import spaces
+import numpy as np
 
-# Import the PocketTank class and inherit from it to override the reward function
 class CustomPocketTank(PocketTank):
     def __init__(self):
         super().__init__()
-
-    # Override the reward function with your custom implementation
-    def reward(self, action, diff_distance):
+        """
+        Define a custom action space but only limit it
+        dont change actual crux or step function wont work
+         """
+        # Example 1
+		self.action_space  =  spaces.MultiDiscrete([100,90,1]) # This limit movement only hit from the current position
+		# Example 2
+		self.action_space  =  spaces.MultiDiscrete([100,45,3]) # Limit the angle
+		# Example 3
+		self.action_space  =  spaces.MultiDiscrete([60,90,3])# Limit the power of firing
+    def reward(self, diff_distance):
         """
         Custom reward function implementation.
 
         Args:
-            action (np.ndarray): Array representing the action taken by the agent.
             diff_distance (float): Difference in distance between the bullet and the target tank.
 
         Returns:
             float: Custom reward value based on the difference in distance.
         """
         # Implement your custom reward logic here
-        custom_reward = 0  # Modify this according to your requirements
+        custom_reward = 1.0 / (1.0 + diff_distance)  # Example: Inverse distance as reward
         return custom_reward
-
-# Train RL Model
 ```
 
+## Dependencies
+
+- `gymnasium`: A toolkit for developing and comparing reinforcement learning algorithms.
+- `numpy`: Library for numerical computations and array operations.
+- `matplotlib`: Library for creating plots and visualizations.
+
+
 ### Action Space
 
 The action space in the Xodia24 PocketTank environment refers to the set of possible actions that the reinforcement learning (RL) agent can take at each time step. In the tank battle scenario, the agent controls one of the tanks and has several actions available to it, including adjusting the power and angle of the tank's cannon and moving the tank across the 2D grid.
 
 #### Available Actions:
 - **Adjust Power**: The agent can adjust the power setting of the tank's cannon, determining the force with which the projectile is fired.
 - **Adjust Angle**: The agent can adjust the angle of the tank's cannon, controlling the direction in which the projectile is launched.
@@ -115,7 +113,49 @@
 - **Tank Positions**: The coordinates of both the agent-controlled tank and the opponent tank on the 2D grid.
 - **Terrain Information**: Information about the terrain features, such as obstacles or cover, that may affect the trajectory of the projectile.
 - **Projectile Position**: The current position of the projectile fired by the tanks.
 
 The observation space can be represented as a vector, matrix, or other data structure depending on the complexity of the environment and the information that needs to be conveyed to the agent.
 
 
+Here's the documentation for the reinforcement learning environment for the Pocket Tanks game, with updated information for the fourth bullet:
+
+
+## Bullet Types
+
+The tank has seven different types of bullets available, each with unique properties and effects. The tank has access to each bullet type an unlimited number of times.
+
+1. *Standard Shell*:
+    - *Description*: A classic projectile bullet that follows projectile motion.
+    - *Damage*: Deals 20 damage upon hitting the target.
+    - *Trajectory*: Parabolic trajectory determined by initial angle and velocity.
+
+2. *Triple Threat*:
+    - *Description*: A bullet that splits into three smaller bullets upon firing.
+    - *Damage*: Each of the three bullets deals 20 damage, similar to the Standard Shell.
+    - *Trajectory*: Parabolic trajectory similar to Standard Shell.
+
+3. *Long Shot*:
+    - *Description*: A bullet that deals more damage based on the distance it travels before hitting the ground.
+    - *Damage*: Damage increases as the distance traveled increases.
+    - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+
+4. *Heavy Impact*:
+    - *Description*: A high-damage bullet with limited range and velocity.
+    - *Damage*: Deals 40 damage upon hitting the target.
+    - *Trajectory*: Limited velocity and range compared to other bullets.
+
+5. *Blast Radius*:
+    - *Description*: A bullet that causes area damage within a radius of 100.
+    - *Damage*: Deals 10 damage in a radius of 100 around the impact point.
+    - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+
+6. *Healing Halo*:
+    - *Description*: A bullet that heals the tank upon impact.
+    - *Healing*: Heals the tank by 10 points upon hitting the ground or a target.
+    - *Trajectory*: Parabolic trajectory similar to the Standard Shell.
+
+7. *Boomerang Blast*:
+    - *Description*: A bullet that follows a unique trajectory resembling a boomerang.
+    - *Damage*: Deals 20 damage upon hitting the target.
+    - *Trajectory*: Follows a curved trajectory that slightly reverses direction, like a boomerang.
+
```

### Comparing `Xodia24-0.0.7/setup.py` & `Xodia24-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
-VERSION = '0.0.7' 
+VERSION = '0.0.9' 
 DESCRIPTION = 'Python package providing a custom environment for simulating tank battles'
 LONG_DESCRIPTION = 'Xodia24 is a Python package providing a custom environment for simulating a tank battle scenario where two tanks are positioned on a 2D grid.'
 
 # Setting up
 setup(
     name="Xodia24",
     version=VERSION,
```

