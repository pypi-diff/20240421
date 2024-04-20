# Comparing `tmp/tomographic_kernel-1.0.1.tar.gz` & `tmp/tomographic_kernel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomographic_kernel-1.0.1.tar", last modified: Wed Oct 18 12:38:29 2023, max compression
+gzip compressed data, was "tomographic_kernel-1.0.2.tar", last modified: Sat Apr 20 22:55:41 2024, max compression
```

## Comparing `tomographic_kernel-1.0.1.tar` & `tomographic_kernel-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-10-18 12:38:29.125500 tomographic_kernel-1.0.1/
--rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-04-10 16:25:06.000000 tomographic_kernel-1.0.1/LICENSE
--rw-r--r--   0 albert    (1000) albert    (1000)      853 2023-10-18 12:38:29.125500 tomographic_kernel-1.0.1/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)       83 2023-04-10 16:25:06.000000 tomographic_kernel-1.0.1/README.md
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-09-18 19:27:25.000000 tomographic_kernel-1.0.1/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-10-18 12:38:29.125500 tomographic_kernel-1.0.1/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)     1129 2023-10-18 12:38:06.000000 tomographic_kernel-1.0.1/setup.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-10-18 12:38:29.125500 tomographic_kernel-1.0.1/tomographic_kernel/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-04-10 16:31:28.000000 tomographic_kernel-1.0.1/tomographic_kernel/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3488 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.1/tomographic_kernel/fourier_kernel.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5165 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.1/tomographic_kernel/frames.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-10-18 12:38:29.125500 tomographic_kernel-1.0.1/tomographic_kernel/models/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-04-10 16:31:28.000000 tomographic_kernel-1.0.1/tomographic_kernel/models/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6786 2023-05-18 10:00:34.000000 tomographic_kernel-1.0.1/tomographic_kernel/models/cannonical_models.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    45343 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.1/tomographic_kernel/plotting.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-10-18 12:38:29.125500 tomographic_kernel-1.0.1/tomographic_kernel/simulation/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-04-10 16:31:28.000000 tomographic_kernel-1.0.1/tomographic_kernel/simulation/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     8270 2023-06-05 21:46:07.000000 tomographic_kernel-1.0.1/tomographic_kernel/simulation/interpolate_h5parm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    19697 2023-10-18 12:35:01.000000 tomographic_kernel-1.0.1/tomographic_kernel/simulation/ionosphere_simulation.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-10-18 12:38:29.125500 tomographic_kernel-1.0.1/tomographic_kernel/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-04-24 09:24:55.000000 tomographic_kernel-1.0.1/tomographic_kernel/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4046 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.1/tomographic_kernel/tests/test_frames.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1479 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.1/tomographic_kernel/tests.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16048 2023-10-18 12:37:45.000000 tomographic_kernel-1.0.1/tomographic_kernel/tomographic_kernel.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    11367 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.1/tomographic_kernel/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-10-18 12:38:29.125500 tomographic_kernel-1.0.1/tomographic_kernel.egg-info/
--rw-r--r--   0 albert    (1000) albert    (1000)      853 2023-10-18 12:38:29.000000 tomographic_kernel-1.0.1/tomographic_kernel.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      824 2023-10-18 12:38:29.000000 tomographic_kernel-1.0.1/tomographic_kernel.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-10-18 12:38:29.000000 tomographic_kernel-1.0.1/tomographic_kernel.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       99 2023-10-18 12:38:29.000000 tomographic_kernel-1.0.1/tomographic_kernel.egg-info/requires.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)       19 2023-10-18 12:38:29.000000 tomographic_kernel-1.0.1/tomographic_kernel.egg-info/top_level.txt
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-04-20 22:55:41.129785 tomographic_kernel-1.0.2/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1077 2023-04-10 16:25:06.000000 tomographic_kernel-1.0.2/LICENSE
+-rw-r--r--   0 albert    (1000) albert    (1000)      834 2024-04-20 22:55:41.129785 tomographic_kernel-1.0.2/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)       83 2023-04-10 16:25:06.000000 tomographic_kernel-1.0.2/README.md
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-09-18 19:27:25.000000 tomographic_kernel-1.0.2/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2024-04-20 22:55:41.129785 tomographic_kernel-1.0.2/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)     1118 2024-04-20 22:54:49.000000 tomographic_kernel-1.0.2/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-04-20 22:55:41.125785 tomographic_kernel-1.0.2/tomographic_kernel/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-04-10 16:31:28.000000 tomographic_kernel-1.0.2/tomographic_kernel/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3488 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.2/tomographic_kernel/fourier_kernel.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4530 2024-04-19 19:52:40.000000 tomographic_kernel-1.0.2/tomographic_kernel/frames.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-04-20 22:55:41.129785 tomographic_kernel-1.0.2/tomographic_kernel/models/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-04-10 16:31:28.000000 tomographic_kernel-1.0.2/tomographic_kernel/models/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6786 2023-05-18 10:00:34.000000 tomographic_kernel-1.0.2/tomographic_kernel/models/cannonical_models.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-04-20 22:55:41.129785 tomographic_kernel-1.0.2/tomographic_kernel/models/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-04-10 16:31:28.000000 tomographic_kernel-1.0.2/tomographic_kernel/models/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5449 2023-10-24 10:55:11.000000 tomographic_kernel-1.0.2/tomographic_kernel/models/tests/test_directional_scale.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4963 2023-10-24 10:32:19.000000 tomographic_kernel-1.0.2/tomographic_kernel/models/tests/test_time_scale.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    45343 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.2/tomographic_kernel/plotting.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-04-20 22:55:41.129785 tomographic_kernel-1.0.2/tomographic_kernel/simulation/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-04-10 16:31:28.000000 tomographic_kernel-1.0.2/tomographic_kernel/simulation/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     8270 2023-06-05 21:46:07.000000 tomographic_kernel-1.0.2/tomographic_kernel/simulation/interpolate_h5parm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    19697 2023-10-18 12:35:01.000000 tomographic_kernel-1.0.2/tomographic_kernel/simulation/ionosphere_simulation.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-04-20 22:55:41.129785 tomographic_kernel-1.0.2/tomographic_kernel/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-04-24 09:24:55.000000 tomographic_kernel-1.0.2/tomographic_kernel/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10261 2024-04-20 22:53:46.000000 tomographic_kernel-1.0.2/tomographic_kernel/tests/test_frames.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1245 2023-10-21 14:31:07.000000 tomographic_kernel-1.0.2/tomographic_kernel/tests/test_geometry.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1479 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.2/tomographic_kernel/tests.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15917 2023-10-24 10:32:19.000000 tomographic_kernel-1.0.2/tomographic_kernel/tomographic_kernel.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    11367 2023-04-10 20:32:19.000000 tomographic_kernel-1.0.2/tomographic_kernel/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2024-04-20 22:55:41.129785 tomographic_kernel-1.0.2/tomographic_kernel.egg-info/
+-rw-r--r--   0 albert    (1000) albert    (1000)      834 2024-04-20 22:55:41.000000 tomographic_kernel-1.0.2/tomographic_kernel.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1027 2024-04-20 22:55:41.000000 tomographic_kernel-1.0.2/tomographic_kernel.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2024-04-20 22:55:41.000000 tomographic_kernel-1.0.2/tomographic_kernel.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       95 2024-04-20 22:55:41.000000 tomographic_kernel-1.0.2/tomographic_kernel.egg-info/requires.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)       19 2024-04-20 22:55:41.000000 tomographic_kernel-1.0.2/tomographic_kernel.egg-info/top_level.txt
```

### Comparing `tomographic_kernel-1.0.1/LICENSE` & `tomographic_kernel-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomographic_kernel-1.0.1/PKG-INFO` & `tomographic_kernel-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: tomographic_kernel
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Tomographic Kernel in JAX for tomographic Gaussian processes.
 Home-page: https://github.com/JoshuaAlbert/tomographic_kernel
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: h5parm>=1.0.5
 Requires-Dist: scipy
-Requires-Dist: astropy
+Requires-Dist: astropy>=6
 Requires-Dist: matplotlib
 Requires-Dist: cmocean
 Requires-Dist: tqdm
 Requires-Dist: jax
 Requires-Dist: jaxlib
-Requires-Dist: tables
 Requires-Dist: tensorflow_probability
 
 # tomographic_kernel
 Provides the tomographic kernel from J. G. Albert et al. 2020
```

### Comparing `tomographic_kernel-1.0.1/setup.py` & `tomographic_kernel-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 from setuptools import find_packages
 from setuptools import setup
 
 install_requires = [
     'numpy',
     'h5parm>=1.0.5',
     'scipy',
-    'astropy',
+    'astropy>=6',
     'matplotlib',
     'cmocean',
     'tqdm',
     'jax',
     'jaxlib',
-    'tables',
     'tensorflow_probability'
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='tomographic_kernel',
-      version='1.0.1',
+      version='1.0.2',
       description='A Tomographic Kernel in JAX for tomographic Gaussian processes.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/JoshuaAlbert/tomographic_kernel",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       install_requires=install_requires,
```

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel/fourier_kernel.py` & `tomographic_kernel-1.0.2/tomographic_kernel/fourier_kernel.py`

 * *Files identical despite different names*

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel/frames.py` & `tomographic_kernel-1.0.2/tomographic_kernel/frames.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,88 +18,81 @@
     * ``obstime``
         The time at which the observation is taken.  Used for determining the
         position and orientation of the Earth.
     * ``location``
         The location on the Earth.  This can be specified either as an
         `~astropy.coordinates.EarthLocation` object or as anything that can be
         transformed to an `~astropy.coordinates.ITRS` frame.
+
     Parameters
     ----------
     representation : `BaseRepresentation` or None
         A representation object or None to have no data (or use the other keywords)
     east : :class:`~astropy.units.Quantity`, optional, must be keyword
         The east coordinate for this object (``north`` and ``up`` must also be given and
         ``representation`` must be None).
     north : :class:`~astropy.units.Quantity`, optional, must be keyword
         The north coordinate for this object (``east`` and ``up`` must also be given and
         ``representation`` must be None).
     up : :class:`~astropy.units.Quantity`, optional, must be keyword
         The up coordinate for this object (``north`` and ``east`` must also be given and
         ``representation`` must be None).
-    Notes
-    -----
-    This is useful as an intermediate frame between ITRS and UVW for radio astronomy
     """
 
     frame_specific_representation_info = {
         'cartesian': [RepresentationMapping('x', 'east'),
                       RepresentationMapping('y', 'north'),
                       RepresentationMapping('z', 'up')],
     }
 
     default_representation = CartesianRepresentation
 
-    obstime = TimeAttribute(default=None)  # at.Time("2000-01-01T00:00:00.000",format="isot",scale="tai"))
+    obstime = TimeAttribute(default=None)
     location = EarthLocationAttribute(default=None)
 
     def __init__(self, *args, **kwargs):
         super(ENU, self).__init__(*args, **kwargs)
 
 
 @frame_transform_graph.transform(FunctionTransform, AltAz, ENU)
-def altaz_to_enu(altaz_coo, enu_frame):
+def altaz_to_enu(altaz_coo: AltAz, enu_frame: ENU):
     '''Defines the transformation between AltAz and the ENU frame.
     AltAz usually has units attached but ENU does not require units
     if it specifies a direction.'''
     is_directional = (isinstance(altaz_coo.data, UnitSphericalRepresentation) or
                       altaz_coo.cartesian.x.unit == u.one)
 
     if is_directional:
         rep = CartesianRepresentation(x=altaz_coo.cartesian.y,
                                       y=altaz_coo.cartesian.x,
                                       z=altaz_coo.cartesian.z,
                                       copy=False)
     else:
-        # location_altaz = ITRS(*enu_frame.location.to_geocentric()).transform_to(
-        #     AltAz(location=enu_frame.location, obstime=enu_frame.obstime))
-        rep = CartesianRepresentation(x=altaz_coo.cartesian.y,  # - location_altaz.cartesian.y,
-                                      y=altaz_coo.cartesian.x,  # - location_altaz.cartesian.x,
-                                      z=altaz_coo.cartesian.z,  # - location_altaz.cartesian.z,
+        rep = CartesianRepresentation(x=altaz_coo.cartesian.y,
+                                      y=altaz_coo.cartesian.x,
+                                      z=altaz_coo.cartesian.z,
                                       copy=False)
     return enu_frame.realize_frame(rep)
 
 
 @frame_transform_graph.transform(FunctionTransform, ENU, AltAz)
-def enu_to_altaz(enu_coo, altaz_frame):
+def enu_to_altaz(enu_coo: ENU, altaz_frame: AltAz):
     is_directional = (isinstance(enu_coo.data, UnitSphericalRepresentation) or
                       enu_coo.cartesian.x.unit == u.one)
 
     if is_directional:
         rep = CartesianRepresentation(x=enu_coo.north,
                                       y=enu_coo.east,
                                       z=enu_coo.up,
                                       copy=False)
     else:
-        # location_altaz = ITRS(*enu_coo.location.to_geocentric()).transform_to(
-        #     AltAz(location=enu_coo.location, obstime=enu_coo.obstime))
-        rep = CartesianRepresentation(x=enu_coo.north,  # + location_altaz.cartesian.x,
-                                      y=enu_coo.east,  # + location_altaz.cartesian.y,
-                                      z=enu_coo.up,  # + location_altaz.cartesian.z,
+        rep = CartesianRepresentation(x=enu_coo.north,
+                                      y=enu_coo.east,
+                                      z=enu_coo.up,
                                       copy=False)
     return altaz_frame.realize_frame(rep)
 
 
 @frame_transform_graph.transform(FunctionTransform, ENU, ENU)
-def enu_to_enu(from_coo, to_frame):
-    # for now we just implement this through AltAz to make sure we get everything
-    # covered
+def enu_to_enu(from_coo: ENU, to_frame: ENU):
+    # To convert from ENU at one location and time to ENU at another location and time, we go through AltAz
     return from_coo.transform_to(AltAz(location=from_coo.location, obstime=from_coo.obstime)).transform_to(to_frame)
```

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel/models/cannonical_models.py` & `tomographic_kernel-1.0.2/tomographic_kernel/models/cannonical_models.py`

 * *Files identical despite different names*

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel/plotting.py` & `tomographic_kernel-1.0.2/tomographic_kernel/plotting.py`

 * *Files identical despite different names*

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel/simulation/interpolate_h5parm.py` & `tomographic_kernel-1.0.2/tomographic_kernel/simulation/interpolate_h5parm.py`

 * *Files identical despite different names*

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel/simulation/ionosphere_simulation.py` & `tomographic_kernel-1.0.2/tomographic_kernel/simulation/ionosphere_simulation.py`

 * *Files identical despite different names*

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel/tests.py` & `tomographic_kernel-1.0.2/tomographic_kernel/tests.py`

 * *Files identical despite different names*

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel/tomographic_kernel.py` & `tomographic_kernel-1.0.2/tomographic_kernel/tomographic_kernel.py`

 * *Files 8% similar despite different names*

```diff
@@ -351,26 +351,14 @@
     u_cross_x = jnp.cross(rotation_axis, y)
     rotated_y = rotation_axis * (rotation_axis @ y) \
                 + jnp.cos(angle) * jnp.cross(u_cross_x, rotation_axis) \
                 + jnp.sin(angle) * u_cross_x
     return rotated_y
 
 
-def test_rotate_vector():
-    x = jnp.asarray([1., 0., 0.])
-    y = jnp.asarray([0., 1., 0.])
-    z = jnp.asarray([0., 0., 1.])
-    angle = jnp.pi / 2.
-    assert jnp.allclose(rotate_vector(x, z, angle), y, atol=1e-6)
-    assert jnp.allclose(rotate_vector(x, y, angle), -z, atol=1e-6)
-    assert jnp.allclose(rotate_vector(z, y, angle), x, atol=1e-6)
-    assert jnp.allclose(rotate_vector(y, x, angle), z, atol=1e-6)
-    assert not jnp.any(jnp.isnan(rotate_vector(y, jnp.asarray([0, 0, 0]), angle)))
-
-
 def frozen_flow_transform(t, y, x0, bottom, earth_centre, wind_velocity=None) -> jnp.ndarray:
     """
     Computes the frozen flow transform on the coordinates.
 
     Args:
         t: time in seconds
         y: position in km, origin at centre of Earth
@@ -402,23 +390,35 @@
     # Rotation
     rotated_y = rotate_vector(y - earth_centre, rotation_axis, angle) + earth_centre
     # logger.info(f"{t} {jnp.linalg.norm(rotated_y-y)}")
     # assert jnp.linalg.norm.(y-rotated_y) < 1e-6
     return rotated_y
 
 
-def test_frozen_flow_transform():
-    earth_centre = jnp.asarray([0., 0., 0.])
-    t = 0.
-    y = jnp.asarray([0., 0., 6400.])
-    x0 = y
-    bottom = 300.
-    wind_velocity = jnp.asarray([-0.240, 0.030, 0.])
-    assert jnp.allclose(y,
-                        frozen_flow_transform(t, y, x0, bottom, earth_centre=earth_centre, wind_velocity=wind_velocity))
-
-    t = 60
-    y = jnp.asarray([0., 0., 6400.])
-    x0 = jnp.asarray([0., 100., 6400.])
-    bottom = 300.
-    wind_velocity = jnp.asarray([-0.240, 0.030, 0.])
-    print(frozen_flow_transform(t, y, x0, bottom, earth_centre=earth_centre, wind_velocity=wind_velocity))
+def mean_square_difference(X1: GeodesicTuple, X2: GeodesicTuple, kernel: MultiLayerTomographicKernel):
+    """
+    Compute the mean square difference of the underlying between two points, i.e.
+
+        E[(DTEC(X1) - DTEC(X2))^2] if the kernel is a DTEC kernel.
+
+    or
+
+        E[(TEC(X1) - TEC(X2))^2] if the kernel is a TEC kernel.
+
+    Args:
+        X1: the first point (GeodesicTuple) of shape [M]
+        X2: the second point (GeodesicTuple) of shape [N]
+        kernel: the kernel
+
+    Returns:
+        the mean square difference of the underlying between X1 and X2 [M, N]
+    """
+    var_1 = jnp.diag(kernel.cov_func(X1, X1))  # [M]
+    var_2 = jnp.diag(kernel.cov_func(X2, X2))  # [N]
+    mu_1 = kernel.mean_func(X1)  # [M]
+    mu_2 = kernel.mean_func(X2)  # [N]
+    cov_12 = kernel.cov_func(X1, X2)  # [M, N]
+    return (
+            var_1[:, None] + mu_1[:, None] ** 2
+            - 2. * (cov_12 + mu_1[:, None] * mu_2[None, :])
+            + var_2[None, :] + mu_2[None, :] ** 2
+    )
```

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel/utils.py` & `tomographic_kernel-1.0.2/tomographic_kernel/utils.py`

 * *Files identical despite different names*

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel.egg-info/PKG-INFO` & `tomographic_kernel-1.0.2/tomographic_kernel.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
-Name: tomographic-kernel
-Version: 1.0.1
+Name: tomographic_kernel
+Version: 1.0.2
 Summary: A Tomographic Kernel in JAX for tomographic Gaussian processes.
 Home-page: https://github.com/JoshuaAlbert/tomographic_kernel
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: h5parm>=1.0.5
 Requires-Dist: scipy
-Requires-Dist: astropy
+Requires-Dist: astropy>=6
 Requires-Dist: matplotlib
 Requires-Dist: cmocean
 Requires-Dist: tqdm
 Requires-Dist: jax
 Requires-Dist: jaxlib
-Requires-Dist: tables
 Requires-Dist: tensorflow_probability
 
 # tomographic_kernel
 Provides the tomographic kernel from J. G. Albert et al. 2020
```

### Comparing `tomographic_kernel-1.0.1/tomographic_kernel.egg-info/SOURCES.txt` & `tomographic_kernel-1.0.2/tomographic_kernel.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,12 +12,16 @@
 ./tomographic_kernel.egg-info/PKG-INFO
 ./tomographic_kernel.egg-info/SOURCES.txt
 ./tomographic_kernel.egg-info/dependency_links.txt
 ./tomographic_kernel.egg-info/requires.txt
 ./tomographic_kernel.egg-info/top_level.txt
 ./tomographic_kernel/models/__init__.py
 ./tomographic_kernel/models/cannonical_models.py
+./tomographic_kernel/models/tests/__init__.py
+./tomographic_kernel/models/tests/test_directional_scale.py
+./tomographic_kernel/models/tests/test_time_scale.py
 ./tomographic_kernel/simulation/__init__.py
 ./tomographic_kernel/simulation/interpolate_h5parm.py
 ./tomographic_kernel/simulation/ionosphere_simulation.py
 ./tomographic_kernel/tests/__init__.py
-./tomographic_kernel/tests/test_frames.py
+./tomographic_kernel/tests/test_frames.py
+./tomographic_kernel/tests/test_geometry.py
```

