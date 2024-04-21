# Comparing `tmp/openmc_geometry_plot-0.4.2.tar.gz` & `tmp/openmc_geometry_plot-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmc_geometry_plot-0.4.2.tar", last modified: Mon Feb 19 20:47:12 2024, max compression
+gzip compressed data, was "openmc_geometry_plot-0.4.3.tar", last modified: Sun Apr 21 02:25:41 2024, max compression
```

## Comparing `openmc_geometry_plot-0.4.2.tar` & `openmc_geometry_plot-0.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:47:12.892166 openmc_geometry_plot-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:47:12.888166 openmc_geometry_plot-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:47:12.888166 openmc_geometry_plot-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/.github/workflows/ci_with_install.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-02-19 20:47:12.892166 openmc_geometry_plot-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 20:47:12.892166 openmc_geometry_plot-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:47:12.888166 openmc_geometry_plot-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:47:12.892166 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/
--rw-r--r--   0 runner    (1001) docker     (127)   295464 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/He4.h5
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-19 20:47:12.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15675 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    27976 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/cross_sections.xml
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:47:12.892166 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-02-19 20:47:12.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-19 20:47:12.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 20:47:12.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-19 20:47:12.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-19 20:47:12.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-19 20:47:12.000000 openmc_geometry_plot-0.4.2/src/openmc_geometry_plot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:47:12.892166 openmc_geometry_plot-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/tests/test_dagmc_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/tests/test_get_slice_of_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/tests/test_get_slice_of_material.py
--rw-r--r--   0 runner    (1001) docker     (127)    58468 2024-02-19 20:46:58.000000 openmc_geometry_plot-0.4.2/tests/two_disconnected_cubes.h5m
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:25:41.892375 openmc_geometry_plot-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:25:41.888375 openmc_geometry_plot-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:25:41.888375 openmc_geometry_plot-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/.github/workflows/ci_with_install.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-21 02:25:41.892375 openmc_geometry_plot-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 02:25:41.892375 openmc_geometry_plot-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:25:41.888375 openmc_geometry_plot-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:25:41.892375 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)   295464 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/He4.h5
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 02:25:41.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15688 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27976 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/cross_sections.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:25:41.892375 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-21 02:25:41.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-21 02:25:41.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 02:25:41.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 02:25:41.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 02:25:41.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 02:25:41.000000 openmc_geometry_plot-0.4.3/src/openmc_geometry_plot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 02:25:41.892375 openmc_geometry_plot-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/tests/test_dagmc_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/tests/test_get_slice_of_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/tests/test_get_slice_of_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58468 2024-04-21 02:25:26.000000 openmc_geometry_plot-0.4.3/tests/two_disconnected_cubes.h5m
```

### Comparing `openmc_geometry_plot-0.4.2/.github/workflows/ci_with_install.yml` & `openmc_geometry_plot-0.4.3/.github/workflows/ci_with_install.yml`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/.github/workflows/python-publish.yml` & `openmc_geometry_plot-0.4.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/.gitignore` & `openmc_geometry_plot-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/PKG-INFO` & `openmc_geometry_plot-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_geometry_plot
-Version: 0.4.2
+Version: 0.4.3
 Summary: Plot OpenMC geometry, interactive or static 2D slice plots.
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/openmc_geometry_plot
 Project-URL: Bug Tracker, https://github.com/fusion-energy/openmc_geometry_plot/issues
 Keywords: openmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openmc_geometry_plot-0.4.2/README.md` & `openmc_geometry_plot-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/pyproject.toml` & `openmc_geometry_plot-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/He4.h5` & `openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/He4.h5`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/app.py` & `openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,18 +201,18 @@
         y_index = {'x':0,'y':1,'z':2}[basis[1]]
         slice_index = {"xy": 2, "xz": 1, "yz": 0}[basis]
         slice_axis = {"xy": 'Z', "xz": 'Y', "yz": 'X'}[basis]
 
         # x axis values
         if np.isinf(bb[0][x_index]) or np.isinf(bb[1][x_index]):
             plot_left = st.sidebar.number_input(
-                value = -2000., label="minimum vertical axis value", key="x_min"
+                value = -2000., label="minimum horizontal axis value", key="x_min"
             )
             plot_right = st.sidebar.number_input(
-                value=2000., label="maximum vertical axis value", key="x_max"
+                value=2000., label="maximum horizontal axis value", key="x_max"
             )
         else:
             x_min = float(bb[0][x_index])
             x_max = float(bb[1][x_index])
             plot_right, plot_left = st.sidebar.slider(
                 label="Left and right values for the horizontal axis",
                 min_value=x_min,
@@ -354,20 +354,19 @@
             elif basis == 'xz':
                 origin=(
                     (plot_left+plot_right)/2,
                     slice_value,
                     (plot_top+plot_bottom)/2,
                 )
 
-            width_x=plot_left-plot_right
-            width_y=plot_top-plot_bottom
+            width_x=abs(plot_left-plot_right)
+            width_y=abs(plot_top-plot_bottom)
             if backend == "matplotlib":
                 print('plotting with matplotlib')
 
-
                 plot = my_geometry.plot(
                     origin=origin,
                     width=[width_x,width_y],
                     pixels=pixels,
                     basis=basis,
                     color_by=color_by,
                     colors=my_colors,
```

### Comparing `openmc_geometry_plot-0.4.2/src/openmc_geometry_plot/core.py` & `openmc_geometry_plot-0.4.3/src/openmc_geometry_plot/core.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/src/openmc_geometry_plot.egg-info/PKG-INFO` & `openmc_geometry_plot-0.4.3/src/openmc_geometry_plot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmc_geometry_plot
-Version: 0.4.2
+Version: 0.4.3
 Summary: Plot OpenMC geometry, interactive or static 2D slice plots.
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/openmc_geometry_plot
 Project-URL: Bug Tracker, https://github.com/fusion-energy/openmc_geometry_plot/issues
 Keywords: openmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `openmc_geometry_plot-0.4.2/src/openmc_geometry_plot.egg-info/SOURCES.txt` & `openmc_geometry_plot-0.4.3/src/openmc_geometry_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/tests/test_dagmc_slice.py` & `openmc_geometry_plot-0.4.3/tests/test_dagmc_slice.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/tests/test_get_slice_of_cell.py` & `openmc_geometry_plot-0.4.3/tests/test_get_slice_of_cell.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/tests/test_get_slice_of_material.py` & `openmc_geometry_plot-0.4.3/tests/test_get_slice_of_material.py`

 * *Files identical despite different names*

### Comparing `openmc_geometry_plot-0.4.2/tests/two_disconnected_cubes.h5m` & `openmc_geometry_plot-0.4.3/tests/two_disconnected_cubes.h5m`

 * *Files identical despite different names*

