# Comparing `tmp/bopt_slf-1.0.1.tar.gz` & `tmp/bopt_slf-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bopt_slf-1.0.1.tar", last modified: Thu Apr  4 02:07:56 2024, max compression
+gzip compressed data, was "bopt_slf-1.0.2.tar", last modified: Fri Apr 19 03:43:03 2024, max compression
```

## Comparing `bopt_slf-1.0.1.tar` & `bopt_slf-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-04 02:07:56.489016 bopt_slf-1.0.1/
--rw-r--r--   0 javiermorlet   (501) staff       (20)     1079 2024-03-23 20:53:34.000000 bopt_slf-1.0.1/LICENSE.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)      515 2024-04-04 02:07:56.488743 bopt_slf-1.0.1/PKG-INFO
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-04 02:07:56.482474 bopt_slf-1.0.1/bopt_slf/
--rw-r--r--   0 javiermorlet   (501) staff       (20)       56 2024-04-03 11:02:39.000000 bopt_slf-1.0.1/bopt_slf/__init__.py
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-04 02:07:56.483950 bopt_slf-1.0.1/bopt_slf/core/
--rw-r--r--   0 javiermorlet   (501) staff       (20)       20 2024-03-23 19:00:17.000000 bopt_slf-1.0.1/bopt_slf/core/__init__.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)    11706 2024-03-21 18:15:49.000000 bopt_slf-1.0.1/bopt_slf/core/main.py
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-04 02:07:56.488099 bopt_slf-1.0.1/bopt_slf/utils/
--rw-r--r--   0 javiermorlet   (501) staff       (20)     2821 2024-03-23 19:06:38.000000 bopt_slf-1.0.1/bopt_slf/utils/Acq_fun.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     4198 2024-03-23 19:07:44.000000 bopt_slf-1.0.1/bopt_slf/utils/Aux.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     7340 2024-03-21 16:30:15.000000 bopt_slf-1.0.1/bopt_slf/utils/Dimension_reduction.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)    11346 2024-03-23 19:11:56.000000 bopt_slf-1.0.1/bopt_slf/utils/Initialize.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     3872 2024-03-23 19:12:48.000000 bopt_slf-1.0.1/bopt_slf/utils/Models.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     4926 2024-03-06 00:57:21.000000 bopt_slf-1.0.1/bopt_slf/utils/Plotting.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     4416 2024-03-05 17:22:52.000000 bopt_slf-1.0.1/bopt_slf/utils/Querry_points.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     5746 2024-03-29 15:39:32.000000 bopt_slf-1.0.1/bopt_slf/utils/Set_level_filtration.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)     1187 2024-03-17 16:50:23.000000 bopt_slf-1.0.1/bopt_slf/utils/Update.py
--rw-r--r--   0 javiermorlet   (501) staff       (20)      609 2024-03-23 19:13:55.000000 bopt_slf-1.0.1/bopt_slf/utils/__init__.py
-drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-04 02:07:56.483248 bopt_slf-1.0.1/bopt_slf.egg-info/
--rw-r--r--   0 javiermorlet   (501) staff       (20)      515 2024-04-04 02:07:56.000000 bopt_slf-1.0.1/bopt_slf.egg-info/PKG-INFO
--rw-r--r--   0 javiermorlet   (501) staff       (20)      538 2024-04-04 02:07:56.000000 bopt_slf-1.0.1/bopt_slf.egg-info/SOURCES.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)        1 2024-04-04 02:07:56.000000 bopt_slf-1.0.1/bopt_slf.egg-info/dependency_links.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)      140 2024-04-04 02:07:56.000000 bopt_slf-1.0.1/bopt_slf.egg-info/requires.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)        9 2024-04-04 02:07:56.000000 bopt_slf-1.0.1/bopt_slf.egg-info/top_level.txt
--rw-r--r--   0 javiermorlet   (501) staff       (20)       38 2024-04-04 02:07:56.489064 bopt_slf-1.0.1/setup.cfg
--rw-r--r--   0 javiermorlet   (501) staff       (20)      615 2024-04-04 02:01:51.000000 bopt_slf-1.0.1/setup.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.503899 bopt_slf-1.0.2/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     1079 2024-03-23 20:53:34.000000 bopt_slf-1.0.2/LICENSE.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      524 2024-04-19 03:43:03.503663 bopt_slf-1.0.2/PKG-INFO
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.498293 bopt_slf-1.0.2/bopt_slf/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)       58 2024-04-19 03:36:26.000000 bopt_slf-1.0.2/bopt_slf/__init__.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.499722 bopt_slf-1.0.2/bopt_slf/core/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)       20 2024-03-23 19:00:17.000000 bopt_slf-1.0.2/bopt_slf/core/__init__.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)    12626 2024-04-16 08:07:37.000000 bopt_slf-1.0.2/bopt_slf/core/main.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.503206 bopt_slf-1.0.2/bopt_slf/utils/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     2256 2024-04-05 04:58:08.000000 bopt_slf-1.0.2/bopt_slf/utils/Acq_fun.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     4235 2024-04-16 03:10:41.000000 bopt_slf-1.0.2/bopt_slf/utils/Aux.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     7155 2024-04-16 07:45:00.000000 bopt_slf-1.0.2/bopt_slf/utils/Dimension_reduction.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)    12137 2024-04-11 07:20:37.000000 bopt_slf-1.0.2/bopt_slf/utils/Initialize.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     3814 2024-04-11 09:08:18.000000 bopt_slf-1.0.2/bopt_slf/utils/Models.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     4748 2024-04-16 03:36:53.000000 bopt_slf-1.0.2/bopt_slf/utils/Plotting.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     3890 2024-04-05 05:04:38.000000 bopt_slf-1.0.2/bopt_slf/utils/Querry_points.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     5908 2024-04-12 09:39:36.000000 bopt_slf-1.0.2/bopt_slf/utils/Set_level_filtration.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)     1187 2024-03-17 16:50:23.000000 bopt_slf-1.0.2/bopt_slf/utils/Update.py
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      614 2024-04-05 04:49:31.000000 bopt_slf-1.0.2/bopt_slf/utils/__init__.py
+drwxr-xr-x   0 javiermorlet   (501) staff       (20)        0 2024-04-19 03:43:03.499054 bopt_slf-1.0.2/bopt_slf.egg-info/
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      524 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/PKG-INFO
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      538 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/SOURCES.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)        1 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/dependency_links.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      140 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/requires.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)        9 2024-04-19 03:43:03.000000 bopt_slf-1.0.2/bopt_slf.egg-info/top_level.txt
+-rw-r--r--   0 javiermorlet   (501) staff       (20)       38 2024-04-19 03:43:03.503952 bopt_slf-1.0.2/setup.cfg
+-rw-r--r--   0 javiermorlet   (501) staff       (20)      595 2024-04-05 04:56:21.000000 bopt_slf-1.0.2/setup.py
```

### Comparing `bopt_slf-1.0.1/LICENSE.txt` & `bopt_slf-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bopt_slf-1.0.1/PKG-INFO` & `bopt_slf-1.0.2/bopt_slf.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: bopt_slf
-Version: 1.0.1
+Name: bopt-slf
+Version: 1.0.2
 Summary: Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems
-Author: Javier Morlet
+Author: Javier Morlet-Espinosa
 Author-email: a00833961@tec.mx
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: GPy>=1.10.0
 Requires-Dist: scipy>=1.10.1
```

### Comparing `bopt_slf-1.0.1/bopt_slf/core/main.py` & `bopt_slf-1.0.2/bopt_slf/core/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 import numpy as np
 import sympy as sp
-import matplotlib.pyplot as plt
-import matplotlib as mpl
 import multiprocess as mp
 import GPy
-import sys
 import warnings
 from ..utils.Initialize import Space, Problem_type, Get_constraints, Times_fun, Points_initial_design, x_Generator, Bounds, Points_mesh, AF_params
 from ..utils.Dimension_reduction import Reduce, Inverse, Train_reducer, Train_inverter, Find_reducer, Find_inverter, Red_bounds
-from ..utils.Models import Select_model, Train_model, Train_models_const, Kernel_ABCD
+from ..utils.Models import Select_model, Train_model, Train_models_const, Kernel_discovery
 from ..utils.Acq_fun import AF
 from ..utils.Set_level_filtration import Slf
 from ..utils.Querry_points import Querry
 from ..utils.Update import Up_mesh
 from ..utils.Aux import Errors, Data_eval, Eval_fun, Eval_const, Regret, Print_results, Create_results
 
 class BO():
 
     def __init__(self, function, domain, sense,
-                 constraints = None,
-                 x_0 = None, 
-                 z_0 = None,
                  surrogate = "GP",
                  acquisition_function = "UCB",
+                 xi = 2,
+                 xi_decay = "yes",
                  kernel = None,
-                 parallelization = "yes",
-                 kern_ABCD = "yes",
+                 kern_discovery = "yes",
+                 kern_discovery_evals = 2,
+                 x_0 = None, 
+                 z_0 = None,
                  design = "LHS",
                  p_design = None,
+                 parallelization = "no",
                  max_iter = 100, 
                  n_restarts = 5,
-                 kern_ABCD_evals = 2,
-                 xi = 2,
-                 xi_decay = "yes",
+                 constraints = None,
                  constraints_method = "PoF",
                  reducer = None,
                  n_components = None,
-                 inverter = None,
+                 inverter_transform = "No",
                  verbose = 0,
                  ):
 
         self.function = function
         self.domain = domain
         self.constraints = constraints
         self.x_0 = x_0
         self.z_0 = z_0
         self.sense = sense
         self.surrogate = surrogate
         self.acquisition_function = acquisition_function
         self.kernel = kernel
         self.parallelization = parallelization
-        self.kern_ABCD = kern_ABCD
+        self.kern_discovery = kern_discovery
         self.design = design
         self.p_design = p_design
         self.max_iter = max_iter
         self.n_restarts = n_restarts
-        self.kern_ABCD_evals = kern_ABCD_evals
+        self.kern_discovery_evals = kern_discovery_evals
         self.xi = xi
         self.xi_decay = xi_decay
         self.constraints_method = constraints_method
         self.reducer = reducer
         self.n_components = n_components
-        self.inverter = inverter
+        self.inverter_transform = inverter_transform
         self.verbose = verbose
 
     def optimize(self):
 
         # *************** Main program ********************
         # Ignore warnings
         warnings.filterwarnings("ignore")
@@ -84,65 +81,81 @@
             # Evaluate an arbitrary point to determine the computation time of the function
             x_trial = x_Generator(x_l, x_u, y_v, n_x, n_y, dims, 1, problem_type, "random")
             x_eval = Data_eval(x_trial, n_c, dims, enc_cat)
             times, z_trial = Times_fun(self.function, x_eval)
             if self.p_design == None:
                 self.p_design = Points_initial_design(times, dims, self.design)
             self.x_0 = x_Generator(x_l, x_u, y_v, n_x, n_y, dims, self.p_design, problem_type, self.design)
-        if self.z_0 is None:
             x_eval = Data_eval(self.x_0, n_c, dims, enc_cat)
             self.z_0 = self.function(x_eval).reshape(-1,1)
+            x, z = np.vstack((self.x_0, x_trial)), np.vstack((self.z_0, z_trial))
         else:
-            self.p_design = len(self.z_0)
-        x, z = np.vstack((self.x_0, x_trial)), np.vstack((self.z_0, z_trial))
+            x = self.x_0
+            if self.z_0 is None:
+                x_eval = Data_eval(self.x_0, n_c, dims, enc_cat)
+                z = self.function(x_eval).reshape(-1,1)
+            else:
+                self.p_design = len(self.z_0)
+                z = self.z_0
         # Generate mesh, or grid
         p_mesh = Points_mesh(dims)
         if p_mesh > 3: 
             mesh = x_Generator(x_l, x_u, y_v, n_x, n_y, dims, p_mesh, problem_type, "Mesh")
         else:
             mesh = x_Generator(x_l, x_u, y_v, n_x, n_y, dims, 1024, problem_type, "Sobol")
-        # Perform dimensionality reduction
+        # Find reducer and perform dimensionality reduction
         if self.reducer is None:
-            self.reducer, reducer_trained, dims_red = Find_reducer(x, n_x, dims, self.n_components, problem_type)
+            if (problem_type == "Continuous") and (n_x < 5):
+                self.reducer = "No"
+                reducer_trained = None
+                dims_red = dims
+                x_red = x
+            else:
+                self.reducer, reducer_trained, dims_red = Find_reducer(x, n_x, dims, self.n_components, problem_type)
+                x_red = Reduce(x, n_x, dims, problem_type, reducer_trained)
         elif self.reducer == "No":
-            self.reducer = None
-        else:
-            x_red, reducer_trained = Train_reducer(x, n_x, dims, problem_type, dims_red, self.reducer)
-        if self.reducer is None:
-            self.inverter = None
+            reducer_trained = None
+            dims_red = dims
             x_red = x
         else:
-            x_red = Reduce(x, n_x, dims, problem_type, reducer_trained)
-            if self.inverter is None:
-                pca_inverse = "no"
-                self.inverter = Find_inverter(x, x_red, n_x, n_y, dims, problem_type)
-                self.inverter = Train_inverter(x, x_red, dims, self.inverter)
-            elif (self.inverter == "No") and (self.reducer.__module__ == 'prince.pca'):
-                pca_inverse = "yes"
-                self.inverter = None
-            else:
-                pass
+            dims_red = self.n_components
+            x_red, reducer_trained = Train_reducer(x, n_x, dims, problem_type, dims_red, self.reducer)
+        # Reduce bounds
         x_l_red, x_u_red = Red_bounds(mesh, x_l, x_u, n_x, dims, dims_red, problem_type, reducer_trained)
+        # Find inverter
+        if self.inverter_transform == "Yes":
+            if self.reducer.__module__ == 'prince.mca' or self.reducer.__module__ == 'prince.famd':
+                raise ValueError("Reducer module has no inverse_transform")
+            else:
+                inverter = reducer_trained
+        elif self.inverter_transform == "No":
+            if self.reducer == "No":
+                inverter = None
+            else:
+                inverter = Find_inverter(x, x_red, n_x, n_y, dims, problem_type)
+                inverter = Train_inverter(x, x_red, dims, inverter)
+        else:
+            pass
         # Generate mesh in the reduced space
-        p_mesh_red = Points_mesh(dims)
+        p_mesh_red = Points_mesh(dims_red)
         mesh_red = x_Generator(x_l_red, x_u_red, 0, 0, 0, dims_red, p_mesh_red, "Continuous", "Mesh")
         p_mesh_0 = p_mesh_red
         p_mesh_red, mesh_red = [p_mesh_red], [mesh_red]
         # Tuple of the bounds
         bounds = Bounds(x_l_red, x_u_red, dims_red)
         # Spawning processes
         if self.parallelization == "yes":
             jobs = mp.cpu_count()
         else:
             jobs = 1
         # Select covariance
-        if self.kern_ABCD == "yes":
-            model = Kernel_ABCD(x_red, z, dims_red, self.surrogate, self.kern_ABCD_evals)
+        if self.kern_discovery == "yes":
+            model = Kernel_discovery(x_red, z, dims_red, self.surrogate, self.kern_discovery_evals)
             kernel = model.kern
-        elif self.kern_ABCD == "no" and self.kernel is None:
+        elif self.kern_discovery == "no" and self.kernel is None:
             kernel = GPy.kern.RBF(input_dim=dims_red, variance=1.0, lengthscale=1.0)
         else:
             kernel = self.kernel
         # Eval and train constraints
         if self.constraints is None:
             models_const = None
         else:
@@ -192,54 +205,59 @@
             model = Train_model(model, self.n_restarts)
             if self.constraints is None:
                 models_const = None
             else:
                 x_eval = Data_eval(x, n_c, dims, enc_cat)
                 g_hat = Eval_const(x_eval, const, n_const, self.constraints_method)
                 models_const = Train_models_const(x_red, g_hat, n_const, self.constraints_method)
-            #
+            # Find conected elements
             connected_elements, n_elements = Slf(mesh_red, p_mesh_red, dims_red, q, jobs, af_params, self.constraints_method, self.sense, model, models_const, AF)
-            #
+            # Querry point
             x_red_new = Querry(x_symb, connected_elements, n_elements, bounds, dims_red, af_params, self.constraints_method, self.sense, model, models_const, AF)
             #
-            if self.inverter is None:
+            if self.reducer == "No":
                 x_new = x_red_new
             else:
-                x_new = Inverse(x_red_new, pca_inverse, self.inverter)
+                x_new = Inverse(x_red_new, self.inverter_transform, inverter)
             #
             x_eval = Data_eval(x_new, n_c, dims, enc_cat)
             z_new = Eval_fun(x_eval, n_elements, self.parallelization, jobs, self.function)
             #
             if jobs == 1:
                 z_new_best = z_new
             else:
                 if self.sense == "maximize":
                     z_new_best = np.max(z_new)
                 elif self.sense == "minimize":
                     z_new_best = np.min(z_new)
                 else:
                     pass
-            #
+            # Update train data
             x, z = np.vstack((x, x_new)), np.vstack((z, z_new))
-            if self.reducer is None:
+            if self.reducer == "No":
                 x_red = np.vstack((x_red, x_red_new))
             else:
                 x_red, reducer_trained = Train_reducer(x, n_x, dims, problem_type, dims_red, self.reducer)
-                self.inverter = Train_inverter(x, x_red, dims, self.inverter)
+                if self.inverter_transform == "No":
+                    inverter = Train_inverter(x, x_red, dims, inverter)
+                elif self.inverter_transform == "Yes":
+                    inverter = reducer_trained
+                else:
+                    pass
             # 
             if self.sense == "maximize":
                 if z_new_best > z_best:
                     flag = 1
             elif self.sense == "minimize":
                 if z_new_best < z_best:
                     flag = 1
             # Update parameters
             if flag == 1:
-                if self.reducer is not None:
-                    connected_elements_inv = [Inverse(connected_elements[i], pca_inverse, self.inverter) for i in range(n_elements)]
+                if self.reducer != "No":
+                    connected_elements_inv = [Inverse(connected_elements[i], self.inverter_transform, inverter) for i in range(n_elements)]
                     connected_elements = [Reduce(connected_elements_inv[i], n_x, dims, problem_type, reducer_trained) for i in range(n_elements)]
                 mesh_red, p_mesh_red = Up_mesh(connected_elements, n_elements, p_mesh_0, dims_red)
                 af_params["xi"] *= af_params["xi_decay"]
                 q_inc += delta_q
                 q = int(round(q_inc/5.0)*5.0)
             rt.append(Regret(z_new, np.array(x_red_new), n_elements, model))
             # Print results
```

### Comparing `bopt_slf-1.0.1/bopt_slf/utils/Aux.py` & `bopt_slf-1.0.2/bopt_slf/utils/Aux.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,16 @@
 
     res = {'x_best': x_best, 'f_best': z_best, 
            'x_init': x[0:points], 'f_init': z[0:points], 
            'x_iters': x[points:-1], 'f_iters': z[points:-1],
            'x_l': x_l, 'x_u': x_u, 
            'dims': dims,
            'iters': max_iter, 
-           'inital_design': design, 
+           'initial_design': design,
+           'initial_points': points,
            'xi': af_params['xi'], 
            'acquisition_function': af_params['AF_name'],
            'regret': rt,
            'constraint_method': constraints_method,
            'models_constraints': models_const,
            'model': model}
```

### Comparing `bopt_slf-1.0.1/bopt_slf/utils/Dimension_reduction.py` & `bopt_slf-1.0.2/bopt_slf/utils/Dimension_reduction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import numpy as np
 from prince import PCA, MCA, FAMD
 from sklearn.ensemble import ExtraTreesRegressor, ExtraTreesClassifier
 from sklearn.model_selection import RandomizedSearchCV, train_test_split
-from sklearn.metrics import mean_squared_error, r2_score
+from sklearn.metrics import r2_score
 
 # *******************************************************
 
 def Trans_data_to_pandas(data, n_x, dims, problem_type):
 
     if problem_type == "Mixed":
         cols = np.arange(1,dims+1)
@@ -25,28 +25,28 @@
     
     data_pd = Trans_data_to_pandas(data, n_x, dims, problem_type)
     
     return np.array(reducer.transform(data_pd))
 
 # *******************************************************
 
-def Inverse(data, pca_inverse, inverter):
+def Inverse(data, inverter_transform, inverter):
 
     def Back_projection(data, model):
 
         predictions = {}
         for col, mod in model.items():
             predictions[col] = mod.predict(data)
         
         return predictions
     
     data = pd.DataFrame(data)
-    if pca_inverse == "yes":
+    if inverter_transform == "Yes":
         data_reconstructed = inverter.inverse_transform(data)
-    elif pca_inverse == "no":
+    elif inverter_transform == "No":
         predictions = Back_projection(data, inverter)
         data_reconstructed = np.vstack(([predictions[i] for i in range(len(inverter))])).T
 
     return data_reconstructed
 
 # *******************************************************
 
@@ -119,32 +119,28 @@
             variance = Red(reducer, data, n)
             if variance >= var_max:
                 break
 
         return n
 
     # Main program
-    if (problem_type == "Continuous") and (n_x < 4):
-        reducer = None
-        reducer_train = None
-        dims_red = dims
+    
+    if problem_type == "Continuous":
+        reducer = PCA()
+        reducer_search = PCA()
+        reducer_train = PCA()
     else:
-        if problem_type == "Continuous":
-            reducer = PCA()
-            reducer_search = PCA()
-            reducer_train = PCA()
+        if problem_type == "Mixed":
+            reducer = FAMD()
+            reducer_train = FAMD()
+        elif problem_type == "Discrete":
+            reducer = MCA()
+            reducer_train = MCA()
         else:
-            if problem_type == "Mixed":
-                reducer = FAMD()
-                reducer_train = FAMD()
-            elif problem_type == "Discrete":
-                reducer = MCA()
-                reducer_train = MCA()
-            else:
-                pass
+            pass
 
     if n_components is None:
         if reducer is None:
             pass
         else:
             data_pd = Trans_data_to_pandas(data, n_x, dims, problem_type)
             if problem_type == "Continuous":
```

### Comparing `bopt_slf-1.0.1/bopt_slf/utils/Initialize.py` & `bopt_slf-1.0.2/bopt_slf/utils/Initialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # Import libraries
 
 import numpy as np
 from scipy.stats import qmc
 from sklearn.preprocessing import OrdinalEncoder
 import time
 
+# *******************************************************
+
 def Space(domain):
 
     """ 
     Gets an array for the lower and upper bounds of the continuous variables, and a tuple for the discrete variables.
     """
 
     dims = len(domain)
@@ -107,127 +109,99 @@
 
 def Times_fun(fun, x):
 
     """ 
     Generates the number of points of the mesh or grid, depending on the cost of the evaluation of the function, and the dimensions of the problem
     """
     
-    #x = np.zeros(dims)
     start = time.time()
     f_eval = fun(x.reshape(1,-1))
     end = time.time()
     
     return (end - start), f_eval
 
 # *******************************************************
 
-def Points_initial_design(times, dims, design):
+def Points_initial_design(times, dims, design, c_param = 50):
 
     if times <= 1:
         exp_param = 0.25
     else: 
         exp_param = 0.95
     
-    c_param = 50
     points_D = int(c_param - c_param/(1+(1/times)**exp_param))
 
     if design == "Mesh":
         points_D = int(np.ceil(points_D)**(1/dims))
     elif design == "Sobol":
-        points = int(np.ceil(np.sqrt(points))**2)
+        points_D = int(np.ceil(np.sqrt(points_D))**2)
     else:
         pass
 
     if points_D < 3:
         points_D = int(3)
 
     return points_D
 
 # *******************************************************
 
 def x_Generator(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type, design_type):
 
     def Random_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type):
 
+        def Bounds_y(y_v, n_y):
+
+            y_l = []
+            y_u = []
+            flag = int(all([(np.diff(y_v[i]) == 1).all() for i in range(n_y)]))
+            
+            for i in range(n_y):
+                if flag == 1:
+                    y_l.append(y_v[i][0])
+                    y_u.append(y_v[i][-1]+1)
+                elif flag == 0:
+                    y_l.append(0)
+                    y_u.append(1)
+                else:
+                    pass
+            return y_l, y_u, flag
+
         def X_rand(x_l, x_u, dims, points):
 
             return np.random.uniform(x_l, x_u, size=(points, dims))
         
         def Y_rand(y_v, n_y, points):
 
-            size_y = [len(y_v[i]) for i in range(n_y)]
-            l = [np.repeat(1/size_y[i], size_y[i]) for i in range(n_y)]
-            sample = [np.random.choice(y_v[i], p=l[i], size=(points, 1)).reshape(-1) for i in range(n_y)]
+            y_l, y_u, flag = Bounds_y(y_v, n_y)
+
+            if flag == 1:
+                y_rand = np.random.randint(y_l, y_u, size=(points, dims))
+            elif flag == 0:
+                size_y = [len(y_v[i]) for i in range(n_y)]
+                l = [np.repeat(1/size_y[i], size_y[i]) for i in range(n_y)]
+                sample = [np.random.choice(y_v[i], p=l[i], size=(points, 1)).reshape(-1) for i in range(n_y)]
+                y_rand = np.array(sample).T
+            else:
+                pass
             
-            return np.array(sample).T
+            return y_rand
 
         if problem_type == "Continuous":
             variables = X_rand(x_l, x_u, dims, points)
         elif problem_type == "Mixed":
             x_variables = X_rand(x_l, x_u, n_x, points)
             y_variables = Y_rand(y_v, n_y, points)
             variables = np.hstack((x_variables, y_variables))
         elif problem_type == "Discrete":
             variables = Y_rand(y_v, dims, points)[0]
         else:
             pass
 
         return variables
     
-    def Mesh_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type):
-
-        def X_mesh(lower_bound, upper_bound, dims, points):
-
-            lists = [np.linspace(lower_bound[i], upper_bound[i], points) for i in range(dims)]
-            mesh = np.meshgrid(*lists)
-            
-            return np.array(mesh).T.reshape(-1, dims)
-        
-        def Bounds_y(n_y):
-
-            y_l = np.zeros(n_y)
-            y_u = np.ones(n_y)
-            
-            return y_l, y_u
-
-        def Assign_y(y_v, n_y, y_norm, points):
-
-                size_y = [len(y_v[i]) for i in range(n_y)]
-                l = [[i/size_y[j] for i in range(size_y[j]+1)] for j in range(n_y)]
-                for i in range(len(l)):
-                    l[i][-1] = l[i][-1] + 0.0001
-                y_new = np.empty([points, n_y])
-
-                for i in range(n_y):
-                    for j in range(len(y_norm[:,i])):
-                        for k in range(len(l[i])-1):
-                            if l[i][k] <= y_norm[j,i] < l[i][k+1]:
-                                y_new[j,i] = y_v[i][k]
-                                break
-                
-                return y_new
-
-        if problem_type == "Continuous":
-            variables = X_mesh(x_l, x_u, dims, points)
-        elif problem_type == "Mixed":
-            y_l, y_u = Bounds_y(n_y)
-            all_vars = X_mesh(np.append(x_l, y_l), np.append(x_u, y_u), dims, points)
-            x_variables = all_vars[:, :n_x]
-            y_norm = all_vars[:, n_x:]
-            y_variables = Assign_y(y_v, n_y, y_norm, y_norm.shape[0])
-            variables = np.hstack((x_variables, y_variables))
-        elif problem_type == "Discrete":
-            y_l, y_u = Bounds_y(n_y)
-            y_norm = X_mesh(y_l, y_u, n_y, points)
-            variables = Assign_y(y_v, n_y, y_norm, y_norm.shape[0])
-        else:
-            pass
-
-        return variables
-    
     def QMC_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type, design_type):
 
         def Bounds_y(y_v, n_y):
 
             y_l = []
             y_u = []
             flag = int(all([(np.diff(y_v[i]) == 1).all() for i in range(n_y)]))
@@ -303,14 +277,64 @@
             method = Select_method(design_type, n_y)
             variables = Y_qmc(y_v, n_y, points, method)
         else:
             pass
 
         return variables
     
+    def Mesh_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type):
+
+        def X_mesh(lower_bound, upper_bound, dims, points):
+
+            lists = [np.linspace(lower_bound[i], upper_bound[i], points) for i in range(dims)]
+            mesh = np.meshgrid(*lists)
+            
+            return np.array(mesh).T.reshape(-1, dims)
+        
+        def Bounds_y(n_y):
+
+            y_l = np.zeros(n_y)
+            y_u = np.ones(n_y)
+            
+            return y_l, y_u
+
+        def Assign_y(y_v, n_y, y_norm, points):
+
+                size_y = [len(y_v[i]) for i in range(n_y)]
+                l = [[i/size_y[j] for i in range(size_y[j]+1)] for j in range(n_y)]
+                for i in range(len(l)):
+                    l[i][-1] = l[i][-1] + 0.0001
+                y_new = np.empty([points, n_y])
+                for i in range(n_y):
+                    for j in range(len(y_norm[:,i])):
+                        for k in range(len(l[i])-1):
+                            if l[i][k] <= y_norm[j,i] < l[i][k+1]:
+                                y_new[j,i] = y_v[i][k]
+                                break
+                
+                return y_new
+
+        if problem_type == "Continuous":
+            variables = X_mesh(x_l, x_u, dims, points)
+        elif problem_type == "Mixed":
+            y_l, y_u = Bounds_y(n_y)
+            all_vars = X_mesh(np.append(x_l, y_l), np.append(x_u, y_u), dims, points)
+            x_variables = all_vars[:, :n_x]
+            y_norm = all_vars[:, n_x:]
+            y_variables = Assign_y(y_v, n_y, y_norm, y_norm.shape[0])
+            variables = np.hstack((x_variables, y_variables))
+        elif problem_type == "Discrete":
+            y_l, y_u = Bounds_y(n_y)
+            y_norm = X_mesh(y_l, y_u, n_y, points)
+            variables = Assign_y(y_v, n_y, y_norm, y_norm.shape[0])
+        else:
+            pass
+
+        return variables
+
     # Main program
     if design_type == "random":
         variables = Random_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type)
     elif design_type == "LHS":
         variables = QMC_design(x_l, x_u, y_v, n_x, n_y, dims, points, problem_type, "LHS")
     elif design_type == "Sobol":
         points = int(np.ceil(np.sqrt(points))**2)
```

### Comparing `bopt_slf-1.0.1/bopt_slf/utils/Models.py` & `bopt_slf-1.0.2/bopt_slf/utils/Models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+# *******************************************************
+# Import libraries
+
 import GPy
 import numpy as np
 import properscoring as ps
 from sklearn.model_selection import train_test_split
-from sklearn.mixture import GaussianMixture
 
 # *******************************************************
 
 def Select_model(x, z, kernel, surrogate):
 
     if surrogate == "GP":
         model = GPy.models.GPRegression(x, z, kernel)
@@ -56,15 +58,15 @@
     else:
         pass
 
     return models_const
 
 # *******************************************************
 
-def Kernel_ABCD(x, z, dims, surrogate, evals, err_min = 0.25):
+def Kernel_discovery(x, z, dims, surrogate, evals, err_min = 0.25):
 
     def Search(x, z,  kernels):
 
         # Train the model with the base kernels
         ll, k, models = [], [], {}
         for name, kernel in kernels.items():
             model = Select_model(x, z, kernel, surrogate)
@@ -88,15 +90,14 @@
 
         return {ordered[0]: models[ordered[0]]}
 
     x_train, x_test, z_train, z_test = train_test_split(x, z, test_size=0.2)
     # Base kernels: SE, Periodic, Linear, RatQuad  
     kernels = {"linear": GPy.kern.Linear(input_dim=dims),
                     "RBF": GPy.kern.RBF(input_dim=dims, variance=1.0, lengthscale=1.0),
-                    "Mater_32": GPy.kern.Matern32(input_dim=dims, variance=1.0, lengthscale=1.0),
                     "Mater_52": GPy.kern.Matern52(input_dim=dims, variance=1.0, lengthscale=1.0),
                     "Periodic": GPy.kern.StdPeriodic(input_dim=dims, variance=1.0, lengthscale=1.0, period=1.0)
                     }
 
     for _ in range(evals):
 
         base_kernels = kernels.copy()
```

### Comparing `bopt_slf-1.0.1/bopt_slf/utils/Plotting.py` & `bopt_slf-1.0.2/bopt_slf/utils/Plotting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,88 @@
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import numpy as np
 from ..utils.Acq_fun import AF
 
+# *******************************************************
+
 def Data_plot(x_l, x_u, dims, n_plot):
 
     lists = [np.linspace(x_l[i], x_u[i], n_plot) for i in range(dims)]
     # Create a meshgrid data
     x_plot = np.meshgrid(*lists)
     x_plot = np.array(x_plot).T.reshape(-1, dims)
     
     return x_plot
 
-def Plot_fun_1D(x_plot, z_plot):
-
-    plt.plot(x_plot, z_plot)
-    plt.xlabel('$x$')
-    plt.ylabel('$f(x)$')
-    plt.title('function')
-    plt.show()
-
-def Plot_fun_2D(x_plot, z_plot, n_plot):
-    
-    x1_plot, x2_plot = x_plot[:,0].reshape(n_plot, n_plot), x_plot[:,1].reshape(n_plot, n_plot)
-    plt.contourf(x1_plot, x2_plot, z_plot, cmap='jet')
-    plt.xlabel('$x_1$')
-    plt.ylabel('$x_2$')
-    plt.title('function')
-    cbar = plt.colorbar(mpl.cm.ScalarMappable(norm=mpl.colors.Normalize(vmin=0, vmax=1), cmap='jet'))
-    plt.show()
+# *******************************************************
 
 def Plot_surrogate(args):
 
-    _, f_best, x_init, f_init, x_iters, f_iters, x_l, x_u, dims, _, _, xi, acquisition_function, _, _, _, model = args.__dict__.values()
-    #x_best, f_best, x_init, f_init, x_iters, f_iters, x_l, x_u, dims, iters, inital_design, xi, acquisition_function, regret, constraint_method, models_const, model = args.__dict__.values()
+    _, _, x_init, f_init, x_iters, f_iters, x_l, x_u, dims, _, _, initial_points, _, _, _, _, _, model = args.__dict__.values()
+    # x_best, f_best, x_init, f_init, x_iters, f_iters, x_l, x_u, dims, iters, initial_design, initial_points, xi, acquisition_function, regret, constraint_method, models_constraints, model
 
     if dims == 1:
         
-        af_params = {'xi': xi, 'xi_decay': None, 'f_best': f_best, 'AF_name': acquisition_function}
+        #af_params = {'xi': xi, 'xi_decay': None, 'f_best': f_best, 'AF_name': acquisition_function}
         fig = plt.figure()
-        n_plot = 500
+        n_plot = 1000
         x_plot = Data_plot(x_l, x_u, dims, n_plot)
         f_mean, f_std = model.predict(x_plot)
 
         plt.plot(x_plot, f_mean)
         plt.fill_between(x_plot.reshape(-1), (f_mean - f_std).reshape(-1), (f_mean + f_std).reshape(-1), alpha=0.2)
         plt.scatter(x_init, f_init, c='k', s=10, label='Training data')
         plt.scatter(x_iters, f_iters, c='r', s=10, label='Observations')
         plt.xlabel('$x$')
         plt.ylabel('$f(x)$')
         plt.title('Surrogate model')
         plt.legend(bbox_to_anchor=(1.03, 1), loc='upper left', borderaxespad=0.)
         
     elif dims == 2:
 
-        af_params = {'xi': xi, 'xi_decay': None, 'f_best': f_best, 'AF_name': acquisition_function}
-        fig = plt.figure()
+        fig, ax = plt.subplots(1, 2, figsize=(15, 5))
         n_plot = 100
         x_plot = Data_plot(x_l, x_u, dims, n_plot)
         f_mean, f_std = model.predict(x_plot)
         x1_plot, x2_plot = x_plot[:,0].reshape(n_plot, n_plot), x_plot[:,1].reshape(n_plot, n_plot)
-
-        plt.contourf(x1_plot, x2_plot, f_mean, cmap='jet')
-        #plt.scatter(x[:,0], x[:,1], c='k', s=10, label='Training data')
-        plt.set_xlabel('$x_1$')
-        plt.set_ylabel('$x_2$')
-        plt.set_title('Acquisition function')
-        #cbar = fig.colorbar(mpl.cm.ScalarMappable(norm=mpl.colors.Normalize(vmin=0, vmax=1), cmap='jet'), ax=ax[1])
-
-        plt.legend(bbox_to_anchor=(1.03, 1), loc='upper left', borderaxespad=0.)
+        x1_init, x2_init = x_init[:,0], x_init[:,1]
+        x1_iters, x2_iters = x_iters[:,0], x_iters[:,1]
+        f_mean, f_std = f_mean.reshape(n_plot, n_plot), f_std.reshape(n_plot, n_plot)
+
+        p1 = ax[0].contourf(x1_plot, x2_plot, f_mean, cmap='jet')
+        ax[0].scatter(x1_init, x2_init, c='k', label='Training data')
+        ax[0].scatter(x1_iters, x2_iters, c='r', label='Observations')
+        ax[0].set_xlabel('$x_1$')
+        ax[0].set_ylabel('$x_2$')
+        ax[0].set_title('Surrogate model \n mean')
+
+        p2 = ax[1].contourf(x1_plot, x2_plot, f_std, cmap='jet')
+        ax[1].scatter(x1_init, x2_init, c='k', label='Training data')
+        ax[1].scatter(x1_iters, x2_iters, c='r', label='Observations')
+        ax[1].set_xlabel('$x_1$')
+        ax[1].set_ylabel('$x_2$')
+        ax[1].set_title('Surrogate model \n uncertanty')
+        
+        plt.colorbar(p1)
+        plt.colorbar(p2)
+        plt.legend(bbox_to_anchor=(1.3, 1), loc='upper left', borderaxespad=0.)
 
     elif dims > 2:
 
         print('not posible to plot')
         fig = None
 
     return fig
 
+# *******************************************************
+
 def Plot_AF(args):
 
-    _, f_best, _, _, _, _, x_l, x_u, dims, _, _, xi, acquisition_function, _, constraints_method, models_const, model = args.__dict__.values()
+    _, f_best, _, _, _, _, x_l, x_u, dims, _, _, _, xi, acquisition_function, _, constraints_method, models_const, model = args.__dict__.values()
 
     if dims == 1:
         
         af_params = {'xi': xi, 'xi_decay': None, 'f_best': f_best, 'AF_name': acquisition_function}
         fig = plt.figure()
         n_plot = 500
         x_plot = Data_plot(x_l, x_u, dims, n_plot)
@@ -96,37 +95,33 @@
         
     elif dims == 2:
 
         af_params = {'xi': xi, 'xi_decay': None, 'f_best': f_best, 'AF_name': acquisition_function}
         fig = plt.figure()
         n_plot = 100
         x_plot = Data_plot(x_l, x_u, dims, n_plot)
-        z_acq, _ = AF(x_plot, af_params, constraints_method, model, models_const)
+        z_acq = AF(x_plot, af_params, constraints_method, model, models_const)
         x1_plot, x2_plot = x_plot[:,0].reshape(n_plot, n_plot), x_plot[:,1].reshape(n_plot, n_plot)
         z_acq = z_acq.reshape(n_plot, n_plot)        
 
         plt.contourf(x1_plot, x2_plot, z_acq, cmap='jet')
-        #plt.scatter(x[:,0], x[:,1], c='k', s=10, label='Training data')
-        plt.set_xlabel('$x_1$')
-        plt.set_ylabel('$x_2$')
-        plt.set_title('Acquisition function')
-        #cbar = fig.colorbar(mpl.cm.ScalarMappable(norm=mpl.colors.Normalize(vmin=0, vmax=1), cmap='jet'), ax=ax[1])
-
-        plt.legend(bbox_to_anchor=(1.03, 1), loc='upper left', borderaxespad=0.)
+        plt.xlabel('$x_1$')
+        plt.ylabel('$x_2$')
+        plt.title('Acquisition function')
 
     elif dims > 2:
 
         print('not posible to plot')
         fig = None
 
     return fig
 
 def Plot_regret(args):
 
-    _, _, _, _, _, _, _, _, dims, _, _, _, _, regret, _, _, _ = args.__dict__.values()
+    _, _, _, _, _, _, _, _, _, _, _, _, _, _, regret, _, _, _ = args.__dict__.values()
     R = np.cumsum(regret)
 
     fig = plt.figure()
 
     plt.plot(regret, label="instantaneous regret")
     plt.plot(R, label="cummulative regret")
     plt.xlabel('Iterations')
```

### Comparing `bopt_slf-1.0.1/bopt_slf/utils/Querry_points.py` & `bopt_slf-1.0.2/bopt_slf/utils/Querry_points.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 # Class to find the optimal points of each of the conected components, and the constrains using the Mahalanobis distance
-# Inputs:
-# x is a vector of the symbolic representation of the variables
-# x_matrix is a numpy array with the mesh data 
-# x_l is the lower bound of the problem
-# x_u is the upper bound of the problem
-# dims is the total dimensions of the reduced representation of the model
-# S is a symbolic vector of the parametrized 
-# model is the GPy Gaussian Process model
-# acquisition_function is the acquisition function
-# Outputs:
-# x_opt is a vector with the querry points
-# x_l_new is the lower bounds of the mesh data
-# x_u_new is the upper bounds of the mesh data
+
+# *******************************************************
+# Import libraries
 
 import numpy as np
 import sympy as sp
 from scipy.optimize import minimize
 
+# *******************************************************
+
 def Querry(x, x_matrix, n_elements, bounds, dims, af_params, constraints_method, sense, model, models_const, Acq_fun):
 
     # Acquisition function for the optimization
     def Acquisition_function_opt(x, af_params, sense, model, models_const):
 
         if sense == "maximize":
             af_opt = -Acq_fun(x.reshape(1,-1), af_params, constraints_method, model, models_const)
@@ -89,24 +81,22 @@
             lam = lambda x: fun(*x)
             return lam
 
         constraints = [Constraint_lambify(const_lamb[i]) for i in range(n_elements)]
         
         return constraints
     
-    # Main code
+    # Main program
     # Check if the initial database is empty
     if x_matrix is None:
         raise ValueError('Initial database is empty')
     # Compute the confidence region
     mu, Sigma, P, chi = Mahalanobis_distance(x_matrix, n_elements)
     # Define the constrains
     constraints = Constrains(x, n_elements, mu, Sigma, chi)
-    #return x_l_new, x_u_new
     # Define the optimization problem
     x_opt = []
     for i in range(n_elements):
-        #bnds = [[x_l_new[i][j], x_u_new[i][j]] for j in range(dims)]
         res = minimize(Acquisition_function_opt, x0=mu[i], args=(af_params, sense, model, models_const), method='SLSQP', bounds=bounds, constraints={'type': 'ineq', 'fun': constraints[i]})
         x_opt.append(res.x)        
 
     return x_opt
```

### Comparing `bopt_slf-1.0.1/bopt_slf/utils/Set_level_filtration.py` & `bopt_slf-1.0.2/bopt_slf/utils/Set_level_filtration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # Create class for the querry points using Gaussian Process, UCB and Set-level filtration
 # Each querry point is a connected component of the matrix of points x in the domain adove the level set
-# The constrains are mean(x) < CI and (x-mu(x))'cov(x)(x-mu(x)) <= CI^2 if the connected component has more than one point
-# D_0: initial database
-# x: variables of the data as a list of symbols
-# dims: number of dimensions of the variables
-# bounds: bounds of the variables as a list
-# kernel: kernel of the Gaussian Process
 
+# *******************************************************
+# Import libraries
 import numpy as np
-import sys
 from itertools import product, permutations
- 
+
+# *******************************************************
+
 def Slf(mesh, p_mesh, dims, q0, jobs, af_params, constraints_method, sense, model, models_const, Acq_fun):
 
     def Flatten(l):
 
         return [item for sublist in l for item in sublist]
 
     def Filtration(x, score, p_x, dims, level, sense):
@@ -97,18 +94,23 @@
         scores_mean = []
 
         for i in range(n_elements):
             #connected_elements[0]
             scores_lst.append(np.array([Replace_val(x[i][j], mesh_all, score_all) for j in range(len(x[i]))]))
 
         for i in range(n_elements):
-            try:
+            if len(scores_lst[i].shape) == 1:
+                scores_mean.append(np.mean([np.mean(scores_lst[i][j]) for j in range(len(scores_lst[i]))]))
+                #for j in range(len(scores_lst[i])):
+                #    scores_mean.append(np.mean(scores_lst[i][j]))
+            else:
                 scores_mean.append(np.mean(scores_lst[i]))
-            except:
-                sys.exit(1)
+            #except:
+            #    print(scores_lst)
+            #    print('Todo: Broadcast error with numpy mean function to be solved')
                 
         if sense == "maximize":
             sorted = np.sort(scores_mean)[::-1][:jobs]
         elif sense == "minimize":
             sorted = np.sort(scores_mean)[:jobs]
         l = np.array([np.where(scores_mean == sorted[i]) for i in range(len(sorted))]).reshape(-1)
         connected_elements = [x[i] for i in l]
```

### Comparing `bopt_slf-1.0.1/bopt_slf/utils/Update.py` & `bopt_slf-1.0.2/bopt_slf/utils/Update.py`

 * *Files identical despite different names*

### Comparing `bopt_slf-1.0.1/bopt_slf/utils/__init__.py` & `bopt_slf-1.0.2/bopt_slf/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 from .Acq_fun import UCB, PI, EI, PoF, Prob_GPC, AF
 from .Aux import Errors, Data_eval, Eval_fun, Eval_const, Regret, Print_results, Create_results
 from .Dimension_reduction import Trans_data_to_pandas, Reduce, Inverse, Train_reducer, Train_inverter, Find_reducer, Find_inverter, Red_bounds
 from .Initialize import Space, Problem_type, Get_constraints, Times_fun, Points_initial_design, x_Generator, Bounds, Points_mesh, AF_params
-from .Models import Select_model, Train_model, Train_models_const, Kernel_ABCD
+from .Models import Select_model, Train_model, Train_models_const, Kernel_discovery
 from .Querry_points import Querry
 from .Set_level_filtration import Slf
 from .Update import Up_mesh
```

### Comparing `bopt_slf-1.0.1/bopt_slf.egg-info/PKG-INFO` & `bopt_slf-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: bopt-slf
-Version: 1.0.1
+Name: bopt_slf
+Version: 1.0.2
 Summary: Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems
-Author: Javier Morlet
+Author: Javier Morlet-Espinosa
 Author-email: a00833961@tec.mx
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.23.5
 Requires-Dist: sympy>=1.11.1
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: GPy>=1.10.0
 Requires-Dist: scipy>=1.10.1
```

### Comparing `bopt_slf-1.0.1/bopt_slf.egg-info/SOURCES.txt` & `bopt_slf-1.0.2/bopt_slf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bopt_slf-1.0.1/setup.py` & `bopt_slf-1.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_packages, setup
 
-
-setup(name='bopt_slf',
-      version='1.0.1',
-      description='Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems',
-      author='Javier Morlet',
-      author_email='a00833961@tec.mx',
-      packages = find_packages(),
-      install_requires=[
-          'numpy>=1.23.5',
-          'sympy>=1.11.1',
-          'pandas>=2.0.3',
-          'GPy>=1.10.0',
-          'scipy>=1.10.1',
-          'scikit-learn>=1.1.3',
-          'properscoring>=0.1',
-          'prince>=0.12.1',
-          'matplotlib>=3.7.3'
-          ]
-     )
+setup(
+    name='bopt_slf',
+    version='1.0.2',
+    description='Bayesian optimization for constrained or unconstrained, continuous, discrete or mixed data problems',
+    author='Javier Morlet-Espinosa',
+    author_email='a00833961@tec.mx',
+    packages = find_packages(),
+    install_requires=[
+        'numpy>=1.23.5',
+        'sympy>=1.11.1',
+        'pandas>=2.0.3',
+        'GPy>=1.10.0',
+        'scipy>=1.10.1',
+        'scikit-learn>=1.1.3',
+        'properscoring>=0.1',
+        'prince>=0.12.1',
+        'matplotlib>=3.7.3'
+        ]
+    )
```

