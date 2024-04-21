# Comparing `tmp/pyechelle-0.3.6.tar.gz` & `tmp/pyechelle-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyechelle-0.3.6.tar", max compression
+gzip compressed data, was "pyechelle-0.3.7.tar", max compression
```

## Comparing `pyechelle-0.3.6.tar` & `pyechelle-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1086 2023-05-11 10:17:14.118690 pyechelle-0.3.6/LICENSE
--rw-r--r--   0        0        0       84 2023-06-06 12:23:50.718422 pyechelle-0.3.6/pyechelle/__init__.py
--rw-r--r--   0        0        0     3422 2023-07-08 10:14:07.560615 pyechelle-0.3.6/pyechelle/benchmark.py
--rw-r--r--   0        0        0     2335 2023-05-11 10:17:14.333485 pyechelle-0.3.6/pyechelle/CCD.py
--rw-r--r--   0        0        0     7239 2023-06-06 12:23:50.718422 pyechelle-0.3.6/pyechelle/efficiency.py
--rw-r--r--   0        0        0     5675 2023-05-11 10:17:14.334635 pyechelle-0.3.6/pyechelle/model_viewer.py
--rw-r--r--   0        0        0       99 2023-07-08 10:14:07.561660 pyechelle-0.3.6/pyechelle/models/available_models.txt
--rw-r--r--   0        0        0     9593 2023-05-11 10:17:14.336183 pyechelle-0.3.6/pyechelle/optics.py
--rw-r--r--   0        0        0     2305 2023-05-11 10:17:14.336415 pyechelle-0.3.6/pyechelle/randomgen.py
--rw-r--r--   0        0        0     9794 2023-05-11 10:17:14.336415 pyechelle-0.3.6/pyechelle/raytrace_cuda.py
--rw-r--r--   0        0        0     8551 2023-05-11 10:17:14.336415 pyechelle-0.3.6/pyechelle/raytracing.py
--rw-r--r--   0        0        0    31886 2023-06-06 12:23:50.722422 pyechelle-0.3.6/pyechelle/simulator.py
--rw-r--r--   0        0        0     4854 2023-05-11 10:17:14.337422 pyechelle-0.3.6/pyechelle/slit.py
--rw-r--r--   0        0        0    19711 2023-06-06 12:23:50.722422 pyechelle-0.3.6/pyechelle/sources.py
--rw-r--r--   0        0        0    30781 2023-07-08 14:06:17.904478 pyechelle-0.3.6/pyechelle/spectrograph.py
--rw-r--r--   0        0        0      853 2023-05-11 10:17:14.337993 pyechelle-0.3.6/pyechelle/telescope.py
--rw-r--r--   0        0        0     1593 2023-07-08 13:18:29.945660 pyechelle-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3528 2023-05-11 10:17:14.118690 pyechelle-0.3.6/README.md
--rw-r--r--   0        0        0     4639 1970-01-01 00:00:00.000000 pyechelle-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-09-30 17:13:02.235155 pyechelle-0.3.7/LICENSE
+-rw-r--r--   0        0        0     3435 2023-09-30 17:13:02.235155 pyechelle-0.3.7/README.md
+-rw-r--r--   0        0        0     3460 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/CCD.py
+-rw-r--r--   0        0        0      724 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/__init__.py
+-rw-r--r--   0        0        0     4883 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/benchmark.py
+-rw-r--r--   0        0        0     7610 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/efficiency.py
+-rw-r--r--   0        0        0     6658 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/hdfbuilder.py
+-rw-r--r--   0        0        0     5949 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/model_viewer.py
+-rw-r--r--   0        0        0      101 2024-04-21 14:51:18.163951 pyechelle-0.3.7/pyechelle/models/available_models.txt
+-rw-r--r--   0        0        0    15497 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/optics.py
+-rw-r--r--   0        0        0     2265 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/randomgen.py
+-rw-r--r--   0        0        0     8021 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/raytrace_cuda.py
+-rw-r--r--   0        0        0    10409 2023-10-01 11:06:02.470585 pyechelle-0.3.7/pyechelle/raytracing.py
+-rwxr-xr-x   0        0        0    34424 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/simulator.py
+-rw-r--r--   0        0        0     4762 2024-04-21 14:51:17.391947 pyechelle-0.3.7/pyechelle/slit.py
+-rw-r--r--   0        0        0    20641 2024-04-21 14:51:17.395947 pyechelle-0.3.7/pyechelle/sources.py
+-rw-r--r--   0        0        0    60842 2024-04-21 14:51:18.151951 pyechelle-0.3.7/pyechelle/spectrograph.py
+-rw-r--r--   0        0        0      819 2024-04-21 14:51:17.395947 pyechelle-0.3.7/pyechelle/telescope.py
+-rw-r--r--   0        0        0     3306 2024-04-21 14:51:17.395947 pyechelle-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 pyechelle-0.3.7/PKG-INFO
```

### Comparing `pyechelle-0.3.6/pyechelle/efficiency.py` & `pyechelle-0.3.7/pyechelle/efficiency.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,197 +1,227 @@
-from __future__ import annotations
-
-import pathlib
-
-import numpy as np
-import skycalc_ipy
-from joblib import Memory
-from numpy import deg2rad
-from numpy import sin, cos, tan, arcsin
-from scipy.interpolate import interp1d
-
-path = pathlib.Path(__file__).parent.resolve()
-cache_path = path.joinpath('.cache')
-# create data directory if it doesn't exist:
-pathlib.Path(cache_path).mkdir(parents=False, exist_ok=True)
-memory = Memory(cache_path, verbose=0)
-
-
-class Efficiency:
-    def __init__(self, name):
-        self.name = name
-
-    def get_efficiency(self, wavelength):
-        raise NotImplementedError
-
-    def get_efficiency_per_order(self, wavelength, order):
-        raise NotImplementedError
-
-
-class ConstantEfficiency(Efficiency):
-    def __init__(self, name, eff=1.):
-        super().__init__(name)
-        self.eff = eff
-
-    def get_efficiency(self, wavelength):
-        return np.ones_like(wavelength) * self.eff
-
-    def get_efficiency_per_order(self, wavelength, order):
-        return self.get_efficiency(wavelength)
-
-
-class BandpassFilter(Efficiency):
-    def __init__(self, minwl, maxwl, name='bandpass'):
-        super().__init__(name=name)
-        self.minwl = minwl
-        self.maxwl = maxwl
-
-    def get_efficiency(self, wavelength):
-        e = np.ones_like(wavelength)
-        idx = np.logical_or((wavelength < self.minwl), (wavelength > self.maxwl))
-        e[idx] = 0.
-        return e
-
-    def get_efficiency_per_order(self, wavelength, order):
-        return self.get_efficiency(wavelength)
-
-
-class SystemEfficiency(Efficiency):
-    def __init__(self, efficiencies: list[Efficiency], name: str):
-        super().__init__(name)
-        self.efficiencies = efficiencies
-
-    def get_efficiency(self, wavelength):
-        e = np.ones_like(wavelength)
-        for ef in self.efficiencies:
-            e *= ef.get_efficiency(wavelength)
-        return e
-
-    def get_efficiency_per_order(self, wavelength, order):
-        e = np.ones_like(wavelength)
-        for ef in self.efficiencies:
-            e *= ef.get_efficiency_per_order(wavelength, order)
-        return e
-
-    def add_efficiency(self, efficiency):
-        self.efficiencies.append(efficiency)
-
-
-class GratingEfficiency(Efficiency):
-    def __init__(self, alpha, blaze, gpmm, peak_efficiency=1.0, name="Grating"):
-        super().__init__(name)
-        self.alpha = deg2rad(alpha)
-        self.blaze = deg2rad(blaze)
-        self.gpmm = gpmm
-        self.peak_efficiency = peak_efficiency
-
-    def calc_efficiency(self, order, wl):
-        bb = np.nan_to_num(
-            arcsin(-sin(self.alpha) + order * wl * 1e-6 / (1.0 / self.gpmm / 1000.0))
-        )
-        # blaze_wavelength = 2.*self.gpmm * sin(self.blaze) / order
-        # fsr = blaze_wavelength / order
-
-        x = (
-                order
-                * (cos(self.alpha) / cos(self.alpha - self.blaze))
-                * (cos(self.blaze) - sin(self.blaze) / tan((self.alpha + bb) / 2.0))
-        )
-        sinc = np.sinc(x)
-
-        return self.peak_efficiency * sinc * sinc
-
-    def get_efficiency(self, wavelength):
-        e = np.zeros_like(wavelength)
-        for o in range(50, 150):
-            e += self.calc_efficiency(o, wavelength)
-        return e
-
-    def get_efficiency_per_order(self, wavelength, order):
-        return self.calc_efficiency(order, wavelength)
-
-
-class TabulatedEfficiency(Efficiency):
-    def __init__(self, name, wavelength, efficiency, orders=None):
-        super().__init__(name)
-        wavelength = np.atleast_1d(wavelength)
-        efficiency = np.atleast_1d(efficiency)
-        assert len(wavelength) == len(efficiency)
-        if orders is None:
-            # do constant extrapolation if only 1 point
-            if len(wavelength) == 1:
-                self.ip = lambda x: efficiency
-            # do linear interpolation if only 2 points
-            elif len(wavelength) == 2:
-                self.ip = interp1d(wavelength, efficiency, kind="linear", fill_value=0., bounds_error=False)
-            # do linear interpolation if only 2 points
-            elif len(wavelength) == 3:
-                self.ip = interp1d(wavelength, efficiency, kind="quadratic", fill_value=0., bounds_error=False)
-            # do cubic interpolation if >= 4 points
-            else:
-                self.ip = interp1d(wavelength, efficiency, kind="cubic", fill_value=0., bounds_error=False)
-            self.ip_per_order = self.ip
-        else:
-            self.ip_per_order = {}
-
-            for o in np.unique(orders):
-                idx = orders == o
-                self.ip_per_order[o] = interp1d(wavelength[idx], efficiency[idx], kind="cubic", fill_value=0.0,
-                                                bounds_error=False)
-
-            y = np.zeros_like(wavelength)
-            for o in np.unique(orders):
-                y += self.ip_per_order[o](wavelength)
-
-            self.ip = interp1d(wavelength, y)
-
-    def get_efficiency(self, wavelength):
-        return self.ip(wavelength)
-
-    def get_efficiency_per_order(self, wavelength, order):
-        if isinstance(self.ip_per_order, dict):
-            return self.ip_per_order[order](wavelength)
-        else:
-            return self.ip_per_order(wavelength)
-
-
-class CSVEfficiency(TabulatedEfficiency):
-    def __init__(self, name, path, delimiter=","):
-        data = np.genfromtxt(path, delimiter=delimiter)
-        if data.shape[1] == 2:  # file contains wavelength, efficiency
-            super().__init__(name, data[:, 0], data[:, 1])
-        if data.shape[1] == 3:  # file contains order, wavelength, efficiency
-            super().__init__(name, data[:, 1], data[:, 2], data[:, 0])
-
-
-class Atmosphere(Efficiency):
-    def __init__(self, name, sky_calc_kwargs=None):
-        super().__init__(name)
-        # set default atmosphere arguments to high-resolution
-        self.kwargs = {"wres": 1E6, "wgrid_mode": "fixed_spectral_resolution"}
-        if sky_calc_kwargs is not None:
-            self.kwargs.update(sky_calc_kwargs)
-
-    def get_efficiency(self, wavelength):
-        return self.get_atmosphere_data(wavelength, self.kwargs)
-
-    def get_efficiency_per_order(self, wavelength, order):
-        return self.get_atmosphere_data(wavelength, self.kwargs)
-
-    @staticmethod
-    @memory.cache
-    def get_atmosphere_data(wavelength, sky_calc_kwargs=None):
-        kwargs = {"wres": 1E6, "wgrid_mode": "fixed_spectral_resolution"}
-        if sky_calc_kwargs is not None:
-            kwargs.update(sky_calc_kwargs)
-        sky = skycalc_ipy.SkyCalc()
-        sky.update(kwargs)  # set sky arguments
-        wmin = np.min(wavelength) * 1000.
-        wmax = np.max(wavelength) * 1000.
-        sky.update({'wmin': wmin, 'wmax': wmax})
-
-        tbl = sky.get_sky_spectrum()
-        # extrapolate is needed because tbl['lam'].data might not contain exact wavelength limits,
-        # since we are in constant resolution mode ("wgrid_mode": "fixed_spectral_resolution")
-        ip = interp1d(tbl['lam'].data, tbl['trans'].data, assume_sorted=True, fill_value="extrapolate")
-
-        return ip(wavelength)
+from __future__ import annotations
+
+import pathlib
+
+import numpy as np
+import skycalc_ipy
+from joblib import Memory
+from numpy import deg2rad
+from numpy import sin, cos, tan, arcsin
+from scipy.interpolate import interp1d
+
+path = pathlib.Path(__file__).parent.resolve()
+cache_path = path.joinpath(".cache")
+# create data directory if it doesn't exist:
+pathlib.Path(cache_path).mkdir(parents=False, exist_ok=True)
+memory = Memory(cache_path, verbose=0)
+
+
+class Efficiency:
+    def __init__(self, name):
+        self.name = name
+
+    def get_efficiency(self, wavelength):
+        raise NotImplementedError
+
+    def get_efficiency_per_order(self, wavelength, order):
+        raise NotImplementedError
+
+
+class ConstantEfficiency(Efficiency):
+    def __init__(self, name, eff=1.0):
+        super().__init__(name)
+        self.eff = eff
+
+    def get_efficiency(self, wavelength):
+        return np.ones_like(wavelength) * self.eff
+
+    def get_efficiency_per_order(self, wavelength, order):
+        return self.get_efficiency(wavelength)
+
+
+class BandpassFilter(Efficiency):
+    def __init__(self, minwl, maxwl, name="bandpass"):
+        super().__init__(name=name)
+        self.minwl = minwl
+        self.maxwl = maxwl
+
+    def get_efficiency(self, wavelength):
+        e = np.ones_like(wavelength)
+        idx = np.logical_or((wavelength < self.minwl), (wavelength > self.maxwl))
+        e[idx] = 0.0
+        return e
+
+    def get_efficiency_per_order(self, wavelength, order):
+        return self.get_efficiency(wavelength)
+
+
+class SystemEfficiency(Efficiency):
+    def __init__(self, efficiencies: list[Efficiency | None], name: str):
+        super().__init__(name)
+        self.efficiencies = efficiencies
+
+    def get_efficiency(self, wavelength):
+        e = np.ones_like(wavelength)
+        for ef in self.efficiencies:
+            if ef is not None:
+                e *= ef.get_efficiency(wavelength)
+        return e
+
+    def get_efficiency_per_order(self, wavelength, order):
+        e = np.ones_like(wavelength)
+        for ef in self.efficiencies:
+            if ef is not None:
+                e *= ef.get_efficiency_per_order(wavelength, order)
+        return e
+
+    def add_efficiency(self, efficiency):
+        self.efficiencies.append(efficiency)
+
+
+class GratingEfficiency(Efficiency):
+    def __init__(self, alpha, blaze, gpmm, peak_efficiency=1.0, name="Grating"):
+        super().__init__(name)
+        self.alpha = deg2rad(alpha)
+        self.blaze = deg2rad(blaze)
+        self.gpmm = gpmm
+        self.peak_efficiency = peak_efficiency
+
+    def calc_efficiency(self, order, wl):
+        bb = np.nan_to_num(
+            arcsin(-sin(self.alpha) + order * wl * 1e-6 / (1.0 / self.gpmm / 1000.0))
+        )
+        # blaze_wavelength = 2.*self.gpmm * sin(self.blaze) / order
+        # fsr = blaze_wavelength / order
+
+        x = (
+            order
+            * (cos(self.alpha) / cos(self.alpha - self.blaze))
+            * (cos(self.blaze) - sin(self.blaze) / tan((self.alpha + bb) / 2.0))
+        )
+        sinc = np.sinc(x)
+
+        return self.peak_efficiency * sinc * sinc
+
+    def get_efficiency(self, wavelength):
+        e = np.zeros_like(wavelength)
+        for o in range(50, 150):
+            e += self.calc_efficiency(o, wavelength)
+        return e
+
+    def get_efficiency_per_order(self, wavelength, order):
+        return self.calc_efficiency(order, wavelength)
+
+
+class TabulatedEfficiency(Efficiency):
+    def __init__(self, name, wavelength, efficiency, orders=None):
+        super().__init__(name)
+        wavelength = np.atleast_1d(wavelength)
+        efficiency = np.atleast_1d(efficiency)
+        assert len(wavelength) == len(efficiency)
+        if orders is None:
+            # do constant extrapolation if only 1 point
+            if len(wavelength) == 1:
+                self.ip = lambda x: efficiency
+            # do linear interpolation if only 2 points
+            elif len(wavelength) == 2:
+                self.ip = interp1d(
+                    wavelength,
+                    efficiency,
+                    kind="linear",
+                    fill_value=0.0,
+                    bounds_error=False,
+                )
+            # do linear interpolation if only 2 points
+            elif len(wavelength) == 3:
+                self.ip = interp1d(
+                    wavelength,
+                    efficiency,
+                    kind="quadratic",
+                    fill_value=0.0,
+                    bounds_error=False,
+                )
+            # do cubic interpolation if >= 4 points
+            else:
+                self.ip = interp1d(
+                    wavelength,
+                    efficiency,
+                    kind="cubic",
+                    fill_value=0.0,
+                    bounds_error=False,
+                )
+            self.ip_per_order = self.ip
+        else:
+            self.ip_per_order = {}
+
+            for o in np.unique(orders):
+                idx = orders == o
+                self.ip_per_order[o] = interp1d(
+                    wavelength[idx],
+                    efficiency[idx],
+                    kind="cubic",
+                    fill_value=0.0,
+                    bounds_error=False,
+                )
+
+            y = np.zeros_like(wavelength)
+            for o in np.unique(orders):
+                y += self.ip_per_order[o](wavelength)
+
+            self.ip = interp1d(wavelength, y)
+
+    def get_efficiency(self, wavelength):
+        return self.ip(wavelength)
+
+    def get_efficiency_per_order(self, wavelength, order):
+        if isinstance(self.ip_per_order, dict):
+            return self.ip_per_order[order](wavelength)
+        else:
+            return self.ip_per_order(wavelength)
+
+
+class CSVEfficiency(TabulatedEfficiency):
+    def __init__(self, name, path, delimiter=","):
+        data = np.genfromtxt(path, delimiter=delimiter)
+        if data.shape[1] == 2:  # file contains wavelength, efficiency
+            super().__init__(name, data[:, 0], data[:, 1])
+        if data.shape[1] == 3:  # file contains order, wavelength, efficiency
+            super().__init__(name, data[:, 1], data[:, 2], data[:, 0])
+
+
+class Atmosphere(Efficiency):
+    def __init__(self, name, sky_calc_kwargs=None):
+        super().__init__(name)
+        # set default atmosphere arguments to high-resolution
+        self.kwargs = {"wres": 1e6, "wgrid_mode": "fixed_spectral_resolution"}
+        if sky_calc_kwargs is not None:
+            self.kwargs.update(sky_calc_kwargs)
+
+    def get_efficiency(self, wavelength):
+        return self.get_atmosphere_data(wavelength, self.kwargs)
+
+    def get_efficiency_per_order(self, wavelength, order):
+        return self.get_atmosphere_data(wavelength, self.kwargs)
+
+    @staticmethod
+    @memory.cache
+    def get_atmosphere_data(wavelength, sky_calc_kwargs=None):
+        kwargs = {"wres": 1e6, "wgrid_mode": "fixed_spectral_resolution"}
+        if sky_calc_kwargs is not None:
+            kwargs.update(sky_calc_kwargs)
+        sky = skycalc_ipy.SkyCalc()
+        sky.update(kwargs)  # set sky arguments
+        wmin = np.min(wavelength) * 1000.0
+        wmax = np.max(wavelength) * 1000.0
+        sky.update({"wmin": wmin, "wmax": wmax})
+
+        tbl = sky.get_sky_spectrum()
+        # extrapolate is needed because tbl['lam'].data might not contain exact wavelength limits,
+        # since we are in constant resolution mode ("wgrid_mode": "fixed_spectral_resolution")
+        ip = interp1d(
+            tbl["lam"].data,
+            tbl["trans"].data,
+            assume_sorted=True,
+            fill_value="extrapolate",
+        )
+
+        return ip(wavelength * 1000.0)
```

### Comparing `pyechelle-0.3.6/pyechelle/model_viewer.py` & `pyechelle-0.3.7/pyechelle/model_viewer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,190 @@
-import argparse
-import sys
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-from pyechelle.optics import convert_matrix
-from pyechelle.simulator import available_models
-from pyechelle.spectrograph import Spectrograph, ZEMAX
-
-
-def plot_transformations(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
-    """ Plot affine transformation matrices
-
-    Args:
-        spectrograph: Spectrograph model
-
-    Returns:
-
-    """
-    fig, ax = plt.subplots(2, 3, sharex=True)
-    fig.suptitle(f"Affine transformations of {spectrograph.name}")
-    if isinstance(spectrograph, ZEMAX):
-        for o in spectrograph.get_orders(fiber, ccd_index):
-            ax[0, 0].set_title("sx")
-            ax[0, 0].plot([af.sx for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[0, 1].set_title("sy")
-            ax[0, 1].plot([af.sy for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[0, 2].set_title("shear")
-            ax[0, 2].plot([af.shear for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[1, 0].set_title("rot")
-            ax[1, 0].plot([af.rot for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[1, 1].set_title("tx")
-            ax[1, 1].plot([af.tx for af in spectrograph.transformations(o, fiber, ccd_index)])
-            ax[1, 2].set_title("ty")
-            ax[1, 2].plot([af.ty for af in spectrograph.transformations(o, fiber, ccd_index)])
-    else:
-        raise NotImplementedError
-    return fig
-
-
-def plot_transformation_matrices(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
-    """ Plot affine transformation matrices
-
-    Args:
-        fiber: fiber index
-        ccd_index: ccd index
-        spectrograph: Spectrograph model
-
-    Returns:
-
-    """
-    fig, ax = plt.subplots(2, 3, sharex=True)
-    fig.suptitle(f"Affine transformation matrices of {spectrograph.name}")
-    for o in spectrograph.get_orders(fiber, ccd_index):
-        if isinstance(spectrograph, ZEMAX):
-            transformations = convert_matrix(
-                np.array([tm.as_matrix() for tm in spectrograph.transformations(o, fiber, ccd_index)]).T)
-            ax[0, 0].set_title("m0")
-            ax[0, 0].plot(transformations[0])
-            ax[0, 1].set_title("m1")
-            ax[0, 1].plot(transformations[1])
-            ax[0, 2].set_title("m2")
-            ax[0, 2].plot(transformations[2])
-            ax[1, 0].set_title("m3")
-            ax[1, 0].plot(transformations[3])
-            ax[1, 1].set_title("m4")
-            ax[1, 1].plot(transformations[4])
-            ax[1, 2].set_title("m5")
-            ax[1, 2].plot(transformations[5])
-        else:
-            raise NotImplementedError
-    return fig
-
-
-def plot_psfs(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
-    """ Plot PSFs as one big map
-    Args:
-        fiber: fiber index
-        ccd_index: ccd index
-        spectrograph: Spectrograph model
-
-    Returns:
-
-    """
-
-    fig, ax = plt.subplots()
-    orders = spectrograph.get_orders(fiber, ccd_index)
-    n_orders = len(orders)
-    if isinstance(spectrograph, ZEMAX):
-        n_psfs = len(spectrograph.psfs(orders[0], fiber, ccd_index))
-    else:
-        n_psfs = 10
-
-    shape_psfs = spectrograph.get_psf(sum(spectrograph.get_wavelength_range(orders[0], fiber, ccd_index)) / 2.,
-                                      orders[0], fiber, ccd_index).data.shape
-
-    # shape_psfs = spectrograph.psfs[next(spectrograph.psfs.keys().__iter__())].psfs[0].data.shape
-    img = np.empty((n_psfs * shape_psfs[0], n_orders * shape_psfs[1]))
-
-    for oo, o in enumerate(np.sort(orders)):
-        if isinstance(spectrograph, ZEMAX):
-            psfs = spectrograph.psfs(o, fiber, ccd_index)
-        else:
-            wl = np.linspace(*spectrograph.get_wavelength_range(o, fiber, ccd_index), num=n_psfs)
-            psfs = [spectrograph.get_psf(w, o, fiber, ccd_index) for w in wl]
-
-        for i, p in enumerate(psfs):
-            if p.data.shape == shape_psfs:
-                img[int(i * shape_psfs[0]):int((i + 1) * shape_psfs[0]),
-                int(oo * shape_psfs[1]):int((oo + 1) * shape_psfs[1])] = p.data
-    ax.imshow(img, vmin=0, vmax=np.mean(img) * 10.0)
-    return fig
-
-
-# def plot_fields(spec: ZEMAX, show=True):
-#     plt.figure()
-#     with h5py.File(spec.modelpath, 'r') as h5f:
-#         for k in h5f.keys():
-#             if 'fiber_' in k:
-#                 a = h5f[k].attrs['norm_field'].decode('utf-8').split('\n')
-#
-#                 for b in a:
-#                     if 'aF' in b:
-#                         print(b[2:])
-
-
-def main(args):
-    if not args:
-        args = sys.argv[1:]
-
-    parser = argparse.ArgumentParser(description='PyEchelle Simulator Model Viewer')
-    parser.add_argument('-s', '--spectrograph', choices=available_models, type=str, default="MaroonX", required=True,
-                        help=f"Filename of spectrograph model. Model file needs to be located in models/ folder. ")
-    parser.add_argument('--fiber', type=int, default=1, required=False)
-    parser.add_argument('--show', action='store_true')
-
-    args = parser.parse_args(args)
-    spec = ZEMAX(args.spectrograph)
-    # if args.plot_transformations:
-    plot_transformations(spec, args.fiber)
-    # if args.plot_transformation_matrices:
-    plot_transformation_matrices(spec, args.fiber)
-    # if args.plot_field:
-    # plot_fields(spec)
-    # if args.plot_psfs:
-    plot_psfs(spec)
-    if args.show:
-        plt.show()
-
-
-if __name__ == "__main__":
-    main(sys.argv[1:])
+import argparse
+import sys
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+from pyechelle.optics import convert_matrix
+from pyechelle.simulator import available_models
+from pyechelle.spectrograph import Spectrograph, ZEMAX
+
+
+def plot_transformations(
+    spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1
+):
+    """Plot affine transformation matrices
+
+    Args:
+        spectrograph: Spectrograph model
+
+    Returns:
+
+    """
+    fig, ax = plt.subplots(2, 3, sharex=True)
+    fig.suptitle(f"Affine transformations of {spectrograph.name}")
+    if isinstance(spectrograph, ZEMAX):
+        for o in spectrograph.get_orders(fiber, ccd_index):
+            ax[0, 0].set_title("sx")
+            ax[0, 0].plot(
+                [af.sx for af in spectrograph.transformations(o, fiber, ccd_index)]
+            )
+            ax[0, 1].set_title("sy")
+            ax[0, 1].plot(
+                [af.sy for af in spectrograph.transformations(o, fiber, ccd_index)]
+            )
+            ax[0, 2].set_title("shear")
+            ax[0, 2].plot(
+                [af.shear for af in spectrograph.transformations(o, fiber, ccd_index)]
+            )
+            ax[1, 0].set_title("rot")
+            ax[1, 0].plot(
+                [af.rot for af in spectrograph.transformations(o, fiber, ccd_index)]
+            )
+            ax[1, 1].set_title("tx")
+            ax[1, 1].plot(
+                [af.tx for af in spectrograph.transformations(o, fiber, ccd_index)]
+            )
+            ax[1, 2].set_title("ty")
+            ax[1, 2].plot(
+                [af.ty for af in spectrograph.transformations(o, fiber, ccd_index)]
+            )
+    else:
+        raise NotImplementedError
+    return fig
+
+
+def plot_transformation_matrices(
+    spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1
+):
+    """Plot affine transformation matrices
+
+    Args:
+        fiber: fiber index
+        ccd_index: ccd index
+        spectrograph: Spectrograph model
+
+    Returns:
+
+    """
+    fig, ax = plt.subplots(2, 3, sharex=True)
+    fig.suptitle(f"Affine transformation matrices of {spectrograph.name}")
+    for o in spectrograph.get_orders(fiber, ccd_index):
+        if isinstance(spectrograph, ZEMAX):
+            transformations = convert_matrix(
+                np.array(
+                    [
+                        tm.as_matrix()
+                        for tm in spectrograph.transformations(o, fiber, ccd_index)
+                    ]
+                ).T
+            )
+            ax[0, 0].set_title("m0")
+            ax[0, 0].plot(transformations[0])
+            ax[0, 1].set_title("m1")
+            ax[0, 1].plot(transformations[1])
+            ax[0, 2].set_title("m2")
+            ax[0, 2].plot(transformations[2])
+            ax[1, 0].set_title("m3")
+            ax[1, 0].plot(transformations[3])
+            ax[1, 1].set_title("m4")
+            ax[1, 1].plot(transformations[4])
+            ax[1, 2].set_title("m5")
+            ax[1, 2].plot(transformations[5])
+        else:
+            raise NotImplementedError
+    return fig
+
+
+def plot_psfs(spectrograph: Spectrograph, fiber: int = 1, ccd_index: int = 1):
+    """Plot PSFs as one big map
+    Args:
+        fiber: fiber index
+        ccd_index: ccd index
+        spectrograph: Spectrograph model
+
+    Returns:
+
+    """
+
+    fig, ax = plt.subplots()
+    orders = spectrograph.get_orders(fiber, ccd_index)
+    n_orders = len(orders)
+    if isinstance(spectrograph, ZEMAX):
+        n_psfs = len(spectrograph.psfs(orders[0], fiber, ccd_index))
+    else:
+        n_psfs = 10
+
+    shape_psfs = spectrograph.get_psf(
+        sum(spectrograph.get_wavelength_range(orders[0], fiber, ccd_index)) / 2.0,
+        orders[0],
+        fiber,
+        ccd_index,
+    ).data.shape
+
+    # shape_psfs = spectrograph.psfs[next(spectrograph.psfs.keys().__iter__())].psfs[0].data.shape
+    img = np.empty((n_psfs * shape_psfs[0], n_orders * shape_psfs[1]))
+
+    for oo, o in enumerate(np.sort(orders)):
+        if isinstance(spectrograph, ZEMAX):
+            psfs = spectrograph.psfs(o, fiber, ccd_index)
+        else:
+            wl = np.linspace(
+                *spectrograph.get_wavelength_range(o, fiber, ccd_index), num=n_psfs
+            )
+            psfs = [spectrograph.get_psf(w, o, fiber, ccd_index) for w in wl]
+
+        for i, p in enumerate(psfs):
+            if p.data.shape == shape_psfs:
+                img[
+                    int(i * shape_psfs[0]) : int((i + 1) * shape_psfs[0]),
+                    int(oo * shape_psfs[1]) : int((oo + 1) * shape_psfs[1]),
+                ] = p.data
+    ax.imshow(img, vmin=0, vmax=np.mean(img) * 10.0)
+    return fig
+
+
+# def plot_fields(spec: ZEMAX, show=True):
+#     plt.figure()
+#     with h5py.File(spec.modelpath, 'r') as h5f:
+#         for k in h5f.keys():
+#             if 'fiber_' in k:
+#                 a = h5f[k].attrs['norm_field'].decode('utf-8').split('\n')
+#
+#                 for b in a:
+#                     if 'aF' in b:
+#                         print(b[2:])
+
+
+def main(args):
+    if not args:
+        args = sys.argv[1:]
+
+    parser = argparse.ArgumentParser(description="PyEchelle Simulator Model Viewer")
+    parser.add_argument(
+        "-s",
+        "--spectrograph",
+        choices=available_models,
+        type=str,
+        default="MaroonX",
+        required=True,
+        help="Filename of spectrograph model. Model file needs to be located in models/ folder. ",
+    )
+    parser.add_argument("--fiber", type=int, default=1, required=False)
+    parser.add_argument("--show", action="store_true")
+
+    args = parser.parse_args(args)
+    spec = ZEMAX(args.spectrograph)
+    # if args.plot_transformations:
+    plot_transformations(spec, args.fiber)
+    # if args.plot_transformation_matrices:
+    plot_transformation_matrices(spec, args.fiber)
+    # if args.plot_field:
+    # plot_fields(spec)
+    # if args.plot_psfs:
+    plot_psfs(spec)
+    if args.show:
+        plt.show()
+
+
+if __name__ == "__main__":
+    main(sys.argv[1:])
```

### Comparing `pyechelle-0.3.6/pyechelle/simulator.py` & `pyechelle-0.3.7/pyechelle/simulator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,591 +1,995 @@
-#!/usr/bin/env python
-from __future__ import annotations
-
-import argparse
-import distutils.util
-import inspect
-import logging
-import pathlib
-import re
-import sys
-import time
-from dataclasses import field, dataclass
-from pathlib import Path
-
-import numpy as np
-from astropy.io import fits
-from joblib import Parallel, delayed
-from numba import cuda
-
-import pyechelle
-import pyechelle.slit
-from pyechelle import sources
-from pyechelle.CCD import CCD
-from pyechelle.efficiency import Efficiency, CSVEfficiency, SystemEfficiency, Atmosphere
-from pyechelle.raytrace_cuda import make_cuda_kernel, raytrace_order_cuda, make_cuda_kernel_singlemode
-from pyechelle.raytracing import raytrace_order_cpu
-from pyechelle.sources import CSV
-from pyechelle.sources import Phoenix, Source
-from pyechelle.spectrograph import Spectrograph, ZEMAX
-from pyechelle.telescope import Telescope
-
-logger = logging.getLogger('Simulator')
-logger.setLevel(level=logging.INFO)
-
-# get list of available spectrograph models
-dir_path = Path(__file__).resolve().parent.joinpath("models").joinpath("available_models.txt")
-with open(dir_path, 'r') as am:
-    available_models = [line.strip() for line in am.readlines() if line.strip() != '']
-
-# get list of available sources
-available_sources = [m[0] for m in inspect.getmembers(pyechelle.sources, inspect.isclass) if
-                     issubclass(m[1], pyechelle.sources.Source) and m[0] != "Source"]
-
-
-def parse_num_list(string_list: str) -> list:
-    """
-    Converts a string specifying a range of numbers (e.g. '1-3') into a list of these numbers ([1,2,3])
-    Args:
-        string_list: string like "[start value]-[end value]"
-
-    Returns:
-        List of integers
-    """
-
-    m = re.match(r'(\d+)(?:-(\d+))?$', string_list)
-    if not m:
-        raise argparse.ArgumentTypeError(
-            "'" + string_list + "' is not a range of number. Expected forms like '0-5' or '2'.")
-    start = m.group(1)
-    end = m.group(2) or start
-    return list(range(int(start, 10), int(end, 10) + 1))
-
-
-def export_to_html(data, filename, include_plotlyjs=False, width=1000, height=300, y_range_min=2000, y_range_max=3000):
-    """
-    Exports a 2D image into a 'standalone' HTML file. This is used e.g. for some examples in the documentation.
-    Args:
-        data: 2d numpy array
-        filename: output filename
-        include_plotlyjs: whether plotlyjs is included in html file or not
-        width: width of the plot in pixel
-        height: height of the plot in pixel
-        y_range_min: minimum y coordinate shown in image
-        y_range_max: maximum y coordinate shown in image
-
-    Returns:
-        None
-    """
-    import plotly.express as px
-    fig = px.imshow(data, binary_string=True, aspect='equal')
-
-    fig.update_traces(
-        hovertemplate=None,
-        hoverinfo='skip'
-    )
-    fig.update_layout(autosize=True, width=width, height=height, margin=dict(l=0, r=0, b=0, t=0))
-    fig.update_yaxes(range=[y_range_min, y_range_max])
-    fig.write_html(filename, include_plotlyjs=include_plotlyjs)
-
-
-def log_elapsed_time(msg: str, t0: float) -> float:
-    t1 = time.time()
-    logger.info(msg + f' (took {t1 - t0:2f} s )')
-    return t1
-
-
-def write_to_fits(c: CCD, filename: str | Path, overwrite: bool = True, append: bool = False, dtype: np.dtype = np.uint16):
-    """ Saves CCD image to disk
-
-    Args:
-        c: CCD object
-        filename: filepath
-        overwrite: if True, file will be overwritten if existing
-        append: if True, CCD data will be added to data in fits file
-        dtype: numpy.dtype object defining the data type of the saved FITS file, defaulting to unsigned 16-bit integers
-
-    Returns:
-        None
-    """
-    old_file_data = np.zeros_like(c.data)
-    if append:
-        if pathlib.Path(filename).is_file():
-            old_file_data = fits.getdata(filename)
-            assert old_file_data.shape == c.data.shape, f"You tried to append data to {filename}, " \
-                                                        f"but the fits file contains" \
-                                                        f"data with a different shape ({old_file_data.shape})."
-    hdu = fits.PrimaryHDU(data=np.array(c.data + old_file_data, dtype=dtype))
-    hdu_list = fits.HDUList([hdu])
-    hdu_list.writeto(filename, overwrite=overwrite or append)
-
-
-@dataclass
-class Simulator:
-    """ PyEchelle simulator
-
-    Simulator class that contains everything needed to generate spectra.
-
-    Attributes:
-        spectrograph (Spectrograph): spectrograph used for simulations
-        fibers (list[int]): fiber / list of fibers to be simulated
-        orders (list[int]): order / list of diffraction orders to be simulated
-        sources (list[Source]): spectral source / list of spectral sources per fiber (same length as fibers)
-        atmosphere (list[bool]): whether to include atmospheric transmission per fiber (same length as fibers)
-        atmosphere_conditions (list[dict | None]): skycalc arguments for atmospheric conditions (same length as sources)
-        rvs (list[float]): radial velocity shifts in [m/s] for sources (same length as fibers)
-        telescope (Telescope): Telescope used for simulations (relevant for 'on-sky' sources)
-        random_seed (int): random seed for the number generator
-        cuda (bool): flat if CUDA is to be used
-        max_cpu (int): number of CPUs used for simulation (if -1, max_cpu is number of available cores)
-        exp_time (float): exposure time to be simulated
-        output (Path): path to output fits file
-        append (bool): flag if simulated counts should be appended to existing image
-        overwrite (bool): flat if output file should be overwritten if existing
-        global_efficiency (Efficiency): overall efficiency curve to be considered
-         (on top of spectrograph efficiency curve and potentially atmosphere)
-
-    """
-    spectrograph: Spectrograph
-    fibers: list[int] = field(init=False, default=None)
-    orders: list[int] = field(init=False, default=None)
-    ccd: int = field(init=False, default=None)
-    sources: list[Source] = field(init=False, default=None)
-    atmosphere: list[bool] = field(init=False, default=None)
-    atmosphere_conditions: list[dict | None] = field(init=False, default=None)
-    rvs: list[float] = field(init=False, default=None)
-    telescope: Telescope = field(init=False, default=None)
-    random_seed: int = field(init=False, default=-1)
-    cuda: bool = field(init=False, default=False)
-    max_cpu: int = field(init=False, default=1)
-    exp_time: float = field(init=False, default=1.)
-    output: Path = field(init=False, default=None)
-    append: bool = field(init=False, default=False)
-    overwrite: bool = field(init=False, default=False)
-    bias: int = field(init=False, default=0)
-    read_noise: float = field(init=False, default=0.)
-    global_efficiency: Efficiency = field(init=False, default=None)
-
-    def set_sources(self, source: Source | list[Source]):
-        assert self.fibers is not None, 'Please set first the fields that you want to simulate.'
-        self.sources = source if isinstance(source, list) else [source] * len(self.fibers)
-        assert len(self.fibers) == len(self.sources), \
-            'Number of sources needs to match the number of fields/fibers (or be 1)'
-
-    def set_atmospheres(self, atmosphere: bool | list[bool], sky_calc_kwargs: dict | list[dict] = None):
-        assert self.sources is not None, 'Please set first the sources that you want to simulate.'
-        self.atmosphere = [atmosphere] * len(self.sources) if isinstance(atmosphere, bool) else atmosphere
-        self.atmosphere_conditions = [sky_calc_kwargs] * len(self.sources) if (
-                isinstance(sky_calc_kwargs, dict) or sky_calc_kwargs is None) else sky_calc_kwargs
-        assert len(self.atmosphere) == len(self.sources), \
-            'Number of atmosphere flags needs to match the number of sources (or be 1)'
-        assert len(self.atmosphere_conditions) == len(self.sources), \
-            'Number of atmosphere condition arguments needs to match the number of sources (or be 1)'
-
-    def set_radial_velocities(self, rvs: float | list[float]):
-        assert self.sources is not None, 'Please set first the sources that you want to simulate.'
-        self.rvs = [rvs] * len(self.sources) if isinstance(rvs, float) else rvs
-        assert len(self.rvs) == len(self.sources), \
-            'Number of radial velocity values needs to match the number of sources (or be 1)'
-
-    def set_telescope(self, telescope: Telescope):
-        self.telescope = telescope
-
-    def set_ccd(self, ccd: int):
-        self.ccd = ccd
-        assert self.ccd in self.spectrograph.get_ccd().keys(), f'You requested simulation of CCD {ccd}, ' \
-                                                               f'which is not available.'
-
-    def set_efficiency(self, eff: Efficiency):
-        assert isinstance(eff, Efficiency)
-        self.global_efficiency = eff
-
-    def set_bias(self, bias_value: int = 0):
-        self.bias = bias_value
-
-    def set_read_noise(self, read_noise: float = 0.):
-        if read_noise > 0.0:
-            assert self.bias > 0, "read noise was specified, but no bias value is set, yet. " \
-                                  "Do so before setting the read noise."
-        self.read_noise = read_noise
-
-    def set_fibers(self, fiber: int | list[int]):
-        assert self.ccd is not None, 'Please set CCD index first.'
-        self.fibers = [fiber] if isinstance(fiber, int) else fiber
-        for f in self.fibers:
-            assert f in self.spectrograph.get_fibers(self.ccd), f'You requested simulation of fiber {f}, which is ' \
-                                                                f'not available for ccd with index {self.ccd}'
-
-    def set_cuda(self, activate: bool = True, seed: int = -1):
-        self.cuda = activate
-        self.random_seed = seed
-
-    def _get_valid_orders(self, fiber: int):
-        valid_orders = []
-
-        requested_orders = self.spectrograph.get_orders(fiber, self.ccd) if self.orders is None else self.orders
-        for o in requested_orders:
-            if o in self.spectrograph.get_orders(fiber, self.ccd):
-                valid_orders.append(o)
-            else:
-                logger.warning(f'Order {o} is requested, but it is not in the Spectrograph model.')
-        return valid_orders
-
-    def _get_slit_function(self, fiber: int):
-        try:
-            if self.cuda:
-                slit_fun = getattr(pyechelle.slit, f"cuda_{self.spectrograph.get_field_shape(fiber, self.ccd)}")
-            else:
-                slit_fun = getattr(pyechelle.slit, self.spectrograph.get_field_shape(fiber, self.ccd))
-        except AttributeError:
-            raise NotImplementedError(
-                f"Field shape {self.spectrograph.get_field_shape(fiber, self.ccd)} is not implemented.")
-        return slit_fun
-
-    def _simulate_multi_cpu(self, orders, fiber, ccd_index, slit_fun, s, rv, integration_time, c, efficiency):
-        simulated_photons = []
-        t0 = time.time()
-        results = Parallel(n_jobs=min(self.max_cpu, len(orders)), backend="threading")(
-            delayed(raytrace_order_cpu)(o, self.spectrograph, s, slit_fun, self.telescope, rv,
-                                        integration_time,
-                                        c, fiber, ccd_index,
-                                        efficiency, self.max_cpu) for o in np.sort(orders))
-        logger.info('Add up orders...')
-        ccd_results = [r[0] for r in results]
-        simulated_photons.extend([r[1] for r in results])
-        c.data = np.sum(ccd_results, axis=0)
-        log_elapsed_time('done.', t0)
-        return simulated_photons
-
-    def _simulate_single_cpu(self, orders, fiber, ccd_index, s, slit_fun, rv, integration_time, c, efficiency):
-        simulated_photons = []
-        for o in np.sort(orders):
-            nphot = raytrace_order_cpu(o, self.spectrograph, s, slit_fun, self.telescope, rv,
-                                       integration_time,
-                                       c, fiber, ccd_index,
-                                       efficiency,
-                                       1)
-            simulated_photons.append(nphot)
-        return simulated_photons
-
-    def _simulate_cuda(self, orders, slit_fun, rv, integration_time, dccd, efficiency, s, c, fiber, ccd_index):
-        if slit_fun is not None:  # multimode
-            cuda_kernel = make_cuda_kernel(slit_fun)
-        else:  # singlemode
-            cuda_kernel = make_cuda_kernel_singlemode()
-        simulated_photons = []
-        for o in np.sort(orders):
-            nphot = raytrace_order_cuda(o, self.spectrograph, s, self.telescope, rv, integration_time, dccd,
-                                        float(c.pixelsize), fiber, ccd_index, efficiency, seed=self.random_seed,
-                                        cuda_kernel=cuda_kernel)
-            simulated_photons.append(nphot)
-        return simulated_photons
-
-    def validate(self):
-        assert self.fibers is not None, 'Please set fibers for simulation'
-        assert self.ccd is not None, 'Please set ccd index/indices for simulation'
-        assert self.output is not None, 'Please set output path for simulation'
-        if self.atmosphere is None:
-            logger.info('It was not explicitly specified whether to consider atmospheric transmission. '
-                        'It is set to False')
-            self.atmosphere = [False] * len(self.sources)
-
-        if self.atmosphere_conditions is None:
-            if self.atmosphere:
-                logger.info('Atmospheric conditions were not specified. The default atmospheric conditions apply. '
-                            '(e.g. airmass 1)')
-            self.atmosphere_conditions = [None] * len(self.sources)
-
-        if self.rvs is None:
-            logger.info('Radial velocities are not specified explicitly. They are therefore set to 0.0')
-            self.rvs = [0.0] * len(self.sources)
-        if self.output.is_file():
-            assert self.overwrite or self.append, f'You specified to save the simulation at {self.output}, ' \
-                                                  f'but this file exists. If you want to overwrite, ' \
-                                                  f'please set the overwrite flag. Or in case you want to append to ' \
-                                                  f'the file: please set the append flag'
-        return True
-
-    def run(self):
-        self.validate()
-        c = self.spectrograph.get_ccd(self.ccd)
-        total_simulated_photons = []
-        t1 = time.time()
-        # copy empty array to CUDA device
-        if self.cuda:
-            dccd = cuda.to_device(np.zeros_like(c.data, dtype=np.uint32))
-
-        for f, s, atm, atm_cond, rv in zip(self.fibers, self.sources, self.atmosphere, self.atmosphere_conditions,
-                                           self.rvs):
-            orders = self.orders if self.orders is not None else self._get_valid_orders(f)
-            slit_fun = self._get_slit_function(f)
-            if self.global_efficiency is None:
-                if atm:
-                    e = SystemEfficiency([self.spectrograph.get_efficiency(f, self.ccd),
-                                          Atmosphere('Atmosphere', sky_calc_kwargs=atm_cond)],
-                                         'Combined Efficiency')
-                else:
-                    e = self.spectrograph.get_efficiency(f, self.ccd)
-            else:
-                if atm:
-                    e = SystemEfficiency([self.spectrograph.get_efficiency(f, self.ccd), self.global_efficiency,
-                                          Atmosphere('Atmosphere', sky_calc_kwargs=atm_cond)],
-                                         'Combined Efficiency')
-                else:
-                    e = SystemEfficiency([self.spectrograph.get_efficiency(f, self.ccd), self.global_efficiency],
-                                         'Combined Efficiency')
-
-            if not self.cuda:
-                if self.max_cpu > 1:
-                    total_simulated_photons.extend(
-                        self._simulate_multi_cpu(orders, f, self.ccd, slit_fun, s, rv, self.exp_time, c, e))
-                else:
-                    total_simulated_photons.extend(
-                        self._simulate_single_cpu(orders, f, self.ccd, s, slit_fun, rv, self.exp_time, c, e))
-            else:
-                total_simulated_photons.extend(
-                    self._simulate_cuda(orders, slit_fun, rv, self.exp_time, dccd, e, s, c, f, self.ccd))
-
-        if self.cuda:
-            dccd.copy_to_host(c.data)
-        logger.info('Finish up simulation and save...')
-        c.clip()
-
-        # add bias / global ccd effects
-        if self.bias > 0:
-            c.add_bias(self.bias)
-        if self.read_noise > 0.:
-            c.add_readnoise(self.read_noise)
-        t2 = time.time()
-
-        write_to_fits(c, self.output, self.overwrite, self.append)
-        logger.info(f"Total time for simulation: {t2 - t1:.3f}s.")
-        logger.info(f"Total simulated photons: {sum(total_simulated_photons)}")
-        return sum(total_simulated_photons)
-
-    def set_exposure_time(self, exp_time: float = 1):
-        self.exp_time = exp_time
-
-    def set_output(self, path: str | Path = Path().cwd().joinpath('test.fits'),
-                   append: bool = False, overwrite: bool = False):
-
-        self.output = path if isinstance(path, Path) else Path(path)
-        self.append = append
-        self.overwrite = overwrite
-        if append and not self.output.is_file():
-            logger.warning(f'You specified that the simulation should be appended to {self.output}, but there is no '
-                           f'such file. It will be created.')
-
-    def set_orders(self, orders: int | list[int] | None):
-        if isinstance(orders, int):
-            self.orders = [orders]
-        self.orders = orders
-        if self.orders is not None:
-            for f in self.fibers:
-                valid_orders = self._get_valid_orders(f)
-                for o in self.orders:
-                    assert o in valid_orders, f'You requested to simulate order {o}, but this order is not available' \
-                                              f'on CCD {self.ccd} and fiber/field {f}'
-
-
-def generate_parser():
-    parser = argparse.ArgumentParser(description='PyEchelle Simulator',
-                                     formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('-s', '--spectrograph', choices=available_models, type=str, default="MaroonX", required=True,
-                        help=f"Filename of spectrograph model. Model file needs to be located in models/ folder. ")
-    parser.add_argument('--ccd', type=int, default=1, required=False, help='Sets CCD index to be simulated.')
-    parser.add_argument('-t', '--integration_time', type=float, default=1.0, required=False,
-                        help=f"Integration time for the simulation in seconds [s].")
-    parser.add_argument('--fiber', type=parse_num_list, required=False,
-                        help='Fiber/Field number(s) to be simulated. Can either be a single integer, or an integer'
-                             'range (e.g. 1-3) ')
-    parser.add_argument('--no_blaze', action='store_true',
-                        help='If set, the blaze efficiency per order will be ignored.')
-    parser.add_argument('--no_efficiency', action='store_true',
-                        help='If set, all instrument/atmosphere efficiencies will be ignored.')
-
-    parser.add_argument('--cuda', action='store_true',
-                        help='If set, CUDA will be used for raytracing. Note: the max_cpu flag is then obsolete.')
-
-    parser.add_argument('--cuda_seed', type=int, default=-1,
-                        help='Random seed for generating CUDA RNG states. If <0, then the seed is choosen randomly.')
-
-    parser.add_argument('--max_cpu', type=int, default=1,
-                        help="Maximum number of CPU cores used. Note: The parallelization happens 'per order'."
-                             " Order-wise images are added up. This requires a large amount of memory at the moment."
-                             "If planning on simulating multiple images, consider using only 1 CPU per simulation "
-                             "and starting multiple simulations instead.")
-
-    atmosphere_group = parser.add_argument_group('Atmosphere')
-    atmosphere_group.add_argument('--atmosphere', nargs='+', required=False,
-                                  help='Add telluric lines to spectrum. For adding tellurics to all spectra just use'
-                                       '--atmosphere Y, for specifying per fiber user e.g. --atmosphere Y N Y',
-                                  type=lambda x: bool(distutils.util.strtobool(x)), default=[False])
-
-    atmosphere_group.add_argument('--airmass', default=1.0, type=float, required=False,
-                                  help='airmass for atmospheric model')
-
-    telescope_group = parser.add_argument_group('Telescope settings')
-    telescope_group.add_argument('--d_primary', type=float, required=False, default=1.0,
-                                 help='Diameter of the primary telescope mirror.')
-    telescope_group.add_argument('--d_secondary', type=float, required=False, default=0,
-                                 help='Diameter of the secondary telescope mirror.')
-
-    parser.add_argument('--orders', type=parse_num_list, nargs='+', required=False,
-                        help='Echelle/Grating order numbers to simulate... '
-                             'if not specified, all orders of the spectrograph are simulated.'
-                             'Can either be a single integer, or a range (e.g. 80-90)')
-
-    parser.add_argument('--sources', nargs='+', choices=available_sources, required=True,
-                        help='Spectral source for the simulation. Can either be a single string, e.g. "Etalon",'
-                             ' or a comma separated list of sources (e.g. "Etalon, Constant, Etalon") which length must'
-                             'match the number of fields/fibers.')
-    parser.add_argument('--rv', nargs='+', type=float, required=False, default=[0.],
-                        help="radial velocity shift of source")
-    const_source_group = parser.add_argument_group('Constant source')
-    const_source_group.add_argument('--constant_intensity', type=float, default=0.0001, required=False,
-                                    help="Flux in microWatts / nanometer for constant flux spectral source")
-    arclamps_group = parser.add_argument_group('Arc Lamps')
-    arclamps_group.add_argument('--scale', default=10.0, required=False,
-                                help='Intensity scale of gas lines (e.g. Ag or Ne) vs metal (Th)')
-
-    csv_group = parser.add_argument_group('CSV')
-    csv_group.add_argument('--csv_filepath', type=argparse.FileType('r'), required=False,
-                           help="Path to .csv file that contains two columns: wavelength and flux. The flux is expected"
-                                "to be in ergs/s/cm^2/cm (like Phoenix spectra) or photons (then set it via "
-                                "--csv_flux_in_photons). The wavelength unit is expected to "
-                                "be angstroms, but it can be changed via --csv_wavelength_unit")
-    csv_group.add_argument('--csv_wavelength_unit', choices=list(CSV.wavelength_scaling.keys()), default='a', type=str,
-                           help=f"Unit of the wavelength column in the .csv file. Options are "
-                                f"{list(CSV.wavelength_scaling.keys())}")
-    csv_group.add_argument('--csv_list_like', type=bool, default=False, help='Set to True if spectrum is discrete.')
-    csv_group.add_argument('--csv_flux_in_photons', type=bool, default=False,
-                           help='Set to True if flux is given in Photons/s rather than ergs')
-    csv_group.add_argument('--csv_stellar_target', type=bool, default=True,
-                           help='Set to True if Source is a stellar target.')
-    csv_group.add_argument('--csv_magnitude', type=float, default=10., required=False,
-                           help='If stellar target, the magnitude value i considered as V magnitude of the object and '
-                                'the flux is scaled accordingly. Ignored if --flux_in_photons is true.')
-    csv_group.add_argument('--csv_delimiter', type=str, required=False, default=',', help='Delimiter of the CSV file')
-
-    csv_eff_group = parser.add_argument_group('CSVEfficiency')
-    csv_eff_group.add_argument('--eff_csv_filepath', type=argparse.FileType('r'), required=False,
-                               help="Path to .csv file that contains two columns: wavelength and efficiency."
-                                    "The wavelength is expected to be in microns, "
-                                    "the efficiency is a real number in [0,1]."
-                                    "PyEchelle will interpolate the given values "
-                                    "for intermediate wavelength positions.")
-    csv_eff_group.add_argument('--eff_csv_delimiter', type=str, required=False, default=',',
-                               help='Delimiter of the CSV file')
-
-    phoenix_group = parser.add_argument_group('Phoenix')
-    phoenix_group.add_argument('--phoenix_t_eff', default=3600,
-                               choices=Phoenix.valid_t,
-                               type=int, required=False,
-                               help="Effective temperature in Kelvins [K].")
-    phoenix_group.add_argument('--phoenix_log_g', default=5.,
-                               choices=Phoenix.valid_g,
-                               type=float, required=False,
-                               help="Surface gravity log g.")
-    phoenix_group.add_argument('--phoenix_z',
-                               choices=Phoenix.valid_z,
-                               type=float, required=False, default=0.,
-                               help="Overall metallicity.")
-    phoenix_group.add_argument('--phoenix_alpha',
-                               choices=Phoenix.valid_a,
-                               type=float, required=False, default=0.,
-                               help="Alpha element abundance.")
-    phoenix_group.add_argument('--phoenix_magnitude', default=10., required=False, type=float,
-                               help='V Magnitude of stellar object.')
-
-    etalon_group = parser.add_argument_group('Etalon')
-    etalon_group.add_argument('--etalon_d', type=float, default=5., required=False,
-                              help='Mirror distance of Fabry Perot etalon in [mm].')
-    etalon_group.add_argument('--etalon_n', type=float, default=1.0, required=False,
-                              help='Refractive index of medium between etalon mirrors.')
-    etalon_group.add_argument('--etalon_theta', type=float, default=0., required=False,
-                              help='angle of incidence of light in radians.')
-    etalon_group.add_argument('--etalon_n_photons', default=1000, required=False,
-                              help='Number of photons per seconds per peak of the etalon spectrum.')
-
-    ccd_group = parser.add_argument_group('CCD')
-    ccd_group.add_argument('--bias', type=int, required=False, default=0)
-    ccd_group.add_argument('--read_noise', type=float, required=False, default=0.)
-
-    parser.add_argument('--show', default=False, action='store_true',
-                        help='If set, the simulated frame will be shown in a matplotlib imshow frame at the end.')
-    parser.add_argument('-o', '--output', type=lambda p: Path(p).absolute(), required=False,
-                        default=Path(__file__).absolute().parent / "test.fits",
-                        help='A .fits file where the simulation is saved.')
-    parser.add_argument('--overwrite', default=False, action='store_true',
-                        help='If set, the output file will be overwritten if it exists already.')
-    parser.add_argument('--append', default=False, action='store_true',
-                        help='If set, the simulated photons will be added to the output file rather than overwriting '
-                             'the content of the output file. If the output file does not exist yet, '
-                             'it will be created.This flag can be used to do more complex multi-fiber simulations as a'
-                             ' sequential manner of simpler simulations.')
-
-    parser.add_argument('--html_export', type=str, default='',
-                        help="If given, the spectrum will be exported to an interactive image using plotly. It's not a"
-                             "standalone html file, but requires plotly.js to be loaded.")
-    return parser
-
-
-def main(args=None):
-    if not args:
-        args = sys.argv[1:]
-    parser = generate_parser()
-    args = parser.parse_args(args)
-    t1 = time.time()
-    sim = Simulator(ZEMAX(args.spectrograph))
-    sim.set_ccd(args.ccd)
-
-    # generate flat list for all fields to simulate
-    if args.fiber is not None:
-        if any(isinstance(el, list) for el in args.fiber):
-            fibers = [item for sublist in args.fiber for item in sublist]
-        else:
-            fibers = args.fiber
-    else:
-        fibers = sim.spectrograph.get_fibers(args.ccd)
-    sim.set_fibers(fibers)
-
-    if args.orders is not None:
-        if any(isinstance(el, list) for el in args.orders):
-            requested_orders = [item for sublist in args.orders for item in sublist]
-        else:
-            requested_orders = args.orders
-        sim.set_orders(requested_orders)
-    # generate flat list of all sources to simulate
-    source_names = args.sources
-    if len(source_names) == 1:
-        source_names = [source_names[0]] * len(
-            fibers)  # generate list of same length as 'fields' if only one source given
-
-    source_kwargs = []
-    # extract kwords specific to selected source
-    for s in source_names:
-        source_args = [ss for ss in vars(args) if ss.startswith(s.lower())]
-        # create dict consisting of kword arguments and values specific to selected source
-        source_kwargs.append(dict(zip([ss.replace(f"{s.lower()}_", "") for ss in source_args],
-                                      [getattr(args, ss) for ss in source_args])))
-
-    sim.set_sources([getattr(sources, source)(**s_args) for source, s_args in zip(source_names, source_kwargs)])
-
-    if args.eff_csv_filepath:
-        sim.set_efficiency(CSVEfficiency('global', args.eff_csv_filepath, args.eff_csv_delimiter))
-    # generate flat list of whether atmosphere is added
-    sim.set_atmospheres(args.atmosphere[0] if len(args.atmosphere) == 1 else args.atmosphere)
-    sim.set_radial_velocities(args.rv[0] if len(args.rv) == 1 else args.rv)
-    sim.set_cuda(args.cuda, args.cuda_seed)
-    sim.set_exposure_time(args.integration_time)
-    sim.set_telescope(Telescope(args.d_primary, args.d_secondary))
-    sim.set_output(args.output, args.append, args.overwrite)
-    sim.set_bias(args.bias)
-    sim.set_read_noise(args.read_noise)
-    sim.run()
-    t2 = time.time()
-    print(f"Simulation took {t2 - t1:.3f} s")
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+from __future__ import annotations
+
+import argparse
+import inspect
+import logging
+import pathlib
+import random
+import re
+import sys
+import time
+from dataclasses import field, dataclass
+from datetime import datetime
+from pathlib import Path
+from typing import Type
+
+import numpy as np
+from astropy.io import fits
+from joblib import Parallel, delayed
+from numba import cuda
+
+import pyechelle
+import pyechelle.slit
+from pyechelle import sources
+from pyechelle.CCD import CCD
+from pyechelle.efficiency import Efficiency, CSVEfficiency, SystemEfficiency, Atmosphere
+from pyechelle.raytrace_cuda import (
+    make_cuda_kernel,
+    raytrace_order_cuda,
+    make_cuda_kernel_singlemode,
+)
+from pyechelle.raytracing import raytrace_order_cpu
+from pyechelle.sources import CSV
+from pyechelle.sources import Phoenix, Source
+from pyechelle.spectrograph import Spectrograph, ZEMAX
+from pyechelle.telescope import Telescope
+
+logger = logging.getLogger("Simulator")
+logger.setLevel(level=logging.INFO)
+
+# get list of available spectrograph models
+dir_path = (
+    Path(__file__).resolve().parent.joinpath("models").joinpath("available_models.txt")
+)
+with open(dir_path, "r") as am:
+    available_models = [line.strip() for line in am.readlines() if line.strip() != ""]
+
+# get list of available sources
+available_sources = [
+    m[0]
+    for m in inspect.getmembers(pyechelle.sources, inspect.isclass)
+    if issubclass(m[1], pyechelle.sources.Source) and m[0] != "Source"
+]
+
+
+def str2bool(v):
+    """Converts string to boolean"""
+    if isinstance(v, bool):
+        return v
+    if v.lower() in ('yes', 'true', 't', 'y', '1'):
+        return True
+    elif v.lower() in ('no', 'false', 'f', 'n', '0'):
+        return False
+    else:
+        raise argparse.ArgumentTypeError('Boolean value expected.')
+
+
+def parse_num_list(string_list: str) -> list:
+    """
+    Converts a string specifying a range of numbers (e.g. '1-3') into a list of these numbers ([1,2,3])
+    Args:
+        string_list: string like "[start value]-[end value]"
+
+    Returns:
+        List of integers
+    """
+
+    m = re.match(r"(\d+)(?:-(\d+))?$", string_list)
+    if not m:
+        raise argparse.ArgumentTypeError(
+            "'"
+            + string_list
+            + "' is not a range of number. Expected forms like '0-5' or '2'."
+        )
+    start = m.group(1)
+    end = m.group(2) or start
+    return list(range(int(start, 10), int(end, 10) + 1))
+
+
+def export_to_html(
+        data,
+        filename,
+        include_plotlyjs=False,
+        width=1000,
+        height=300,
+        y_range_min=2000,
+        y_range_max=3000,
+):
+    """
+    Exports a 2D image into a 'standalone' HTML file. This is used e.g. for some examples in the documentation.
+    Args:
+        data: 2d numpy array
+        filename: output filename
+        include_plotlyjs: whether plotlyjs is included in html file or not
+        width: width of the plot in pixel
+        height: height of the plot in pixel
+        y_range_min: minimum y coordinate shown in image
+        y_range_max: maximum y coordinate shown in image
+
+    Returns:
+        None
+    """
+    import plotly.express as px
+
+    fig = px.imshow(data, binary_string=True, aspect="equal")
+
+    fig.update_traces(hovertemplate=None, hoverinfo="skip")
+    fig.update_layout(
+        autosize=True, width=width, height=height, margin=dict(l=0, r=0, b=0, t=0)
+    )
+    fig.update_yaxes(range=[y_range_min, y_range_max])
+    fig.write_html(filename, include_plotlyjs=include_plotlyjs)
+
+
+def log_elapsed_time(msg: str, t0: float) -> float:
+    t1 = time.time()
+    logger.info(msg + f" (took {t1 - t0:2f} s )")
+    return t1
+
+
+def write_to_fits(
+        c: CCD,
+        filename: str | Path,
+        overwrite: bool = True,
+        append: bool = False,
+        dtype: Type | np.dtype = np.uint16,
+        metadata: dict = None,
+):
+    """Saves CCD image to disk
+
+    Args:
+        c: CCD object
+        filename: filepath
+        overwrite: if True, file will be overwritten if existing
+        append: if True, CCD data will be added to data in fits file
+        dtype: numpy.dtype object defining the data type of the saved FITS file, defaulting to unsigned 16-bit integers
+        metadata: dictionary with additional metadata that should be saved to the FITS header
+
+    Returns:
+        None
+    """
+    old_file_data = np.zeros_like(c.data)
+    if append:
+        if pathlib.Path(filename).is_file():
+            old_file_data = fits.getdata(filename)
+            assert old_file_data.shape == c.data.shape, (
+                f"You tried to append data to {filename}, "
+                f"but the fits file contains"
+                f"data with a different shape ({old_file_data.shape})."
+            )
+
+    hdu = fits.PrimaryHDU(data=np.array(c.data + old_file_data, dtype=dtype))
+    # unfortunately, long HIERARCH keywords and long values exclude each other:
+    # see
+    # https://stackoverflow.com/questions/29950918/astropy-io-fits-hierarch-keywords-dont-work-with-continue-cards-bug-or-feat
+    # therefore, we add short meaningless keywords.
+    if metadata is not None:
+        for i, (key, value) in enumerate(metadata.items()):
+            hdu.header.set(f"PYE{i}", f"{key}: {str(value)}")
+
+    hdu_list = fits.HDUList([hdu])
+    hdu_list.writeto(filename, overwrite=overwrite or append)
+
+
+@dataclass
+class Simulator:
+    """PyEchelle simulator
+
+    Simulator class that contains everything needed to generate spectra.
+
+    Attributes:
+        spectrograph (Spectrograph): spectrograph used for simulations
+        fibers (list[int]): fiber / list of fibers to be simulated
+        orders (list[int]): order / list of diffraction orders to be simulated
+        sources (list[Source]): spectral source / list of spectral sources per fiber (same length as fibers)
+        atmosphere (list[bool]): whether to include atmospheric transmission per fiber (same length as fibers)
+        atmosphere_conditions (list[dict | None]): skycalc arguments for atmospheric conditions (same length as sources)
+        rvs (list[float]): radial velocity shifts in [m/s] for sources (same length as fibers)
+        telescope (Telescope): Telescope used for simulations (relevant for 'on-sky' sources)
+        random_seed (int): random seed for the number generator
+        cuda (bool): flat if CUDA is to be used
+        max_cpu (int): number of CPUs used for simulation (if -1, max_cpu is number of available cores)
+        exp_time (float): exposure time to be simulated
+        output (Path): path to output fits file
+        append (bool): flag if simulated counts should be appended to existing image
+        overwrite (bool): flat if output file should be overwritten if existing
+        global_efficiency (Efficiency): overall efficiency curve to be considered
+         (on top of spectrograph efficiency curve and potentially atmosphere)
+
+    """
+
+    spectrograph: Spectrograph
+    fibers: list[int] = field(init=False, default=None)
+    orders: list[int] = field(init=False, default=None)
+    ccd: int = field(init=False, default=None)
+    sources: list[Source] = field(init=False, default=None)
+    atmosphere: list[bool] = field(init=False, default=None)
+    atmosphere_conditions: list[dict | None] = field(init=False, default=None)
+    rvs: list[float] = field(init=False, default=None)
+    telescope: Telescope = field(init=False, default=None)
+    random_seed: int = field(init=False, default=-1)
+    cuda: bool = field(init=False, default=False)
+    max_cpu: int = field(init=False, default=1)
+    exp_time: float = field(init=False, default=1.0)
+    output: Path = field(init=False, default=None)
+    append: bool = field(init=False, default=False)
+    overwrite: bool = field(init=False, default=False)
+    bias: int = field(init=False, default=0)
+    read_noise: float = field(init=False, default=0.0)
+    global_efficiency: Efficiency = field(init=False, default=None)
+
+    def set_sources(self, source: Source | list[Source]):
+        assert (
+                self.fibers is not None
+        ), "Please set first the fields that you want to simulate."
+        self.sources = (
+            source if isinstance(source, list) else [source] * len(self.fibers)
+        )
+        assert len(self.fibers) == len(
+            self.sources
+        ), "Number of sources needs to match the number of fields/fibers (or be 1)"
+
+    def set_atmospheres(
+            self, atmosphere: bool | list[bool], sky_calc_kwargs: dict | list[dict] = None
+    ):
+        assert (
+                self.sources is not None
+        ), "Please set first the sources that you want to simulate."
+        self.atmosphere = (
+            [atmosphere] * len(self.sources)
+            if isinstance(atmosphere, bool)
+            else atmosphere
+        )
+        self.atmosphere_conditions = (
+            [sky_calc_kwargs] * len(self.sources)
+            if (isinstance(sky_calc_kwargs, dict) or sky_calc_kwargs is None)
+            else sky_calc_kwargs
+        )
+        assert len(self.atmosphere) == len(
+            self.sources
+        ), "Number of atmosphere flags needs to match the number of sources (or be 1)"
+        assert (
+                len(self.atmosphere_conditions) == len(self.sources)
+        ), "Number of atmosphere condition arguments needs to match the number of sources (or be 1)"
+
+    def set_radial_velocities(self, rvs: float | list[float]):
+        assert (
+                self.sources is not None
+        ), "Please set first the sources that you want to simulate."
+        self.rvs = [rvs] * len(self.sources) if isinstance(rvs, float) else rvs
+        assert (
+                len(self.rvs) == len(self.sources)
+        ), "Number of radial velocity values needs to match the number of sources (or be 1)"
+
+    def set_telescope(self, telescope: Telescope):
+        self.telescope = telescope
+
+    def set_ccd(self, ccd: int):
+        self.ccd = ccd
+        assert self.ccd in self.spectrograph.get_ccd().keys(), (
+            f"You requested simulation of CCD {ccd}, " f"which is not available."
+        )
+
+    def set_efficiency(self, eff: Efficiency):
+        assert isinstance(eff, Efficiency)
+        self.global_efficiency = eff
+
+    def set_bias(self, bias_value: int = 0):
+        self.bias = bias_value
+
+    def set_read_noise(self, read_noise: float = 0.0):
+        if read_noise > 0.0:
+            assert self.bias > 0, (
+                "read noise was specified, but no bias value is set, yet. "
+                "Do so before setting the read noise."
+            )
+        self.read_noise = read_noise
+
+    def set_fibers(self, fiber: int | list[int]):
+        assert self.ccd is not None, "Please set CCD index first."
+        self.fibers = [fiber] if isinstance(fiber, int) else fiber
+        for f in self.fibers:
+            assert f in self.spectrograph.get_fibers(self.ccd), (
+                f"You requested simulation of fiber {f}, which is "
+                f"not available for ccd with index {self.ccd}"
+            )
+
+    def set_cuda(self, activate: bool = True, seed: int = -1):
+        self.cuda = activate
+        self.random_seed = seed
+
+    def _get_valid_orders(self, fiber: int):
+        valid_orders = []
+
+        requested_orders = (
+            self.spectrograph.get_orders(fiber, self.ccd)
+            if self.orders is None
+            else self.orders
+        )
+        for o in requested_orders:
+            if o in self.spectrograph.get_orders(fiber, self.ccd):
+                valid_orders.append(o)
+            else:
+                logger.warning(
+                    f"Order {o} is requested, but it is not in the Spectrograph model."
+                )
+        return valid_orders
+
+    def _get_slit_function(self, fiber: int):
+        try:
+            if self.cuda:
+                slit_fun = getattr(
+                    pyechelle.slit,
+                    f"cuda_{self.spectrograph.get_field_shape(fiber, self.ccd)}",
+                )
+            else:
+                slit_fun = getattr(
+                    pyechelle.slit, self.spectrograph.get_field_shape(fiber, self.ccd)
+                )
+        except AttributeError:
+            raise NotImplementedError(
+                f"Field shape {self.spectrograph.get_field_shape(fiber, self.ccd)} is not implemented."
+            )
+        return slit_fun
+
+    def _simulate_multi_cpu(
+            self, orders, fiber, ccd_index, slit_fun, s, rv, integration_time, c, efficiency
+    ):
+        simulated_photons = []
+        t0 = time.time()
+        results = Parallel(n_jobs=min(self.max_cpu, len(orders)), backend="threading")(
+            delayed(raytrace_order_cpu)(
+                o,
+                self.spectrograph,
+                s,
+                slit_fun,
+                self.telescope,
+                rv,
+                integration_time,
+                c,
+                fiber,
+                ccd_index,
+                efficiency,
+                self.max_cpu,
+            )
+            for o in np.sort(orders)
+        )
+        logger.info("Add up orders...")
+        ccd_results = [r[0] for r in results]
+        simulated_photons.extend([r[1] for r in results])
+        c.data = np.sum(ccd_results, axis=0)
+        log_elapsed_time("done.", t0)
+        return simulated_photons
+
+    def _simulate_single_cpu(
+            self, orders, fiber, ccd_index, s, slit_fun, rv, integration_time, c, efficiency
+    ):
+        simulated_photons = []
+        for o in np.sort(orders):
+            n_phot = raytrace_order_cpu(
+                o,
+                self.spectrograph,
+                s,
+                slit_fun,
+                self.telescope,
+                rv,
+                integration_time,
+                c,
+                fiber,
+                ccd_index,
+                efficiency,
+                1,
+            )
+            simulated_photons.append(n_phot)
+        return simulated_photons
+
+    def _simulate_cuda(
+            self,
+            orders,
+            slit_fun,
+            rv,
+            integration_time,
+            dccd,
+            efficiency,
+            s,
+            c,
+            fiber,
+            ccd_index,
+    ):
+        if slit_fun is not None:  # multimode
+            cuda_kernel = make_cuda_kernel(slit_fun)
+        else:  # singlemode
+            cuda_kernel = make_cuda_kernel_singlemode()
+        simulated_photons = []
+        for o in np.sort(orders):
+            if self.random_seed < 0:
+                ii16 = np.iinfo(np.uint32)
+                seed = random.randint(1, ii16.max - 1)
+            else:
+                seed = self.random_seed
+            nphot = raytrace_order_cuda(
+                o,
+                self.spectrograph,
+                s,
+                self.telescope,
+                rv,
+                integration_time,
+                dccd,
+                float(c.pixelsize),
+                fiber,
+                ccd_index,
+                efficiency,
+                seed=seed,
+                cuda_kernel=cuda_kernel,
+            )
+            simulated_photons.append(nphot)
+        return simulated_photons
+
+    def validate(self):
+        assert self.fibers is not None, "Please set fibers for simulation"
+        assert self.ccd is not None, "Please set ccd index/indices for simulation"
+        assert self.output is not None, "Please set output path for simulation"
+        if self.atmosphere is None:
+            logger.info(
+                "It was not explicitly specified whether to consider atmospheric transmission. "
+                "It is set to False"
+            )
+            self.atmosphere = [False] * len(self.sources)
+
+        if self.atmosphere_conditions is None:
+            if self.atmosphere:
+                logger.info(
+                    "Atmospheric conditions were not specified. The default atmospheric conditions apply. "
+                    "(e.g. airmass 1)"
+                )
+            self.atmosphere_conditions = [None] * len(self.sources)
+
+        if self.rvs is None:
+            logger.info(
+                "Radial velocities are not specified explicitly. They are therefore set to 0.0"
+            )
+            self.rvs = [0.0] * len(self.sources)
+        if self.output.is_file():
+            assert self.overwrite or self.append, (
+                f"You specified to save the simulation at {self.output}, "
+                f"but this file exists. If you want to overwrite, "
+                f"please set the overwrite flag. Or in case you want to append to "
+                f"the file: please set the append flag"
+            )
+        return True
+
+    def run(self):
+        self.validate()
+        c = self.spectrograph.get_ccd(self.ccd)
+        total_simulated_photons = []
+        t1 = time.time()
+        # copy empty array to CUDA device
+        if self.cuda:
+            dccd = cuda.to_device(np.zeros_like(c.data, dtype=np.uint32))
+        metadata = {
+            "pyechelle.version": pyechelle.__version__,
+            "pyechelle.spectrograph": self.spectrograph.name,
+            "pyechelle.cuda": self.cuda,
+            "pyechelle.seed": self.random_seed,
+            "pyechelle.EXPTIME": self.exp_time,
+            "pyechelle.CCD": self.ccd,
+            "pyechelle.bias": self.bias,
+            "pyechelle.readnoise": self.read_noise,
+            "pyechelle.sim_start_utc": datetime.utcnow().isoformat(),
+        }
+
+        for f, s, atm, atm_cond, rv in zip(
+                self.fibers,
+                self.sources,
+                self.atmosphere,
+                self.atmosphere_conditions,
+                self.rvs,
+        ):
+            orders = (
+                self.orders if self.orders is not None else self._get_valid_orders(f)
+            )
+            slit_fun = self._get_slit_function(f)
+            metadata.update(
+                {
+                    f"pyechelle.fiber{f}.orders": orders,
+                    f"pyechelle.fiber{f}.source": str(s),
+                    f"pyechelle.fiber{f}.rv": rv,
+                    f"pyechelle.fiber{f}.atmosphere": atm,
+                }
+            )
+            # TODO: add also atmospheric keywords to fits header
+
+            e = SystemEfficiency(
+                [
+                    self.spectrograph.get_efficiency(f, self.ccd),
+                    self.global_efficiency,
+                    Atmosphere("Atmosphere", sky_calc_kwargs=atm_cond) if atm else None,
+                ],
+                "Combined Efficiency",
+            )
+
+            if not self.cuda:
+                if self.max_cpu > 1:
+                    total_simulated_photons.extend(
+                        self._simulate_multi_cpu(
+                            orders, f, self.ccd, slit_fun, s, rv, self.exp_time, c, e
+                        )
+                    )
+                else:
+                    total_simulated_photons.extend(
+                        self._simulate_single_cpu(
+                            orders, f, self.ccd, s, slit_fun, rv, self.exp_time, c, e
+                        )
+                    )
+            else:
+                total_simulated_photons.extend(
+                    self._simulate_cuda(
+                        orders, slit_fun, rv, self.exp_time, dccd, e, s, c, f, self.ccd
+                    )
+                )
+
+        if self.cuda:
+            dccd.copy_to_host(c.data)
+        logger.info("Finish up simulation and save...")
+        c.clip()
+
+        # add bias / global ccd effects
+        if self.bias > 0:
+            c.add_bias(self.bias)
+        if self.read_noise > 0.0:
+            c.add_readnoise(self.read_noise)
+        t2 = time.time()
+        metadata.update({"pyechelle.sim_end_utc": datetime.utcnow().isoformat()})
+        write_to_fits(
+            c,
+            self.output,
+            self.overwrite,
+            self.append,
+            dtype=np.uint16,
+            metadata=metadata,
+        )
+        logger.info(f"Total time for simulation: {t2 - t1:.3f}s.")
+        logger.info(f"Total simulated photons: {sum(total_simulated_photons)}")
+        return sum(total_simulated_photons)
+
+    def set_exposure_time(self, exp_time: float = 1):
+        self.exp_time = exp_time
+
+    def set_output(
+            self,
+            path: str | Path = Path().cwd().joinpath("test.fits"),
+            append: bool = False,
+            overwrite: bool = False,
+    ):
+        self.output = path if isinstance(path, Path) else Path(path)
+        self.append = append
+        self.overwrite = overwrite
+        if append and not self.output.is_file():
+            logger.warning(
+                f"You specified that the simulation should be appended to {self.output}, but there is no "
+                f"such file. It will be created."
+            )
+
+    def set_orders(self, orders: int | list[int] | None):
+        if isinstance(orders, int):
+            self.orders = [orders]
+        self.orders = orders
+        if self.orders is not None:
+            for f in self.fibers:
+                valid_orders = self._get_valid_orders(f)
+                for o in self.orders:
+                    assert o in valid_orders, (
+                        f"You requested to simulate order {o}, but this order is not available"
+                        f"on CCD {self.ccd} and fiber/field {f}"
+                    )
+
+
+def generate_parser():
+    parser = argparse.ArgumentParser(
+        description="PyEchelle Simulator",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
+    parser.add_argument(
+        "-s",
+        "--spectrograph",
+        choices=available_models,
+        type=str,
+        default="MaroonX",
+        required=True,
+        help="Filename of spectrograph model. Model file needs to be located in models/ folder. ",
+    )
+    parser.add_argument(
+        "--ccd",
+        type=int,
+        default=1,
+        required=False,
+        help="Sets CCD index to be simulated.",
+    )
+    parser.add_argument(
+        "-t",
+        "--integration_time",
+        type=float,
+        default=1.0,
+        required=False,
+        help="Integration time for the simulation in seconds [s].",
+    )
+    parser.add_argument(
+        "--fiber",
+        type=parse_num_list,
+        required=False,
+        help="Fiber/Field number(s) to be simulated. Can either be a single integer, or an integer"
+             "range (e.g. 1-3) ",
+    )
+    parser.add_argument(
+        "--no_blaze",
+        action="store_true",
+        help="If set, the blaze efficiency per order will be ignored.",
+    )
+    parser.add_argument(
+        "--no_efficiency",
+        action="store_true",
+        help="If set, all instrument/atmosphere efficiencies will be ignored.",
+    )
+
+    parser.add_argument(
+        "--cuda",
+        action="store_true",
+        help="If set, CUDA will be used for raytracing. Note: the max_cpu flag is then obsolete.",
+    )
+
+    parser.add_argument(
+        "--cuda_seed",
+        type=int,
+        default=-1,
+        help="Random seed for generating CUDA RNG states. If <0, then the seed is chosen randomly.",
+    )
+
+    parser.add_argument(
+        "--max_cpu",
+        type=int,
+        default=1,
+        help="Maximum number of CPU cores used. Note: The parallelization happens 'per order'."
+             " Order-wise images are added up. This requires a large amount of memory at the moment."
+             "If planning on simulating multiple images, consider using only 1 CPU per simulation "
+             "and starting multiple simulations instead.",
+    )
+
+    atmosphere_group = parser.add_argument_group("Atmosphere")
+    atmosphere_group.add_argument(
+        "--atmosphere",
+        nargs="+",
+        required=False,
+        help="Add telluric lines to spectrum. For adding tellurics to all spectra just use"
+             "--atmosphere Y, for specifying per fiber user e.g. --atmosphere Y N Y",
+        type=lambda x: str2bool(x),
+        default=[False],
+    )
+
+    atmosphere_group.add_argument(
+        "--airmass",
+        default=1.0,
+        type=float,
+        required=False,
+        help="airmass for atmospheric model",
+    )
+
+    telescope_group = parser.add_argument_group("Telescope settings")
+    telescope_group.add_argument(
+        "--d_primary",
+        type=float,
+        required=False,
+        default=1.0,
+        help="Diameter of the primary telescope mirror.",
+    )
+    telescope_group.add_argument(
+        "--d_secondary",
+        type=float,
+        required=False,
+        default=0,
+        help="Diameter of the secondary telescope mirror.",
+    )
+
+    parser.add_argument(
+        "--orders",
+        type=parse_num_list,
+        nargs="+",
+        required=False,
+        help="Echelle/Grating order numbers to simulate... "
+             "if not specified, all orders of the spectrograph are simulated."
+             "Can either be a single integer, or a range (e.g. 80-90)",
+    )
+
+    parser.add_argument(
+        "--sources",
+        nargs="+",
+        choices=available_sources,
+        required=True,
+        help='Spectral source for the simulation. Can either be a single string, e.g. "Etalon",'
+             ' or a comma separated list of sources (e.g. "Etalon, Constant, Etalon") which length must'
+             "match the number of fields/fibers.",
+    )
+    parser.add_argument(
+        "--rv",
+        nargs="+",
+        type=float,
+        required=False,
+        default=[0.0],
+        help="radial velocity shift of source",
+    )
+    const_source_group = parser.add_argument_group("Constant source")
+    const_source_group.add_argument(
+        "--constant_intensity",
+        type=float,
+        default=0.0001,
+        required=False,
+        help="Flux in microWatts / nanometer for constant flux spectral source",
+    )
+    arclamps_group = parser.add_argument_group("Arc Lamps")
+    arclamps_group.add_argument(
+        "--scale",
+        default=10.0,
+        required=False,
+        help="Intensity scale of gas lines (e.g. Ag or Ne) vs metal (Th)",
+    )
+
+    csv_group = parser.add_argument_group("CSV")
+    csv_group.add_argument(
+        "--csv_filepath",
+        type=argparse.FileType("r"),
+        required=False,
+        help="Path to .csv file that contains two columns: wavelength and flux. The flux is expected"
+             "to be in ergs/s/cm^2/cm (like Phoenix spectra) or photons (then set it via "
+             "--csv_flux_in_photons). The wavelength unit is expected to "
+             "be angstroms, but it can be changed via --csv_wavelength_unit",
+    )
+    csv_group.add_argument(
+        "--csv_wavelength_unit",
+        choices=list(CSV.wavelength_scaling.keys()),
+        default="a",
+        type=str,
+        help=f"Unit of the wavelength column in the .csv file. Options are "
+             f"{list(CSV.wavelength_scaling.keys())}",
+    )
+    csv_group.add_argument(
+        "--csv_list_like",
+        type=bool,
+        default=False,
+        help="Set to True if spectrum is discrete.",
+    )
+    csv_group.add_argument(
+        "--csv_flux_in_photons",
+        type=bool,
+        default=False,
+        help="Set to True if flux is given in Photons/s rather than ergs",
+    )
+    csv_group.add_argument(
+        "--csv_stellar_target",
+        type=bool,
+        default=True,
+        help="Set to True if Source is a stellar target.",
+    )
+    csv_group.add_argument(
+        "--csv_magnitude",
+        type=float,
+        default=10.0,
+        required=False,
+        help="If stellar target, the magnitude value i considered as V magnitude of the object and "
+             "the flux is scaled accordingly. Ignored if --flux_in_photons is true.",
+    )
+    csv_group.add_argument(
+        "--csv_delimiter",
+        type=str,
+        required=False,
+        default=",",
+        help="Delimiter of the CSV file",
+    )
+
+    csv_eff_group = parser.add_argument_group("CSVEfficiency")
+    csv_eff_group.add_argument(
+        "--eff_csv_filepath",
+        type=argparse.FileType("r"),
+        required=False,
+        help="Path to .csv file that contains two columns: wavelength and efficiency."
+             "The wavelength is expected to be in microns, "
+             "the efficiency is a real number in [0,1]."
+             "PyEchelle will interpolate the given values "
+             "for intermediate wavelength positions.",
+    )
+    csv_eff_group.add_argument(
+        "--eff_csv_delimiter",
+        type=str,
+        required=False,
+        default=",",
+        help="Delimiter of the CSV file",
+    )
+
+    phoenix_group = parser.add_argument_group("Phoenix")
+    phoenix_group.add_argument(
+        "--phoenix_t_eff",
+        default=3600,
+        choices=Phoenix.valid_t,
+        type=int,
+        required=False,
+        help="Effective temperature in Kelvins [K].",
+    )
+    phoenix_group.add_argument(
+        "--phoenix_log_g",
+        default=5.0,
+        choices=Phoenix.valid_g,
+        type=float,
+        required=False,
+        help="Surface gravity log g.",
+    )
+    phoenix_group.add_argument(
+        "--phoenix_z",
+        choices=Phoenix.valid_z,
+        type=float,
+        required=False,
+        default=0.0,
+        help="Overall metallicity.",
+    )
+    phoenix_group.add_argument(
+        "--phoenix_alpha",
+        choices=Phoenix.valid_a,
+        type=float,
+        required=False,
+        default=0.0,
+        help="Alpha element abundance.",
+    )
+    phoenix_group.add_argument(
+        "--phoenix_magnitude",
+        default=10.0,
+        required=False,
+        type=float,
+        help="V Magnitude of stellar object.",
+    )
+
+    etalon_group = parser.add_argument_group("Etalon")
+    etalon_group.add_argument(
+        "--etalon_d",
+        type=float,
+        default=5.0,
+        required=False,
+        help="Mirror distance of Fabry Perot etalon in [mm].",
+    )
+    etalon_group.add_argument(
+        "--etalon_n",
+        type=float,
+        default=1.0,
+        required=False,
+        help="Refractive index of medium between etalon mirrors.",
+    )
+    etalon_group.add_argument(
+        "--etalon_theta",
+        type=float,
+        default=0.0,
+        required=False,
+        help="angle of incidence of light in radians.",
+    )
+    etalon_group.add_argument(
+        "--etalon_n_photons",
+        default=1000,
+        required=False,
+        help="Number of photons per seconds per peak of the etalon spectrum.",
+    )
+
+    ccd_group = parser.add_argument_group("CCD")
+    ccd_group.add_argument("--bias", type=int, required=False, default=0)
+    ccd_group.add_argument("--read_noise", type=float, required=False, default=0.0)
+
+    parser.add_argument(
+        "--show",
+        default=False,
+        action="store_true",
+        help="If set, the simulated frame will be shown in a matplotlib imshow frame at the end.",
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=lambda p: Path(p).absolute(),
+        required=False,
+        default=Path(__file__).absolute().parent / "test.fits",
+        help="A .fits file where the simulation is saved.",
+    )
+    parser.add_argument(
+        "--overwrite",
+        default=False,
+        action="store_true",
+        help="If set, the output file will be overwritten if it exists already.",
+    )
+    parser.add_argument(
+        "--append",
+        default=False,
+        action="store_true",
+        help="If set, the simulated photons will be added to the output file rather than overwriting "
+             "the content of the output file. If the output file does not exist yet, "
+             "it will be created.This flag can be used to do more complex multi-fiber simulations as a"
+             " sequential manner of simpler simulations.",
+    )
+
+    parser.add_argument(
+        "--html_export",
+        type=str,
+        default="",
+        help="If given, the spectrum will be exported to an interactive image using plotly. It's not a"
+             "standalone html file, but requires plotly.js to be loaded.",
+    )
+    return parser
+
+
+def main(args=None):
+    if not args:
+        args = sys.argv[1:]
+    parser = generate_parser()
+    args = parser.parse_args(args)
+    t1 = time.time()
+    sim = Simulator(ZEMAX(args.spectrograph))
+    sim.set_ccd(args.ccd)
+
+    # generate flat list for all fields to simulate
+    if args.fiber is not None:
+        if any(isinstance(el, list) for el in args.fiber):
+            fibers = [item for sublist in args.fiber for item in sublist]
+        else:
+            fibers = args.fiber
+    else:
+        fibers = sim.spectrograph.get_fibers(args.ccd)
+    sim.set_fibers(fibers)
+
+    if args.orders is not None:
+        if any(isinstance(el, list) for el in args.orders):
+            requested_orders = [item for sublist in args.orders for item in sublist]
+        else:
+            requested_orders = args.orders
+        sim.set_orders(requested_orders)
+    # generate flat list of all sources to simulate
+    source_names = args.sources
+    if len(source_names) == 1:
+        source_names = [source_names[0]] * len(
+            fibers
+        )  # generate list of same length as 'fields' if only one source given
+
+    source_kwargs = []
+    # extract kwords specific to selected source
+    for s in source_names:
+        source_args = [ss for ss in vars(args) if ss.startswith(s.lower())]
+        # create dict consisting of kword arguments and values specific to selected source
+        source_kwargs.append(
+            dict(
+                zip(
+                    [ss.replace(f"{s.lower()}_", "") for ss in source_args],
+                    [getattr(args, ss) for ss in source_args],
+                )
+            )
+        )
+
+    sim.set_sources(
+        [
+            getattr(sources, source)(**s_args)
+            for source, s_args in zip(source_names, source_kwargs)
+        ]
+    )
+
+    if args.eff_csv_filepath:
+        sim.set_efficiency(
+            CSVEfficiency("global", args.eff_csv_filepath, args.eff_csv_delimiter)
+        )
+    # generate flat list of whether atmosphere is added
+    sim.set_atmospheres(
+        args.atmosphere[0] if len(args.atmosphere) == 1 else args.atmosphere
+    )
+    sim.set_radial_velocities(args.rv[0] if len(args.rv) == 1 else args.rv)
+    sim.set_cuda(args.cuda, args.cuda_seed)
+    sim.set_exposure_time(args.integration_time)
+    sim.set_telescope(Telescope(args.d_primary, args.d_secondary))
+    sim.set_output(args.output, args.append, args.overwrite)
+    sim.set_bias(args.bias)
+    sim.set_read_noise(args.read_noise)
+    sim.run()
+    t2 = time.time()
+    print(f"Simulation took {t2 - t1:.3f} s")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pyechelle-0.3.6/pyechelle/slit.py` & `pyechelle-0.3.7/pyechelle/slit.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,154 +1,158 @@
-""" Slit transformation functions
-
-This module implements various coordinate transformations for implementing different slit shapes such as circular,
-octagonal etc.
-Both, numba compiled functions and cuda device functions are implemented.
-
-In general, a slit function transforms a random coordinate x, y (both from the interval [0, 1]) to a random coordinate
-x', y'
-
-A special case is the 'singlemode' slit, since here, no transformation is required.
-
-
-.. plot::
-
-    import matplotlib.pyplot as plt
-    import random
-    import numpy
-    import pyechelle.slit
-    import inspect
-    from numba.core.registry import CPUDispatcher
-
-    available_slits = [m[0] for m in inspect.getmembers(pyechelle.slit) if isinstance(m[1], CPUDispatcher)]
-
-
-    fig, ax = plt.subplots(1, len(available_slits), sharey=True, sharex=True,figsize=(len(available_slits)*3, 3))
-    fig.suptitle('Supported slit functions')
-    for i, slit in enumerate(available_slits):
-        s = getattr(pyechelle.slit, slit)
-        xy = [s(random.random(), random.random()) for _ in range(2000)]
-        ax[i].scatter(*numpy.array(xy).T, s=1)
-        ax[i].set_aspect('equal', 'box')
-        ax[i].set_title(slit)
-    plt.tight_layout()
-    plt.show()
-
-"""
-import math
-import random
-
-import numba.cuda.random
-from numba import njit, float64, cuda
-from numba.types import UniTuple
-
-# single mode slit just return 'None'
-singlemode = None
-cuda_singlemode = None
-
-
-@njit(UniTuple(float64, 2)(float64, float64))
-def rectangular(xx, yy):
-    """ Rectangular transformation
-    """
-    return xx, yy
-
-
-@njit(UniTuple(float64, 2)(float64, float64))
-def circular(xx, yy):
-    """ Circular transformation
-    """
-    r = math.sqrt(xx) / 2.
-    phi = yy * math.pi * 2
-    return r * math.cos(phi) + 0.5, r * math.sin(phi) + 0.5
-
-
-@njit(UniTuple(float64, 2)(float64, float64))
-def octagonal(r1, r2):
-    """ Octagonal transformation
-    """
-    phi = 0.
-    s1 = math.sqrt(r1)
-    phi_segment = 2. * math.pi / 8
-
-    b = [1., 0.]
-    c = [math.cos(phi_segment), math.sin(phi_segment)]
-    x = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
-    y = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
-
-    segments = random.randint(0, 7)
-    arg_values = phi_segment * segments + phi
-    cos_values = math.cos(arg_values)
-    sin_values = math.sin(arg_values)
-    x_new = x * cos_values - y * sin_values
-    y_new = x * sin_values + y * cos_values
-    return x_new / 2. + 0.5, y_new / 2. + 0.5
-
-
-@njit(UniTuple(float64, 2)(float64, float64))
-def hexagonal(r1, r2):
-    """ Hexagonal transformation
-    """
-    phi = 0.
-    s1 = math.sqrt(r1)
-    phi_segment = 2. * math.pi / 6
-
-    b = [1., 0.]
-    c = [math.cos(phi_segment), math.sin(phi_segment)]
-    x = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
-    y = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
-
-    segments = random.randint(0, 5)
-    arg_values = phi_segment * segments + phi
-    cos_values = math.cos(arg_values)
-    sin_values = math.sin(arg_values)
-    xnew = x * cos_values - y * sin_values
-    ynew = x * sin_values + y * cos_values
-    return xnew / 2. + 0.5, ynew / 2. + 0.5
-
-
-@cuda.jit(inline=True, device=True)
-def cuda_rectangular(x, y, rng_states, thread_id):
-    return x, y
-
-
-@cuda.jit(inline=True, device=True)
-def cuda_circular(x, y, rng_states, thread_id):
-    r = math.sqrt(x) / 2.
-    phi = y * math.pi * 2
-    return r * math.cos(phi) + 0.5, r * math.sin(phi) + 0.5
-
-
-@cuda.jit(inline=True, device=True)
-def cuda_octagonal(r1, r2, rng_states, thread_id):
-    phi = 0.
-    s1 = math.sqrt(r1)
-    phi_segment = 2. * math.pi / 8.
-
-    b = (1., 0.)
-    c = (math.cos(phi_segment), math.sin(phi_segment))
-    xx = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
-    yy = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
-
-    segments = math.floor(numba.cuda.random.xoroshiro128p_uniform_float64(rng_states, thread_id) * 8.)
-    arg_values = phi_segment * segments + phi
-    cos_values = math.cos(arg_values)
-    sin_values = math.sin(arg_values)
-    return (xx * cos_values - yy * sin_values) / 2. + 0.5, (xx * sin_values + yy * cos_values) / 2. + 0.5
-
-
-@cuda.jit(inline=True, device=True)
-def cuda_hexagonal(r1, r2, rng_states, thread_id):
-    phi = 0.
-    s1 = math.sqrt(r1)
-    phi_segment = 2. * math.pi / 6.
-
-    b = (1., 0.)
-    c = (math.cos(phi_segment), math.sin(phi_segment))
-    xx = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
-    yy = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
-
-    segments = math.floor(numba.cuda.random.xoroshiro128p_uniform_float64(rng_states, thread_id) * 6.)
-    arg_values = phi_segment * segments + phi
-    cos_values = math.cos(arg_values)
-    sin_values = math.sin(arg_values)
-    return (xx * cos_values - yy * sin_values) / 2. + 0.5, (xx * sin_values + yy * cos_values) / 2. + 0.5
+""" Slit transformation functions
+
+This module implements various coordinate transformations for implementing different slit shapes such as circular,
+octagonal etc.
+Both, numba compiled functions and cuda device functions are implemented.
+
+In general, a slit function transforms a random coordinate x, y (both from the interval [0, 1]) to a random coordinate
+x', y'
+
+A special case is the 'singlemode' slit, since here, no transformation is required.
+
+
+.. plot::
+
+    import matplotlib.pyplot as plt
+    import random
+    import numpy
+    import pyechelle.slit
+    import inspect
+    from numba.core.registry import CPUDispatcher
+
+    available_slits = [m[0] for m in inspect.getmembers(pyechelle.slit) if isinstance(m[1], CPUDispatcher)]
+
+
+    fig, ax = plt.subplots(1, len(available_slits), sharey=True, sharex=True,figsize=(len(available_slits)*3, 3))
+    fig.suptitle('Supported slit functions')
+    for i, slit in enumerate(available_slits):
+        s = getattr(pyechelle.slit, slit)
+        xy = [s(random.random(), random.random()) for _ in range(2000)]
+        ax[i].scatter(*numpy.array(xy).T, s=1)
+        ax[i].set_aspect('equal', 'box')
+        ax[i].set_title(slit)
+    plt.tight_layout()
+    plt.show()
+
+"""
+import math
+import random
+
+import numba.cuda.random
+from numba import njit, float64, cuda
+from numba.types import UniTuple
+
+# single mode slit just return 'None'
+singlemode = None
+cuda_singlemode = None
+
+
+@njit(UniTuple(float64, 2)(float64, float64))
+def rectangular(xx, yy):
+    """Rectangular transformation"""
+    return xx, yy
+
+
+@njit(UniTuple(float64, 2)(float64, float64))
+def circular(xx, yy):
+    """Circular transformation"""
+    r = math.sqrt(xx) / 2.0
+    phi = yy * math.pi * 2
+    return r * math.cos(phi) + 0.5, r * math.sin(phi) + 0.5
+
+
+@njit(UniTuple(float64, 2)(float64, float64))
+def octagonal(r1, r2):
+    """Octagonal transformation"""
+    phi = 0.0
+    s1 = math.sqrt(r1)
+    phi_segment = 2.0 * math.pi / 8
+
+    b = [1.0, 0.0]
+    c = [math.cos(phi_segment), math.sin(phi_segment)]
+    x = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
+    y = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
+
+    segments = random.randint(0, 7)
+    arg_values = phi_segment * segments + phi
+    cos_values = math.cos(arg_values)
+    sin_values = math.sin(arg_values)
+    x_new = x * cos_values - y * sin_values
+    y_new = x * sin_values + y * cos_values
+    return x_new / 2.0 + 0.5, y_new / 2.0 + 0.5
+
+
+@njit(UniTuple(float64, 2)(float64, float64))
+def hexagonal(r1, r2):
+    """Hexagonal transformation"""
+    phi = 0.0
+    s1 = math.sqrt(r1)
+    phi_segment = 2.0 * math.pi / 6
+
+    b = [1.0, 0.0]
+    c = [math.cos(phi_segment), math.sin(phi_segment)]
+    x = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
+    y = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
+
+    segments = random.randint(0, 5)
+    arg_values = phi_segment * segments + phi
+    cos_values = math.cos(arg_values)
+    sin_values = math.sin(arg_values)
+    xnew = x * cos_values - y * sin_values
+    ynew = x * sin_values + y * cos_values
+    return xnew / 2.0 + 0.5, ynew / 2.0 + 0.5
+
+
+@cuda.jit(inline=True, device=True)
+def cuda_rectangular(x, y, rng_states, thread_id):
+    return x, y
+
+
+@cuda.jit(inline=True, device=True)
+def cuda_circular(x, y, rng_states, thread_id):
+    r = math.sqrt(x) / 2.0
+    phi = y * math.pi * 2
+    return r * math.cos(phi) + 0.5, r * math.sin(phi) + 0.5
+
+
+@cuda.jit(inline=True, device=True)
+def cuda_octagonal(r1, r2, rng_states, thread_id):
+    phi = 0.0
+    s1 = math.sqrt(r1)
+    phi_segment = 2.0 * math.pi / 8.0
+
+    b = (1.0, 0.0)
+    c = (math.cos(phi_segment), math.sin(phi_segment))
+    xx = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
+    yy = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
+
+    segments = math.floor(
+        numba.cuda.random.xoroshiro128p_uniform_float64(rng_states, thread_id) * 8.0
+    )
+    arg_values = phi_segment * segments + phi
+    cos_values = math.cos(arg_values)
+    sin_values = math.sin(arg_values)
+    return (xx * cos_values - yy * sin_values) / 2.0 + 0.5, (
+        xx * sin_values + yy * cos_values
+    ) / 2.0 + 0.5
+
+
+@cuda.jit(inline=True, device=True)
+def cuda_hexagonal(r1, r2, rng_states, thread_id):
+    phi = 0.0
+    s1 = math.sqrt(r1)
+    phi_segment = 2.0 * math.pi / 6.0
+
+    b = (1.0, 0.0)
+    c = (math.cos(phi_segment), math.sin(phi_segment))
+    xx = b[0] * (1.0 - r2) * s1 + c[0] * r2 * s1
+    yy = b[1] * (1.0 - r2) * s1 + c[1] * r2 * s1
+
+    segments = math.floor(
+        numba.cuda.random.xoroshiro128p_uniform_float64(rng_states, thread_id) * 6.0
+    )
+    arg_values = phi_segment * segments + phi
+    cos_values = math.cos(arg_values)
+    sin_values = math.sin(arg_values)
+    return (xx * cos_values - yy * sin_values) / 2.0 + 0.5, (
+        xx * sin_values + yy * cos_values
+    ) / 2.0 + 0.5
```

### Comparing `pyechelle-0.3.6/pyechelle/sources.py` & `pyechelle-0.3.7/pyechelle/sources.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,470 +1,611 @@
-""" Spectral sources
-
-Implementing various spectral sources that can be used in pyechelle.
-
-.. plot::
-
-    import matplotlib.pyplot as plt
-    import numpy as np
-    import pyechelle.sources as sources
-    from pyechelle.simulator import available_sources
-
-    available_sources.remove('CSV')
-
-    fig, ax = plt.subplots(len(available_sources), 1, figsize=(9, len(available_sources) * 2.5), sharex=True)
-    fig.suptitle('Supported source functions')
-    for i, source_name in enumerate(available_sources):
-        wavelength = np.linspace(0.4999, 0.501, 1000, dtype=float)
-        source = getattr(sources, source_name)()
-        sd = source.get_spectral_density(wavelength)
-        if source.list_like:
-            if isinstance(sd, tuple):
-                ax[i].vlines(sd[0], [0]*len(sd[1]), sd[1])
-            else:
-                ax[i].vlines(wavelength, [0]*len(sd), sd)
-        else:
-            if isinstance(sd, tuple):
-                ax[i].plot(*sd)
-            else:
-                ax[i].plot(wavelength, sd)
-        ax[i].set_title(source_name)
-        ax[i].set_ylabel("")
-        ax[i].set_yticks([])
-    ax[-1].set_xlabel("Wavelength [microns]")
-    plt.tight_layout()
-    plt.show()
-"""
-from __future__ import annotations
-
-import io
-import pathlib
-import urllib.request
-
-import astropy.io.fits as fits
-import astropy.units as u
-import numpy as np
-import pandas as pd
-import scipy.interpolate
-from joblib import Memory
-from synphot import SourceSpectrum, SpectralElement, BlackBodyNorm1D, units
-
-try:
-    from astroquery.nist import Nist
-except ImportError:
-    Nist = None
-
-path = pathlib.Path(__file__).parent.resolve()
-cache_path = path.joinpath('.cache')
-# create data directory if it doesn't exist:
-pathlib.Path(cache_path).mkdir(parents=False, exist_ok=True)
-memory = Memory(cache_path, verbose=0)
-
-
-@memory.cache
-def pull_catalogue_lines(min_wl: float, max_wl: float, catalogue: str = 'Th', wavelength_type: str = 'vacuum'):
-    """
-    Reads NIST catalogue lines between min_wl and max_wl of catalogue.
-
-    Args:
-        min_wl: minimum wavelength bound [micron]
-        max_wl: maximum wavelength bound [micron]
-        catalogue: catalogue appreciation label, e.g. 'Th', 'Ar', etc.
-        wavelength_type: either 'var+air' or 'vacuum'
-
-    Returns:
-        (tuple) line catalogue wavelength and relative intensities. wavelength is in [angstrom]
-    """
-    try:
-        table_lines = Nist.query(min_wl * u.micron, max_wl * u.micron, linename=catalogue, output_order='wavelength',
-                                 wavelength_type=wavelength_type)[['Ritz', 'Rel.']]
-        df = table_lines.filled(0).to_pandas()
-        df['Rel.'] = pd.to_numeric(df['Rel.'], downcast='float', errors='coerce')
-        df['Ritz'] = pd.to_numeric(df['Ritz'], downcast='float', errors='coerce')
-        df.dropna(inplace=True)
-        idx = np.logical_and(df['Rel.'] > 0, df['Ritz'] > 0)
-        return df['Ritz'].values[idx], df['Rel.'].values[idx]
-    except Exception as e:
-        print(e)
-        print(f"Warning: Couldn't retrieve {catalogue} catalogue data between {min_wl} and {max_wl} micron")
-        return np.array([]), np.array([])
-
-
-def calc_flux_scale(source_wavelength, source_spectral_density, mag):
-    # V - band-filter
-    v_filter_wl = [0.47, 0.48, 0.49, 0.5, 0.51, 0.52, 0.53, 0.54, 0.55, 0.56, 0.57, 0.58, 0.59, 0.6,
-                   0.61, 0.62, 0.63, 0.64, 0.65, 0.66, 0.67, 0.68, 0.69, 0.7]
-    v_filter_tp = [0, 0.03, 0.163, 0.458, 0.78, 0.967, 1, 0.973, 0.898, 0.792, 0.684, 0.574, 0.461,
-                   0.359, 0.27, 0.197, 0.135, 0.081, 0.045, 0.025, 0.017, 0.013, 0.009, 0]
-
-    # Reference flux obtained from integration of vega over bessel filter (units are microwatts/m^2*micrometer)
-    v_zp = 3.68E-02
-
-    v_filter_interp = scipy.interpolate.interp1d(v_filter_wl, v_filter_tp)
-
-    # get total flux in filter/source range
-    lower_wl_limit = max(np.min(source_wavelength), np.min(v_filter_wl))
-    upper_wl_limit = min(np.max(source_wavelength), np.max(v_filter_wl))
-
-    idx = np.logical_and(source_wavelength > lower_wl_limit, source_wavelength < upper_wl_limit)
-
-    step = np.ediff1d(source_wavelength[idx], source_wavelength[idx][-1] - source_wavelength[idx][-2])
-    total_flux = np.sum(source_spectral_density[idx] * v_filter_interp(source_wavelength[idx]) * step)
-
-    return pow(10, mag / (-2.5)) * v_zp / total_flux
-
-
-class Source:
-    """ A spectral source.
-
-    This class should be subclassed to implement different spectral sources.
-
-    Attributes:
-        name (str): name of the source. This will end up in the .fits header.
-        min_wl (float): lower wavelength limit [nm] (for normalization purposes)
-        max_wl (float): upper wavelength limit [nm] (for normalization purposes)
-        list_like (bool): if True, the Source has a bunch of discrete wavelength, rather than a continuous spectral
-        density.
-        flux_in_photons (bool): if True, get_spectral_density() returns flux in photons rather than micro watts
-
-    """
-
-    def __init__(self, min_wl=599.8, max_wl=600.42, name="", list_like=False, flux_in_photons=False,
-                 stellar_target=False):
-        self.name = name
-        self.min_wl = min_wl
-        self.max_wl = max_wl
-        self.stellar_target = stellar_target
-        self.flux_in_photons = flux_in_photons
-        self.list_like = list_like
-
-    def get_spectral_density(self, wavelength):
-        raise NotImplementedError()
-
-    def get_spectral_density_rv(self, wavelength, rv=0.):
-        c = 299792458.  # m/s
-        rv_shifted = wavelength * ((c - rv) / c)
-
-        spec_density = self.get_spectral_density(rv_shifted)
-        # first case: source returns own wavelength vector:
-        if isinstance(spec_density, tuple):
-            wl, sd = spec_density
-            return wl * ((c - rv) / c), sd
-        else:
-            return spec_density
-
-
-class Constant(Source):
-    """ Constant spectral density.
-
-    Implements a constant spectral density with given intensity [microW / microns*s]
-
-    """
-
-    def __init__(self, intensity=0.001, **kwargs):
-        super().__init__(**kwargs, name="Constant", list_like=False)
-        self.intensity = intensity
-
-    def get_spectral_density(self, wavelength):
-        return np.ones_like(wavelength) * self.intensity
-
-
-class ConstantPhotons(Source):
-    """ Constant spectral density.
-
-    Implements a constant photon flux density with given intensity [photons / microns*s]
-
-    """
-
-    def __init__(self, intensity=1000, **kwargs):
-        super().__init__(**kwargs, name="ConstantPhotons", list_like=False)
-        self.intensity = intensity
-        self.flux_in_photons = True
-        self.stellar_target = False
-
-    def get_spectral_density(self, wavelength):
-        return np.ones_like(wavelength) * self.intensity
-
-
-class ThAr(Source):
-    """ Thorium-Argon lamp
-
-    Implements a Thorium Argon arc-lamp.
-    Uses NIST vacuum catalogue wavelength as source.
-
-    Attributes:
-         scale (float): relative intensity scaling factor between the Thorium and the Argon lines.
-
-    """
-
-    def __init__(self, argon_to_thorium_factor=10):
-        super().__init__(name='ThAr', list_like=True)
-        self.flux_in_photons = True
-        self.scale = argon_to_thorium_factor
-
-    def get_spectral_density(self, wavelength):
-        minwl = np.min(wavelength)
-        maxwl = np.max(wavelength)
-        thwl, thint = pull_catalogue_lines(minwl, maxwl, 'Th')
-        arwl, arint = pull_catalogue_lines(minwl, maxwl, 'Ar')
-        arint *= self.scale
-        return np.hstack((thwl / 10000., arwl / 10000.)), np.hstack((thint, arint))
-
-
-class ThNe(Source):
-    """ Thorium-Neon lamp
-
-    Implements a Thorium Neon arc-lamp.
-    Uses NIST vacuum catalogue wavelength as source.
-
-    Attributes:
-         scale (float): relative intensity scaling factor between the Thorium and the Neon lines.
-
-    """
-
-    def __init__(self, neon_to_thorium_factor=10):
-        super().__init__(name='ThNe', list_like=True)
-        self.flux_in_photons = True
-        self.scale = neon_to_thorium_factor
-
-    def get_spectral_density(self, wavelength):
-        minwl = np.min(wavelength)
-        maxwl = np.max(wavelength)
-        thwl, thint = pull_catalogue_lines(minwl, maxwl, 'Th')
-        newl, neint = pull_catalogue_lines(minwl, maxwl, 'Ne')
-        neint *= self.scale
-
-        return np.hstack((thwl / 10000., newl / 10000.)), np.hstack((thint, neint))
-
-
-class Etalon(Source):
-    r""" Fabry-Perot etalon.
-
-    Implements spectrum of an ideal (i.e. dispersion-free) Fabry-Perot etalon.
-    This means, the peak wavelength are at:
-
-    .. math::
-        \lambda_{peak} = \frac{d \cdot n \cdot \cos{(\theta)}}{m}
-
-    Attributes:
-        d (float): mirror distance [mm]
-        n (float): refractive index between mirrors
-        theta (float): angle of incidence onto mirrors
-        min_m (int): minimum peak interference number
-        max_m (int): maximum peak interference number
-        n_photons (int): number of photons per peak per second
-
-    """
-
-    def __init__(self, d=5.0, n=1.0, theta=0.0, n_photons=1000, **kwargs):
-        super().__init__(**kwargs, name="Etalon", list_like=True)
-        self.d = d
-        self.n = n
-        self.theta = theta
-        self.min_m = np.ceil(2e3 * d * np.cos(theta) / self.max_wl)
-        self.max_m = np.floor(2e3 * d * np.cos(theta) / self.min_wl)
-        self.n_photons = n_photons
-        self.flux_in_photons = True
-
-    @staticmethod
-    def peak_wavelength_etalon(m, d=10.0, n=1.0, theta=0.0):
-        return 2e3 * d * n * np.cos(theta) / m
-
-    def get_spectral_density(self, wavelength):
-        self.min_m = np.ceil(2e3 * self.d * np.cos(self.theta) / np.max(wavelength))
-        self.max_m = np.floor(2e3 * self.d * np.cos(self.theta) / np.min(wavelength))
-        intensity = np.ones_like(np.arange(self.min_m, self.max_m), dtype=float) * float(self.n_photons)
-        return self.peak_wavelength_etalon(
-            np.arange(self.min_m, self.max_m), self.d, self.n, self.theta
-        ), np.asarray(intensity, dtype=int)
-
-
-class Phoenix(Source):
-    """ Phoenix M-dwarf spectra.
-
-    This class provides a convenient handling of PHOENIX M-dwarf spectra.
-    For a given set of effective Temperature, log g, metalicity and alpha, it downloads the spectrum from PHOENIX ftp
-    server.
-
-    See the `original paper <http://dx.doi.org/10.1051/0004-6361/201219058>`_ for more details.
-
-
-    Attributes:
-        t_eff (float): effective Temperature [K]
-        log_g (float): surface gravity
-        z (float): metalicity [Fe/H]
-        alpha (float): abundance of alpha elements [α/Fe]
-
-    """
-    valid_t = [*list(range(2300, 7000, 100)), *list((range(7000, 12200, 200)))]
-    valid_g = [*list(np.arange(0, 6, 0.5))]
-    valid_z = [*list(np.arange(-4, -2, 1)), *list(np.arange(-2.0, 1.5, 0.5))]
-    valid_a = [-0.2, 0., 0.2, 0.4, 0.6, 0.8, 1.0, 1.2, 1.4]
-
-    def __init__(
-            self, t_eff=3600, log_g=5.0, z=0, alpha=0.0, magnitude=10, **kwargs
-    ):
-        assert t_eff in self.valid_t, f'Not a valid effective Temperature {t_eff}'
-        assert log_g in self.valid_g, f'Not a valid log g value {log_g}'
-        assert alpha in self.valid_a, f'Not a valid alpha value {alpha}'
-        assert z in self.valid_z, f'Not a valid metalicity value {z}'
-        if not np.isclose(alpha, 0.):
-            assert 3500. <= t_eff <= 8000. and -3. <= z <= 0., 'PHOENIX parameters are not valid. Please check them ' \
-                                                               'again. '
-        self.t_eff = t_eff
-        self.log_g = log_g
-        self.z = z
-        self.alpha = alpha
-        self.magnitude = magnitude
-        super().__init__(**kwargs, name="phoenix")
-        self.stellar_target = True
-
-        wavelength_path = cache_path.joinpath('WAVE_PHOENIX-ACES-AGSS-COND-2011.fits')
-
-        if not wavelength_path.is_file():
-            print("Download Phoenix wavelength file...")
-            with urllib.request.urlopen(self.get_wavelength_url()) as response, open(wavelength_path,
-                                                                                     "wb") as out_file:
-                data = response.read()
-                out_file.write(data)
-
-        self.wl_data = fits.getdata(wavelength_path) / 10000.0
-        url = self.get_spectrum_url(t_eff, alpha, log_g, z)
-        spectrum_path = cache_path.joinpath(url.split("/")[-1])
-
-        if not spectrum_path.is_file():
-            print(f"Download Phoenix spectrum from {url}...")
-            with urllib.request.urlopen(url) as response, open(spectrum_path, "wb") as out_file:
-                print("Trying to download:" + url)
-                data = response.read()
-                out_file.write(data)
-
-        self.spectrum_data = 0.1 * fits.getdata(spectrum_path)  # convert ergs/s/cm^2/cm to uW/m^2/um
-        self.spectrum_data *= calc_flux_scale(self.wl_data, self.spectrum_data, self.magnitude)
-        self.ip_spectra = scipy.interpolate.interp1d(self.wl_data, self.spectrum_data)
-
-    @staticmethod
-    def get_wavelength_url():
-        return "ftp://phoenix.astro.physik.uni-goettingen.de/HiResFITS/WAVE_PHOENIX-ACES-AGSS-COND-2011.fits"
-
-    @staticmethod
-    def get_spectrum_url(t_eff, alpha, log_g, z):
-        zstring = f"{'+' if z > 0 else '-'}{abs(z):2.1f}"
-        alphastring = f"" if np.isclose(alpha, 0.) else f".Alpha={alpha:+2.2f}"
-
-        url = (
-            f"ftp://phoenix.astro.physik.uni-goettingen.de/"
-            f"HiResFITS/PHOENIX-ACES-AGSS-COND-2011/Z{zstring}{alphastring}/lte{t_eff:05}-{log_g:2.2f}{zstring}"
-            f"{alphastring}.PHOENIX-ACES-AGSS-COND-2011-HiRes.fits"
-        )
-        return url
-
-    def get_spectral_density(self, wavelength):
-        idx = np.logical_and(self.wl_data > np.min(wavelength), self.wl_data < np.max(wavelength))
-        return self.wl_data[idx], self.ip_spectra(self.wl_data[idx])
-
-
-class CSV(Source):
-    """ Spectral source based on custom .csv file
-
-    The .csv file needs to have two columns, a wavelength column and a flux column. The wavelength must be given
-    in either angstroms, nanometers, microns or meters (specified via wavelength_unit), while the flux must either be in
-    ergs/s/cm^2/cm (like Phoenix spectra) for stellar targets, or in photons/s.
-
-    Attributes:
-         name: name of the spectrum
-         list_like: when True, no wavelength interpolation is active (useful for non-continuous spectra e.g.
-         custom line lists)
-         flux_in_photons: if True, flux column treated as photons/s otherwise ergs/s/cm^2/cm
-         stellar_target: if True, flux is expected to be in ergs/s/cm^2/cm and will scale with telescope size
-         magnitude: V magnitude in case of stellar_target
-    """
-    wavelength_scaling = {'a': 1E-4, 'nm': 1E-3, 'micron': 1, 'm': 1E-6}
-
-    def __init__(self, filepath: str | pathlib.Path, name: str | None = None, list_like: bool = False,
-                 wavelength_unit: str = 'a', flux_in_photons: bool = False, stellar_target: bool = False,
-                 magnitude: float = 10., delimiter: str = ','):
-        """ Constructor
-
-        Args:
-         filepath: path to .csv file
-         name: name of the spectrum
-         list_like: when True, no wavelength interpolation is active (useful for non-continuous spectra e.g.
-         custom line lists)
-         wavelength_unit: either 'a', 'nm', 'micron', or 'm' specifying the unit of the wavelength column
-         flux_in_photons: if True, flux column treated as photons/s otherwise ergs/s/cm^2/cm
-         stellar_target: if True, flux is expected to be in ergs/s/cm^2/cm and will scale with telescope size
-         magnitude: V magnitude in case of stellar_target
-         delimiter: delimiter character of .csv file
-        """
-        assert wavelength_unit in self.wavelength_scaling.keys(), f'Supported wavelength units are ' \
-                                                                  f'{self.wavelength_scaling.keys()}'
-        if isinstance(filepath, io.TextIOWrapper):
-            filepath = filepath.name
-        if isinstance(filepath, str):
-            filepath = pathlib.Path(filepath)
-        if name is None:
-            name = filepath.name
-        super().__init__(name=name, list_like=list_like, flux_in_photons=flux_in_photons, stellar_target=stellar_target)
-        self.magnitude = magnitude
-        print(f'{filepath=}, {type(filepath)}')
-        data = pd.read_csv(filepath, delimiter=delimiter)
-
-        self.wl_data = data.iloc[:, 0].values * self.wavelength_scaling[wavelength_unit]
-        self.flux_data = data.iloc[:, 1].values
-        if not flux_in_photons:
-            self.flux_data *= 0.1  # convert ergs/s/cm^2/cm to uW/m^2/um
-            self.flux_data *= calc_flux_scale(self.wl_data, self.flux_data, self.magnitude)
-
-    def get_spectral_density(self, wavelength):
-        idx = np.logical_and(self.wl_data > np.min(wavelength), self.wl_data < np.max(wavelength))
-        return self.wl_data[idx], self.flux_data[idx]
-
-
-class LineList(Source):
-    """ Line-list spectrum
-
-    Attributes:
-        wavelengths: wavelengths [micron] of line(s)
-        intensities: intensities [photons] of line(s)
-    """
-
-    def __init__(self, wavelengths: list[float] | np.ndarray | float = 0.5,
-                 intensities: list[float] | np.ndarray | float = 1000.):
-        super().__init__(name='LineList', list_like=True)
-        # convert always to numpy array
-        self.wavelengths = np.array([wavelengths] if isinstance(wavelengths, float) else wavelengths)
-
-        self.intensities = np.ones_like(self.wavelengths) * intensities if isinstance(intensities,
-                                                                                      float) else intensities
-        assert len(self.wavelengths) == len(self.intensities), 'wavelengths and intensities do not have the same length'
-        self.flux_in_photons = True
-
-    def get_spectral_density(self, wavelength):
-        idx = np.logical_and(self.wavelengths > np.min(wavelength), self.wavelengths < np.max(wavelength))
-        return self.wavelengths[idx], self.intensities[idx]
-
-
-class Blackbody(Source):
-    """ Blackbody spectrum
-
-    Implements a (stellar) blackbody spectrum of given temperature and V-magnitude.
-    """
-
-    def __init__(self, temperature: float = 6000, magnitude: float = 15., name='blackbody'):
-        """
-
-        Args:
-            temperature: effective temperature of blackbody [K]
-            magnitude: Johnson V magnitude of blackbody [mag]
-            name: name of the source (default: blackbody)
-        """
-        super().__init__(name=name, stellar_target=True, flux_in_photons=False)
-        self._sp = SourceSpectrum(BlackBodyNorm1D(temperature=temperature))
-        self._bp = SpectralElement.from_filter('johnson_v')
-        self._vega = SourceSpectrum.from_vega()  # For unit conversion
-        self._sp_norm = self._sp.normalize(magnitude * units.VEGAMAG, self._bp, vegaspec=self._vega)
-
-    def get_spectral_density(self, wavelength):
-        # convert input wavelength from micron to angstrom
-        # convert output from FLAM (erg/s/cm^2/A) to (microW/m^2/microns)
-        return wavelength, self._sp_norm(wavelength * 10000., flux_unit=units.FLAM).value * 1E8
+""" Spectral sources
+
+Implementing various spectral sources that can be used in pyechelle.
+
+.. plot::
+
+    import matplotlib.pyplot as plt
+    import numpy as np
+    import pyechelle.sources as sources
+    from pyechelle.simulator import available_sources
+
+    available_sources.remove('CSV')
+
+    fig, ax = plt.subplots(len(available_sources), 1, figsize=(9, len(available_sources) * 2.5), sharex=True)
+    fig.suptitle('Supported source functions')
+    for i, source_name in enumerate(available_sources):
+        wavelength = np.linspace(0.4999, 0.501, 1000, dtype=float)
+        source = getattr(sources, source_name)()
+        sd = source.get_spectral_density(wavelength)
+        if source.list_like:
+            if isinstance(sd, tuple):
+                ax[i].vlines(sd[0], [0]*len(sd[1]), sd[1])
+            else:
+                ax[i].vlines(wavelength, [0]*len(sd), sd)
+        else:
+            if isinstance(sd, tuple):
+                ax[i].plot(*sd)
+            else:
+                ax[i].plot(wavelength, sd)
+        ax[i].set_title(source_name)
+        ax[i].set_ylabel("")
+        ax[i].set_yticks([])
+    ax[-1].set_xlabel("Wavelength [microns]")
+    plt.tight_layout()
+    plt.show()
+"""
+from __future__ import annotations
+
+import io
+import pathlib
+import urllib.request
+
+import astropy.io.fits as fits
+import astropy.units as u
+import numpy as np
+import pandas as pd
+import scipy.interpolate
+from joblib import Memory
+from synphot import SourceSpectrum, SpectralElement, BlackBodyNorm1D, units
+
+try:
+    from astroquery.nist import Nist
+except ImportError:
+    Nist = None
+
+path = pathlib.Path(__file__).parent.resolve()
+cache_path = path.joinpath(".cache")
+# create data directory if it doesn't exist:
+pathlib.Path(cache_path).mkdir(parents=False, exist_ok=True)
+memory = Memory(cache_path, verbose=0)
+
+
+@memory.cache
+def pull_catalogue_lines(
+    min_wl: float, max_wl: float, catalogue: str = "Th", wavelength_type: str = "vacuum"
+):
+    """
+    Reads NIST catalogue lines between min_wl and max_wl of catalogue.
+
+    Args:
+        min_wl: minimum wavelength bound [micron]
+        max_wl: maximum wavelength bound [micron]
+        catalogue: catalogue appreciation label, e.g. 'Th', 'Ar', etc.
+        wavelength_type: either 'var+air' or 'vacuum'
+
+    Returns:
+        (tuple) line catalogue wavelength and relative intensities. wavelength is in [angstrom]
+    """
+    try:
+        table_lines = Nist.query(
+            min_wl * u.micron,
+            max_wl * u.micron,
+            linename=catalogue,
+            output_order="wavelength",
+            wavelength_type=wavelength_type,
+        )[["Ritz", "Rel."]]
+        df = table_lines.filled(0).to_pandas()
+        df["Rel."] = pd.to_numeric(df["Rel."], downcast="float", errors="coerce")
+        df["Ritz"] = pd.to_numeric(df["Ritz"], downcast="float", errors="coerce")
+        df.dropna(inplace=True)
+        idx = np.logical_and(df["Rel."] > 0, df["Ritz"] > 0)
+        return df["Ritz"].values[idx], df["Rel."].values[idx]
+    except Exception as e:
+        print(e)
+        print(
+            f"Warning: Couldn't retrieve {catalogue} catalogue data between {min_wl} and {max_wl} micron"
+        )
+        return np.array([]), np.array([])
+
+
+def calc_flux_scale(source_wavelength, source_spectral_density, mag):
+    # V - band-filter
+    v_filter_wl = [
+        0.47,
+        0.48,
+        0.49,
+        0.5,
+        0.51,
+        0.52,
+        0.53,
+        0.54,
+        0.55,
+        0.56,
+        0.57,
+        0.58,
+        0.59,
+        0.6,
+        0.61,
+        0.62,
+        0.63,
+        0.64,
+        0.65,
+        0.66,
+        0.67,
+        0.68,
+        0.69,
+        0.7,
+    ]
+    v_filter_tp = [
+        0,
+        0.03,
+        0.163,
+        0.458,
+        0.78,
+        0.967,
+        1,
+        0.973,
+        0.898,
+        0.792,
+        0.684,
+        0.574,
+        0.461,
+        0.359,
+        0.27,
+        0.197,
+        0.135,
+        0.081,
+        0.045,
+        0.025,
+        0.017,
+        0.013,
+        0.009,
+        0,
+    ]
+
+    # Reference flux obtained from integration of vega over bessel filter (units are microwatts/m^2*micrometer)
+    v_zp = 3.68e-02
+
+    v_filter_interp = scipy.interpolate.interp1d(v_filter_wl, v_filter_tp)
+
+    # get total flux in filter/source range
+    lower_wl_limit = max(np.min(source_wavelength), np.min(v_filter_wl))
+    upper_wl_limit = min(np.max(source_wavelength), np.max(v_filter_wl))
+
+    idx = np.logical_and(
+        source_wavelength > lower_wl_limit, source_wavelength < upper_wl_limit
+    )
+
+    step = np.ediff1d(
+        source_wavelength[idx], source_wavelength[idx][-1] - source_wavelength[idx][-2]
+    )
+    total_flux = np.sum(
+        source_spectral_density[idx] * v_filter_interp(source_wavelength[idx]) * step
+    )
+
+    return pow(10, mag / (-2.5)) * v_zp / total_flux
+
+
+class Source:
+    """A spectral source.
+
+    This class should be subclassed to implement different spectral sources.
+
+    Attributes:
+        name (str): name of the source. This will end up in the .fits header.
+        min_wl (float): lower wavelength limit [nm] (for normalization purposes)
+        max_wl (float): upper wavelength limit [nm] (for normalization purposes)
+        list_like (bool): if True, the Source has a bunch of discrete wavelength, rather than a continuous spectral
+        density.
+        flux_in_photons (bool): if True, get_spectral_density() returns flux in photons rather than micro watts
+
+    """
+
+    def __init__(
+        self,
+        min_wl=599.8,
+        max_wl=600.42,
+        name="",
+        list_like=False,
+        flux_in_photons=False,
+        stellar_target=False,
+    ):
+        self.name = name
+        self.min_wl = min_wl
+        self.max_wl = max_wl
+        self.stellar_target = stellar_target
+        self.flux_in_photons = flux_in_photons
+        self.list_like = list_like
+
+    def get_spectral_density(self, wavelength):
+        raise NotImplementedError()
+
+    def get_spectral_density_rv(self, wavelength, rv=0.0):
+        c = 299792458.0  # m/s
+        rv_shifted = wavelength * ((c - rv) / c)
+
+        spec_density = self.get_spectral_density(rv_shifted)
+        # first case: source returns own wavelength vector:
+        if isinstance(spec_density, tuple):
+            wl, sd = spec_density
+            return wl * ((c - rv) / c), sd
+        else:
+            return spec_density
+
+    def __str__(self):
+        return self.name
+
+
+class Constant(Source):
+    """Constant spectral density.
+
+    Implements a constant spectral density with given intensity [microW / microns*s]
+
+    """
+
+    def __init__(self, intensity=0.001, **kwargs):
+        super().__init__(**kwargs, name="Constant", list_like=False)
+        self.intensity = intensity
+
+    def get_spectral_density(self, wavelength):
+        return np.ones_like(wavelength) * self.intensity
+
+    def __str__(self):
+        return self.name + f": intensity: {self.intensity}"
+
+
+class ConstantPhotons(Source):
+    """Constant spectral density.
+
+    Implements a constant photon flux density with given intensity [photons / microns*s]
+
+    """
+
+    def __init__(self, intensity=1e8, **kwargs):
+        super().__init__(**kwargs, name="ConstantPhotons", list_like=False)
+        self.intensity = intensity
+        self.flux_in_photons = True
+        self.stellar_target = False
+
+    def get_spectral_density(self, wavelength):
+        return np.ones_like(wavelength) * self.intensity
+
+    def __str__(self):
+        return self.name + f": intensity: {self.intensity}"
+
+
+class ThAr(Source):
+    """Thorium-Argon lamp
+
+    Implements a Thorium Argon arc-lamp.
+    Uses NIST vacuum catalogue wavelength as source.
+
+    Attributes:
+         scale (float): relative intensity scaling factor between the Thorium and the Argon lines.
+
+    """
+
+    def __init__(self, argon_to_thorium_factor=10):
+        super().__init__(name="ThAr", list_like=True)
+        self.flux_in_photons = True
+        self.scale = argon_to_thorium_factor
+
+    def get_spectral_density(self, wavelength):
+        minwl = np.min(wavelength)
+        maxwl = np.max(wavelength)
+        thwl, thint = pull_catalogue_lines(minwl, maxwl, "Th")
+        arwl, arint = pull_catalogue_lines(minwl, maxwl, "Ar")
+        arint *= self.scale
+        return np.hstack((thwl / 10000.0, arwl / 10000.0)), np.hstack((thint, arint))
+
+
+class ThNe(Source):
+    """Thorium-Neon lamp
+
+    Implements a Thorium Neon arc-lamp.
+    Uses NIST vacuum catalogue wavelength as source.
+
+    Attributes:
+         scale (float): relative intensity scaling factor between the Thorium and the Neon lines.
+
+    """
+
+    def __init__(self, neon_to_thorium_factor=10):
+        super().__init__(name="ThNe", list_like=True)
+        self.flux_in_photons = True
+        self.scale = neon_to_thorium_factor
+
+    def get_spectral_density(self, wavelength):
+        minwl = np.min(wavelength)
+        maxwl = np.max(wavelength)
+        thwl, thint = pull_catalogue_lines(minwl, maxwl, "Th")
+        newl, neint = pull_catalogue_lines(minwl, maxwl, "Ne")
+        neint *= self.scale
+
+        return np.hstack((thwl / 10000.0, newl / 10000.0)), np.hstack((thint, neint))
+
+
+class Etalon(Source):
+    r"""Fabry-Perot etalon.
+
+    Implements spectrum of an ideal (i.e. dispersion-free) Fabry-Perot etalon.
+    This means, the peak wavelength are at:
+
+    .. math::
+        \lambda_{peak} = \frac{d \cdot n \cdot \cos{(\theta)}}{m}
+
+    Attributes:
+        d (float): mirror distance [mm]
+        n (float): refractive index between mirrors
+        theta (float): angle of incidence onto mirrors
+        min_m (int): minimum peak interference number
+        max_m (int): maximum peak interference number
+        n_photons (int): number of photons per peak per second
+
+    """
+
+    def __init__(self, d=5.0, n=1.0, theta=0.0, n_photons=1000, **kwargs):
+        super().__init__(**kwargs, name="Etalon", list_like=True)
+        self.d = d
+        self.n = n
+        self.theta = theta
+        self.min_m = np.ceil(2e3 * d * np.cos(theta) / self.max_wl)
+        self.max_m = np.floor(2e3 * d * np.cos(theta) / self.min_wl)
+        self.n_photons = n_photons
+        self.flux_in_photons = True
+
+    @staticmethod
+    def peak_wavelength_etalon(m, d=10.0, n=1.0, theta=0.0):
+        return 2e3 * d * n * np.cos(theta) / m
+
+    def get_spectral_density(self, wavelength):
+        self.min_m = np.ceil(2e3 * self.d * np.cos(self.theta) / np.max(wavelength))
+        self.max_m = np.floor(2e3 * self.d * np.cos(self.theta) / np.min(wavelength))
+        intensity = np.ones_like(
+            np.arange(self.min_m, self.max_m), dtype=float
+        ) * float(self.n_photons)
+        return self.peak_wavelength_etalon(
+            np.arange(self.min_m, self.max_m), self.d, self.n, self.theta
+        ), np.asarray(intensity, dtype=int)
+
+    def __str__(self):
+        return self.name + f": d={self.d},n={self.n},theta={self.theta}"
+
+
+class Phoenix(Source):
+    """Phoenix M-dwarf spectra.
+
+    This class provides a convenient handling of PHOENIX M-dwarf spectra.
+    For a given set of effective Temperature, log g, metalicity and alpha, it downloads the spectrum from PHOENIX ftp
+    server.
+
+    See the `original paper <http://dx.doi.org/10.1051/0004-6361/201219058>`_ for more details.
+
+
+    Attributes:
+        t_eff (float): effective Temperature [K]
+        log_g (float): surface gravity
+        z (float): metalicity [Fe/H]
+        alpha (float): abundance of alpha elements [α/Fe]
+
+    """
+
+    valid_t = [*list(range(2300, 7000, 100)), *list((range(7000, 12200, 200)))]
+    valid_g = [*list(np.arange(0, 6, 0.5))]
+    valid_z = [*list(np.arange(-4, -2, 1)), *list(np.arange(-2.0, 1.5, 0.5))]
+    valid_a = [-0.2, 0.0, 0.2, 0.4, 0.6, 0.8, 1.0, 1.2, 1.4]
+
+    def __init__(self, t_eff=3600, log_g=5.0, z=0, alpha=0.0, magnitude=10, **kwargs):
+        assert t_eff in self.valid_t, f"Not a valid effective Temperature {t_eff}"
+        assert log_g in self.valid_g, f"Not a valid log g value {log_g}"
+        assert alpha in self.valid_a, f"Not a valid alpha value {alpha}"
+        assert z in self.valid_z, f"Not a valid metalicity value {z}"
+        if not np.isclose(alpha, 0.0):
+            assert 3500.0 <= t_eff <= 8000.0 and -3.0 <= z <= 0.0, (
+                "PHOENIX parameters are not valid. Please check them " "again. "
+            )
+        self.t_eff = t_eff
+        self.log_g = log_g
+        self.z = z
+        self.alpha = alpha
+        self.magnitude = magnitude
+        super().__init__(**kwargs, name="phoenix")
+        self.stellar_target = True
+
+        wavelength_path = cache_path.joinpath("WAVE_PHOENIX-ACES-AGSS-COND-2011.fits")
+
+        if not wavelength_path.is_file():
+            print("Download Phoenix wavelength file...")
+            with urllib.request.urlopen(self.get_wavelength_url()) as response, open(
+                wavelength_path, "wb"
+            ) as out_file:
+                data = response.read()
+                out_file.write(data)
+
+        self.wl_data = fits.getdata(wavelength_path) / 10000.0
+        url = self.get_spectrum_url(t_eff, alpha, log_g, z)
+        spectrum_path = cache_path.joinpath(url.split("/")[-1])
+
+        if not spectrum_path.is_file():
+            print(f"Download Phoenix spectrum from {url}...")
+            with urllib.request.urlopen(url) as response, open(
+                spectrum_path, "wb"
+            ) as out_file:
+                print("Trying to download:" + url)
+                data = response.read()
+                out_file.write(data)
+
+        self.spectrum_data = 0.1 * fits.getdata(
+            spectrum_path
+        )  # convert ergs/s/cm^2/cm to uW/m^2/um
+        self.spectrum_data *= calc_flux_scale(
+            self.wl_data, self.spectrum_data, self.magnitude
+        )
+        self.ip_spectra = scipy.interpolate.interp1d(self.wl_data, self.spectrum_data)
+
+    @staticmethod
+    def get_wavelength_url():
+        return "ftp://phoenix.astro.physik.uni-goettingen.de/HiResFITS/WAVE_PHOENIX-ACES-AGSS-COND-2011.fits"
+
+    @staticmethod
+    def get_spectrum_url(t_eff, alpha, log_g, z):
+        zstring = f"{'+' if z > 0 else '-'}{abs(z):2.1f}"
+        alphastring = "" if np.isclose(alpha, 0.0) else f".Alpha={alpha:+2.2f}"
+
+        url = (
+            f"ftp://phoenix.astro.physik.uni-goettingen.de/"
+            f"HiResFITS/PHOENIX-ACES-AGSS-COND-2011/Z{zstring}{alphastring}/lte{t_eff:05}-{log_g:2.2f}{zstring}"
+            f"{alphastring}.PHOENIX-ACES-AGSS-COND-2011-HiRes.fits"
+        )
+        return url
+
+    def get_spectral_density(self, wavelength):
+        idx = np.logical_and(
+            self.wl_data > np.min(wavelength), self.wl_data < np.max(wavelength)
+        )
+        return self.wl_data[idx], self.ip_spectra(self.wl_data[idx])
+
+    def __str__(self):
+        return (
+            self.name
+            + f": t={self.t_eff},g={self.log_g},z={self.z},a={self.alpha},mag={self.magnitude}"
+        )
+
+
+class CSV(Source):
+    """Spectral source based on custom .csv file
+
+    The .csv file needs to have two columns, a wavelength column and a flux column. The wavelength must be given
+    in either angstroms, nanometers, microns or meters (specified via wavelength_unit), while the flux must either be in
+    ergs/s/cm^2/cm (like Phoenix spectra) for stellar targets, or in photons/s.
+
+    Attributes:
+         name: name of the spectrum
+         list_like: when True, no wavelength interpolation is active (useful for non-continuous spectra e.g.
+         custom line lists)
+         flux_in_photons: if True, flux column treated as photons/s otherwise ergs/s/cm^2/cm
+         stellar_target: if True, flux is expected to be in ergs/s/cm^2/cm and will scale with telescope size
+         magnitude: V magnitude in case of stellar_target
+    """
+
+    wavelength_scaling = {"a": 1e-4, "nm": 1e-3, "micron": 1, "m": 1e-6}
+
+    def __init__(
+        self,
+        filepath: str | pathlib.Path,
+        name: str | None = None,
+        list_like: bool = False,
+        wavelength_unit: str = "a",
+        flux_in_photons: bool = False,
+        stellar_target: bool = False,
+        magnitude: float = 10.0,
+        delimiter: str = ",",
+    ):
+        """Constructor
+
+        Args:
+         filepath: path to .csv file
+         name: name of the spectrum
+         list_like: when True, no wavelength interpolation is active (useful for non-continuous spectra e.g.
+         custom line lists)
+         wavelength_unit: either 'a', 'nm', 'micron', or 'm' specifying the unit of the wavelength column
+         flux_in_photons: if True, flux column treated as photons/s otherwise ergs/s/cm^2/cm
+         stellar_target: if True, flux is expected to be in ergs/s/cm^2/cm and will scale with telescope size
+         magnitude: V magnitude in case of stellar_target
+         delimiter: delimiter character of .csv file
+        """
+        assert wavelength_unit in self.wavelength_scaling.keys(), (
+            f"Supported wavelength units are " f"{self.wavelength_scaling.keys()}"
+        )
+        if isinstance(filepath, io.TextIOWrapper):
+            filepath = filepath.name
+        if isinstance(filepath, str):
+            filepath = pathlib.Path(filepath)
+        if name is None:
+            name = filepath.name
+        super().__init__(
+            name=name,
+            list_like=list_like,
+            flux_in_photons=flux_in_photons,
+            stellar_target=stellar_target,
+        )
+        self.magnitude = magnitude
+        print(f"{filepath=}, {type(filepath)}")
+        data = pd.read_csv(filepath, delimiter=delimiter)
+
+        self.wl_data = data.iloc[:, 0].values * self.wavelength_scaling[wavelength_unit]
+        self.flux_data = data.iloc[:, 1].values
+        if not flux_in_photons:
+            self.flux_data *= 0.1  # convert ergs/s/cm^2/cm to uW/m^2/um
+            self.flux_data *= calc_flux_scale(
+                self.wl_data, self.flux_data, self.magnitude
+            )
+
+    def get_spectral_density(self, wavelength):
+        idx = np.logical_and(
+            self.wl_data > np.min(wavelength), self.wl_data < np.max(wavelength)
+        )
+        return self.wl_data[idx], self.flux_data[idx]
+
+
+class LineList(Source):
+    """Line-list spectrum
+
+    Attributes:
+        wavelengths: wavelengths [micron] of line(s)
+        intensities: intensities [photons] of line(s)
+    """
+
+    def __init__(
+        self,
+        wavelengths: list[float] | np.ndarray | float = 0.5,
+        intensities: list[float] | np.ndarray | float = 1000.0,
+    ):
+        super().__init__(name="LineList", list_like=True)
+        # convert always to numpy array
+        self.wavelengths = np.array(
+            [wavelengths] if isinstance(wavelengths, float) else wavelengths
+        )
+
+        self.intensities = (
+            np.ones_like(self.wavelengths) * intensities
+            if isinstance(intensities, float)
+            else intensities
+        )
+        assert len(self.wavelengths) == len(
+            self.intensities
+        ), "wavelengths and intensities do not have the same length"
+        self.flux_in_photons = True
+
+    def get_spectral_density(self, wavelength):
+        idx = np.logical_and(
+            self.wavelengths > np.min(wavelength), self.wavelengths < np.max(wavelength)
+        )
+        return self.wavelengths[idx], self.intensities[idx]
+
+
+class Blackbody(Source):
+    """Blackbody spectrum
+
+    Implements a (stellar) blackbody spectrum of given temperature and V-magnitude.
+    """
+
+    def __init__(
+        self, temperature: float = 6000, magnitude: float = 15.0, name="blackbody"
+    ):
+        """
+
+        Args:
+            temperature: effective temperature of blackbody [K]
+            magnitude: Johnson V magnitude of blackbody [mag]
+            name: name of the source (default: blackbody)
+        """
+        super().__init__(name=name, stellar_target=True, flux_in_photons=False)
+        self.magnitude = magnitude
+        self.temperature = temperature
+        self._sp = SourceSpectrum(BlackBodyNorm1D(temperature=temperature))
+        self._bp = SpectralElement.from_filter("johnson_v")
+        self._vega = SourceSpectrum.from_vega()  # For unit conversion
+        self._sp_norm = self._sp.normalize(
+            magnitude * units.VEGAMAG, self._bp, vegaspec=self._vega
+        )
+
+    def get_spectral_density(self, wavelength):
+        # convert input wavelength from micron to angstrom
+        # convert output from FLAM (erg/s/cm^2/A) to (microW/m^2/microns)
+        return wavelength, self._sp_norm(
+            wavelength * 10000.0, flux_unit=units.FLAM
+        ).value * 1e8
+
+    def __str__(self):
+        return self.name + f"temp={self.temperature},mag={self.magnitude}"
```

### Comparing `pyechelle-0.3.6/README.md` & `pyechelle-0.3.7/README.md`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# PyEchelle
-
-PyEchelle is a simulation tool, to generate realistic 2D spectra, in particular cross-dispersed echelle spectra.
-However, it is not limited to echelle spectrographs, but allows simulating arbitrary spectra for any fiber-fed or slit
-spectrograph, where a model file is available. Optical aberrations are treated accurately, the simulated spectra include
-photon and read-out noise.
-
-PyEchelle uses numba for implementing fast Python-based simulation code. It also comes with **CUDA support** for major
-speed improvements.
-
-### Example usage
-
-You can use PyEchelle directly from the console:
-
-```bash
-pyechelle --spectrograph MaroonX --fiber 2-4 --sources Phoenix --phoenix_t_eff 3500 -t 10 --rv 100 -o mdwarf.fit
-```
-
-If you rather script in python, you can do the same as above with the following python script:
-
-```python
-
-from pyechelle.simulator import Simulator
-from pyechelle.sources import Phoenix
-from pyechelle.spectrograph import ZEMAX
-
-sim = Simulator(ZEMAX("MaroonX"))
-sim.set_ccd(1)
-sim.set_fibers([2, 3, 4])
-sim.set_sources(Phoenix(t_eff=3500))
-sim.set_exposure_time(10.)
-sim.set_radial_velocities(100.)
-sim.set_output('mdwarf.fits', overwrite=True)
-sim.run()
-
-```
-
-Both times, a PHOENIX M-dwarf spectrum with the given stellar parameters, and a RV shift of 100m/s for the MAROON-X
-spectrograph is simulated.
-
-The output is a 2D raw frame (.fits) and will look similar to:
-
-![](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/mdwarf.jpg "")
-
-Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
-
-Pyechelle is the successor of [Echelle++](https://github.com/Stuermer/EchelleSimulator) which has a similar
-functionality but was written in C++. This package was rewritten in python for better maintainability, easier package
-distribution and for smoother cross-platform development.
-
-# Installation
-
-As simple as
-
-```bash
-pip install pyechelle
-```
-
-Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/installation.html) for alternative installation instruction.
-
-# Usage
-
-See
-
-```bash
-pyechelle -h
-```
-
-for all available command line options.
-
-See [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
-
-# Concept:
-
-The basic idea is that any spectrograph can be modelled with a set of wavelength-dependent transformation matrices and
-point spread functions which describe the spectrographs' optics:
-
-First, wavelength-dependent **affine transformation matrices** are extracted from the ZEMAX model of the spectrograph.
-As the underlying geometric transformations (scaling, rotation, shearing, translation) vary smoothly across an echelle
-order, these matrices can be interpolated for any intermediate wavelength.
-
-Second, a wavelength-dependent **point spread functions (PSFs)** is applied on the transformed slit images to properly
-account for optical aberrations. Again, the PSF is only slowly varying across an echelle order, allowing for
-interpolation at intermediate wavelength.
-
-![Echelle simulation](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/intro.png "Echelle simulation")
-
-**Both, the matrices and the PSFs have to be extracted from ZEMAX only once. It is therefore possible to simulate
-spectra without access to ZEMAX**
-
-# Citation
-
-Please cite this [paper](http://dx.doi.org/10.1088/1538-3873/aaec2e) if you find this work useful in your research.
+# PyEchelle
+
+PyEchelle is a simulation tool, to generate realistic 2D spectra, in particular cross-dispersed echelle spectra.
+However, it is not limited to echelle spectrographs, but allows simulating arbitrary spectra for any fiber-fed or slit
+spectrograph, where a model file is available. Optical aberrations are treated accurately, the simulated spectra include
+photon and read-out noise.
+
+PyEchelle uses numba for implementing fast Python-based simulation code. It also comes with **CUDA support** for major
+speed improvements.
+
+### Example usage
+
+You can use PyEchelle directly from the console:
+
+```bash
+pyechelle --spectrograph MaroonX --fiber 2-4 --sources Phoenix --phoenix_t_eff 3500 -t 10 --rv 100 -o mdwarf.fit
+```
+
+If you rather script in python, you can do the same as above with the following python script:
+
+```python
+
+from pyechelle.simulator import Simulator
+from pyechelle.sources import Phoenix
+from pyechelle.spectrograph import ZEMAX
+
+sim = Simulator(ZEMAX("MaroonX"))
+sim.set_ccd(1)
+sim.set_fibers([2, 3, 4])
+sim.set_sources(Phoenix(t_eff=3500))
+sim.set_exposure_time(10.)
+sim.set_radial_velocities(100.)
+sim.set_output('mdwarf.fits', overwrite=True)
+sim.run()
+
+```
+
+Both times, a PHOENIX M-dwarf spectrum with the given stellar parameters, and a RV shift of 100m/s for the MAROON-X
+spectrograph is simulated.
+
+The output is a 2D raw frame (.fits) and will look similar to:
+
+![](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/mdwarf.jpg "")
+
+Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
+
+Pyechelle is the successor of [Echelle++](https://github.com/Stuermer/EchelleSimulator) which has a similar
+functionality but was written in C++. This package was rewritten in python for better maintainability, easier package
+distribution and for smoother cross-platform development.
+
+# Installation
+
+As simple as
+
+```bash
+pip install pyechelle
+```
+
+Check out the [Documentation](https://stuermer.gitlab.io/pyechelle/installation.html) for alternative installation instruction.
+
+# Usage
+
+See
+
+```bash
+pyechelle -h
+```
+
+for all available command line options.
+
+See [Documentation](https://stuermer.gitlab.io/pyechelle/usage.html) for more examples.
+
+# Concept:
+
+The basic idea is that any spectrograph can be modelled with a set of wavelength-dependent transformation matrices and
+point spread functions which describe the spectrographs' optics:
+
+First, wavelength-dependent **affine transformation matrices** are extracted from the ZEMAX model of the spectrograph.
+As the underlying geometric transformations (scaling, rotation, shearing, translation) vary smoothly across an echelle
+order, these matrices can be interpolated for any intermediate wavelength.
+
+Second, a wavelength-dependent **point spread functions (PSFs)** is applied on the transformed slit images to properly
+account for optical aberrations. Again, the PSF is only slowly varying across an echelle order, allowing for
+interpolation at intermediate wavelength.
+
+![Echelle simulation](https://gitlab.com/Stuermer/pyechelle/-/raw/master/docs/source/_static/plots/intro.png "Echelle simulation")
+
+**Both, the matrices and the PSFs have to be extracted from ZEMAX only once. It is therefore possible to simulate
+spectra without access to ZEMAX**
+
+# Citation
+
+Please cite this [paper](http://dx.doi.org/10.1088/1538-3873/aaec2e) if you find this work useful in your research.
```

### Comparing `pyechelle-0.3.6/PKG-INFO` & `pyechelle-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: pyechelle
-Version: 0.3.6
+Version: 0.3.7
 Summary: A fast generic spectrum simulator
 Home-page: https://gitlab.com/Stuermer/pyechelle
 License: MIT
 Author: Julian Stuermer
 Author-email: julian@stuermer.science
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: astropy (>=5.2.2,<6.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: astropy (>=5.3.4,<6.0.0)
 Requires-Dist: astroquery (>=0.4.6,<0.5.0)
-Requires-Dist: h5py (>=3.9.0,<4.0.0)
-Requires-Dist: joblib (>=1.3.1,<2.0.0)
-Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
-Requires-Dist: numba (>=0.57.1,<0.58.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: parmap (>=1.6.0,<2.0.0)
-Requires-Dist: plotly (>=5.15.0,<6.0.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0)
-Requires-Dist: skycalc-ipy (>=0.1.3,<0.2.0)
-Requires-Dist: synphot (>=1.2.1,<2.0.0)
+Requires-Dist: h5py (>=3.10.0,<4.0.0)
+Requires-Dist: joblib (>=1.3.2,<2.0.0)
+Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
+Requires-Dist: numba (>=0.59,<0.60)
+Requires-Dist: pandas (>=2.2.0,<3.0.0)
+Requires-Dist: parmap (>=1.7.0,<2.0.0)
+Requires-Dist: plotly (>=5.17.0,<6.0.0)
+Requires-Dist: scipy (>=1.12.0,<2.0.0)
+Requires-Dist: skycalc-ipy (>=0.4.0,<0.5.0)
+Requires-Dist: synphot (>=1.3.post0,<2.0)
+Requires-Dist: zospy (>=1.1.1,<2.0.0) ; python_version >= "3.9" and python_version < "3.12" and platform_system == "Windows"
 Project-URL: Documentation, https://stuermer.gitlab.io/pyechelle/
 Project-URL: Repository, https://gitlab.com/Stuermer/pyechelle
 Description-Content-Type: text/markdown
 
 # PyEchelle
 
 PyEchelle is a simulation tool, to generate realistic 2D spectra, in particular cross-dispersed echelle spectra.
```

