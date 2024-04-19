# Comparing `tmp/RMCgp-0.0.15.tar.gz` & `tmp/RMCgp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RMCgp-0.0.15.tar", last modified: Sun Apr 14 05:04:49 2024, max compression
+gzip compressed data, was "RMCgp-0.0.2.tar", last modified: Fri Apr 19 04:00:13 2024, max compression
```

## Comparing `RMCgp-0.0.15.tar` & `RMCgp-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.353339 RMCgp-0.0.15/
--rw-r--r--   0 taung      (501) staff       (20)    11344 2024-03-29 05:02:13.000000 RMCgp-0.0.15/LICENSE.txt
--rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-14 05:04:49.353098 RMCgp-0.0.15/PKG-INFO
--rw-r--r--   0 taung      (501) staff       (20)     2065 2024-03-29 06:55:32.000000 RMCgp-0.0.15/README.md
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.344726 RMCgp-0.0.15/RMC/
--rw-r--r--   0 taung      (501) staff       (20)      194 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/__init__.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.345629 RMCgp-0.0.15/RMC/costfunctions/
--rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-01 23:53:14.000000 RMCgp-0.0.15/RMC/costfunctions/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      908 2024-04-02 05:45:17.000000 RMCgp-0.0.15/RMC/costfunctions/finalCosts.py
--rw-r--r--   0 taung      (501) staff       (20)     2234 2024-04-02 00:02:53.000000 RMCgp-0.0.15/RMC/costfunctions/runningCosts.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.346258 RMCgp-0.0.15/RMC/design/
--rw-r--r--   0 taung      (501) staff       (20)       45 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/design/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      943 2024-04-03 23:22:58.000000 RMCgp-0.0.15/RMC/design/generate_design.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.347002 RMCgp-0.0.15/RMC/emulator/
--rw-r--r--   0 taung      (501) staff       (20)     1372 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/emulator/GP.py
--rw-r--r--   0 taung      (501) staff       (20)       33 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/emulator/__init__.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.348593 RMCgp-0.0.15/RMC/model/
--rw-r--r--   0 taung      (501) staff       (20)       43 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/model/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     1834 2024-04-02 00:55:41.000000 RMCgp-0.0.15/RMC/model/hybridcontrol.py
--rw-r--r--   0 taung      (501) staff       (20)    10628 2024-04-14 00:34:05.000000 RMCgp-0.0.15/RMC/model/hybridrunner.py
--rw-r--r--   0 taung      (501) staff       (20)      376 2024-04-02 00:24:04.000000 RMCgp-0.0.15/RMC/model/test_inputs.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.349148 RMCgp-0.0.15/RMC/optimization/
--rw-r--r--   0 taung      (501) staff       (20)       49 2024-03-29 03:57:09.000000 RMCgp-0.0.15/RMC/optimization/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     1973 2024-04-04 00:16:01.000000 RMCgp-0.0.15/RMC/optimization/onestepOptimization.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.350764 RMCgp-0.0.15/RMC/simulate/
--rw-r--r--   0 taung      (501) staff       (20)      678 2024-04-13 22:03:27.000000 RMCgp-0.0.15/RMC/simulate/CIR.py
--rw-r--r--   0 taung      (501) staff       (20)      661 2024-04-13 22:03:23.000000 RMCgp-0.0.15/RMC/simulate/OU.py
--rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-13 22:45:04.000000 RMCgp-0.0.15/RMC/simulate/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      685 2024-04-13 22:45:29.000000 RMCgp-0.0.15/RMC/simulate/jacobi.py
--rw-r--r--   0 taung      (501) staff       (20)     3895 2024-04-13 22:34:36.000000 RMCgp-0.0.15/RMC/simulate/sim.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-14 05:04:49.352245 RMCgp-0.0.15/RMCgp.egg-info/
--rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/PKG-INFO
--rw-r--r--   0 taung      (501) staff       (20)      687 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/SOURCES.txt
--rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/dependency_links.txt
--rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/not-zip-safe
--rw-r--r--   0 taung      (501) staff       (20)      137 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/requires.txt
--rw-r--r--   0 taung      (501) staff       (20)        4 2024-04-14 05:04:49.000000 RMCgp-0.0.15/RMCgp.egg-info/top_level.txt
--rw-r--r--   0 taung      (501) staff       (20)       38 2024-04-14 05:04:49.353388 RMCgp-0.0.15/setup.cfg
--rw-r--r--   0 taung      (501) staff       (20)     1474 2024-04-14 05:03:59.000000 RMCgp-0.0.15/setup.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.773229 RMCgp-0.0.2/
+-rw-r--r--   0 taung      (501) staff       (20)    11344 2024-03-29 05:02:13.000000 RMCgp-0.0.2/LICENSE.txt
+-rw-r--r--   0 taung      (501) staff       (20)      806 2024-04-19 04:00:13.772978 RMCgp-0.0.2/PKG-INFO
+-rw-r--r--   0 taung      (501) staff       (20)     2065 2024-03-29 06:55:32.000000 RMCgp-0.0.2/README.md
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.764574 RMCgp-0.0.2/RMC/
+-rw-r--r--   0 taung      (501) staff       (20)      194 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/__init__.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.765563 RMCgp-0.0.2/RMC/costfunctions/
+-rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-01 23:53:14.000000 RMCgp-0.0.2/RMC/costfunctions/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      908 2024-04-02 05:45:17.000000 RMCgp-0.0.2/RMC/costfunctions/finalCosts.py
+-rw-r--r--   0 taung      (501) staff       (20)     2234 2024-04-02 00:02:53.000000 RMCgp-0.0.2/RMC/costfunctions/runningCosts.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.766210 RMCgp-0.0.2/RMC/design/
+-rw-r--r--   0 taung      (501) staff       (20)       45 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/design/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      943 2024-04-03 23:22:58.000000 RMCgp-0.0.2/RMC/design/generate_design.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.766821 RMCgp-0.0.2/RMC/emulator/
+-rw-r--r--   0 taung      (501) staff       (20)     1372 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/emulator/GP.py
+-rw-r--r--   0 taung      (501) staff       (20)       33 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/emulator/__init__.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.768518 RMCgp-0.0.2/RMC/model/
+-rw-r--r--   0 taung      (501) staff       (20)       43 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/model/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)     1834 2024-04-02 00:55:41.000000 RMCgp-0.0.2/RMC/model/hybridcontrol.py
+-rw-r--r--   0 taung      (501) staff       (20)    14221 2024-04-19 01:52:41.000000 RMCgp-0.0.2/RMC/model/hybridrunner.py
+-rw-r--r--   0 taung      (501) staff       (20)      376 2024-04-02 00:24:04.000000 RMCgp-0.0.2/RMC/model/test_inputs.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.769234 RMCgp-0.0.2/RMC/optimization/
+-rw-r--r--   0 taung      (501) staff       (20)       49 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/optimization/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)     2209 2024-04-18 23:03:13.000000 RMCgp-0.0.2/RMC/optimization/onestepOptimization.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.771045 RMCgp-0.0.2/RMC/simulate/
+-rw-r--r--   0 taung      (501) staff       (20)      678 2024-04-13 22:03:27.000000 RMCgp-0.0.2/RMC/simulate/CIR.py
+-rw-r--r--   0 taung      (501) staff       (20)      661 2024-04-13 22:03:23.000000 RMCgp-0.0.2/RMC/simulate/OU.py
+-rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-13 22:45:04.000000 RMCgp-0.0.2/RMC/simulate/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      685 2024-04-13 22:45:29.000000 RMCgp-0.0.2/RMC/simulate/jacobi.py
+-rw-r--r--   0 taung      (501) staff       (20)     3895 2024-04-13 22:34:36.000000 RMCgp-0.0.2/RMC/simulate/sim.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.772375 RMCgp-0.0.2/RMCgp.egg-info/
+-rw-r--r--   0 taung      (501) staff       (20)      806 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/PKG-INFO
+-rw-r--r--   0 taung      (501) staff       (20)      687 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/SOURCES.txt
+-rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/dependency_links.txt
+-rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/not-zip-safe
+-rw-r--r--   0 taung      (501) staff       (20)      137 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/requires.txt
+-rw-r--r--   0 taung      (501) staff       (20)        4 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/top_level.txt
+-rw-r--r--   0 taung      (501) staff       (20)       38 2024-04-19 04:00:13.773287 RMCgp-0.0.2/setup.cfg
+-rw-r--r--   0 taung      (501) staff       (20)     1473 2024-04-19 04:00:11.000000 RMCgp-0.0.2/setup.py
```

### Comparing `RMCgp-0.0.15/LICENSE.txt` & `RMCgp-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/PKG-INFO` & `RMCgp-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMCgp
-Version: 0.0.15
+Version: 0.0.2
 Summary: RMC for stochastic control.
 Home-page: https://github.com/thihaa2019/RMCgp
 Author: Thiha Aung
 Author-email: taung@ucsb.edu
 Maintainer: Thiha Aung
 Maintainer-email: taung@ucsb.edu
 License: Apache-2.0
```

### Comparing `RMCgp-0.0.15/README.md` & `RMCgp-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMC/costfunctions/finalCosts.py` & `RMCgp-0.0.2/RMC/costfunctions/finalCosts.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMC/costfunctions/runningCosts.py` & `RMCgp-0.0.2/RMC/costfunctions/runningCosts.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMC/design/generate_design.py` & `RMCgp-0.0.2/RMC/design/generate_design.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMC/emulator/GP.py` & `RMCgp-0.0.2/RMC/emulator/GP.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMC/model/hybridcontrol.py` & `RMCgp-0.0.2/RMC/model/hybridcontrol.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMC/model/hybridrunner.py` & `RMCgp-0.0.2/RMC/model/hybridrunner.py`

 * *Files 24% similar despite different names*

```diff
@@ -67,28 +67,28 @@
             kern = self.policy_kernel(control_input.shape[1],ARD = True)
         
 
         control_map = policyGP(control_input,control_output,kernel =kern,normalizer= True)
         #control_map.optimize_restarts(num_restarts=2)
         control_map.optimize()
 
-        MSE = self.MSE_evaluation(control_output.flatten(),control_map.predict(control_input)[0].flatten(),"Policy",I_train)
-        while MSE>=1e-1:
-            X_lb,X_ub = np.min(X_train),np.max(X_train)
-            X_new,I_new = design_generator(50,X_lb,X_ub,self.Ilb,self.Iub).create_samples
-            new_control_input = np.column_stack((X_new,I_new))
-            new_control_output = np.zeros(50)
-            for i in range(len(new_control_output)):
-                new_control_output[i] = self.optimizer.optimize(X_new[i],I_new[i],value_map,*args)
-            new_control_output = new_control_output.reshape(-1,1)
-            control_map.set_XY(np.vstack((control_map.X, new_control_input)), np.vstack((control_map.Y, new_control_output)))
-            control_map.optimize_restarts(num_restarts=2)
-            control_map.optimize()
-            MSE = self.MSE_evaluation(control_map.Y.flatten(),control_map.predict(control_map.X)[0].flatten(),\
-                                        "Policy",control_map.X[:,1])
+        self.MSE_evaluation(control_output.flatten(),control_map.predict(control_input)[0].flatten(),"Policy",I_train)
+        #while MSE>=1e-1:
+            #X_lb,X_ub = np.min(X_train),np.max(X_train)
+            #X_new,I_new = design_generator(50,X_lb,X_ub,self.Ilb,self.Iub).create_samples
+            #new_control_input = np.column_stack((X_new,I_new))
+            #new_control_output = np.zeros(50)
+            #for i in range(len(new_control_output)):
+            #    new_control_output[i] = self.optimizer.optimize(X_new[i],I_new[i],value_map,*args)
+            #new_control_output = new_control_output.reshape(-1,1)
+            #control_map.set_XY(np.vstack((control_map.X, new_control_input)), np.vstack((control_map.Y, new_control_output)))
+            #control_map.optimize_restarts(num_restarts=2)
+            #control_map.optimize()
+            #MSE = self.MSE_evaluation(control_map.Y.flatten(),control_map.predict(control_map.X)[0].flatten(),\
+                                      #  "Policy",control_map.X[:,1])
         #print(len(control_map.optimization_runs))
         return control_map
 
     def train_value(self,X_train,I_train,pointwisevalues):
         value_input = np.column_stack((X_train,I_train))
         value_output= pointwisevalues.reshape(-1,1)
         if self.value_kernel is None:
@@ -112,23 +112,26 @@
             X_prev_rep= np.repeat(X_prev,self.batch_size)
             I_next_rep= np.repeat(I_next,self.batch_size)
 
         X_next_rep= self.process.onestepsimulate(int(self.nsim*reshape_dim),X_prev_rep,drift_p1,drift_p2,vol_p1,vol_p2,step)
         power_outputs = policy_map.predict(np.column_stack((X_next_rep,I_next_rep)))[0].flatten()
         LB = np.maximum(self.Bmin,self.charging_eff*(self.Ilb- I_next_rep)/self.dt)
         UB = np.minimum(self.Bmax,(self.Iub-I_next_rep)/(self.charging_eff*self.dt))
+        # according to scipy.optimize, B>0 when X>=M
         pos_outputs = np.where(power_outputs>0)
-        # When X> M , cap B>0 by X-B, do not charge more and make Ot< Mt, when Ot guaranteed > M given X
+        # do not charge more than X-M, causing O < M , ensures B<= X-M or M<=X-B
         upper_charging_bound  = np.maximum(X_next_rep[pos_outputs]-target,0)
         power_outputs[pos_outputs] = np.minimum(power_outputs[pos_outputs],upper_charging_bound)
 
-        # DO NOT CHARGE WHEN X < M, otherwise Ot= X-B < X< M
-        # Dont make undersupply worse
-        idx = (X_next_rep < target ) & (power_outputs>0)
-        power_outputs[idx]=0
+        # according to scipy.optimize, B<0 when X<=M
+        neg_outputs = np.where(power_outputs<0)
+        # do not discharge more than X-M, causing O > M , ensures B>= X-M or M>=X-B
+        lower_charging_bound  = np.minimum(X_next_rep[neg_outputs]-target,0)
+        power_outputs[neg_outputs] = np.maximum(power_outputs[neg_outputs],lower_charging_bound)
+
         power_outputs = np.maximum(LB,np.minimum(power_outputs,UB))
         I_nextnext = I_next_rep + power_outputs *(self.charging_eff *(power_outputs>0) + 1/self.charging_eff * (power_outputs<0))*self.dt
         if isinstance(value_map,final_SOCcontraint):
             pointwise_v = self.running_cost.cost(power_outputs,X_next_rep,target,lower_target,upper_target) * self.dt + value_map.cost(I_nextnext)
         if isinstance(value_map,GPy.core.GP):
             inp = np.column_stack((X_next_rep,I_nextnext))
             pointwise_v = self.running_cost.cost(power_outputs,X_next_rep,target,lower_target,upper_target) * self.dt + value_map.predict(inp)[0].flatten()
@@ -186,14 +189,82 @@
     def policy_maps(self):
         return self.policies
     
     @property
     def value_maps(self):
         return self.values
     
+
+    def onePath_control(self,A_t,I0):
+        X_vec = A_t
+        I_vec = np.zeros(len(X_vec)+1)
+        assert I0<= self.Iub and I0>=self.Ilb, "I not in bound"
+        I_vec[0] =I0
+        B_vec = np.zeros(len(X_vec))
+        total_cost = 0
+        for i in range(24):
+            cur_X =  X_vec[i]
+            cur_I  = I_vec[i]
+            inp_vec = np.array([cur_X,cur_I]).reshape(1,-1)
+            B = self.policy_maps[i].predict(inp_vec)[0].flatten()
+
+            if B >0:
+                B= np.minimum(B,cur_X-self.targets[i])
+            if B<0:
+                B = np.maximum(cur_X-self.targets[i],B)
+            LB = np.maximum(self.Bmin,self.charging_eff*(self.Ilb- cur_I)/self.dt)
+            UB = np.minimum(self.Bmax,(self.Iub-cur_I)/(self.charging_eff*self.dt))
+            B = np.maximum(LB,np.minimum(B,UB))
+
+            B_vec[i] = B
+            cur_I = cur_I + B * ( (B>0) * self.charging_eff + (B<0) *1/self.charging_eff) * self.dt
+            total_cost = total_cost+ self.running_cost.cost(B,cur_X,self.targets[i],self.lower_targets[i],self.upper_targets[i])* self.dt
+            I_vec[i+1]=cur_I
+        total_cost += self.final_cost.cost(I_vec[-1])
+        return X_vec,I_vec,B_vec,total_cost
+
+    def monteCarlo_control(self,X0,I0,N_MC,init_sigma = None, randomize = False):
+        X_init = np.ones(N_MC)*X0
+        if randomize:
+            assert init_sigma>0, "Sigma must be positive"
+            X_init = np.minimum(np.random.normal(X0,init_sigma,size = (N_MC) ),self.process.UB)
+            X_init = np.maximum(X_init,self.process.LB)
+
+        self.process.nsim = N_MC
+        X_sims = self.process.simulate()
+        Bts = np.zeros((N_MC,self.nstep))
+        Is = np.zeros((N_MC,self.nstep+1)); Is[:,0] = I0 *np.ones(N_MC)
+
+        running_cost = np.zeros((N_MC,self.nstep))
+
+        for i in range(self.nstep):
+            LB = np.maximum(self.Bmin,self.charging_eff*(self.Ilb- Is[:,i])/self.dt)
+            UB = np.minimum(self.Bmax,(self.Iub-Is[:,i])/(self.charging_eff*self.dt))
+            inp = np.column_stack((X_sims[:,i],Is[:,i]))
+            Bts[:,i] = self.policy_maps[i].predict(inp)[0].flatten()
+            # according to scipy.optimize, B>0 when X>=M
+            pos_outputs = np.where(Bts[:,i] >0)
+            # do not charge more than X-M, causing O < M , ensures B<= X-M or M<=X-B
+            upper_charging_bound  = np.maximum(X_sims[pos_outputs,i]-self.targets[i],0)
+            Bts[pos_outputs,i] = np.minimum(Bts[pos_outputs,i],upper_charging_bound)
+
+            # according to scipy.optimize, B<0 when X<=M
+            neg_outputs = np.where(Bts[:,i] >0)
+            # do not discharge more than X-M, causing O > M , ensures B>= X-M or M>=X-B
+            lower_charging_bound  = np.minimum(X_sims[neg_outputs,i]-self.targets[i],0)
+            Bts[neg_outputs,i]= np.maximum(Bts[neg_outputs,i],lower_charging_bound)
+            Bts[:,i] = np.maximum(LB,np.minimum(Bts[:,i],UB))
+            Is[:,i+1] = Is[:,i]+Bts[:,i]*(self.charging_eff*(Bts[:,i]>0) +1/self.charging_eff *(Bts[:,i]<0))*self.dt
+            running_cost[:,i] = self.running_cost.cost(Bts[:,i],X_sims[:,i],self.targets[i],self.lower_targets[i],self.upper_targets[i])* self.dt
+        total_cost = np.sum(running_cost,axis = 1) +self.final_cost.cost(Is[:,-1]).flatten()
+
+        mean_total_cost = np.mean(total_cost)
+
+        return X_sims,Is,Bts, mean_total_cost
+
     def MSE_evaluation(self,y_true,GP_output,map_type,*args):
         if map_type == "Policy":
             cur_I = args[0]
             LB = np.maximum(self.Bmin,self.charging_eff*(self.Ilb- cur_I)/self.dt)
             UB = np.minimum(self.Bmax,(self.Iub-cur_I)/(self.charging_eff*self.dt))
             p1 = np.maximum(LB,np.minimum(y_true,UB))
             p2 = np.maximum(LB,np.minimum(GP_output,UB))
```

### Comparing `RMCgp-0.0.15/RMC/optimization/onestepOptimization.py` & `RMCgp-0.0.2/RMC/optimization/onestepOptimization.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,11 +36,18 @@
 
         cost_derivative = self.running_cost.derivative(B[0],X,*args) * self.dt + q_derivative* self.dt
         return cost_derivative
 
     def optimize(self,X,I,q,*remainingargs):
         target = remainingargs[0]
         starter = X- target
-
+        # excess gen imply charge only >0
+        if starter >0:
+            B_bnds = [(0,None)]
+        # under gen imply discharge only <0
+        elif starter<0:
+            B_bnds = [(None,0)]
+        else:
+            B_bnds = None
         opt_B = scipy.optimize.minimize(self.cost_togo, jac= self.cost_togo_derivative,x0=starter, \
                                        args=(X,I,q,*remainingargs),method = "L-BFGS-B",bounds=None)
         return opt_B.x[0]
```

### Comparing `RMCgp-0.0.15/RMC/simulate/CIR.py` & `RMCgp-0.0.2/RMC/simulate/CIR.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMC/simulate/OU.py` & `RMCgp-0.0.2/RMC/simulate/OU.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMC/simulate/jacobi.py` & `RMCgp-0.0.2/RMC/simulate/jacobi.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMC/simulate/sim.py` & `RMCgp-0.0.2/RMC/simulate/sim.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/RMCgp.egg-info/PKG-INFO` & `RMCgp-0.0.2/RMCgp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMCgp
-Version: 0.0.15
+Version: 0.0.2
 Summary: RMC for stochastic control.
 Home-page: https://github.com/thihaa2019/RMCgp
 Author: Thiha Aung
 Author-email: taung@ucsb.edu
 Maintainer: Thiha Aung
 Maintainer-email: taung@ucsb.edu
 License: Apache-2.0
```

### Comparing `RMCgp-0.0.15/RMCgp.egg-info/SOURCES.txt` & `RMCgp-0.0.2/RMCgp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.15/setup.py` & `RMCgp-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "GPy>=1.13.0",
     "scikit-learn>=1.3.0",
     "scipy>=1.1.4",
     "matplotlib>=3.8.0"
 ]
 
 setuptools.setup(name='RMCgp',
-                 version='0.0.15',
+                 version='0.0.2',
                  author='Thiha Aung',
                  author_email='taung@ucsb.edu',
                  maintainer='Thiha Aung',
                  maintainer_email='taung@ucsb.edu',
                  description='RMC for stochastic control.',
                  long_description=readme,
                  url='https://github.com/thihaa2019/RMCgp',
```

