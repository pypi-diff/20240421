# Comparing `tmp/dukes-1.3.1.tar.gz` & `tmp/dukes-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dukes-1.3.1.tar", last modified: Mon Apr 15 23:06:04 2024, max compression
+gzip compressed data, was "dukes-1.4.0.tar", last modified: Sun Apr 21 15:25:21 2024, max compression
```

## Comparing `dukes-1.3.1.tar` & `dukes-1.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.918317 dukes-1.3.1/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-28 13:38:04.000000 dukes-1.3.1/LICENSE
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45756 2024-04-15 23:06:04.918317 dukes-1.3.1/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     4767 2024-04-15 01:45:28.000000 dukes-1.3.1/README.md
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1058 2024-04-15 23:04:35.000000 dukes-1.3.1/pyproject.toml
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-04-15 23:06:04.918317 dukes-1.3.1/setup.cfg
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 dukes-1.3.1/setup.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.914317 dukes-1.3.1/src/
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.914317 dukes-1.3.1/src/dukes/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1077 2024-04-14 10:11:57.000000 dukes-1.3.1/src/dukes/__init__.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     3177 2024-04-05 11:34:53.000000 dukes-1.3.1/src/dukes/constant.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.914317 dukes-1.3.1/src/dukes/dat/
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       13 2024-03-28 13:38:04.000000 dukes-1.3.1/src/dukes/dat/__init__.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      911 2024-04-04 16:32:02.000000 dukes-1.3.1/src/dukes/dat/cosmicAgeFit.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      619 2024-03-28 13:38:04.000000 dukes-1.3.1/src/dukes/dat/densityParamFit.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)  1936503 2024-03-28 13:38:04.000000 dukes-1.3.1/src/dukes/dat/galacticAreaDensityFit.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    20184 2024-04-15 22:53:31.000000 dukes-1.3.1/src/dukes/dukesMain.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     7209 2024-04-03 08:17:21.000000 dukes-1.3.1/src/dukes/galDensity.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     2827 2024-04-04 16:29:42.000000 dukes-1.3.1/src/dukes/galMassFunction.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      973 2024-04-01 23:57:07.000000 dukes-1.3.1/src/dukes/sysmsg.py
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    13664 2024-04-15 22:53:47.000000 dukes-1.3.1/src/dukes/utils.py
-drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-15 23:06:04.918317 dukes-1.3.1/src/dukes.egg-info/
--rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    45756 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/PKG-INFO
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      493 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/SOURCES.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/dependency_links.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       41 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/requires.txt
--rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        6 2024-04-15 23:06:04.000000 dukes-1.3.1/src/dukes.egg-info/top_level.txt
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-21 15:25:21.840589 dukes-1.4.0/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    35129 2024-03-28 13:38:04.000000 dukes-1.4.0/LICENSE
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    46064 2024-04-21 15:25:21.840589 dukes-1.4.0/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     5075 2024-04-17 13:35:28.000000 dukes-1.4.0/README.md
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1058 2024-04-21 15:24:51.000000 dukes-1.4.0/pyproject.toml
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       38 2024-04-21 15:25:21.840589 dukes-1.4.0/setup.cfg
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       49 2024-03-28 13:38:04.000000 dukes-1.4.0/setup.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-21 15:25:21.836588 dukes-1.4.0/src/
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-21 15:25:21.840589 dukes-1.4.0/src/dukes/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     1077 2024-04-21 15:24:51.000000 dukes-1.4.0/src/dukes/__init__.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     3177 2024-04-05 11:34:53.000000 dukes-1.4.0/src/dukes/constant.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-21 15:25:21.840589 dukes-1.4.0/src/dukes/dat/
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       13 2024-03-28 13:38:04.000000 dukes-1.4.0/src/dukes/dat/__init__.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      911 2024-04-04 16:32:02.000000 dukes-1.4.0/src/dukes/dat/cosmicAgeFit.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      619 2024-03-28 13:38:04.000000 dukes-1.4.0/src/dukes/dat/densityParamFit.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)  1936503 2024-03-28 13:38:04.000000 dukes-1.4.0/src/dukes/dat/galacticAreaDensityFit.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    20324 2024-04-21 14:37:44.000000 dukes-1.4.0/src/dukes/dukesMain.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     7209 2024-04-03 08:17:21.000000 dukes-1.4.0/src/dukes/galDensity.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)     2827 2024-04-04 16:29:42.000000 dukes-1.4.0/src/dukes/galMassFunction.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      973 2024-04-01 23:57:07.000000 dukes-1.4.0/src/dukes/sysmsg.py
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)    13691 2024-04-21 14:37:05.000000 dukes-1.4.0/src/dukes/utils.py
+drwxrwxr-x   0 yenhsun   (1000) yenhsun   (1000)        0 2024-04-21 15:25:21.840589 dukes-1.4.0/src/dukes.egg-info/
+-rw-r--r--   0 yenhsun   (1000) yenhsun   (1000)    46064 2024-04-21 15:25:21.000000 dukes-1.4.0/src/dukes.egg-info/PKG-INFO
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)      493 2024-04-21 15:25:21.000000 dukes-1.4.0/src/dukes.egg-info/SOURCES.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        1 2024-04-21 15:25:21.000000 dukes-1.4.0/src/dukes.egg-info/dependency_links.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)       41 2024-04-21 15:25:21.000000 dukes-1.4.0/src/dukes.egg-info/requires.txt
+-rw-rw-r--   0 yenhsun   (1000) yenhsun   (1000)        6 2024-04-21 15:25:21.000000 dukes-1.4.0/src/dukes.egg-info/top_level.txt
```

### Comparing `dukes-1.3.1/LICENSE` & `dukes-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dukes-1.3.1/PKG-INFO` & `dukes-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukes
-Version: 1.3.1
+Version: 1.4.0
 Summary: This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,20 +682,26 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: vegas>=6.0.1
 
+[![Python](https://img.shields.io/badge/python-3.8-blue.svg)](https://python.org)
+[![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)](https://choosealicense.com/licenses/gpl-3.0/)
+[![ArXiv](https://img.shields.io/badge/arXiv-2404.08528-yellowgreen.svg)](https://arxiv.org/abs/2404.08528) 
+
+
 # dukes: *D*iff*U*se-boosted dar*K* matt*E*r by *S*upernova neutrinos
 
 
 `dukes` is a pyhon package for evaluating the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe based on [arXiv:2404.08528](https://arxiv.org/abs/2404.08528).
 It also supports an *experimental* feature that implements particle-model-dependent differential cross sections for DM-neutrino and DM-electron.
 
+
 ### Citation
 
 If you use this package or part of the code in your research, please cite the following:
 
 1. Yen-Hsun Lin and Meng-Ru Wu, *Echoes of darkness: Supernova-neutrino-boosted dark matter from all galaxies*, arXiv:2404.08528
 2. `dukes`: https://github.com/yenhsunlin/dukes
```

### Comparing `dukes-1.3.1/README.md` & `dukes-1.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+[![Python](https://img.shields.io/badge/python-3.8-blue.svg)](https://python.org)
+[![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)](https://choosealicense.com/licenses/gpl-3.0/)
+[![ArXiv](https://img.shields.io/badge/arXiv-2404.08528-yellowgreen.svg)](https://arxiv.org/abs/2404.08528) 
+
+
 # dukes: *D*iff*U*se-boosted dar*K* matt*E*r by *S*upernova neutrinos
 
 
 `dukes` is a pyhon package for evaluating the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe based on [arXiv:2404.08528](https://arxiv.org/abs/2404.08528).
 It also supports an *experimental* feature that implements particle-model-dependent differential cross sections for DM-neutrino and DM-electron.
 
+
 ### Citation
 
 If you use this package or part of the code in your research, please cite the following:
 
 1. Yen-Hsun Lin and Meng-Ru Wu, *Echoes of darkness: Supernova-neutrino-boosted dark matter from all galaxies*, arXiv:2404.08528
 2. `dukes`: https://github.com/yenhsunlin/dukes
```

### Comparing `dukes-1.3.1/pyproject.toml` & `dukes-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dukes"
-version = "1.3.1"
+version = "1.4.0"
 description = "This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe"
 readme = "README.md"
 authors = [{ name = "Yen-Hsun Lin", email = "yenhsun@phys.ncku.edu.tw" }]
 license = { file = "LICENSE" }
 dependencies = [
     "numpy >= 1.20.0",
     "scipy >= 1.10.0",
     "vegas >= 6.0.1",]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/yenhsunlin/dukes"
 
 [tool.bumpver]
-current_version = "1.3.0"
+current_version = "1.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `dukes-1.3.1/src/dukes/__init__.py` & `dukes-1.4.0/src/dukes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 __name__         = 'dukes'
-__version__      = '1.3.0'
+__version__      = '1.4.0'
 __description__  = 'This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe'
 __author__       = 'Yen-Hsun Lin'
 __email__        = 'yenhsun@phys.ncku.edu.tw'
 __url__          = 'https://github.com/yenhsunlin/dukes'
 __license__      = 'GNU GPL-3.0'
 
 from .dukesMain import *
```

### Comparing `dukes-1.3.1/src/dukes/constant.py` & `dukes-1.4.0/src/dukes/constant.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.1/src/dukes/dat/cosmicAgeFit.py` & `dukes-1.4.0/src/dukes/dat/cosmicAgeFit.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.1/src/dukes/dat/densityParamFit.py` & `dukes-1.4.0/src/dukes/dat/densityParamFit.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.1/src/dukes/dat/galacticAreaDensityFit.py` & `dukes-1.4.0/src/dukes/dat/galacticAreaDensityFit.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.1/src/dukes/dukesMain.py` & `dukes-1.4.0/src/dukes/dukesMain.py`

 * *Files 3% similar despite different names*

```diff
@@ -415,26 +415,28 @@
 #    """
 #    # this is energy-independent cross section
 #    # divided by 4*np implying isotropic in CM frame
 #    return print('Academics is a place full of PUA!')
 #    return 1e-35
 
 
-def supernovaNuFlux(Ev,l) -> float:
+def supernovaNuFlux(Ev,l,is_density=False) -> float:
     """
     SN neutrino flux after propagating a distance l
     
     Input
     ------
     Ev: SN neutrino energy, MeV
     l: propagation distance, kpc
+    is_density: output neutrino number denisty within shell
     
     Output
     ------
-    flux: #/Ev/cm^2/s
+    flux: #/Ev/cm^2/s, if is_density is False
+    number density: #/Ev/cm^3, if is_density is True
     """
     Lv = constant.Lv*constant.erg2MeV
     l = l*constant.kpc2cm
     
     #Fermi-Dirac distribution
     def _fv(Ev,Tv):
         exponent = Ev/Tv - 3
@@ -447,15 +449,21 @@
     # distributions for nu_e and anti-nu_e
     nue_dist = _fv(Ev,2.76)/11
     nueb_dist = _fv(Ev,4.01)/16
     # distributions for the rest 4 species
     nux_dist = _fv(Ev,6.26)/25
     
     L = Lv/(4*_np.pi*l**2)
-    return L*(nue_dist + nueb_dist + 4*nux_dist)
+    flux = L*(nue_dist + nueb_dist + 4*nux_dist)
+    if is_density is False:
+        return flux
+    elif is_density is True:
+        return flux/constant.c
+    else:
+        raise FlagError('Flag \'is_density\' must be a boolean.')
 
 
 
 # ----- Diffuse boosted dark matter -----
 
 class dbdmSpectrum(constant):
     
@@ -473,64 +481,63 @@
             vx = vBDM(Tx,mx)  #  
             nx = dmNumberDensity(r,mx,MG,is_spike,sigv,tBH,rhosMW,rsMW,eta)
             dsigma0 = constant.sigma0  # differential DM-nu cross section in CM frame, cm^2/sr
             return l**2*_np.sin(theta)*_np.sin(thetaCM)*nx*dsigma0*supernovaNuFlux(Ev,l)*(dEvdTx*vx)
         else:
             return 0
     
-    def _dbdmSpectrum(self,z,m,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,rhosMW,rsMW,eta) -> float:
+    def _dbdmSpectrum(self,z,MG,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,rhosMW,rsMW,eta) -> float:
         """
         DBDM spectrume yielded by SN at arbitrary position R
         """
         Txp = (1 + z)*Tx 
         tBH = cosmicAgeFit(z)*1e9 # convert to years
         if Txp < 150:  # discard the BDM signature if it requires Ev > 150 MeV at z 
-            MG = 10**m
-            return MG*dnG(m,z)*rhoDotSFR(z)*self._diffSpectrum(Txp,mx,
-                                                               MG,R,l,theta,
-                                                               thetaCM,
-                                                               is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)
+            m = _np.log10(MG)
+            return dnG(m,z)*rhoDotSFR(z)*self._diffSpectrum(Txp,mx,
+                                                            MG,R,l,theta,
+                                                            thetaCM,
+                                                            is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)
         else:
             return 0
         
-    def _dbdmSpectrumWeighted(self,z,m,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,rhosMW,rsMW,eta,usefit) -> float:
+    def _dbdmSpectrumWeighted(self,z,MG,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,rhosMW,rsMW,eta,usefit) -> float:
         """
         DBDM spectrume yielded by SN at position R weighted by galactic baryonic distribution
         """
         Txp = (1 + z)*Tx 
         tBH = cosmicAgeFit(z)*1e9 # convert to years
         if Txp < 150:  # discard the BDM signature if it requires Ev > 130 MeV at z
-            MG = 10**m
             # adopt fitting data for galactic area density?
+            m = _np.log10(MG)
             if usefit is True:
                 galArealDensity = galacticAreaDensityFit((R,m))
             elif usefit is False:
                 galArealDensity = galacticAreaDensity(R,zRange=[-10,10],MG=MG)
             else:
                 raise FlagError('Flag \'usefit\' must be a boolean.')
-            
             return (2*_np.pi*R)*rhoDotSFR(z)*galArealDensity*dnG(m,z)*self._diffSpectrum(Txp,mx,
                                                                                          MG,R,l,theta,
                                                                                          thetaCM,
-                                                                                         is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)    
+                                                                                         is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)/MG    
         else:
             return 0
     
-    def __call__(self,z,m,Tx,mx,R,l,theta,thetaCM,is_spike,is_weighted,sigv,rhosMW,rsMW,eta,usefit):
+    def __call__(self,z,MG,Tx,mx,R,l,theta,thetaCM,is_spike,is_weighted,sigv,rhosMW,rsMW,eta,usefit):
         if is_weighted is True:
-            return self._dbdmSpectrumWeighted(z,m,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,rhosMW,rsMW,eta,usefit)
+            return self._dbdmSpectrumWeighted(z,MG,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,rhosMW,rsMW,eta,usefit)
         elif is_weighted is False:
-            return self._dbdmSpectrum(z,m,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,rhosMW,rsMW,eta)
+            return self._dbdmSpectrum(z,MG,Tx,mx,R,l,theta,thetaCM,is_spike,sigv,rhosMW,rsMW,eta)
         else:
             raise FlagError('Flag \'is_weighted\' must be a boolean.')
 
 
-def flux(Tx,mx,                                                           \
-         R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,      \
-         sigv=None,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True, \
+def flux(Tx,mx,
+         R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,
+         sigv=None,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True,
          nitn=10,neval=50000):
     """
     DBDM flux for given (Tx,mx) assuming isotropic and energy-independent
     differential DM-nuetrino cross section in CM frame with the value
     1e-35/4/pi cm^2/std
     
     In
@@ -557,33 +564,33 @@
     Flux: per MeV per cm^2 per second
     """
     preFactor = constant.MagicalNumber  # constant.D_H0*0.017/constant.Mmw/rhoDotSFR(0)/1e6/constant.kpc2cm**2/constant.year2Seconds
                                         # 0.017: SN in MW per year; 1e6: converting Mpc^2 to kpc^2
     lmax = Rmax + rmax
     spectrum  = dbdmSpectrum()
     if is_average is True:
-        integrator = _vegas.Integrator([[0,8],[6,12],[0,Rmax],[0,lmax],[0,_np.pi],[0,_np.pi]]) #(z,m,R,l,theta,thetaCM)
-        result = integrator(lambda x: spectrum(z=x[0],m=x[1],Tx=Tx,mx=mx,R=x[2],l=x[3],theta=x[4],thetaCM=x[5], \
-                                               is_spike=is_spike,is_weighted=is_average,sigv=sigv,      \
+        integrator = _vegas.Integrator([[0,8],[1e6,1e12],[0,Rmax],[0,lmax],[0,_np.pi],[0,_np.pi]]) #(z,m,R,l,theta,thetaCM)
+        result = integrator(lambda x: spectrum(z=x[0],MG=x[1],Tx=Tx,mx=mx,R=x[2],l=x[3],theta=x[4],thetaCM=x[5],
+                                               is_spike=is_spike,is_weighted=is_average,sigv=sigv,
                                                rhosMW=rhosMW,rsMW=rsMW,eta=eta,usefit=usefit),nitn=nitn,neval=neval).mean
         flux = 4*_np.pi**2*tau*result*constant.kpc2cm**3*vBDM(Tx,mx)*preFactor
     elif is_average is False:
-        integrator = _vegas.Integrator([[0,8],[6,12],[0,lmax],[0,_np.pi],[0,_np.pi]]) #(z,m,l,theta,thetaCM)
-        result = integrator(lambda x: spectrum(z=x[0],m=x[1],Tx=Tx,mx=mx,R=R,l=x[2],theta=x[3],thetaCM=x[4],    \
-                                               is_spike=is_spike,is_weighted=is_average,sigv=sigv,      \
+        integrator = _vegas.Integrator([[0,8],[1e6,1e12],[0,lmax],[0,_np.pi],[0,_np.pi]]) #(z,m,l,theta,thetaCM)
+        result = integrator(lambda x: spectrum(z=x[0],MG=x[1],Tx=Tx,mx=mx,R=R,l=x[2],theta=x[3],thetaCM=x[4],
+                                               is_spike=is_spike,is_weighted=is_average,sigv=sigv,
                                                rhosMW=rhosMW,rsMW=rsMW,eta=eta,usefit=usefit),nitn=nitn,neval=neval).mean
         flux = 4*_np.pi**2*tau*result*constant.kpc2cm**3*vBDM(Tx,mx)*preFactor
     else:
         raise FlagError('Flag \'is_average\' must be a boolean.')
     return flux
 
 
-def event(mx,                                                                          \
-          TxRange=[5,30],R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,  \
-          sigv=None,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True,             \
+def event(mx,
+          TxRange=[5,30],R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,
+          sigv=None,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True,
           nitn=10,neval=50000):
     """
     DBDM event per electron per second for given mx assuming isotropic
     and energy-independent differential DM-nuetrino cross section in CM
     frame with the value 1e-35/4/pi cm^2/std. The total DM-electron cross
     section is assumed 1e-35 cm^2
     
@@ -612,23 +619,23 @@
     Event: per electron per second
     """
     preFactor = constant.MagicalNumber     # constant.D_H0*0.017/constant.Mmw/rhoDotSFR(0)/1e6/constant.kpc2cm**2/constant.year2Seconds
     preFactor *= constant.sigma0*4*_np.pi  # multiplying total DM-electron cross section
     lmax = Rmax + rmax
     spectrum  = dbdmSpectrum()
     if is_average is True:
-        integrator = _vegas.Integrator([[0,8],[6,12],[0,Rmax],[0,lmax],[0,_np.pi],[0,_np.pi],TxRange]) #(z,m,R,l,theta,thetaCM)
-        result = integrator(lambda x: spectrum(z=x[0],m=x[1],Tx=x[6],mx=mx,R=x[2],l=x[3],theta=x[4],thetaCM=x[5],  \
-                                               is_spike=is_spike,is_weighted=is_average,sigv=sigv,         \
-                                               rhosMW=rhosMW,rsMW=rsMW,eta=eta,usefit=usefit)*vBDM(Tx=x[6],mx=mx), \
+        integrator = _vegas.Integrator([[0,8],[1e6,1e12],[0,Rmax],[0,lmax],[0,_np.pi],[0,_np.pi],TxRange]) #(z,m,R,l,theta,thetaCM)
+        result = integrator(lambda x: spectrum(z=x[0],MG=x[1],Tx=x[6],mx=mx,R=x[2],l=x[3],theta=x[4],thetaCM=x[5],
+                                               is_spike=is_spike,is_weighted=is_average,sigv=sigv,
+                                               rhosMW=rhosMW,rsMW=rsMW,eta=eta,usefit=usefit)*vBDM(Tx=x[6],mx=mx),
                             nitn=nitn,neval=neval).mean
         event = 4*_np.pi**2*tau*result*constant.kpc2cm**3*preFactor
     elif is_average is False:
-        integrator = _vegas.Integrator([[0,8],[6,12],[0,lmax],[0,_np.pi],[0,_np.pi],TxRange]) #(z,m,l,theta,thetaCM,Tx)
-        result = integrator(lambda x: spectrum(z=x[0],m=x[1],Tx=x[5],mx=mx,R=R,l=x[2],theta=x[3],thetaCM=x[4],     \
-                                               is_spike=is_spike,is_weighted=is_average,sigv=sigv,         \
-                                               rhosMW=rhosMW,rsMW=rsMW,eta=eta,usefit=usefit)*vBDM(Tx=x[5],mx=mx), \
+        integrator = _vegas.Integrator([[0,8],[1e6,1e12],[0,lmax],[0,_np.pi],[0,_np.pi],TxRange]) #(z,m,l,theta,thetaCM,Tx)
+        result = integrator(lambda x: spectrum(z=x[0],MG=x[1],Tx=x[5],mx=mx,R=R,l=x[2],theta=x[3],thetaCM=x[4],
+                                               is_spike=is_spike,is_weighted=is_average,sigv=sigv,
+                                               rhosMW=rhosMW,rsMW=rsMW,eta=eta,usefit=usefit)*vBDM(Tx=x[5],mx=mx),
                             nitn=nitn,neval=neval).mean
         event = 4*_np.pi**2*tau*result*constant.kpc2cm**3*preFactor
     else:
         raise FlagError('Flag \'is_average\' must be a boolean.')
     return event
```

### Comparing `dukes-1.3.1/src/dukes/galDensity.py` & `dukes-1.4.0/src/dukes/galDensity.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.1/src/dukes/galMassFunction.py` & `dukes-1.4.0/src/dukes/galMassFunction.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.1/src/dukes/sysmsg.py` & `dukes-1.4.0/src/dukes/sysmsg.py`

 * *Files identical despite different names*

### Comparing `dukes-1.3.1/src/dukes/utils.py` & `dukes-1.4.0/src/dukes/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,49 +143,49 @@
             vx = vBDM(Tx,mx)  #  
             nx = dmNumberDensity(r,mx,MG,is_spike,sigv,tBH,rhosMW,rsMW,eta)
             dsigma0 = self.dsigmaNu(Ev,mx,thetaCM_vx) #self.dsigmaNu(Ev,mx,thetaCM_vx)
             return l**2*_np.sin(theta)*_np.sin(thetaCM_vx)*nx*dsigma0*supernovaNuFlux(Ev,l)*(dEvdTx*vx)
         else:
             return 0
     
-    def _dbdmSpectrum(self,z,m,Tx,mx,R,l,theta,thetaCM_vx,is_spike,sigv,rhosMW,rsMW,eta) -> float:
+    def _dbdmSpectrum(self,z,MG,Tx,mx,R,l,theta,thetaCM_vx,is_spike,sigv,rhosMW,rsMW,eta) -> float:
         """
         DBDM spectrume yielded by SN at arbitrary position R
         """
         Txp = (1 + z)*Tx
         tBH = cosmicAgeFit(z)*1e9 # convert to years 
         if Txp < 150:  # discard the BDM signature if it requires Ev > 150 MeV at z 
-            MG = 10**m
-            return MG*dnG(m,z)*rhoDotSFR(z)*self._diffSpectrum(Txp,mx,
-                                                               MG,R,l,theta,
-                                                               thetaCM_vx,
-                                                               is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)
+            m = _np.log10(MG)
+            return dnG(m,z)*rhoDotSFR(z)*self._diffSpectrum(Txp,mx,
+                                                            MG,R,l,theta,
+                                                            thetaCM_vx,
+                                                            is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)
         else:
             return 0
         
-    def _dbdmSpectrumWeighted(self,z,m,Tx,mx,R,l,theta,thetaCM_vx,is_spike,sigv,rhosMW,rsMW,eta,usefit) -> float:
+    def _dbdmSpectrumWeighted(self,z,MG,Tx,mx,R,l,theta,thetaCM_vx,is_spike,sigv,rhosMW,rsMW,eta,usefit) -> float:
         """
         DBDM spectrume yielded by SN at position R weighted by galactic baryonic distribution
         """
         Txp = (1 + z)*Tx
         tBH = cosmicAgeFit(z)*1e9 # convert to years 
         if Txp < 150:  # discard the BDM signature if it requires Ev > 150 MeV at z
-            MG = 10**m
             # adopt fitting data for galactic area density?
+            m = _np.log10(MG)
             if usefit is True:
                 galArealDensity = galacticAreaDensityFit((R,m))
             elif usefit is False:
                 galArealDensity = galacticAreaDensity(R,zRange=[-10,10],MG=MG)
             else:
                 raise FlagError('Flag \'usefit\' must be a boolean.')
             
             return (2*_np.pi*R)*rhoDotSFR(z)*galArealDensity*dnG(m,z)*self._diffSpectrum(Txp,mx,
                                                                                          MG,R,l,theta,
                                                                                          thetaCM_vx, 
-                                                                                         is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)
+                                                                                         is_spike,sigv,tBH,rhosMW,rsMW,eta)/_E(z)/MG
         else:
             return 0
 
     def flux(self,Tx,mx,                                                          
              R=0,Rmax=30,rmax=30,tau=10,is_spike=True,is_average=True,      
              sigv=None,rhosMW=184,rsMW=24.42,eta=24.3856,usefit=True, 
              nitn=10,neval=50000) -> float:
@@ -217,22 +217,22 @@
         ------
         Flux: per MeV per cm^2 per second
         """
         preFactor = self.MagicalNumber  # constant.D_H0*0.017/constant.Mmw/rhoDotSFR(0)/1e6/constant.kpc2cm**2/constant.year2Seconds
                                         # 0.017: SN in MW per year; 1e6: converting Mpc^2 to kpc^2
         lmax = Rmax + rmax
         if is_average is True:
-            integrator = _vegas.Integrator([[0,8],[6,12],[0,Rmax],[0,lmax],[0,_np.pi],[0,_np.pi]]) #(z,m,R,l,theta,thetaCM_vx)
-            result = integrator(lambda x: self._dbdmSpectrumWeighted(z=x[0],m=x[1],Tx=Tx,mx=mx,R=x[2],l=x[3],theta=x[4],thetaCM_vx=x[5],    
+            integrator = _vegas.Integrator([[0,8],[1e6,1e12],[0,Rmax],[0,lmax],[0,_np.pi],[0,_np.pi]]) #(z,m,R,l,theta,thetaCM_vx)
+            result = integrator(lambda x: self._dbdmSpectrumWeighted(z=x[0],MG=x[1],Tx=Tx,mx=mx,R=x[2],l=x[3],theta=x[4],thetaCM_vx=x[5],    
                                                                      is_spike=is_spike,sigv=sigv,rhosMW=rhosMW,rsMW=rsMW,eta=eta,usefit=usefit),
                                 nitn=nitn,neval=neval).mean
             flux = 4*_np.pi**2*tau*result*self.kpc2cm**3*vBDM(Tx,mx)*preFactor
         elif is_average is False:
-            integrator = _vegas.Integrator([[0,8],[6,12],[0,lmax],[0,_np.pi],[0,_np.pi]]) #(z,m,l,theta,thetaCM_vx)
-            result = integrator(lambda x: self._dbdmSpectrum(z=x[0],m=x[1],Tx=Tx,mx=mx,R=R,l=x[2],theta=x[3],thetaCM_vx=x[4], 
+            integrator = _vegas.Integrator([[0,8],[1e6,1e12],[0,lmax],[0,_np.pi],[0,_np.pi]]) #(z,m,l,theta,thetaCM_vx)
+            result = integrator(lambda x: self._dbdmSpectrum(z=x[0],MG=x[1],Tx=Tx,mx=mx,R=R,l=x[2],theta=x[3],thetaCM_vx=x[4], 
                                                              is_spike=is_spike,sigv=sigv,rhosMW=rhosMW,rsMW=rsMW,eta=eta),      
                                 nitn=nitn,neval=neval).mean
             flux = 4*_np.pi**2*tau*result*self.kpc2cm**3*vBDM(Tx,mx)*preFactor
         else:
             raise FlagError('Flag \'is_average\' must be a boolean.')
         return flux
 
@@ -267,23 +267,23 @@
         Out
         ------
         Event: per electron per second
         """
         preFactor = self.MagicalNumber  # constant.D_H0*0.017/constant.Mmw/rhoDotSFR(0)/1e6/constant.kpc2cm**2/constant.year2Seconds
         lmax = Rmax + rmax
         if is_average is True:
-            integrator = _vegas.Integrator([[0,8],[6,12],[0,Rmax],[0,lmax],[0,_np.pi],[0,_np.pi],[0,_np.pi],TxRange]) #(z,m,R,l,theta,thetaCM_vx,thetaCM_xe,Tx)
-            result = integrator(lambda x: self._dbdmSpectrumWeighted(z=x[0],m=x[1],Tx=x[7],mx=mx,R=x[2],l=x[3],theta=x[4],thetaCM_vx=x[5],  
+            integrator = _vegas.Integrator([[0,8],[1e6,1e12],[0,Rmax],[0,lmax],[0,_np.pi],[0,_np.pi],[0,_np.pi],TxRange]) #(z,m,R,l,theta,thetaCM_vx,thetaCM_xe,Tx)
+            result = integrator(lambda x: self._dbdmSpectrumWeighted(z=x[0],MG=x[1],Tx=x[7],mx=mx,R=x[2],l=x[3],theta=x[4],thetaCM_vx=x[5],  
                                                is_spike=is_spike,sigv=sigv,         
                                                rhosMW=rhosMW,rsMW=rsMW,eta=eta,usefit=usefit)*vBDM(Tx=x[7],mx=mx)*self.dsigmaE(x[7],mx,x[6])*_np.sin(x[6]), 
                             nitn=nitn,neval=neval).mean
             event = 4*_np.pi**2*tau*result*self.kpc2cm**3*preFactor*(2*_np.pi)  # the last 2pi is due to diff cross section for DM-e is independent of azimuthal angle 
         elif is_average is False:
-            integrator = _vegas.Integrator([[0,8],[6,12],[0,lmax],[0,_np.pi],[0,_np.pi],[0,_np.pi],TxRange]) #(z,m,l,theta,thetaCM,thetaCM_xe,Tx)
-            result = integrator(lambda x: self._dbdmSpectrum(z=x[0],m=x[1],Tx=x[6],mx=mx,R=R,l=x[2],theta=x[3],thetaCM_vx=x[4],     
+            integrator = _vegas.Integrator([[0,8],[1e6,1e12],[0,lmax],[0,_np.pi],[0,_np.pi],[0,_np.pi],TxRange]) #(z,m,l,theta,thetaCM,thetaCM_xe,Tx)
+            result = integrator(lambda x: self._dbdmSpectrum(z=x[0],MG=x[1],Tx=x[6],mx=mx,R=R,l=x[2],theta=x[3],thetaCM_vx=x[4],     
                                                is_spike=is_spike,sigv=sigv,         
                                                rhosMW=rhosMW,rsMW=rsMW,eta=eta)*vBDM(Tx=x[6],mx=mx)*self.dsigmaE(x[6],mx,x[5])*_np.sin(x[5]), 
                                 nitn=nitn,neval=neval).mean
             event = 4*_np.pi**2*tau*result*self.kpc2cm**3*preFactor*(2*_np.pi)  # the last 2pi is due to diff cross section for DM-e is independent of azimuthal angle 
         else:
             raise FlagError('Flag \'is_average\' must be a boolean.')
         return event
```

### Comparing `dukes-1.3.1/src/dukes.egg-info/PKG-INFO` & `dukes-1.4.0/src/dukes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dukes
-Version: 1.3.1
+Version: 1.4.0
 Summary: This package evaluates the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe
 Author-email: Yen-Hsun Lin <yenhsun@phys.ncku.edu.tw>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,20 +682,26 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: vegas>=6.0.1
 
+[![Python](https://img.shields.io/badge/python-3.8-blue.svg)](https://python.org)
+[![License](https://img.shields.io/badge/License-GPL_3.0-blue.svg)](https://choosealicense.com/licenses/gpl-3.0/)
+[![ArXiv](https://img.shields.io/badge/arXiv-2404.08528-yellowgreen.svg)](https://arxiv.org/abs/2404.08528) 
+
+
 # dukes: *D*iff*U*se-boosted dar*K* matt*E*r by *S*upernova neutrinos
 
 
 `dukes` is a pyhon package for evaluating the signatures of diffuse boosted dark matter by supernova neutrinos in the early Universe based on [arXiv:2404.08528](https://arxiv.org/abs/2404.08528).
 It also supports an *experimental* feature that implements particle-model-dependent differential cross sections for DM-neutrino and DM-electron.
 
+
 ### Citation
 
 If you use this package or part of the code in your research, please cite the following:
 
 1. Yen-Hsun Lin and Meng-Ru Wu, *Echoes of darkness: Supernova-neutrino-boosted dark matter from all galaxies*, arXiv:2404.08528
 2. `dukes`: https://github.com/yenhsunlin/dukes
```

