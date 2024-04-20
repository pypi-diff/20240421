# Comparing `tmp/RMCgp-0.0.2.tar.gz` & `tmp/RMCgp-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RMCgp-0.0.2.tar", last modified: Fri Apr 19 04:00:13 2024, max compression
+gzip compressed data, was "RMCgp-0.0.22.tar", last modified: Sat Apr 20 23:56:04 2024, max compression
```

## Comparing `RMCgp-0.0.2.tar` & `RMCgp-0.0.22.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.773229 RMCgp-0.0.2/
--rw-r--r--   0 taung      (501) staff       (20)    11344 2024-03-29 05:02:13.000000 RMCgp-0.0.2/LICENSE.txt
--rw-r--r--   0 taung      (501) staff       (20)      806 2024-04-19 04:00:13.772978 RMCgp-0.0.2/PKG-INFO
--rw-r--r--   0 taung      (501) staff       (20)     2065 2024-03-29 06:55:32.000000 RMCgp-0.0.2/README.md
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.764574 RMCgp-0.0.2/RMC/
--rw-r--r--   0 taung      (501) staff       (20)      194 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/__init__.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.765563 RMCgp-0.0.2/RMC/costfunctions/
--rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-01 23:53:14.000000 RMCgp-0.0.2/RMC/costfunctions/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      908 2024-04-02 05:45:17.000000 RMCgp-0.0.2/RMC/costfunctions/finalCosts.py
--rw-r--r--   0 taung      (501) staff       (20)     2234 2024-04-02 00:02:53.000000 RMCgp-0.0.2/RMC/costfunctions/runningCosts.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.766210 RMCgp-0.0.2/RMC/design/
--rw-r--r--   0 taung      (501) staff       (20)       45 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/design/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      943 2024-04-03 23:22:58.000000 RMCgp-0.0.2/RMC/design/generate_design.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.766821 RMCgp-0.0.2/RMC/emulator/
--rw-r--r--   0 taung      (501) staff       (20)     1372 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/emulator/GP.py
--rw-r--r--   0 taung      (501) staff       (20)       33 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/emulator/__init__.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.768518 RMCgp-0.0.2/RMC/model/
--rw-r--r--   0 taung      (501) staff       (20)       43 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/model/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     1834 2024-04-02 00:55:41.000000 RMCgp-0.0.2/RMC/model/hybridcontrol.py
--rw-r--r--   0 taung      (501) staff       (20)    14221 2024-04-19 01:52:41.000000 RMCgp-0.0.2/RMC/model/hybridrunner.py
--rw-r--r--   0 taung      (501) staff       (20)      376 2024-04-02 00:24:04.000000 RMCgp-0.0.2/RMC/model/test_inputs.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.769234 RMCgp-0.0.2/RMC/optimization/
--rw-r--r--   0 taung      (501) staff       (20)       49 2024-03-29 03:57:09.000000 RMCgp-0.0.2/RMC/optimization/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)     2209 2024-04-18 23:03:13.000000 RMCgp-0.0.2/RMC/optimization/onestepOptimization.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.771045 RMCgp-0.0.2/RMC/simulate/
--rw-r--r--   0 taung      (501) staff       (20)      678 2024-04-13 22:03:27.000000 RMCgp-0.0.2/RMC/simulate/CIR.py
--rw-r--r--   0 taung      (501) staff       (20)      661 2024-04-13 22:03:23.000000 RMCgp-0.0.2/RMC/simulate/OU.py
--rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-13 22:45:04.000000 RMCgp-0.0.2/RMC/simulate/__init__.py
--rw-r--r--   0 taung      (501) staff       (20)      685 2024-04-13 22:45:29.000000 RMCgp-0.0.2/RMC/simulate/jacobi.py
--rw-r--r--   0 taung      (501) staff       (20)     3895 2024-04-13 22:34:36.000000 RMCgp-0.0.2/RMC/simulate/sim.py
-drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-19 04:00:13.772375 RMCgp-0.0.2/RMCgp.egg-info/
--rw-r--r--   0 taung      (501) staff       (20)      806 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/PKG-INFO
--rw-r--r--   0 taung      (501) staff       (20)      687 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/SOURCES.txt
--rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/dependency_links.txt
--rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/not-zip-safe
--rw-r--r--   0 taung      (501) staff       (20)      137 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/requires.txt
--rw-r--r--   0 taung      (501) staff       (20)        4 2024-04-19 04:00:13.000000 RMCgp-0.0.2/RMCgp.egg-info/top_level.txt
--rw-r--r--   0 taung      (501) staff       (20)       38 2024-04-19 04:00:13.773287 RMCgp-0.0.2/setup.cfg
--rw-r--r--   0 taung      (501) staff       (20)     1473 2024-04-19 04:00:11.000000 RMCgp-0.0.2/setup.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-20 23:56:04.868041 RMCgp-0.0.22/
+-rw-r--r--   0 taung      (501) staff       (20)    11344 2024-03-29 05:02:13.000000 RMCgp-0.0.22/LICENSE.txt
+-rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-20 23:56:04.867789 RMCgp-0.0.22/PKG-INFO
+-rw-r--r--   0 taung      (501) staff       (20)     2065 2024-03-29 06:55:32.000000 RMCgp-0.0.22/README.md
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-20 23:56:04.854195 RMCgp-0.0.22/RMC/
+-rw-r--r--   0 taung      (501) staff       (20)      194 2024-03-29 03:57:09.000000 RMCgp-0.0.22/RMC/__init__.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-20 23:56:04.855364 RMCgp-0.0.22/RMC/costfunctions/
+-rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-01 23:53:14.000000 RMCgp-0.0.22/RMC/costfunctions/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      908 2024-04-02 05:45:17.000000 RMCgp-0.0.22/RMC/costfunctions/finalCosts.py
+-rw-r--r--   0 taung      (501) staff       (20)     2234 2024-04-02 00:02:53.000000 RMCgp-0.0.22/RMC/costfunctions/runningCosts.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-20 23:56:04.856269 RMCgp-0.0.22/RMC/design/
+-rw-r--r--   0 taung      (501) staff       (20)       45 2024-03-29 03:57:09.000000 RMCgp-0.0.22/RMC/design/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      943 2024-04-03 23:22:58.000000 RMCgp-0.0.22/RMC/design/generate_design.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-20 23:56:04.857462 RMCgp-0.0.22/RMC/emulator/
+-rw-r--r--   0 taung      (501) staff       (20)     1372 2024-03-29 03:57:09.000000 RMCgp-0.0.22/RMC/emulator/GP.py
+-rw-r--r--   0 taung      (501) staff       (20)       33 2024-03-29 03:57:09.000000 RMCgp-0.0.22/RMC/emulator/__init__.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-20 23:56:04.860830 RMCgp-0.0.22/RMC/model/
+-rw-r--r--   0 taung      (501) staff       (20)       43 2024-03-29 03:57:09.000000 RMCgp-0.0.22/RMC/model/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)     1834 2024-04-02 00:55:41.000000 RMCgp-0.0.22/RMC/model/hybridcontrol.py
+-rw-r--r--   0 taung      (501) staff       (20)    14221 2024-04-20 21:34:38.000000 RMCgp-0.0.22/RMC/model/hybridrunner.py
+-rw-r--r--   0 taung      (501) staff       (20)      376 2024-04-02 00:24:04.000000 RMCgp-0.0.22/RMC/model/test_inputs.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-20 23:56:04.862018 RMCgp-0.0.22/RMC/optimization/
+-rw-r--r--   0 taung      (501) staff       (20)       49 2024-03-29 03:57:09.000000 RMCgp-0.0.22/RMC/optimization/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)     2015 2024-04-19 16:55:59.000000 RMCgp-0.0.22/RMC/optimization/onestepOptimization.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-20 23:56:04.865477 RMCgp-0.0.22/RMC/simulate/
+-rw-r--r--   0 taung      (501) staff       (20)      678 2024-04-13 22:03:27.000000 RMCgp-0.0.22/RMC/simulate/CIR.py
+-rw-r--r--   0 taung      (501) staff       (20)      661 2024-04-13 22:03:23.000000 RMCgp-0.0.22/RMC/simulate/OU.py
+-rw-r--r--   0 taung      (501) staff       (20)       87 2024-04-13 22:45:04.000000 RMCgp-0.0.22/RMC/simulate/__init__.py
+-rw-r--r--   0 taung      (501) staff       (20)      685 2024-04-13 22:45:29.000000 RMCgp-0.0.22/RMC/simulate/jacobi.py
+-rw-r--r--   0 taung      (501) staff       (20)     3895 2024-04-13 22:34:36.000000 RMCgp-0.0.22/RMC/simulate/sim.py
+drwxr-xr-x   0 taung      (501) staff       (20)        0 2024-04-20 23:56:04.867202 RMCgp-0.0.22/RMCgp.egg-info/
+-rw-r--r--   0 taung      (501) staff       (20)      807 2024-04-20 23:56:04.000000 RMCgp-0.0.22/RMCgp.egg-info/PKG-INFO
+-rw-r--r--   0 taung      (501) staff       (20)      687 2024-04-20 23:56:04.000000 RMCgp-0.0.22/RMCgp.egg-info/SOURCES.txt
+-rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-20 23:56:04.000000 RMCgp-0.0.22/RMCgp.egg-info/dependency_links.txt
+-rw-r--r--   0 taung      (501) staff       (20)        1 2024-04-20 23:56:04.000000 RMCgp-0.0.22/RMCgp.egg-info/not-zip-safe
+-rw-r--r--   0 taung      (501) staff       (20)      137 2024-04-20 23:56:04.000000 RMCgp-0.0.22/RMCgp.egg-info/requires.txt
+-rw-r--r--   0 taung      (501) staff       (20)        4 2024-04-20 23:56:04.000000 RMCgp-0.0.22/RMCgp.egg-info/top_level.txt
+-rw-r--r--   0 taung      (501) staff       (20)       38 2024-04-20 23:56:04.868094 RMCgp-0.0.22/setup.cfg
+-rw-r--r--   0 taung      (501) staff       (20)     1474 2024-04-20 23:55:02.000000 RMCgp-0.0.22/setup.py
```

### Comparing `RMCgp-0.0.2/LICENSE.txt` & `RMCgp-0.0.22/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/PKG-INFO` & `RMCgp-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMCgp
-Version: 0.0.2
+Version: 0.0.22
 Summary: RMC for stochastic control.
 Home-page: https://github.com/thihaa2019/RMCgp
 Author: Thiha Aung
 Author-email: taung@ucsb.edu
 Maintainer: Thiha Aung
 Maintainer-email: taung@ucsb.edu
 License: Apache-2.0
```

### Comparing `RMCgp-0.0.2/README.md` & `RMCgp-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/costfunctions/finalCosts.py` & `RMCgp-0.0.22/RMC/costfunctions/finalCosts.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/costfunctions/runningCosts.py` & `RMCgp-0.0.22/RMC/costfunctions/runningCosts.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/design/generate_design.py` & `RMCgp-0.0.22/RMC/design/generate_design.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/emulator/GP.py` & `RMCgp-0.0.22/RMC/emulator/GP.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/model/hybridcontrol.py` & `RMCgp-0.0.22/RMC/model/hybridcontrol.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/model/hybridrunner.py` & `RMCgp-0.0.22/RMC/model/hybridrunner.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/optimization/onestepOptimization.py` & `RMCgp-0.0.22/RMC/optimization/onestepOptimization.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,17 +37,11 @@
         cost_derivative = self.running_cost.derivative(B[0],X,*args) * self.dt + q_derivative* self.dt
         return cost_derivative
 
     def optimize(self,X,I,q,*remainingargs):
         target = remainingargs[0]
         starter = X- target
         # excess gen imply charge only >0
-        if starter >0:
-            B_bnds = [(0,None)]
-        # under gen imply discharge only <0
-        elif starter<0:
-            B_bnds = [(None,0)]
-        else:
-            B_bnds = None
+
         opt_B = scipy.optimize.minimize(self.cost_togo, jac= self.cost_togo_derivative,x0=starter, \
                                        args=(X,I,q,*remainingargs),method = "L-BFGS-B",bounds=None)
         return opt_B.x[0]
```

### Comparing `RMCgp-0.0.2/RMC/simulate/CIR.py` & `RMCgp-0.0.22/RMC/simulate/CIR.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/simulate/OU.py` & `RMCgp-0.0.22/RMC/simulate/OU.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/simulate/jacobi.py` & `RMCgp-0.0.22/RMC/simulate/jacobi.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMC/simulate/sim.py` & `RMCgp-0.0.22/RMC/simulate/sim.py`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/RMCgp.egg-info/PKG-INFO` & `RMCgp-0.0.22/RMCgp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RMCgp
-Version: 0.0.2
+Version: 0.0.22
 Summary: RMC for stochastic control.
 Home-page: https://github.com/thihaa2019/RMCgp
 Author: Thiha Aung
 Author-email: taung@ucsb.edu
 Maintainer: Thiha Aung
 Maintainer-email: taung@ucsb.edu
 License: Apache-2.0
```

### Comparing `RMCgp-0.0.2/RMCgp.egg-info/SOURCES.txt` & `RMCgp-0.0.22/RMCgp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RMCgp-0.0.2/setup.py` & `RMCgp-0.0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "GPy>=1.13.0",
     "scikit-learn>=1.3.0",
     "scipy>=1.1.4",
     "matplotlib>=3.8.0"
 ]
 
 setuptools.setup(name='RMCgp',
-                 version='0.0.2',
+                 version='0.0.22',
                  author='Thiha Aung',
                  author_email='taung@ucsb.edu',
                  maintainer='Thiha Aung',
                  maintainer_email='taung@ucsb.edu',
                  description='RMC for stochastic control.',
                  long_description=readme,
                  url='https://github.com/thihaa2019/RMCgp',
```

