# Comparing `tmp/jsmfsb-0.0.3.tar.gz` & `tmp/jsmfsb-0.0.4.tar.gz`

## Comparing `jsmfsb-0.0.3.tar` & `jsmfsb-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,30 @@
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/.readthedocs.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/Makefile
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/demos/lv.pdf
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/demos/lv.py
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/demos/lvH.pdf
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/demos/shbuild.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/Makefile
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/conf.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/make.bat
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/requirements.txt
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/source/jsmfsb.rst
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/docs/source/modules.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/models.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/sim.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/smfsbSbml.py
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/src/jsmfsb/spn.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/tests/test_sim.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/tests/test_spn.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/LICENSE
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/README.md
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 jsmfsb-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/Makefile
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/Makefile
+-rw-r--r--   0        0        0    12569 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/lv.pdf
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/lv.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/lv.txt
+-rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/lvH.pdf
+-rw-r--r--   0        0        0    11053 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/shbuild.pdf
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/shbuild.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/shbuild.txt
+-rw-r--r--   0        0        0     9250 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/demos/shbuildH.pdf
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/Makefile
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/conf.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/make.bat
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/requirements.txt
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/source/jsmfsb.rst
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/docs/source/modules.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/models.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/sim.py
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/smfsbSbml.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/src/jsmfsb/spn.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/tests/test_sim.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/tests/test_spn.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/README.md
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 jsmfsb-0.0.4/PKG-INFO
```

### Comparing `jsmfsb-0.0.3/.readthedocs.yaml` & `jsmfsb-0.0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/demos/lv.pdf` & `jsmfsb-0.0.4/demos/lv.pdf`

 * *Files 12% similar despite different names*

#### Comparing `jsmfsb-0.0.3/demos/lv.pdf` & `jsmfsb-0.0.4/demos/lv.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240419190531+01'00'"
+CreationDate: "D:20240420231036+01'00'"
 Creator: 'Matplotlib v3.8.4, https://matplotlib.org'
 Producer: 'Matplotlib pdf backend v3.8.4'
```

#### pdftotext {} -

```diff
@@ -1,15 +1,20 @@
+450
+
 Prey
 Predator
+
 400
+350
 300
+250
 200
+150
 100
-0
-
+50
 0
 
 50
 
 100
 
 150
```

### Comparing `jsmfsb-0.0.3/demos/lv.py` & `jsmfsb-0.0.4/demos/lv.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/demos/lvH.pdf` & `jsmfsb-0.0.4/demos/lvH.pdf`

 * *Files 2% similar despite different names*

#### Comparing `jsmfsb-0.0.3/demos/lvH.pdf` & `jsmfsb-0.0.4/demos/lvH.pdf`

 * *Document info*

```diff
@@ -1,3 +1,3 @@
-CreationDate: "D:20240419190537+01'00'"
+CreationDate: "D:20240420231042+01'00'"
 Creator: 'Matplotlib v3.8.4, https://matplotlib.org'
 Producer: 'Matplotlib pdf backend v3.8.4'
```

### Comparing `jsmfsb-0.0.3/docs/Makefile` & `jsmfsb-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/docs/conf.py` & `jsmfsb-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/docs/make.bat` & `jsmfsb-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/docs/source/jsmfsb.rst` & `jsmfsb-0.0.4/docs/source/jsmfsb.rst`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/src/jsmfsb/models.py` & `jsmfsb-0.0.4/src/jsmfsb/models.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/src/jsmfsb/sim.py` & `jsmfsb-0.0.4/src/jsmfsb/sim.py`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/src/jsmfsb/smfsbSbml.py` & `jsmfsb-0.0.4/src/jsmfsb/smfsbSbml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # smfsbSbml.py
 # Import SBML models into an smfsb Spn
 
 import libsbml
 import sys
 from jsmfsb import Spn
-import numpy as np
+import jax.numpy as jnp
 from sbmlsh import mod2sbml
 
 
 def mod2Spn(filename, verb=False):
     """Convert an SBML-shorthand model into a Spn object
 
     Read a file containing a model in SBML-shorthand and convert into
@@ -169,32 +169,32 @@
         gpd[param.getId()] = param.getValue()
     if (verb):
         print(gpd)
     # Reactions
     nr = m.getNumReactions()
     if (verb):
         print(str(nr)+" reactions")
-    pre = np.zeros((nr, ns))
-    post = np.zeros((nr, ns))
+    pre = jnp.zeros((nr, ns))
+    post = jnp.zeros((nr, ns))
     rn = []
     kl = []
     lpl = []
     for i in range(nr):
         r = m.getReaction(i)
         rn += [r.getId()]
         nPre = r.getNumReactants()
         for j in range(nPre):
             sr = r.getReactant(j)
             sto = sr.getStoichiometry()
-            pre[i, nl.index(sr.getSpecies())] = sto
+            pre = pre.at[i, nl.index(sr.getSpecies())].set(sto)
         nPost = r.getNumProducts()
         for j in range(nPost):
             sr = r.getProduct(j)
             sto = sr.getStoichiometry()
-            post[i, nl.index(sr.getSpecies())] = sto
+            post= post.at[i, nl.index(sr.getSpecies())].set(sto)
         kli = r.getKineticLaw()
         kl += [libsbml.formulaToString(kli.getMath())]
         nlp = kli.getNumLocalParameters()
         lpd = {}
         for j in range(nlp):
             param = kli.getLocalParameter(j)
             lpd[param.getId()] = param.getValue()
@@ -205,20 +205,20 @@
         print(pre)
         print("Post:")
         print(post)
         print(kl)
         print(lpl)
     gpd.update(cd)
     def haz(x, t):
-        h = np.zeros(nr)
+        h = jnp.zeros(nr)
         xd = dict(zip(nl, x))
         glob = gpd.copy()
         glob.update(xd)
         for i in range(nr):
-            h[i] = eval(kl[i], glob, lpl[i])
+            h = h.at[i].set(eval(kl[i], glob, lpl[i]))
         return(h)
     spn = Spn(nl, rn, pre, post, haz, ml)
     spn.comp = cd
     spn.gp = gpd
     spn.kl = kl
     spn.lp = lpl
     return(spn)
```

### Comparing `jsmfsb-0.0.3/src/jsmfsb/spn.py` & `jsmfsb-0.0.4/src/jsmfsb/spn.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,32 +97,31 @@
         >>> stepLv = lv.stepGillespie()
         >>> stepLv(jax.random.key(42), lv.m, 0, 1)
         """
         S = (self.post - self.pre).T
         u, v = S.shape
         @jit
         def advance(state):
-            key, x, t = state
+            key, xo, x, t = state
             h = self.h(x, t)
             h0 = jnp.sum(h)
             key, k1, k2 = jax.random.split(key, 3)
             t = jnp.where(h0 > maxHaz, 1e90, t)
             t = jnp.where(h0 < minHaz, 1e90,
                           t + jax.random.exponential(k1)/h0)
             j = jax.random.choice(k2, v, p=h/h0)
-            x = jnp.add(x, S[:,j])
-            return (key, x, t)
+            xn = jnp.add(x, S[:,j])
+            return (key, x, xn, t)
         @jit
         def step(key, x0, t0, deltat):
             t = t0
             x = x0
             termt = t0 + deltat
-            # TODO: this isn't quite right, as we want the final state _before_ termt
-            key, x, t = jl.while_loop(lambda state: state[2] < termt,
-                                      advance, (key, x, t))
+            key, x, xn, t = jl.while_loop(lambda state: state[3] < termt,
+                                      advance, (key, x, x, t))
             return x
         return step
 
 
     def stepCLE(self, dt = 0.01):
         """Create a function for advancing the state of an SPN by using a simple
         Euler-Maruyama integration method for the associated CLE
```

### Comparing `jsmfsb-0.0.3/.gitignore` & `jsmfsb-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/LICENSE` & `jsmfsb-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/README.md` & `jsmfsb-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jsmfsb-0.0.3/pyproject.toml` & `jsmfsb-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jsmfsb"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Darren Wilkinson", email="darrenjwilkinson@btinternet.com" },
 ]
 description = "Python+JAX code relating to the textbook, Stochastic modelling for systems biology, third edition"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `jsmfsb-0.0.3/PKG-INFO` & `jsmfsb-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jsmfsb
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python+JAX code relating to the textbook, Stochastic modelling for systems biology, third edition
 Project-URL: Homepage, https://github.com/darrenjw/jax-smfsb
 Project-URL: Documentation, https://jax-smfsb.readthedocs.io/
 Project-URL: Issues, https://github.com/darrenjw/jax-smfsb/issues
 Author-email: Darren Wilkinson <darrenjwilkinson@btinternet.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
```

