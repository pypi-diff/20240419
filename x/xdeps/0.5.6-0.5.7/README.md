# Comparing `tmp/xdeps-0.5.6.tar.gz` & `tmp/xdeps-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdeps-0.5.6.tar", last modified: Mon Feb 19 08:44:13 2024, max compression
+gzip compressed data, was "xdeps-0.5.7.tar", last modified: Fri Apr 19 13:21:11 2024, max compression
```

## Comparing `xdeps-0.5.6.tar` & `xdeps-0.5.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:44:13.297374 xdeps-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-02-19 08:44:02.000000 xdeps-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-19 08:44:13.297374 xdeps-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-19 08:44:02.000000 xdeps-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 08:44:13.297374 xdeps-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-02-19 08:44:02.000000 xdeps-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:44:13.293374 xdeps-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-19 08:44:02.000000 xdeps-0.5.6/tests/test_madxparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-02-19 08:44:02.000000 xdeps-0.5.6/tests/test_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-02-19 08:44:02.000000 xdeps-0.5.6/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-02-19 08:44:02.000000 xdeps-0.5.6/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-02-19 08:44:02.000000 xdeps-0.5.6/tests/test_xdeps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:44:13.297374 xdeps-0.5.6/xdeps/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/generate_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/madxutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:44:13.297374 xdeps-0.5.6/xdeps/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/optimize/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (127)    33117 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)  1723637 2024-02-19 08:44:12.000000 xdeps-0.5.6/xdeps/refs.c
--rw-r--r--   0 runner    (1001) docker     (127)    28509 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    19116 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-02-19 08:44:02.000000 xdeps-0.5.6/xdeps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 08:44:13.297374 xdeps-0.5.6/xdeps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-19 08:44:13.000000 xdeps-0.5.6/xdeps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-19 08:44:13.000000 xdeps-0.5.6/xdeps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 08:44:13.000000 xdeps-0.5.6/xdeps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-19 08:44:13.000000 xdeps-0.5.6/xdeps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-19 08:44:13.000000 xdeps-0.5.6/xdeps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:21:11.752910 xdeps-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-19 13:21:06.000000 xdeps-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 13:21:11.752910 xdeps-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 13:21:06.000000 xdeps-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:21:11.752910 xdeps-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-19 13:21:06.000000 xdeps-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:21:11.748911 xdeps-0.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-19 13:21:06.000000 xdeps-0.5.7/tests/test_madxparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-19 13:21:06.000000 xdeps-0.5.7/tests/test_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-19 13:21:06.000000 xdeps-0.5.7/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-04-19 13:21:06.000000 xdeps-0.5.7/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-19 13:21:06.000000 xdeps-0.5.7/tests/test_xdeps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:21:11.752910 xdeps-0.5.7/xdeps/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/generate_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/madxutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:21:11.752910 xdeps-0.5.7/xdeps/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/optimize/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34454 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1724125 2024-04-19 13:21:11.000000 xdeps-0.5.7/xdeps/refs.c
+-rw-r--r--   0 runner    (1001) docker     (127)    28509 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19238 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19116 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-19 13:21:06.000000 xdeps-0.5.7/xdeps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:21:11.752910 xdeps-0.5.7/xdeps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 13:21:11.000000 xdeps-0.5.7/xdeps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 13:21:11.000000 xdeps-0.5.7/xdeps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:21:11.000000 xdeps-0.5.7/xdeps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 13:21:11.000000 xdeps-0.5.7/xdeps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 13:21:11.000000 xdeps-0.5.7/xdeps.egg-info/top_level.txt
```

### Comparing `xdeps-0.5.6/LICENSE` & `xdeps-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/PKG-INFO` & `xdeps-0.5.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdeps
-Version: 0.5.6
+Version: 0.5.7
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xdeps-0.5.6/setup.py` & `xdeps-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/tests/test_madxparser.py` & `xdeps-0.5.7/tests/test_madxparser.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/tests/test_refs.py` & `xdeps-0.5.7/tests/test_refs.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/tests/test_table.py` & `xdeps-0.5.7/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/tests/test_tasks.py` & `xdeps-0.5.7/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/tests/test_xdeps.py` & `xdeps-0.5.7/tests/test_xdeps.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/xdeps/generate_refs.py` & `xdeps-0.5.7/xdeps/generate_refs.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/xdeps/madxutils.py` & `xdeps-0.5.7/xdeps/madxutils.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/xdeps/optimize/jacobian.py` & `xdeps-0.5.7/xdeps/optimize/jacobian.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/xdeps/optimize/optimize.py` & `xdeps-0.5.7/xdeps/optimize/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,27 +142,29 @@
     def target(self, tar, value, **kwargs):
         return Target(tar, value, action=self, **kwargs)
 
 class MeritFunctionForMatch:
 
     def __init__(self, vary, targets, actions, return_scalar,
                  call_counter, verbose, tw_kwargs, steps_for_jacobian,
+                 check_limits,
                  show_call_counter=True):
 
         self.vary = vary
         self.targets = targets
         self.actions = actions
         self.return_scalar = return_scalar
         self.call_counter = call_counter
         self.verbose = verbose
         self.tw_kwargs = tw_kwargs
         self.steps_for_jacobian = steps_for_jacobian
         self.found_point_within_tol= False
         self.zero_if_met = False
         self.show_call_counter = show_call_counter
+        self.check_limits=check_limits
 
     def _x_to_knobs(self, x):
         knob_values = np.array(x).copy()
         for ii, vv in enumerate(self.vary):
             if vv.weight is not None:
                 knob_values[ii] *= vv.weight
         return knob_values
@@ -203,21 +205,24 @@
         x_limits = np.array([[hh, ll] for hh, ll in zip(x_lim_low, x_lim_high)])
         return x_limits
 
     def get_merit_function(self, check_limits=True, return_scalar=None):
         return MeritFuctionView(self, check_limits=check_limits,
                                 return_scalar=return_scalar)
 
-    def __call__(self, x=None, check_limits=True, return_scalar=None):
+    def __call__(self, x=None, check_limits=None, return_scalar=None):
 
         if x is None:
             knob_values = self._extract_knob_values()
         else:
             knob_values = self._x_to_knobs(x)
 
+
+        if check_limits is None:
+            check_limits = self.check_limits
         # Set knobs
         for vv, val in zip(self.vary, knob_values):
             if vv.active:
                 if check_limits and vv.limits is not None and vv.limits[0] is not None:
                     if val < vv.limits[0]:
                         raise ValueError(
                             f'Knob {vv.name} is below lower limit.')
@@ -401,14 +406,15 @@
 
     def __init__(self, vary, targets, restore_if_fail=True,
                  solver=None,
                  verbose=False, assert_within_tol=True,
                  n_steps_max=20,
                  solver_options={},
                  show_call_counter=True,
+                 check_limits=True,
                  **kwargs):
 
         """
         Numerical optimizer for matching.
 
         Parameters
         ----------
@@ -432,14 +438,15 @@
             Options to pass to the solver. Defaults to {}.
 
         """
 
         if isinstance(vary, (str, Vary)):
             vary = [vary]
 
+
         input_vary = vary
         vary = []
         for ii, rr in enumerate(input_vary):
             if isinstance(rr, Vary):
                 vary.append(rr)
             elif isinstance(rr, str):
                 vary.append(Vary(rr))
@@ -505,14 +512,15 @@
         return_scalar = {'fsolve': False, 'bfgs': True, 'jacobian': False}[solver]
 
         _err = MeritFunctionForMatch(
                     vary=vary, targets=targets,
                     actions=actions,
                     return_scalar=return_scalar, call_counter=0, verbose=verbose,
                     tw_kwargs=kwargs, steps_for_jacobian=steps,
+                    check_limits=check_limits,
                     show_call_counter=show_call_counter)
 
         if solver == 'jacobian':
             self.solver = JacobianSolver(
                 func=_err, verbose=verbose,
                 **solver_options)
         else:
@@ -535,14 +543,16 @@
         Perform one or more optimization steps.
 
         Parameters
         ----------
         n_steps : int, optional
             Number of steps to perform. Defaults to 1.
         """
+        if not self.check_limits:
+            self._clip_to_limits()
 
         for i_step in range(n_steps):
             knobs_before = self._extract_knob_values()
 
             x = self._err._knobs_to_x(knobs_before)
             mskinp = self._err.mask_input
             if (self.solver.x is None or
@@ -628,17 +638,29 @@
         vvv['lower_limit'] = np.array([
             (vv.limits[0] if vv.limits is not None else None) for vv in self.vary])
         vvv['upper_limit'] = np.array([
             (vv.limits[1] if vv.limits is not None else None) for vv in self.vary])
         vvv[f'val_at_iter_{iter_ref}'] = self.log().vary[iter_ref, :]
         vvv['step'] = np.array([vv.step for vv in self.vary])
         vvv['weight'] = np.array([vv.weight for vv in self.vary])
+
+        # check if variable is in limits
+        in_lim=[]
+        for vv,cv,lo,hi in  zip(self.vary,vvv['current_val'],vvv['lower_limit'],vvv['upper_limit']):
+            good='OK'
+            if lo is not None and cv<lo:
+                good='LOW'
+            if hi is not None and cv>hi:
+                good='HIGH'
+            in_lim.append(good)
+        vvv['in_lim']=np.array(in_lim)
+
         vvv._col_names = [
             'id', 'state', 'tag', 'name', 'lower_limit', 'current_val',
-            'upper_limit',f'val_at_iter_{iter_ref}', 'step', 'weight']
+            'upper_limit', 'in_lim', f'val_at_iter_{iter_ref}', 'step', 'weight' ]
 
         print('Vary status:                 ')
         vvv.show(max_col_width=max_col_width, maxwidth=1000)
 
         if ret:
             return vvv
 
@@ -944,14 +966,35 @@
             If True, return a scalar value. If False, return an array.
             If None, use the default value for the solver. Defaults to None.
         """
 
         return self._err.get_merit_function(check_limits=check_limits,
                                             return_scalar=return_scalar)
 
+    def _clip_to_limits(self):
+        vals = self._err._extract_knob_values()
+        for vv,cv in zip(self.vary,vals):
+            if vv.limits is None:
+                continue
+            if vv.limits[0] is not None:
+                if cv < vv.limits[0]:
+                    vv.container[vv.name]=vv.limits[0]
+            if vv.limits[1] is not None:
+                if cv > vv.limits[1]:
+                    vv.container[vv.name]=vv.limits[1]
+
+
+    @property
+    def check_limits(self):
+        return self._err.check_limits
+
+    @check_limits.setter
+    def check_limits(self, value):
+        self._err.check_limits = value
+
     @property
     def _err(self):
         return self.solver.func
 
     @property
     def actions(self):
         return self._err.actions
```

### Comparing `xdeps-0.5.6/xdeps/refs.c` & `xdeps-0.5.7/xdeps/refs.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "xdeps.refs",
         "sources": [
             "xdeps/refs.py"
@@ -32,18 +32,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -127,14 +127,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -188,14 +190,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -249,60 +253,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -385,14 +412,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -728,16 +758,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1081,15 +1116,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1168,15 +1203,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1271,32 +1306,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -32188,24 +32206,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_5xdeps_4refs___pyx_scope_struct__genexpr *__pyx_freelist_5xdeps_4refs___pyx_scope_struct__genexpr[8];
 static int __pyx_freecount_5xdeps_4refs___pyx_scope_struct__genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_5xdeps_4refs___pyx_scope_struct__genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_5xdeps_4refs___pyx_scope_struct__genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_5xdeps_4refs___pyx_scope_struct__genexpr)))) {
     o = (PyObject*)__pyx_freelist_5xdeps_4refs___pyx_scope_struct__genexpr[--__pyx_freecount_5xdeps_4refs___pyx_scope_struct__genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_5xdeps_4refs___pyx_scope_struct__genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -32226,15 +32246,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_param);
   Py_CLEAR(p->__pyx_t_0);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_5xdeps_4refs___pyx_scope_struct__genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_5xdeps_4refs___pyx_scope_struct__genexpr)))) {
     __pyx_freelist_5xdeps_4refs___pyx_scope_struct__genexpr[__pyx_freecount_5xdeps_4refs___pyx_scope_struct__genexpr++] = ((struct __pyx_obj_5xdeps_4refs___pyx_scope_struct__genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -40416,15 +40436,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `xdeps-0.5.6/xdeps/refs.py` & `xdeps-0.5.7/xdeps/refs.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/xdeps/sorting.py` & `xdeps-0.5.7/xdeps/sorting.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/xdeps/table.py` & `xdeps-0.5.7/xdeps/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,17 @@
         # each element.
         fmt = "%%.%d%s" % (digits, fixed)
         out = np.char.mod(fmt, arr)
     elif arr.dtype.kind == "O" and isinstance(arr[0], Collection):
         # If array of collections (array with dtype=object) or list, give shape
         lengths = []
         for entry in arr:
-            if isinstance(entry, np.ndarray):
+            if isinstance(entry, str):
+                lengths.append(entry)
+            elif isinstance(entry, np.ndarray):
                 lengths.append(f'<array of shape {entry.shape}>')
             elif isinstance(entry, Collection):
                 lengths.append(f'<collection of length {len(entry)}>')
             else:
                 lengths.append(str(entry))
         out = np.array(lengths)
     else:
```

### Comparing `xdeps-0.5.6/xdeps/tasks.py` & `xdeps-0.5.7/xdeps/tasks.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/xdeps/utils.py` & `xdeps-0.5.7/xdeps/utils.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.5.6/xdeps.egg-info/PKG-INFO` & `xdeps-0.5.7/xdeps.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdeps
-Version: 0.5.6
+Version: 0.5.7
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xdeps-0.5.6/xdeps.egg-info/SOURCES.txt` & `xdeps-0.5.7/xdeps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

