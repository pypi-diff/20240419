# Comparing `tmp/galmoss-2.0.7.tar.gz` & `tmp/galmoss-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/galmoss-2.0.7.tar", last modified: Tue Apr 16 14:50:34 2024, max compression
+gzip compressed data, was "dist/galmoss-2.0.8.tar", last modified: Fri Apr 19 08:26:22 2024, max compression
```

## Comparing `galmoss-2.0.7.tar` & `galmoss-2.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-16 14:50:34.000000 galmoss-2.0.7/
--rw-rw-rw-   0 cmloveczy   (501) staff       (20)    35148 2022-03-08 07:22:55.000000 galmoss-2.0.7/LICENSE
--rw-r--r--   0 cmloveczy   (501) staff       (20)     6749 2024-04-16 14:50:34.000000 galmoss-2.0.7/PKG-INFO
--rw-r--r--   0 cmloveczy   (501) staff       (20)     6049 2024-04-16 14:49:21.000000 galmoss-2.0.7/README.rst
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-16 14:50:34.000000 galmoss-2.0.7/galmoss/
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-16 14:50:34.000000 galmoss-2.0.7/galmoss/Parameter/
--rw-rw-r--   0 cmloveczy   (501) staff       (20)        0 2024-03-12 18:15:25.000000 galmoss-2.0.7/galmoss/Parameter/__init__.py
--rw-rw-r--   0 cmloveczy   (501) staff       (20)    19164 2024-04-16 14:24:00.000000 galmoss-2.0.7/galmoss/Parameter/basic.py
--rw-rw-r--   0 cmloveczy   (501) staff       (20)    15957 2024-04-16 14:22:51.000000 galmoss-2.0.7/galmoss/Parameter/decorater.py
--rw-rw-r--   0 cmloveczy   (501) staff       (20)      212 2024-04-16 14:38:04.000000 galmoss-2.0.7/galmoss/__init__.py
--rw-rw-r--   0 cmloveczy   (501) staff       (20)    12422 2024-04-16 14:05:57.000000 galmoss-2.0.7/galmoss/data.py
--rw-rw-r--   0 cmloveczy   (501) staff       (20)    26616 2024-04-16 07:21:44.000000 galmoss-2.0.7/galmoss/fitting.py
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-16 14:50:34.000000 galmoss-2.0.7/galmoss/profile/
--rw-rw-r--   0 cmloveczy   (501) staff       (20)        0 2024-03-12 18:15:25.000000 galmoss-2.0.7/galmoss/profile/__init__.py
--rw-rw-r--   0 cmloveczy   (501) staff       (20)     8488 2024-03-12 18:15:26.000000 galmoss-2.0.7/galmoss/profile/basic.py
--rw-rw-r--   0 cmloveczy   (501) staff       (20)    15121 2024-04-12 03:39:58.000000 galmoss-2.0.7/galmoss/profile/light_profile.py
--rw-rw-r--   0 cmloveczy   (501) staff       (20)    16971 2024-04-12 03:39:02.000000 galmoss-2.0.7/galmoss/uncertainty.py
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-16 14:50:34.000000 galmoss-2.0.7/galmoss.egg-info/
--rw-r--r--   0 cmloveczy   (501) staff       (20)     6749 2024-04-16 14:50:34.000000 galmoss-2.0.7/galmoss.egg-info/PKG-INFO
--rw-r--r--   0 cmloveczy   (501) staff       (20)      403 2024-04-16 14:50:34.000000 galmoss-2.0.7/galmoss.egg-info/SOURCES.txt
--rw-r--r--   0 cmloveczy   (501) staff       (20)        1 2024-04-16 14:50:34.000000 galmoss-2.0.7/galmoss.egg-info/dependency_links.txt
--rw-r--r--   0 cmloveczy   (501) staff       (20)        8 2024-04-16 14:50:34.000000 galmoss-2.0.7/galmoss.egg-info/top_level.txt
--rw-r--r--   0 cmloveczy   (501) staff       (20)       38 2024-04-16 14:50:34.000000 galmoss-2.0.7/setup.cfg
--rw-rw-rw-   0 cmloveczy   (501) staff       (20)      952 2024-04-16 14:49:11.000000 galmoss-2.0.7/setup.py
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-19 08:26:22.000000 galmoss-2.0.8/
+-rw-rw-rw-   0 cmloveczy   (501) staff       (20)    35148 2022-03-08 07:22:55.000000 galmoss-2.0.8/LICENSE
+-rw-r--r--   0 cmloveczy   (501) staff       (20)     6749 2024-04-19 08:26:22.000000 galmoss-2.0.8/PKG-INFO
+-rw-r--r--   0 cmloveczy   (501) staff       (20)     6049 2024-04-16 14:49:21.000000 galmoss-2.0.8/README.rst
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-19 08:26:22.000000 galmoss-2.0.8/galmoss/
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-19 08:26:22.000000 galmoss-2.0.8/galmoss/Parameter/
+-rw-r--r--   0 cmloveczy   (501) staff       (20)        0 2024-04-19 08:14:26.000000 galmoss-2.0.8/galmoss/Parameter/__init__.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    19164 2024-04-19 08:14:26.000000 galmoss-2.0.8/galmoss/Parameter/basic.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    15957 2024-04-19 08:14:26.000000 galmoss-2.0.8/galmoss/Parameter/decorater.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)      212 2024-04-19 08:14:50.000000 galmoss-2.0.8/galmoss/__init__.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    12422 2024-04-19 08:14:26.000000 galmoss-2.0.8/galmoss/data.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    26642 2024-04-19 08:14:26.000000 galmoss-2.0.8/galmoss/fitting.py
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-19 08:26:22.000000 galmoss-2.0.8/galmoss/profile/
+-rw-r--r--   0 cmloveczy   (501) staff       (20)        0 2024-04-19 08:14:26.000000 galmoss-2.0.8/galmoss/profile/__init__.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)     8488 2024-04-19 08:14:26.000000 galmoss-2.0.8/galmoss/profile/basic.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    14997 2024-04-19 08:14:26.000000 galmoss-2.0.8/galmoss/profile/light_profile.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    16971 2024-04-19 08:14:26.000000 galmoss-2.0.8/galmoss/uncertainty.py
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-04-19 08:26:22.000000 galmoss-2.0.8/galmoss.egg-info/
+-rw-r--r--   0 cmloveczy   (501) staff       (20)     6749 2024-04-19 08:26:21.000000 galmoss-2.0.8/galmoss.egg-info/PKG-INFO
+-rw-r--r--   0 cmloveczy   (501) staff       (20)      403 2024-04-19 08:26:21.000000 galmoss-2.0.8/galmoss.egg-info/SOURCES.txt
+-rw-r--r--   0 cmloveczy   (501) staff       (20)        1 2024-04-19 08:26:21.000000 galmoss-2.0.8/galmoss.egg-info/dependency_links.txt
+-rw-r--r--   0 cmloveczy   (501) staff       (20)        8 2024-04-19 08:26:21.000000 galmoss-2.0.8/galmoss.egg-info/top_level.txt
+-rw-r--r--   0 cmloveczy   (501) staff       (20)       38 2024-04-19 08:26:22.000000 galmoss-2.0.8/setup.cfg
+-rw-rw-rw-   0 cmloveczy   (501) staff       (20)      952 2024-04-19 08:25:51.000000 galmoss-2.0.8/setup.py
```

### Comparing `galmoss-2.0.7/LICENSE` & `galmoss-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `galmoss-2.0.7/PKG-INFO` & `galmoss-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galmoss
-Version: 2.0.7
+Version: 2.0.8
 Summary: A Python-based, Torch-powered tool for two-dimensional fitting of galaxy profiles. By seamlessly enabling GPU parallelization, GalMOSS meets the high computational demands of large-scale galaxy surveys.
 Home-page: https://github.com/Chenmi0619/GALMoss
 Author: Chen Mi
 Author-email: chenmiastro@gmail.com
 Keywords: Astronomy data analysis,Astronomy toolbox,Galaxy profile fitting
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `galmoss-2.0.7/README.rst` & `galmoss-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `galmoss-2.0.7/galmoss/Parameter/basic.py` & `galmoss-2.0.8/galmoss/Parameter/basic.py`

 * *Files identical despite different names*

### Comparing `galmoss-2.0.7/galmoss/Parameter/decorater.py` & `galmoss-2.0.8/galmoss/Parameter/decorater.py`

 * *Files identical despite different names*

### Comparing `galmoss-2.0.7/galmoss/data.py` & `galmoss-2.0.8/galmoss/data.py`

 * *Files identical despite different names*

### Comparing `galmoss-2.0.7/galmoss/fitting.py` & `galmoss-2.0.8/galmoss/fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,14 +532,15 @@
         
         if iter == 0:
             batched_best_chi_mu = chi_mu
             stop_update_count += 1
             self.update_param_best_value(index=None)
            
         else: 
+            print(chi_mu)
             is_better = chi_mu < batched_best_chi_mu
             improvement_small = ((torch.abs(chi_mu - 1) 
                                  < torch.abs(batched_best_chi_mu - 1)) 
                                  & ((batched_best_chi_mu - chi_mu) 
                                     / batched_best_chi_mu  < self.threshold))
             
             batched_eff_iter[is_better] = iter
```

### Comparing `galmoss-2.0.7/galmoss/profile/basic.py` & `galmoss-2.0.8/galmoss/profile/basic.py`

 * *Files identical despite different names*

### Comparing `galmoss-2.0.7/galmoss/profile/light_profile.py` & `galmoss-2.0.8/galmoss/profile/light_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,14 @@
              * (torch.exp(torch.lgamma(2 * self.ser_n.value(mode))))  
              / torch.pow(10, 
                          2 * self.ser_n.value(mode) 
                          *torch.log10(self.sersic_constant(self.ser_n.value(mode)))
                          )
              )
              )
-        # np.save("/data/public/ChenM/MIFIT/MANGA/data/g/final_paper_data/ie.npy", I_e.detach().cpu().numpy())
-        # exit()
         return (I_e 
                 * torch.exp(-self.sersic_constant(self.ser_n.value(mode))
                             * ( torch.pow(radius / self.eff_r.value(mode), 
                                           1.0 / self.ser_n.value(mode))
                                - 1)
                             )
                 )
@@ -495,13 +493,13 @@
         Returns the model image of the flat sky light profile from a grid.
 
         Parameters
         ----------
         grid
             The coordinate grid (galaxy-centered).
         """        
-        return torch.ones_like([0]) * self.sky_bg.value(mode)
+        return torch.ones_like(grid[0]) * self.sky_bg.value(mode)
```

### Comparing `galmoss-2.0.7/galmoss/uncertainty.py` & `galmoss-2.0.8/galmoss/uncertainty.py`

 * *Files identical despite different names*

### Comparing `galmoss-2.0.7/galmoss.egg-info/PKG-INFO` & `galmoss-2.0.8/galmoss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galmoss
-Version: 2.0.7
+Version: 2.0.8
 Summary: A Python-based, Torch-powered tool for two-dimensional fitting of galaxy profiles. By seamlessly enabling GPU parallelization, GalMOSS meets the high computational demands of large-scale galaxy surveys.
 Home-page: https://github.com/Chenmi0619/GALMoss
 Author: Chen Mi
 Author-email: chenmiastro@gmail.com
 Keywords: Astronomy data analysis,Astronomy toolbox,Galaxy profile fitting
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `galmoss-2.0.7/setup.py` & `galmoss-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r',encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='galmoss',
-    version='2.0.7',
+    version='2.0.8',
     description='A Python-based, Torch-powered tool for two-dimensional fitting of galaxy profiles. By seamlessly enabling GPU parallelization, GalMOSS meets the high computational demands of large-scale galaxy surveys.',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url='https://github.com/Chenmi0619/GALMoss',
     keywords=['Astronomy data analysis', 'Astronomy toolbox', 'Galaxy profile fitting'],
     author='Chen Mi',
     author_email='chenmiastro@gmail.com',
```

