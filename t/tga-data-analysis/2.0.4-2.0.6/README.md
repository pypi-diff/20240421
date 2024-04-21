# Comparing `tmp/tga_data_analysis-2.0.4.tar.gz` & `tmp/tga_data_analysis-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tga_data_analysis-2.0.4.tar", last modified: Thu Apr  4 18:13:20 2024, max compression
+gzip compressed data, was "tga_data_analysis-2.0.6.tar", last modified: Sun Apr 21 12:01:14 2024, max compression
```

## Comparing `tga_data_analysis-2.0.4.tar` & `tga_data_analysis-2.0.6.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.240611 tga_data_analysis-2.0.4/
--rw-rw-rw-   0        0        0     2012 2024-04-04 18:13:20.233645 tga_data_analysis-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.4/README.md
--rw-rw-rw-   0        0        0      783 2024-04-04 18:13:10.000000 tga_data_analysis-2.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 18:13:20.242604 tga_data_analysis-2.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.133967 tga_data_analysis-2.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.167854 tga_data_analysis-2.0.4/src/tga_data_analysis/
--rw-rw-rw-   0        0        0        0 2024-04-03 01:21:24.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/__init__.py
--rw-rw-rw-   0        0        0    10611 2024-04-02 13:30:00.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/kas_kinetics.py
--rw-rw-rw-   0        0        0     4340 2024-04-03 01:44:48.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/measure.py
--rw-rw-rw-   0        0        0    23737 2024-04-03 01:58:28.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/myfigure.py
--rw-rw-rw-   0        0        0    64691 2024-04-04 02:03:14.000000 tga_data_analysis-2.0.4/src/tga_data_analysis/tga.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.227654 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/
--rw-rw-rw-   0        0        0     2012 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-04 18:13:20.000000 tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 18:13:20.221675 tga_data_analysis-2.0.4/tests/
--rw-rw-rw-   0        0        0     1855 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.4/tests/test_measure.py
--rw-rw-rw-   0        0        0     3964 2024-04-02 01:28:57.000000 tga_data_analysis-2.0.4/tests/test_my_figure.py
--rw-rw-rw-   0        0        0       42 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.4/tests/test_sample.py
--rw-rw-rw-   0        0        0      911 2024-04-01 20:45:06.000000 tga_data_analysis-2.0.4/tests/test_tga.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.027941 tga_data_analysis-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.027941 tga_data_analysis-2.0.6/src/tga_data_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/myfigure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63386 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/src/tga_data_analysis/tga.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-21 12:01:14.000000 tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:01:14.031941 tga_data_analysis-2.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_kas_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_my_figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_oxidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_proximate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-21 12:01:07.000000 tga_data_analysis-2.0.6/tests/test_soliddist.py
```

### Comparing `tga_data_analysis-2.0.4/PKG-INFO` & `tga_data_analysis-2.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-Metadata-Version: 2.1
-Name: tga_data_analysis
-Version: 2.0.4
-Summary: Tool for automatic analysis of multiple TGA results
-Author: Matteo Pecchi
-License: MIT
-Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
-Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: numpy>=1.21.2
-Requires-Dist: pandas>=1.3.3
-Requires-Dist: matplotlib>=3.4.3
-Requires-Dist: seaborn>=0.11.2
-Requires-Dist: openpyxl
-Requires-Dist: pyarrow
-Requires-Dist: scipy>=1.7.1
-Requires-Dist: lmfit>=1.0.2
-
-# Thermogravimetric Analysis in Python
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-## Overview
-PyTGA is a Python module designed for conducting and analyzing Thermogravimetric Analysis (TGA) experiments. It offers tools for loading, processing, and analyzing TGA data, focusing on proximate and oxidation analysis, solid distillation analysis, and deconvolution analysis.
-
-## Features
-- **Data Loading**: Supports loading TGA data from files.
-- **Proximate Analysis**: Calculates moisture, ash, and volatile matter.
-- **Oxidation Analysis**: Computes Ti, Tp, Tb, etc.
-- **Solid Distillation Analysis**: Analyzes solid distillation over time.
-- **Deconvolution Analysis**: Deconvolutes TGA curves for peak analysis.
-- **Plotting and Visualization**: Functions for TGA data visualization.
-
-## Example
-The example is available in the example folder that can be found using the project link homepage. Necessary data are provided. The example demonstrates how to use the tga_data_analysis package for basic TGA data analysis and visualization, the example requires downloading the data, installing the package, and setting the folder path to the example data folder.
+Metadata-Version: 2.1
+Name: tga_data_analysis
+Version: 2.0.6
+Summary: Tool for automatic analysis of multiple TGA results
+Author: Matteo Pecchi
+License: MIT
+Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
+Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.21.2
+Requires-Dist: pandas>=1.3.3
+Requires-Dist: matplotlib>=3.4.3
+Requires-Dist: seaborn>=0.11.2
+Requires-Dist: openpyxl
+Requires-Dist: pyarrow
+Requires-Dist: scipy>=1.7.1
+Requires-Dist: lmfit>=1.0.2
+
+# Thermogravimetric Analysis in Python
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Testing (CI)](https://github.com/mpecchi/tga_data_analysis/actions/workflows/continuous_integration.yaml/badge.svg)](https://github.com/mpecchi/tga_data_analysis/actions/workflows/continuous_integration.yaml)
+## Overview
+PyTGA is a Python module designed for conducting and analyzing Thermogravimetric Analysis (TGA) experiments. It offers tools for loading, processing, and analyzing TGA data, focusing on proximate and oxidation analysis, solid distillation analysis, and deconvolution analysis.
+
+## Features
+- **Data Loading**: Supports loading TGA data from files.
+- **Proximate Analysis**: Calculates moisture, ash, and volatile matter.
+- **Oxidation Analysis**: Computes Ti, Tp, Tb, etc.
+- **Solid Distillation Analysis**: Analyzes solid distillation over time.
+- **Deconvolution Analysis**: Deconvolutes TGA curves for peak analysis.
+- **Plotting and Visualization**: Functions for TGA data visualization.
+
+
+## Documentation
+
+Check out the [documentation](https://tga-data-analysis.readthedocs.io/).
+
+## Installation
+
+You can install the package from [PyPI](https://pypi.org/project/tga_data_analysis/):
+
+```bash
+pip install tga_data_analysis
```

### Comparing `tga_data_analysis-2.0.4/src/tga_data_analysis/kas_kinetics.py` & `tga_data_analysis-2.0.6/src/tga_data_analysis/kas_kinetics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-# %%
-import numpy as np
-import pathlib as plib
-from tga_data_analysis.tga import Project, Sample
-from tga_data_analysis.myfigure import MyFigure, clrs, lttrs, lnstls, mrkrs
-
-
-class KasSample:
-    """
-    A class to handle and analyze kinetic data using the Kissinger-Akahira-Sunose (KAS) method.
-    It provides functionalities to perform KAS analysis on a set of samples, plot analysis results,
-    and compare different samples' kinetic parameters.
-    """
-
-    def __init__(
-        self,
-        project: Project,
-        samples: list[Sample] | None = None,
-        name: str | None = None,
-        ramps: list[float] | None = None,
-        alpha: list[float] | None = None,
-    ):
-        """
-        Initialize a KasSample object with parameters for KAS analysis.
-
-        :param project: The Project object associated with the kinetic analysis.
-        :type project: Project
-        :param samples: A list of Sample objects to be analyzed. If None, all samples in the project are used.
-        :type samples: list[Sample], optional
-        :param name: An optional name for the KasSample object, used for identification.
-        :type name: str, optional
-        :param ramps: A list of heating rates for each sample. If None, the heating rates are taken from the samples.
-        :type ramps: list[float], optional
-        :param alpha: A list of conversion values to be analyzed. If None, a default range is used.
-        :type alpha: list[float], optional
-        """
-        self.plot_grid = project.plot_grid
-        self.plot_font = project.plot_font
-        self.out_path = plib.Path(project.out_path, "kas_analysis")
-        if samples is None:
-            self.samples = project.samples
-        else:
-            self.samples = samples
-        self.samplenames = [sample.name for sample in self.samples]
-        if name is None:
-            self.name = "".join(
-                [
-                    char
-                    for char in self.samplenames[0]
-                    if all(char in samplename for samplename in self.samplenames)
-                ]
-            )
-        else:
-            self.name = name
-
-        if ramps is None:
-            self.ramps = [sample.heating_rate_deg_min for sample in self.samples]
-        else:
-            self.ramps = ramps
-        if alpha is None:
-            self.alpha = np.arange(0.1, 0.85, 0.05)
-        else:
-            self.alpha = alpha
-
-        self.activation_energy = np.zeros(len(self.alpha))
-        self.activation_energy_std = np.zeros(len(self.alpha))
-        self.x_matrix = np.zeros((len(self.alpha), len(self.ramps)))
-        self.y_matrix = np.zeros((len(self.alpha), len(self.ramps)))
-        self.fits: list[np.poly1d] = []
-
-        self.kas_analysis_computed: bool = False
-
-    def kas_analysis(
-        self,
-    ):
-        """
-        Perform the KAS analysis across the provided samples, calculating the activation energy for different conversions.
-
-        This method computes the activation energy for the given conversion values (alpha) using the KAS method.
-        The results are stored within the object for later access and visualization.
-        """
-
-        r_gas_constant = 8.314462618  # Universal gas constant in J/(mol*K)
-        c_to_k = 273.15
-
-        for idx, sample in enumerate(self.samples):
-            temp = sample.temp_dtg + c_to_k if sample.temp_unit == "C" else sample.temp_dtg
-            alpha_mass = 1 - (sample.mp_db_dtg() - np.min(sample.mp_db_dtg())) / (
-                np.max(sample.mp_db_dtg()) - np.min(sample.mp_db_dtg())
-            )
-            for alpha_idx, alpha_val in enumerate(self.alpha):
-                conversion_index = np.argmax(alpha_mass > alpha_val)
-                self.x_matrix[alpha_idx, idx] = 1000 / temp[conversion_index]
-                self.y_matrix[alpha_idx, idx] = np.log(
-                    self.ramps[idx] / temp[conversion_index] ** 2
-                )
-        for i in range(len(self.alpha)):
-            p, cov = np.polyfit(self.x_matrix[i, :], self.y_matrix[i, :], 1, cov=True)
-            self.fits.append(np.poly1d(p))
-            self.activation_energy[i] = -p[0] * r_gas_constant
-            self.activation_energy_std[i] = np.sqrt(cov[0][0]) * r_gas_constant
-
-        self.kas_analysis_computed = True
-        return None
-
-    def plot_isolines(
-        self,
-        **kwargs,
-    ) -> MyFigure:
-        """
-        Plot the KAS analysis isolines for the set of samples.
-
-        This method generates a plot of the KAS isolines, providing a visual representation of the kinetic analysis results.
-
-        :param kwargs: Additional keyword arguments for plot customization.
-        :type kwargs: dict
-        :return: A MyFigure instance containing the isoline plot.
-        :rtype: MyFigure
-        """
-
-        if not self.kas_analysis_computed:
-            self.kas_analysis()
-
-        out_path = plib.Path(self.out_path, "isolines_plots")
-        out_path.mkdir(parents=True, exist_ok=True)
-
-        default_kwargs = {
-            "filename": self.name + "_isolines",
-            "out_path": out_path,
-            "height": 4,
-            "width": 5,
-            "grid": self.plot_grid,
-            "text_font": self.plot_font,
-            "x_lab": "1000/T [1/K]",
-            "y_lab": r"ln($\beta$/T$^{2}$)",
-        }
-        # Update kwargs with the default key-value pairs if the key is not present in kwargs
-        kwargs = {**default_kwargs, **kwargs}
-        myfig = MyFigure(rows=1, cols=1, **kwargs)
-
-        for i, alpha_val in enumerate(self.alpha):
-            lab = rf"$\alpha$={alpha_val:0.2f}"
-            # Assuming self.fits[i] is the fit for the i-th alpha
-            fit_fn = self.fits[i]
-            x_new = np.linspace(np.min(self.x_matrix[i, :]), np.max(self.x_matrix[i, :]), 100)
-            y_new = fit_fn(x_new)
-
-            # Plotting the fit line
-            myfig.axs[0].plot(x_new, y_new, color=clrs[i], linestyle=lnstls[i], label=lab)
-
-            # Plotting the data points
-            myfig.axs[0].plot(
-                self.x_matrix[i, :],
-                self.y_matrix[i, :],
-                color=clrs[i],
-                linestyle="None",
-                marker=mrkrs[i],
-            )
-        myfig.save_figure()
-        return myfig
-
-    def plot_activation_energy(
-        self,
-        **kwargs,
-    ) -> MyFigure:
-        """
-        Plot the activation energy as a function of conversion for the analyzed samples.
-
-        This method generates a plot showing the variation of activation energy with conversion, offering insights into the kinetic behavior of the sample.
-
-        :param kwargs: Additional keyword arguments for plot customization.
-        :type kwargs: dict
-        :return: A MyFigure instance containing the activation energy plot.
-        :rtype: MyFigure
-        """
-        if not self.kas_analysis_computed:
-            self.kas_analysis()
-
-        out_path = plib.Path(self.out_path, "activation_energy_plots")
-        out_path.mkdir(parents=True, exist_ok=True)
-
-        default_kwargs = {
-            "filename": self.name + "_isolines",
-            "out_path": out_path,
-            "height": 4,
-            "width": 4,
-            "grid": self.plot_grid,
-            "text_font": self.plot_font,
-            "x_lab": r"$\alpha$ [-]",
-            "y_lab": r"$E_{a}$ [kJ/mol]",
-            "legend": None,
-        }
-        # Update kwargs with the default key-value pairs if the key is not present in kwargs
-        kwargs = {**default_kwargs, **kwargs}
-        myfig = MyFigure(rows=1, cols=1, **kwargs)
-
-        myfig.axs[0].plot(self.alpha, self.activation_energy)
-
-        # Plotting the data points
-        myfig.axs[0].fill_between(
-            self.alpha,
-            self.activation_energy - self.activation_energy_std,
-            self.activation_energy + self.activation_energy_std,
-            alpha=0.3,
-        )
-        myfig.save_figure()
-        return myfig
-
-
-def plot_multi_activation_energy(
-    kassamples: list[KasSample],
-    labels: list[str] | None = None,
-    filename: str = "plot",
-    **kwargs,
-) -> MyFigure:
-    """
-    Plot the activation energy for multiple KAS analyses, comparing their kinetic parameters.
-
-    This function creates a plot showing the activation energy against conversion for a series of KasSample objects,
-    allowing for a comparative analysis of different samples or conditions.
-
-    :param kassamples: A list of KasSample objects for which the activation energy plots are generated.
-    :type kassamples: list[KasSample]
-    :param labels: Labels corresponding to each KasSample object. If None, the names of the samples are used.
-    :type labels: list[str], optional
-    :param filename: The base name for the file to save the plot. Defaults to "plot".
-    :type filename: str
-    :param kwargs: Additional keyword arguments for plot customization.
-    :type kwargs: dict
-    :return: A MyFigure instance containing the comparative activation energy plot.
-    :rtype: MyFigure
-    """
-
-    if labels is None:
-        labels = [sample.name for sample in kassamples]
-    for sample in kassamples:
-        if not sample.kas_analysis_computed:
-            sample.kas_analysis()
-
-    out_path = plib.Path(kassamples[0].out_path, "multisample_plots")
-    out_path.mkdir(parents=True, exist_ok=True)
-
-    default_kwargs = {
-        "filename": filename + "_activation_energy",
-        "out_path": out_path,
-        "height": 4,
-        "width": 4,
-        "grid": kassamples[0].plot_grid,
-        "text_font": kassamples[0].plot_font,
-        "x_lab": r"$\alpha$ [-]",
-        "y_lab": r"$E_{a}$ [kJ/mol]",
-    }
-    kwargs = {**default_kwargs, **kwargs}
-    myfig = MyFigure(
-        rows=1,
-        cols=1,
-        **kwargs,
-    )
-    for i, sample in enumerate(kassamples):
-        myfig.axs[0].plot(
-            sample.alpha,
-            sample.activation_energy,
-            color=clrs[i],
-            linestyle=lnstls[i],
-            label=labels[i],
-        )
-
-        # Plotting the data points
-        myfig.axs[0].fill_between(
-            sample.alpha,
-            sample.activation_energy - sample.activation_energy_std,
-            sample.activation_energy + sample.activation_energy_std,
-            alpha=0.3,
-            color=clrs[i],
-            linestyle=lnstls[i],
-        )
-    myfig.save_figure()
-    return myfig
+# %%
+import numpy as np
+import pathlib as plib
+from tga_data_analysis.tga import Project, Sample
+from tga_data_analysis.myfigure import MyFigure, colors, letters, linestyles, markers
+
+
+class KasSample:
+    """
+    A class to handle and analyze kinetic data using the Kissinger-Akahira-Sunose (KAS) method.
+    It provides functionalities to perform KAS analysis on a set of samples, plot analysis results,
+    and compare different samples' kinetic parameters.
+    """
+
+    def __init__(
+        self,
+        project: Project,
+        samples: list[Sample] | None = None,
+        name: str | None = None,
+        ramps: list[float] | None = None,
+        alpha: list[float] | None = None,
+    ):
+        """
+        Initialize a KasSample object with parameters for KAS analysis.
+
+        :param project: The Project object associated with the kinetic analysis.
+        :type project: Project
+        :param samples: A list of Sample objects to be analyzed. If None, all samples in the project are used.
+        :type samples: list[Sample], optional
+        :param name: An optional name for the KasSample object, used for identification.
+        :type name: str, optional
+        :param ramps: A list of heating rates for each sample. If None, the heating rates are taken from the samples.
+        :type ramps: list[float], optional
+        :param alpha: A list of conversion values to be analyzed. If None, a default range is used.
+        :type alpha: list[float], optional
+        """
+        self.plot_grid = project.plot_grid
+        self.plot_font = project.plot_font
+        self.out_path = plib.Path(project.out_path, "kas_analysis")
+        if samples is None:
+            self.samples = project.samples
+        else:
+            self.samples = samples
+        self.samplenames = [sample.name for sample in self.samples]
+        if name is None:
+            self.name = "".join(
+                [
+                    char
+                    for char in self.samplenames[0]
+                    if all(char in samplename for samplename in self.samplenames)
+                ]
+            )
+        else:
+            self.name = name
+
+        if ramps is None:
+            self.ramps = [sample.heating_rate_deg_min for sample in self.samples]
+        else:
+            self.ramps = ramps
+        if alpha is None:
+            self.alpha = np.arange(0.1, 0.85, 0.05)
+        else:
+            self.alpha = alpha
+
+        self.activation_energy = np.zeros(len(self.alpha))
+        self.activation_energy_std = np.zeros(len(self.alpha))
+        self.x_matrix = np.zeros((len(self.alpha), len(self.ramps)))
+        self.y_matrix = np.zeros((len(self.alpha), len(self.ramps)))
+        self.fits: list[np.poly1d] = []
+
+        self.kas_analysis_computed: bool = False
+
+    def kas_analysis(
+        self,
+    ):
+        """
+        Perform the KAS analysis across the provided samples, calculating the activation energy for different conversions.
+
+        This method computes the activation energy for the given conversion values (alpha) using the KAS method.
+        The results are stored within the object for later access and visualization.
+        """
+
+        r_gas_constant = 8.314462618  # Universal gas constant in J/(mol*K)
+        c_to_k = 273.15
+
+        for idx, sample in enumerate(self.samples):
+            temp = sample.temp_dtg + c_to_k if sample.temp_unit == "C" else sample.temp_dtg
+            alpha_mass = 1 - (sample.mp_db_dtg() - np.min(sample.mp_db_dtg())) / (
+                np.max(sample.mp_db_dtg()) - np.min(sample.mp_db_dtg())
+            )
+            for alpha_idx, alpha_val in enumerate(self.alpha):
+                conversion_index = np.argmax(alpha_mass > alpha_val)
+                self.x_matrix[alpha_idx, idx] = 1000 / temp[conversion_index]
+                self.y_matrix[alpha_idx, idx] = np.log(
+                    self.ramps[idx] / temp[conversion_index] ** 2
+                )
+        for i in range(len(self.alpha)):
+            p, cov = np.polyfit(self.x_matrix[i, :], self.y_matrix[i, :], 1, cov=True)
+            self.fits.append(np.poly1d(p))
+            self.activation_energy[i] = -p[0] * r_gas_constant
+            self.activation_energy_std[i] = np.sqrt(cov[0][0]) * r_gas_constant
+
+        self.kas_analysis_computed = True
+        return None
+
+    def plot_isolines(
+        self,
+        **kwargs,
+    ) -> MyFigure:
+        """
+        Plot the KAS analysis isolines for the set of samples.
+
+        This method generates a plot of the KAS isolines, providing a visual representation of the kinetic analysis results.
+
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the isoline plot.
+        :rtype: MyFigure
+        """
+
+        if not self.kas_analysis_computed:
+            self.kas_analysis()
+
+        out_path = plib.Path(self.out_path, "isolines_plots")
+        out_path.mkdir(parents=True, exist_ok=True)
+
+        default_kwargs = {
+            "filename": self.name + "_isolines",
+            "out_path": out_path,
+            "height": 4,
+            "width": 5,
+            "grid": self.plot_grid,
+            "text_font": self.plot_font,
+            "x_lab": "1000/T [1/K]",
+            "y_lab": r"ln($\beta$/T$^{2}$)",
+        }
+        # Update kwargs with the default key-value pairs if the key is not present in kwargs
+        kwargs = {**default_kwargs, **kwargs}
+        myfig = MyFigure(rows=1, cols=1, **kwargs)
+
+        for i, alpha_val in enumerate(self.alpha):
+            lab = rf"$\alpha$={alpha_val:0.2f}"
+            # Assuming self.fits[i] is the fit for the i-th alpha
+            fit_fn = self.fits[i]
+            x_new = np.linspace(np.min(self.x_matrix[i, :]), np.max(self.x_matrix[i, :]), 100)
+            y_new = fit_fn(x_new)
+
+            # Plotting the fit line
+            myfig.axs[0].plot(x_new, y_new, color=colors[i], linestyle=linestyles[i], label=lab)
+
+            # Plotting the data points
+            myfig.axs[0].plot(
+                self.x_matrix[i, :],
+                self.y_matrix[i, :],
+                color=colors[i],
+                linestyle="None",
+                marker=markers[i],
+            )
+        myfig.save_figure()
+        return myfig
+
+    def plot_activation_energy(
+        self,
+        **kwargs,
+    ) -> MyFigure:
+        """
+        Plot the activation energy as a function of conversion for the analyzed samples.
+
+        This method generates a plot showing the variation of activation energy with conversion, offering insights into the kinetic behavior of the sample.
+
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the activation energy plot.
+        :rtype: MyFigure
+        """
+        if not self.kas_analysis_computed:
+            self.kas_analysis()
+
+        out_path = plib.Path(self.out_path, "activation_energy_plots")
+        out_path.mkdir(parents=True, exist_ok=True)
+
+        default_kwargs = {
+            "filename": self.name + "_isolines",
+            "out_path": out_path,
+            "height": 4,
+            "width": 4,
+            "grid": self.plot_grid,
+            "text_font": self.plot_font,
+            "x_lab": r"$\alpha$ [-]",
+            "y_lab": r"$E_{a}$ [kJ/mol]",
+            "legend": None,
+        }
+        # Update kwargs with the default key-value pairs if the key is not present in kwargs
+        kwargs = {**default_kwargs, **kwargs}
+        myfig = MyFigure(rows=1, cols=1, **kwargs)
+
+        myfig.axs[0].plot(self.alpha, self.activation_energy)
+
+        # Plotting the data points
+        myfig.axs[0].fill_between(
+            self.alpha,
+            self.activation_energy - self.activation_energy_std,
+            self.activation_energy + self.activation_energy_std,
+            alpha=0.3,
+        )
+        myfig.save_figure()
+        return myfig
+
+
+def plot_multi_activation_energy(
+    kassamples: list[KasSample],
+    labels: list[str] | None = None,
+    filename: str = "plot",
+    **kwargs,
+) -> MyFigure:
+    """
+    Plot the activation energy for multiple KAS analyses, comparing their kinetic parameters.
+
+    This function creates a plot showing the activation energy against conversion for a series of KasSample objects,
+    allowing for a comparative analysis of different samples or conditions.
+
+    :param kassamples: A list of KasSample objects for which the activation energy plots are generated.
+    :type kassamples: list[KasSample]
+    :param labels: Labels corresponding to each KasSample object. If None, the names of the samples are used.
+    :type labels: list[str], optional
+    :param filename: The base name for the file to save the plot. Defaults to "plot".
+    :type filename: str
+    :param kwargs: Additional keyword arguments for plot customization.
+    :type kwargs: dict
+    :return: A MyFigure instance containing the comparative activation energy plot.
+    :rtype: MyFigure
+    """
+
+    if labels is None:
+        labels = [sample.name for sample in kassamples]
+    for sample in kassamples:
+        if not sample.kas_analysis_computed:
+            sample.kas_analysis()
+
+    out_path = plib.Path(kassamples[0].out_path, "multisample_plots")
+    out_path.mkdir(parents=True, exist_ok=True)
+
+    default_kwargs = {
+        "filename": filename + "_activation_energy",
+        "out_path": out_path,
+        "height": 4,
+        "width": 4,
+        "grid": kassamples[0].plot_grid,
+        "text_font": kassamples[0].plot_font,
+        "x_lab": r"$\alpha$ [-]",
+        "y_lab": r"$E_{a}$ [kJ/mol]",
+    }
+    kwargs = {**default_kwargs, **kwargs}
+    myfig = MyFigure(
+        rows=1,
+        cols=1,
+        **kwargs,
+    )
+    for i, sample in enumerate(kassamples):
+        myfig.axs[0].plot(
+            sample.alpha,
+            sample.activation_energy,
+            color=colors[i],
+            linestyle=linestyles[i],
+            label=labels[i],
+        )
+
+        # Plotting the data points
+        myfig.axs[0].fill_between(
+            sample.alpha,
+            sample.activation_energy - sample.activation_energy_std,
+            sample.activation_energy + sample.activation_energy_std,
+            alpha=0.3,
+            color=colors[i],
+            linestyle=linestyles[i],
+        )
+    myfig.save_figure()
+    return myfig
```

### Comparing `tga_data_analysis-2.0.4/src/tga_data_analysis/measure.py` & `tga_data_analysis-2.0.6/src/tga_data_analysis/measure.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-from __future__ import annotations
-import numpy as np
-import pandas as pd
-from typing import Literal
-
-
-class Measure:
-    """
-    A class to handle and analyze a series of measurements or data points. It provides functionalities
-    to add new data, compute averages, and calculate standard deviations, supporting the analysis
-    of replicated measurement data.
-    """
-
-    std_type: Literal["population", "sample"] = "population"
-    if std_type == "population":
-        np_ddof: int = 0
-    elif std_type == "sample":
-        np_ddof: int = 1
-
-    @classmethod
-    def set_std_type(cls, new_std_type: Literal["population", "sample"]):
-        """
-        Set the standard deviation type for all instances of Measure.
-
-        This class method configures whether the standard deviation calculation should be
-        performed as a sample standard deviation or a population standard deviation.
-
-        :param new_std_type: The type of standard deviation to use ('population' or 'sample').
-        :type new_std_type: Literal["population", "sample"]
-        """
-        cls.std_type = new_std_type
-        if new_std_type == "population":
-            cls.np_ddof: int = 0
-        elif new_std_type == "sample":
-            cls.np_ddof: int = 1
-
-    def __init__(self, name: str | None = None):
-        """
-        Initialize a Measure object to store and analyze data.
-
-        :param name: An optional name for the Measure object, used for identification and reference in analyses.
-        :type name: str, optional
-        """
-        self.name = name
-        self._stk: dict[int : np.ndarray | float] = {}
-        self._ave: np.ndarray | float | None = None
-        self._std: np.ndarray | float | None = None
-
-    def __call__(self):
-        return self.ave()
-
-    def add(self, replicate: int, value: np.ndarray | pd.Series | float | int) -> None:
-        """
-        Add a new data point or series of data points to the Measure object.
-
-        :param replicate: The identifier for the replicate to which the data belongs.
-        :type replicate: int
-        :param value: The data point(s) to be added. Can be a single value or a series of values.
-        :type value: np.ndarray | pd.Series | float | int
-        """
-        if isinstance(value, (pd.Series, pd.DataFrame)):
-            value = value.to_numpy()
-        elif isinstance(value, np.ndarray):
-            value = value.flatten()
-        elif isinstance(value, (list, tuple)):
-            value = np.asarray(value)
-        self._stk[replicate] = value
-
-    def stk(self, replicate: int | None = None) -> np.ndarray | float:
-        """
-        Retrieve the data points for a specific replicate or all data if no replicate is specified.
-
-        :param replicate: The identifier for the replicate whose data is to be retrieved. If None, data for all replicates is returned.
-        :type replicate: int, optional
-        :return: The data points for the specified replicate or all data.
-        :rtype: np.ndarray | float
-        """
-        if replicate is None:
-            return self._stk
-        else:
-            return self._stk.get(replicate)
-
-    def ave(self) -> np.ndarray:
-        """
-        Calculate and return the average of the data points across all replicates.
-
-        :return: The average values for the data points.
-        :rtype: np.ndarray
-        """
-        if all(isinstance(v, np.ndarray) for v in self._stk.values()):
-            self._ave = np.mean(np.column_stack(list(self._stk.values())), axis=1)
-            return self._ave
-        else:
-            self._ave = np.mean(list(self._stk.values()))
-            return self._ave
-
-    def std(self) -> np.ndarray:
-        """
-        Calculate and return the standard deviation of the data points across all replicates.
-
-        :return: The standard deviation of the data points.
-        :rtype: np.ndarray
-        """
-        if all(isinstance(v, np.ndarray) for v in self._stk.values()):
-            self._std = np.std(
-                np.column_stack(list(self._stk.values())), axis=1, ddof=Measure.np_ddof
-            )
-            return self._std
-        else:
-            self._std = np.std(list(self._stk.values()), ddof=Measure.np_ddof)
-            return self._std
+from __future__ import annotations
+import numpy as np
+import pandas as pd
+from typing import Literal
+
+
+class Measure:
+    """
+    A class to handle and analyze a series of measurements or data points. It provides functionalities
+    to add new data, compute averages, and calculate standard deviations, supporting the analysis
+    of replicated measurement data.
+    """
+
+    std_type: Literal["population", "sample"] = "population"
+    if std_type == "population":
+        np_ddof: int = 0
+    elif std_type == "sample":
+        np_ddof: int = 1
+
+    @classmethod
+    def set_std_type(cls, new_std_type: Literal["population", "sample"]):
+        """
+        Set the standard deviation type for all instances of Measure.
+
+        This class method configures whether the standard deviation calculation should be
+        performed as a sample standard deviation or a population standard deviation.
+
+        :param new_std_type: The type of standard deviation to use ('population' or 'sample').
+        :type new_std_type: Literal["population", "sample"]
+        """
+        cls.std_type = new_std_type
+        if new_std_type == "population":
+            cls.np_ddof: int = 0
+        elif new_std_type == "sample":
+            cls.np_ddof: int = 1
+
+    def __init__(self, name: str | None = None):
+        """
+        Initialize a Measure object to store and analyze data.
+
+        :param name: An optional name for the Measure object, used for identification and reference in analyses.
+        :type name: str, optional
+        """
+        self.name = name
+        self._stk: dict[int : np.ndarray | float] = {}
+        self._ave: np.ndarray | float | None = None
+        self._std: np.ndarray | float | None = None
+
+    def __call__(self):
+        return self.ave()
+
+    def add(self, replicate: int, value: np.ndarray | pd.Series | float | int) -> None:
+        """
+        Add a new data point or series of data points to the Measure object.
+
+        :param replicate: The identifier for the replicate to which the data belongs.
+        :type replicate: int
+        :param value: The data point(s) to be added. Can be a single value or a series of values.
+        :type value: np.ndarray | pd.Series | float | int
+        """
+        if isinstance(value, (pd.Series, pd.DataFrame)):
+            value = value.to_numpy()
+        elif isinstance(value, np.ndarray):
+            value = value.flatten()
+        elif isinstance(value, (list, tuple)):
+            value = np.asarray(value)
+        self._stk[replicate] = value
+
+    def stk(self, replicate: int | None = None) -> np.ndarray | float:
+        """
+        Retrieve the data points for a specific replicate or all data if no replicate is specified.
+
+        :param replicate: The identifier for the replicate whose data is to be retrieved. If None, data for all replicates is returned.
+        :type replicate: int, optional
+        :return: The data points for the specified replicate or all data.
+        :rtype: np.ndarray | float
+        """
+        if replicate is None:
+            return self._stk
+        else:
+            return self._stk.get(replicate)
+
+    def ave(self) -> np.ndarray:
+        """
+        Calculate and return the average of the data points across all replicates.
+
+        :return: The average values for the data points.
+        :rtype: np.ndarray
+        """
+        if all(isinstance(v, np.ndarray) for v in self._stk.values()):
+            self._ave = np.mean(np.column_stack(list(self._stk.values())), axis=1)
+            return self._ave
+        else:
+            self._ave = np.mean(list(self._stk.values()))
+            return self._ave
+
+    def std(self) -> np.ndarray:
+        """
+        Calculate and return the standard deviation of the data points across all replicates.
+
+        :return: The standard deviation of the data points.
+        :rtype: np.ndarray
+        """
+        if all(isinstance(v, np.ndarray) for v in self._stk.values()):
+            self._std = np.std(
+                np.column_stack(list(self._stk.values())), axis=1, ddof=Measure.np_ddof
+            )
+            return self._std
+        else:
+            self._std = np.std(list(self._stk.values()), ddof=Measure.np_ddof)
+            return self._std
```

### Comparing `tga_data_analysis-2.0.4/src/tga_data_analysis/tga.py` & `tga_data_analysis-2.0.6/src/tga_data_analysis/tga.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1514 +1,1518 @@
-from __future__ import annotations
-from typing import Literal, Any
-import pathlib as plib
-import numpy as np
-import pandas as pd
-from scipy.signal import savgol_filter
-from lmfit.models import GaussianModel, LinearModel
-from tga_data_analysis.measure import Measure
-from tga_data_analysis.myfigure import MyFigure, clrs, lnstls
-
-
-
-class Project:
-    """
-    Represents a project (identified by the folder where the data is stored) for TGA data analysis.
-
-    """
-
-    def __init__(
-        self,
-        folder_path: plib.Path,
-        name: str | None = None,
-        temp_unit: Literal["C", "K"] = "C",
-        plot_font: Literal["Dejavu Sans", "Times New Roman"] = "Dejavu Sans",
-        dtg_basis: Literal["temperature", "time"] = "temperature",
-        temp_i_temp_b_threshold: float = 0.01,  # % of the peak that is used for Ti and Tb
-        resolution_sec_deg_dtg: int = 5,
-        dtg_window_filter: int = 101,
-        plot_grid: bool = False,
-        column_name_mapping: dict[str, str] | None = None,
-        load_skiprows: int = 0,
-        time_moist: float = 38.0,
-        time_vm: float = 147.0,
-        temp_initial_celsius: float = 40,
-        temp_lim_dtg_celsius: tuple[float] | None = None,
-        auto_save_reports: bool = True,
-    ):
-        """
-        Initialize a new Project instance with various parameters for analysis.
-
-        :param folder_path: The path to the folder containing the project data.
-        :type folder_path: plib.Path
-        :param name: The name of the project. Defaults to the last part of the folder path if None.
-        :type name: str, optional
-        :param temp_unit: The unit of temperature used in the project ('C':Celsius, 'K':Kelvin).
-        :type temp_unit: Literal["C", "K"]
-        :param plot_font: The font used in plots, either 'Dejavu Sans' or 'Times New Roman'.
-        :type plot_font: Literal["Dejavu Sans", "Times New Roman"]
-        :param dtg_basis: The basis for DTG calculations, either 'temperature' or 'time'.
-        :type dtg_basis: Literal["temperature", "time"]
-        :param temp_i_temp_b_threshold: The threshold for Ti and Tb calculation in DTG analysis.
-        :type temp_i_temp_b_threshold: float
-        :param resolution_sec_deg_dtg: The resolution in seconds or degrees for DTG analysis.
-        :type resolution_sec_deg_dtg: int
-        :param dtg_window_filter: The window size for the Savitzky-Golay filter in DTG analysis.
-        :type dtg_window_filter: int
-        :param plot_grid: Whether to display a grid in the plots.
-        :type plot_grid: bool
-        :param column_name_mapping: Mapping of column names from file to standard names used in the analysis.
-        :type column_name_mapping: dict[str, str], optional
-        :param load_skiprows: The number of rows to skip when loading data files.
-        :type load_skiprows: int
-        :param time_moist: The time considered for the moisture analysis.
-        :type time_moist: float
-        :param time_vm: The time considered for the volatile matter analysis.
-        :type time_vm: float
-        :param temp_initial_celsius: The initial temperature for certain calculations, in Celsius.
-        :type temp_initial_celsius: float
-        :param temp_lim_dtg_celsius: The temperature limits for DTG analysis, in Celsius.
-        :type temp_lim_dtg_celsius: tuple[float], optional
-        :param auto_save_reports: Whether to automatically save generated reports.
-        :type auto_save_reports: bool
-        """
-        self.folder_path = folder_path
-        self.out_path = plib.Path(folder_path, "output")
-        if name is None:
-            self.name = self.folder_path.parts[-1]
-        else:
-            self.name = name
-        self.temp_unit = temp_unit
-        self.plot_font = plot_font
-        self.plot_grid = plot_grid
-        self.dtg_basis = dtg_basis
-        self.temp_i_temp_b_threshold = temp_i_temp_b_threshold
-        self.resolution_sec_deg_dtg = resolution_sec_deg_dtg
-        self.dtg_window_filter = dtg_window_filter
-        self.load_skiprows = load_skiprows
-        self.time_moist = time_moist
-        self.time_vm = time_vm
-        self.temp_initial_celsius = temp_initial_celsius
-        self.auto_save_reports = auto_save_reports
-
-        if self.temp_unit == "C":
-            self.temp_symbol = "°C"
-        elif self.temp_unit == "K":
-            self.temp_symbol = "K"
-
-        self.tg_label = "TG [wt%]"
-        if self.dtg_basis == "temperature":
-            self.dtg_label = "DTG [wt%/" + self.temp_symbol + "]"
-        elif self.dtg_basis == "time":
-            self.dtg_label = "DTG [wt%/min]"
-
-        if temp_lim_dtg_celsius is None:
-            self.temp_lim_dtg_celsius = (120, 880)
-        else:
-            self.temp_lim_dtg_celsius = temp_lim_dtg_celsius
-        if self.temp_unit == "C":
-            self.temp_lim_dtg = self.temp_lim_dtg_celsius
-        elif self.temp_unit == "K":
-            self.temp_lim_dtg = [t + 273.15 for t in self.temp_lim_dtg_celsius]
-        else:
-            raise ValueError(f"{self.temp_unit = } is not acceptable")
-
-        self.len_dtg_db: int = int(
-            (self.temp_lim_dtg[1] - self.temp_lim_dtg[0]) * self.resolution_sec_deg_dtg
-        )
-        self.temp_dtg: np.ndarray = np.linspace(
-            self.temp_lim_dtg[0], self.temp_lim_dtg[1], self.len_dtg_db
-        )
-
-        if column_name_mapping is None:
-            self.column_name_mapping = {
-                "Time": "t_min",
-                "Temperature": "T_C",
-                "Weight": "m_p",
-                "Weight.1": "m_mg",
-                "Heat Flow": "heatflow_mW",
-                "##Temp./>C": "T_C",
-                "Time/min": "t_min",
-                "Mass/%": "m_p",
-                "Segment": "segment",
-            }
-        else:
-            self.column_name_mapping = column_name_mapping
-        #
-        self.samples: dict[str, Sample] = {}
-        self.samplenames: list[str] = []
-
-        self.multireports: dict[str, pd.DataFrame] = {}
-        self.multireport_types_computed: list[str] = []
-
-    def add_sample(self, samplename: str, sample: Sample):
-        """
-        Add a sample to the project.
-
-        :param samplename: The name of the sample to add.
-        :type samplename: str
-        :param sample: The sample object to add.
-        :type sample: Sample
-        """
-        if samplename not in self.samplenames:
-            self.samplenames.append(samplename)
-            self.samples[samplename] = sample
-        else:
-            print(f"{samplename = } already present in project. Sample not added.")
-
-    def multireport(
-        self,
-        samples: list[Sample] | None = None,
-        labels: list[str] | None = None,
-        report_type: Literal[
-            "proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"
-        ] = "proximate",
-        report_style: Literal["repl_ave_std", "ave_std", "ave_pm_std"] = "ave_std",
-        decimals_in_ave_pm_std: int = 2,
-        filename: str | None = None,
-    ) -> pd.DataFrame:
-        """
-        Generate a multi-sample report based on the specified report type and style.
-
-        :param samples: A list of Sample objects to include in the report. If None, uses all samples in the project.
-        :type samples: list[Sample], optional
-        :param labels: A list of labels corresponding to each sample. If None, sample names are used as labels.
-        :type labels: list[str], optional
-        :param report_type: The type of report to generate, choices include 'proximate', 'oxidation', 'oxidation_extended', 'soliddist', and 'soliddist_extended'.
-        :type report_type: Literal["proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"]
-        :param report_style: The style of the report, choices are 'repl_ave_std', 'ave_std', and 'ave_pm_std'.
-        :type report_style: Literal["repl_ave_std", "ave_std", "ave_pm_std"]
-        :param decimals_in_ave_pm_std: The number of decimal places to use for the average plus-minus standard deviation format.
-        :type decimals_in_ave_pm_std: int
-        :param filename: The name of the file to save the report. If None, the report is not saved.
-        :type filename: str, optional
-        :return: A pandas DataFrame containing the generated report.
-        :rtype: pd.DataFrame
-        """
-        if samples is None:
-            samples = list(self.samples.values())
-
-        samplenames = [sample.name for sample in samples]
-
-        if labels is None:
-            labels = samplenames
-        for sample in samples:
-            if report_type not in sample.report_types_computed:
-                sample.report(report_type)
-
-        if report_type == "soliddist":
-            reports = [sample.reports[report_type] for sample in samples]
-            reports = self._reformat_ave_std_columns(reports)
-        elif report_type == "soliddist_extended":
-            raise ValueError(
-                f"{report_type = } not allowed for multireport, use 'soliddist' instead"
-            )
-        else:
-            reports = [sample.reports[report_type] for sample in samples]
-
-        if report_style == "repl_ave_std":
-            # Concatenate all individual reports
-            report = pd.concat(reports, keys=labels)
-            report.index.names = [None, None]  # Remove index names
-
-        elif report_style == "ave_std":
-            # Keep only the average and standard deviation
-            ave_std_dfs = []
-            for label, report in zip(labels, reports):
-                ave_std_dfs.append(report.loc[["ave", "std"]])
-            report = pd.concat(ave_std_dfs, keys=labels)
-            report.index.names = [None, None]  # Remove index names
-
-        elif report_style == "ave_pm_std":
-            # Format as "ave ± std" and use sample name as the index
-            rows = []
-            for label, report in zip(labels, reports):
-                row = {
-                    col: f"{report.at['ave', col]:.{decimals_in_ave_pm_std}f} ± {report.at['std', col]:.{decimals_in_ave_pm_std}f}"
-                    for col in report.columns
-                }
-                rows.append(pd.Series(row, name=label))
-            report = pd.DataFrame(rows)
-
-        else:
-            raise ValueError(f"{report_style = } is not a valid option")
-        self.multireport_types_computed.append(report_type)
-        self.multireports[report_type] = report
-        if self.auto_save_reports:
-            out_path = plib.Path(self.out_path, "multireports")
-            out_path.mkdir(parents=True, exist_ok=True)
-            if filename is None:
-                filename = f"{self.name}_{report_type}_{report_style}.xlsx"
-            else:
-                filename = filename + ".xlsx"
-            report.to_excel(plib.Path(out_path, filename))
-        return report
-
-    def plot_multireport(
-        self,
-        filename: str = "plot",
-        samples: list[Sample] | None = None,
-        labels: list[str] | None = None,
-        report_type: Literal["proximate", "oxidation", "soliddist"] = "proximate",
-        bar_labels: list[str] | None = None,
-        **kwargs,
-    ) -> MyFigure:
-        """
-        Generate a plot for the multi-sample report.
-
-        :param filename: The name of the file to save the plot. Defaults to "plot".
-        :type filename: str
-        :param samples: A list of Sample objects to include in the plot. If None, uses all samples in the project.
-        :type samples: list[Sample], optional
-        :param labels: A list of labels corresponding to each sample. If None, sample names are used as labels.
-        :type labels: list[str], optional
-        :param report_type: The type of report to plot, choices include 'proximate', 'oxidation', and 'soliddist'.
-        :type report_type: Literal["proximate", "oxidation", "soliddist"]
-        :param bar_labels: Labels for the bars in the plot. If None, default labels based on the report type are used.
-        :type bar_labels: list[str], optional
-        :param kwargs: Additional keyword arguments to pass to the plotting function.
-        :type kwargs: dict
-        :return: An instance of MyFigure containing the generated plot.
-        :rtype: MyFigure
-        """
-        if samples is None:
-            samples = list(self.samples.values())
-
-        samplenames = [sample.name for sample in samples]
-        if labels is None:
-            labels = samplenames
-
-        df = self.multireport(samples, labels, report_type, report_style="ave_std")
-        df_ave = df.xs("ave", level=1, drop_level=False)
-        df_std = df.xs("std", level=1, drop_level=False)
-        # drop the multi-level index to simplify the DataFrame
-        df_ave = df_ave.droplevel(1)
-        df_std = df_std.droplevel(1)
-
-        if report_type == "proximate":
-            if bar_labels is None:
-                vars_bar = ["moisture (stb)", "VM (db)", "FC (db)", "ash (db)"]
-            else:
-                vars_bar = bar_labels
-            df_ave.columns = vars_bar
-            df_std.columns = vars_bar
-            bar_yaxis = vars_bar
-            bar_ytaxis = None
-            twinx = None
-            y_lab = self.tg_label
-            yt_lab = None
-
-        elif report_type == "oxidation":
-            if bar_labels is None:
-                vars_bar = ["T$_i$", "T$_p$", "T$_b$", "S"]
-            else:
-                vars_bar = bar_labels
-            df_ave.columns = vars_bar
-            df_std.columns = vars_bar
-            bar_yaxis = vars_bar[:3]
-            bar_ytaxis = vars_bar[-1]
-            twinx = True
-            y_lab = f"T [{self.temp_symbol}]"
-            yt_lab = "S (comb. index)"
-
-        elif report_type == "soliddist":
-            if bar_labels is None:
-                vars_bar = [f"{col.split(" ")[0]} {col.split(" ")[-1]}" for col in df_ave.columns]
-            else:
-                vars_bar = bar_labels
-            df_ave.columns = vars_bar
-            df_std.columns = vars_bar
-            bar_yaxis = vars_bar
-            bar_ytaxis = None
-            twinx = None
-            y_lab = "step mass loss [wt%]"
-            yt_lab = None
-
-        out_path = plib.Path(self.out_path, "multireport_plots")
-        out_path.mkdir(parents=True, exist_ok=True)
-        default_kwargs = {
-            "filename": filename + report_type,
-            "out_path": out_path,
-            "height": 3.2,
-            "width": 3.2,
-            "grid": self.plot_grid,
-            "text_font": self.plot_font,
-        }
-        # Update kwargs with the default key-value pairs if the key is not present in kwargs
-        kwargs = {**default_kwargs, **kwargs}
-        myfig = MyFigure(
-            rows=1,
-            cols=1,
-            twinx=twinx,
-            y_lab=y_lab,
-            yt_lab=yt_lab,
-            **kwargs,
-        )
-        df_ave[bar_yaxis].plot(
-            ax=myfig.axs[0],
-            kind="bar",
-            yerr=df_std[bar_yaxis],
-            capsize=2,
-            width=0.85,
-            ecolor="k",
-            edgecolor="black",
-        )
-        if bar_ytaxis is not None:
-            myfig.axts[0].scatter(
-                df_ave.index,
-                df_ave[bar_ytaxis],
-                label=bar_ytaxis,
-                edgecolor="black",
-                color=clrs[3],
-                # s=100
-            )
-            myfig.axts[0].errorbar(
-                df_ave.index,
-                df_ave[bar_ytaxis],
-                yerr=df_std[bar_ytaxis],
-                ecolor="k",
-                linestyle="None",
-                capsize=2,
-            )
-        myfig.save_figure()
-        return myfig
-
-    def plot_multi_tg(
-        self,
-        filename: str = "plot",
-        samples: list[Sample] | None = None,
-        labels: list[str] | None = None,
-        **kwargs,
-    ) -> MyFigure:
-        """
-        Plot multiple thermogravimetric (TG) curves for the given samples.
-
-        :param filename: The name of the file to save the plot. Defaults to "plot".
-        :type filename: str
-        :param samples: A list of Sample objects to be plotted. If None, plots all samples in the project.
-        :type samples: list[Sample], optional
-        :param labels: Labels for each sample in the plot. If None, sample names are used.
-        :type labels: list[str], optional
-        :param kwargs: Additional keyword arguments for plotting customization.
-        :type kwargs: dict
-        :return: A MyFigure instance containing the plot.
-        :rtype: MyFigure
-        """
-        if samples is None:
-            samples = list(self.samples.values())
-
-        samplenames = [sample.name for sample in samples]
-        if labels is None:
-            labels = samplenames
-        for sample in samples:
-            if not sample.proximate_computed:
-                sample.proximate_analysis()
-
-        out_path = plib.Path(self.out_path, "multisample_plots")
-        out_path.mkdir(parents=True, exist_ok=True)
-
-        default_kwargs = {
-            "filename": filename + "_tg",
-            "out_path": out_path,
-            "height": 3.2,
-            "width": 3.2,
-            "grid": self.plot_grid,
-            "text_font": self.plot_font,
-            "x_lab": f"T [{self.temp_symbol}]",
-            "y_lab": self.tg_label,
-            "x_lim": self.temp_lim_dtg,
-        }
-        # Update kwargs with the default key-value pairs if the key is not present in kwargs
-        kwargs = {**default_kwargs, **kwargs}
-
-        myfig = MyFigure(
-            rows=1,
-            cols=1,
-            **kwargs,
-        )
-        for i, sample in enumerate(samples):
-            myfig.axs[0].plot(
-                sample.temp.ave(),
-                sample.mp_db.ave(),
-                color=clrs[i],
-                linestyle=lnstls[i],
-                label=labels[i],
-            )
-            myfig.axs[0].fill_between(
-                sample.temp.ave(),
-                sample.mp_db.ave() - sample.mp_db.std(),
-                sample.mp_db.ave() + sample.mp_db.std(),
-                color=clrs[i],
-                alpha=0.3,
-            )
-        myfig.save_figure()
-        return myfig
-
-    def plot_multi_dtg(
-        self,
-        filename: str = "plot",
-        samples: list[Sample] | None = None,
-        labels: list[str] | None = None,
-        **kwargs,
-    ) -> MyFigure:
-        """
-        Plot multiple derivative thermogravimetric (DTG) curves for the given samples.
-
-        :param filename: The name of the file to save the plot. Defaults to "plot".
-        :type filename: str
-        :param samples: A list of Sample objects to be plotted. If None, plots all samples in the project.
-        :type samples: list[Sample], optional
-        :param labels: Labels for each sample in the plot. If None, sample names are used.
-        :type labels: list[str], optional
-        :param kwargs: Additional keyword arguments for plotting customization.
-        :type kwargs: dict
-        :return: A MyFigure instance containing the plot.
-        :rtype: MyFigure
-        """
-        if samples is None:
-            samples = list(self.samples.values())
-
-        samplenames = [sample.name for sample in samples]
-        if labels is None:
-            labels = samplenames
-        for sample in samples:
-            if not sample.proximate_computed:
-                sample.proximate_analysis()
-
-        out_path = plib.Path(self.out_path, "multisample_plots")
-        out_path.mkdir(parents=True, exist_ok=True)
-        default_kwargs = {
-            "filename": filename + "_dtg",
-            "out_path": out_path,
-            "height": 3.2,
-            "width": 3.2,
-            "grid": self.plot_grid,
-            "text_font": self.plot_font,
-            "x_lab": f"T [{self.temp_symbol}]",
-            "y_lab": self.dtg_label,
-            "x_lim": self.temp_lim_dtg,
-        }
-        # Update kwargs with the default key-value pairs if the key is not present in kwargs
-        kwargs = {**default_kwargs, **kwargs}
-
-        myfig = MyFigure(
-            rows=1,
-            cols=1,
-            **kwargs,
-        )
-        for i, sample in enumerate(samples):
-            myfig.axs[0].plot(
-                sample.temp_dtg,
-                sample.dtg_db.ave(),
-                color=clrs[i],
-                linestyle=lnstls[i],
-                label=labels[i],
-            )
-            myfig.axs[0].fill_between(
-                sample.temp_dtg,
-                sample.dtg_db.ave() - sample.dtg_db.std(),
-                sample.dtg_db.ave() + sample.dtg_db.std(),
-                color=clrs[i],
-                alpha=0.3,
-            )
-        myfig.save_figure()
-        return myfig
-
-    def plot_multi_soliddist(
-        self,
-        filename: str = "plot",
-        samples: list[Sample] | None = None,
-        labels: list[str] | None = None,
-        **kwargs,
-    ) -> MyFigure:
-        """
-        Plot multiple solid distribution curves for the given samples.
-
-        :param filename: The name of the file to save the plot. Defaults to "plot".
-        :type filename: str
-        :param samples: A list of Sample objects to be plotted. If None, plots all samples in the project.
-        :type samples: list[Sample], optional
-        :param labels: Labels for each sample in the plot. If None, sample names are used.
-        :type labels: list[str], optional
-        :param kwargs: Additional keyword arguments for plotting customization.
-        :type kwargs: dict
-        :return: A MyFigure instance containing the plot.
-        :rtype: MyFigure
-        """
-        if samples is None:
-            samples = list(self.samples.values())
-
-        samplenames = [sample.name for sample in samples]
-        if labels is None:
-            labels = samplenames
-        for sample in samples:
-            if not sample.proximate_computed:
-                sample.proximate_analysis()
-
-        out_path = plib.Path(self.out_path, "multisample_plots")
-        out_path.mkdir(parents=True, exist_ok=True)
-        default_kwargs = {
-            "filename": filename + "_soliddist",
-            "out_path": out_path,
-            "height": 3.2,
-            "width": 3.2,
-            "grid": self.plot_grid,
-            "text_font": self.plot_font,
-            "x_lab": "time [min]",
-            "y_lab": self.tg_label,
-            "yt_lab": f"T [{self.temp_symbol}]",
-            "legend_loc": "center left",
-        }
-        # Update kwargs with the default key-value pairs if the key is not present in kwargs
-        kwargs = {**default_kwargs, **kwargs}
-
-        myfig = MyFigure(
-            rows=1,
-            twinx=True,
-            **kwargs,
-        )
-        myfig.axts[0].plot(
-            samples[0].time.ave(), samples[0].temp.ave(), color="k", linestyle=lnstls[1], label="T"
-        )
-        for i, sample in enumerate(samples):
-
-            myfig.axs[0].plot(
-                sample.time.ave(),
-                sample.mp_db.ave(),
-                color=clrs[i],
-                linestyle=lnstls[i],
-                label=labels[i],
-            )
-            myfig.axs[0].fill_between(
-                sample.time.ave(),
-                sample.mp_db.ave() - sample.mp_db.std(),
-                sample.mp_db.ave() + sample.mp_db.std(),
-                color=clrs[i],
-                alpha=0.3,
-            )
-        myfig.save_figure()
-        return myfig
-
-    def _reformat_ave_std_columns(self, reports):
-        """
-        Reformat the columns of the given reports to have standard deviation and average values.
-
-        This method is intended to be used internally within the Project class to standardize
-        the report dataframes before generating multi-sample reports.
-
-        :param reports: A list of report DataFrames to reformat.
-        :type reports: list[pd.DataFrame]
-        :return: A list of reformatted DataFrames.
-        :rtype: list[pd.DataFrame]
-        """
-        # Check that all reports have the same number of columns
-        num_columns = len(reports[0].columns)
-        if not all(len(report.columns) == num_columns for report in reports):
-            raise ValueError("All reports must have the same number of columns.")
-
-        # Initialize a list to hold the new formatted column names
-        formatted_column_names = []
-
-        # Iterate over each column index
-        for i in range(num_columns):
-            # Extract the numeric part of the column name (assume it ends with ' K' or ' C')
-            column_values = [float(report.columns[i].split()[0]) for report in reports]
-            ave = np.mean(column_values)
-            std = np.std(column_values)
-
-            # Determine the unit (assuming all columns have the same unit)
-            unit = reports[0].columns[i].split()[-1]
-
-            # Create the new column name with the unit
-            formatted_column_name = f"{ave:.0f} ± {std:.0f} {unit}"
-            formatted_column_names.append(formatted_column_name)
-
-        # Rename the columns in each report using the new formatted names
-        for report in reports:
-            report.columns = formatted_column_names
-
-        return reports
-
-
-class Sample:
-    """
-    A class representing a sample in the project, containing methods for loading, processing,
-    and analyzing thermogravimetric analysis (TGA) data associated with the sample.
-    """
-
-    def __init__(
-        self,
-        project: Project,
-        name: str,
-        filenames: list[str],
-        folder_path: plib.Path | None = None,
-        label: str | None = None,
-        correct_ash_mg: list[float] | None = None,
-        correct_ash_fr: list[float] | None = None,
-        column_name_mapping: dict[str:str] | None = None,
-        load_skiprows: int = 0,
-        time_moist: float = 38.0,
-        time_vm: float = 147,
-        heating_rate_deg_min: float | None = None,
-        temp_i_temp_b_threshold: float | None = None,
-    ):
-        """
-        Initialize a new Sample instance with parameters for TGA data analysis.
-
-        :param project: The Project object to which this sample belongs.
-        :type project: Project
-        :param name: The name of the sample.
-        :type name: str
-        :param filenames: A list of filenames associated with the sample.
-        :type filenames: list[str]
-        :param folder_path: The path to the folder containing the sample data. If None, the project's folder path is used.
-        :type folder_path: plib.Path, optional
-        :param label: A label for the sample. If None, the sample's name is used as the label.
-        :type label: str, optional
-        :param correct_ash_mg: A list of ash correction values in milligrams, one per file.
-        :type correct_ash_mg: list[float], optional
-        :param correct_ash_fr: A list of ash correction values as a fraction, one per file.
-        :type correct_ash_fr: list[float], optional
-        :param column_name_mapping: A dictionary mapping file column names to standardized column names for analysis.
-        :type column_name_mapping: dict[str, str], optional
-        :param load_skiprows: The number of rows to skip at the beginning of the files when loading.
-        :type load_skiprows: int
-        :param time_moist: The time considered for the moisture analysis.
-        :type time_moist: float
-        :param time_vm: The time considered for the volatile matter analysis.
-        :type time_vm: float
-        :param heating_rate_deg_min: The heating rate in degrees per minute, used for certain calculations.
-        :type heating_rate_deg_min: float, optional
-        :param temp_i_temp_b_threshold: The threshold percentage used for calculating initial and final temperatures in DTG analysis.
-        :type temp_i_temp_b_threshold: float, optional
-        """
-        # store the sample in the project
-        self.project_name = project.name
-        project.add_sample(name, self)
-        # prject defaults unless specified
-
-        self.out_path = project.out_path
-        self.temp_unit = project.temp_unit
-        self.temp_symbol = project.temp_symbol
-        self.tg_label = project.tg_label
-        self.dtg_label = project.dtg_label
-        self.plot_font = project.plot_font
-        self.plot_grid = project.plot_grid
-        self.dtg_basis = project.dtg_basis
-        self.temp_lim_dtg = project.temp_lim_dtg
-        self.len_dtg_db = project.len_dtg_db
-        self.temp_dtg = project.temp_dtg
-        self.auto_save_reports = project.auto_save_reports
-
-        self.resolution_sec_deg_dtg = project.resolution_sec_deg_dtg
-        self.dtg_window_filter = project.dtg_window_filter
-        self.temp_initial_celsius = project.temp_initial_celsius
-        self.dtg_window_filter = project.dtg_window_filter
-        if folder_path is None:
-            self.folder_path = project.folder_path
-        else:
-            self.folder_path = folder_path
-        if column_name_mapping is None:
-            self.column_name_mapping = project.column_name_mapping
-        else:
-            self.column_name_mapping = column_name_mapping
-        if load_skiprows is None:
-            self.load_skiprows = project.load_skiprows
-        else:
-            self.load_skiprows = load_skiprows
-        if time_moist is None:
-            self.time_moist = project.time_moist
-        else:
-            self.time_moist = time_moist
-        if time_vm is None:
-            self.time_vm = project.time_vm
-        else:
-            self.time_vm = time_vm
-        if temp_i_temp_b_threshold is None:
-            self.temp_i_temp_b_threshold = project.temp_i_temp_b_threshold
-        else:
-            self.temp_i_temp_b_threshold = temp_i_temp_b_threshold
-        # sample default
-        self.name = name
-        self.filenames = filenames
-        self.n_repl = len(self.filenames)
-        self.heating_rate_deg_min = heating_rate_deg_min
-        self.correct_ash_mg = self._broadcast_value_prop(correct_ash_mg)
-        self.correct_ash_fr = self._broadcast_value_prop(correct_ash_fr)
-        if not label:
-            self.label = name
-        else:
-            self.label = label
-
-        # for variables and computations
-        self.files: dict[str : pd.DataFrame] = {}
-        self.len_files: dict[str : pd.DataFrame] = {}
-        self.len_sample: int = 0
-
-        # proximate
-        self.temp: Measure = Measure(name="temp_" + self.temp_unit)
-        self.time: Measure = Measure(name="time")
-        self.m_ar: Measure = Measure(name="m_ar")
-        self.mp_ar: Measure = Measure(name="mp_ar")
-        self.idx_moist: Measure = Measure(name="idx_moist")
-        self.idx_vm: Measure = Measure(name="idx_vm")
-        self.moist_ar: Measure = Measure(name="moist_ar")
-        self.ash_ar: Measure = Measure(name="ash_ar")
-        self.fc_ar: Measure = Measure(name="fc_ar")
-        self.vm_ar: Measure = Measure(name="vm_ar")
-        self.mp_db: Measure = Measure(name="mp_db")
-        self.ash_db: Measure = Measure(name="ash_db")
-        self.fc_db: Measure = Measure(name="fc_db")
-        self.vm_db: Measure = Measure(name="vm_db")
-        self.mp_daf: Measure = Measure(name="mp_daf")
-        self.fc_daf: Measure = Measure(name="fc_daf")
-        self.vm_daf: Measure = Measure(name="vm_daf")
-        self.time_dtg: Measure = Measure(name="time_dtg")
-        self.mp_db_dtg: Measure = Measure(name="mp_db_dtg")
-        self.dtg_db: Measure = Measure(name="dtg_db")
-        self.ave_dev_tga_perc: float | None = None
-        # oxidation
-        self.temp_i_idx: Measure = Measure(name="temp_i_idx")
-        self.temp_i: Measure = Measure(name="temp_i_" + self.temp_unit)
-        self.temp_p_idx: Measure = Measure(name="temp_p_idx")
-        self.temp_p: Measure = Measure(name="temp_p_" + self.temp_unit)
-        self.temp_b_idx: Measure = Measure(name="temp_b_idx")
-        self.temp_b: Measure = Measure(name="temp_b_" + self.temp_unit)
-        self.dwdtemp_max: Measure = Measure(name="dwdtemp_max")
-        self.dwdtemp_mean: Measure = Measure(name="dwdtemp_mean")
-        self.s_combustion_index: Measure = Measure(name="s_combustion_index")
-        # soliddist
-        self.temp_soliddist: Measure = Measure(name="temp_dist_" + self.temp_unit)
-        self.time_soliddist: Measure = Measure(name="time_dist")
-        self.dmp_soliddist: Measure = Measure(name="dmp_dist")
-        self.loc_soliddist: Measure = Measure(name="loc_dist")
-        # deconvolution
-        self.dcv_best_fit: Measure = Measure(name="dcv_best_fit")
-        self.dcv_r2: Measure = Measure(name="dcv_r2")
-        self.dcv_peaks: list[Measure] = []
-        # Flag to track if data is loaded
-        self.proximate_computed = False
-        self.files_loaded = False
-        self.oxidation_computed = False
-        self.soliddist_computed = False
-        self.deconv_computed = False
-        # for reports
-        self.reports: dict[str, pd.DataFrame] = {}
-        self.report_types_computed: list[str] = []
-
-        self.load_files()
-        self.proximate_analysis()
-
-    def _broadcast_value_prop(self, prop: list | str | float | int | bool) -> list:
-        """
-        Broadcast a single value or a list of values to match the number of replicates.
-
-        This method is used internally to ensure that properties like corrections have a value
-        for each replicate, even if a single value is provided for all.
-
-        :param prop: A single value or a list of values to be broadcasted.
-        :type prop: list | float | int | bool
-        :return: A list of values with length equal to the number of replicates.
-        :rtype: list
-        """
-        if prop is None:
-            broad_prop = [None] * self.n_repl
-        if isinstance(prop, (list, tuple)):
-            # If it's a list or tuple, but we're not expecting pairs, it's a single value per axis.
-            if len(prop) == self.n_repl:
-                broad_prop = prop
-            else:
-                raise ValueError(
-                    f"The size of the property '{prop}' does not match the number of replicates."
-                )
-        if isinstance(prop, (str, float, int, bool)):
-            broad_prop = [prop] * self.n_repl
-        return broad_prop
-
-    def load_single_file(
-        self,
-        filename: str,
-        folder_path: plib.Path | None = None,
-        load_skiprows: int | None = None,
-        column_name_mapping: dict | None = None,
-    ) -> pd.DataFrame:
-        """
-        Load data from a single file associated with the sample.
-
-        :param filename: The name of the file to be loaded.
-        :type filename: str
-        :param folder_path: The folder path where the file is located. If None, uses the sample's folder path.
-        :type folder_path: plib.Path, optional
-        :param load_skiprows: The number of rows to skip at the beginning of the file. If None, uses the sample's default.
-        :type load_skiprows: int, optional
-        :param column_name_mapping: A mapping of file column names to standardized column names. If None, uses the sample's default.
-        :type column_name_mapping: dict, optional
-        :return: The loaded data as a pandas DataFrame.
-        :rtype: pd.DataFrame
-        """
-        if column_name_mapping is None:
-            column_name_mapping = self.column_name_mapping
-        if folder_path is None:
-            folder_path = self.folder_path
-        if load_skiprows is None:
-            load_skiprows = self.load_skiprows
-        file_path = plib.Path(folder_path, filename + ".txt")
-        if not file_path.is_file():
-            file_path = plib.Path(folder_path, filename + ".csv")
-        file = pd.read_csv(file_path, sep="\t", skiprows=load_skiprows)
-        if file.shape[1] < 3:
-            file = pd.read_csv(file_path, sep=",", skiprows=load_skiprows)
-        file = file.rename(columns={col: column_name_mapping.get(col, col) for col in file.columns})
-        for column in file.columns:
-            file[column] = pd.to_numeric(file[column], errors="coerce")
-        file.dropna(inplace=True)
-        return file
-
-    def correct_file_values(
-        self,
-        file: pd.DataFrame,
-        correct_ash_fr: float | None,
-        correct_ash_mg: float | None,
-    ):
-        """
-        Apply corrections to the loaded file data.
-
-        This method adjusts the mass measurements in the file based on provided ash correction values.
-
-        :param file: The data file to be corrected.
-        :type file: pd.DataFrame
-        :param correct_ash_mg: The correction value for ash in milligrams. If None, no correction is applied.
-        :type correct_ash_mg: float, optional
-        :param correct_ash_fr: The correction value for ash as a fraction. If None, no correction is applied.
-        :type correct_ash_fr: float, optional
-        :return: The corrected data as a pandas DataFrame.
-        :rtype: pd.DataFrame
-        """
-        if correct_ash_mg is not None:
-            file["m_mg"] = file["m_mg"] - np.min(file["m_mg"]) + correct_ash_mg
-        try:
-            if file["m_mg"].iloc[-1] < 0:
-                print(
-                    "neg. mass correction: Max [mg]",
-                    np.round(np.max(file["m_mg"]), 3),
-                    "; Min [mg]",
-                    np.round(np.min(file["m_mg"]), 3),
-                )
-                file["m_mg"] = file["m_mg"] - np.min(file["m_mg"])
-        except KeyError:
-            file["m_mg"] = file["m_p"]
-        file["m_p"] = file["m_mg"] / np.max(file["m_mg"]) * 100
-        if correct_ash_fr is not None:
-            file["m_p"] = file["m_p"] - np.min(file["m_p"]) + correct_ash_fr
-            file["m_p"] = file["m_p"] / np.max(file["m_p"]) * 100
-        file = file[file["T_C"] >= self.temp_initial_celsius].copy()
-        file["T_K"] = file["T_C"] + 273.15
-        return file
-
-    def load_files(self):
-        """
-        Load all files associated with this sample, applying necessary corrections and adjustments.
-
-        This method loads and processes each file, ensuring consistent data structure and applying
-        corrections such as ash content adjustments.
-
-        :return: A dictionary where keys are filenames and values are the corresponding corrected data as pandas DataFrames.
-        :rtype: dict[str, pd.DataFrame]
-        """
-        print("\n" + self.name)
-        # import files and makes sure that replicates have the same size
-        for f, filename in enumerate(self.filenames):
-            print(filename)
-            file_to_correct = self.load_single_file(filename)
-
-            file = self.correct_file_values(
-                file_to_correct, self.correct_ash_fr[f], self.correct_ash_fr[f]
-            )
-            # FILE CORRECTION
-            self.files[filename] = file
-            self.len_files[filename] = max(file.shape)
-        self.len_sample = min(self.len_files.values())
-        # keep the shortest vector size for all replicates, create the object
-        for filename in self.filenames:
-            self.files[filename] = self.files[filename].head(self.len_sample)
-        self.files_loaded = True  # Flag to track if data is loaded
-        return self.files
-
-    def proximate_analysis(self):
-        """
-        Perform proximate analysis on the loaded data for the sample.
-
-        This analysis calculates moisture content, ash content, volatile matter, and fixed carbon
-        based on the thermogravimetric data. The results are stored in the instance's attributes for later use.
-        """
-        if not self.files_loaded:
-            self.load_files()
-
-        for f, file in enumerate(self.files.values()):
-            if self.temp_unit == "C":
-                self.temp.add(f, file["T_C"])
-            elif self.temp_unit == "K":
-                self.temp.add(f, file["T_K"])
-            self.time.add(f, file["t_min"])
-
-            self.m_ar.add(f, file["m_mg"])
-            self.mp_ar.add(f, file["m_p"])
-
-            self.idx_moist.add(f, np.argmax(self.time.stk(f) > self.time_moist + 0.01))
-
-            self.moist_ar.add(f, 100 - self.mp_ar.stk(f)[self.idx_moist.stk(f)])
-            self.ash_ar.add(f, self.mp_ar.stk(f)[-1])
-            self.mp_db.add(f, self.mp_ar.stk(f) * 100 / (100 - self.moist_ar.stk(f)))
-            self.mp_db.add(f, np.where(self.mp_db.stk(f) > 100, 100, self.mp_db.stk(f)))
-            self.ash_db.add(f, self.ash_ar.stk(f) * 100 / (100 - self.moist_ar.stk(f)))
-            self.mp_daf.add(
-                f, ((self.mp_db.stk(f) - self.ash_db.stk(f)) * 100 / (100 - self.ash_db.stk(f)))
-            )
-            if self.time_vm is not None:
-                self.idx_vm.add(f, np.argmax(self.time.stk(f) > self.time_vm))
-                self.fc_ar.add(f, self.mp_ar.stk(f)[self.idx_vm.stk(f)] - self.ash_ar.stk(f))
-                self.vm_ar.add(
-                    f, (100 - self.moist_ar.stk(f) - self.ash_ar.stk(f) - self.fc_ar.stk(f))
-                )
-                self.vm_db.add(f, self.vm_ar.stk(f) * 100 / (100 - self.moist_ar.stk(f)))
-                self.fc_db.add(f, self.fc_ar.stk(f) * 100 / (100 - self.moist_ar.stk(f)))
-
-                self.vm_daf.add(
-                    f, ((self.vm_db.stk(f) - self.ash_db.stk(f)) * 100 / (100 - self.ash_db.stk(f)))
-                )
-                self.fc_daf.add(
-                    f, ((self.fc_db.stk(f) - self.ash_db.stk(f)) * 100 / (100 - self.ash_db.stk(f)))
-                )
-
-            idxs_dtg = [
-                np.argmax(self.temp.stk(f) > self.temp_lim_dtg[0]),
-                np.argmax(self.temp.stk(f) > self.temp_lim_dtg[1]),
-            ]
-            # temp_dtg is taken fixed
-
-            # time start from 0 and consideres a fixed heating rate
-            self.time_dtg.add(
-                f,
-                np.linspace(
-                    0,
-                    self.time.stk(f)[idxs_dtg[1]] - self.time.stk(f)[idxs_dtg[0]],
-                    self.len_dtg_db,
-                ),
-            )
-
-            self.mp_db_dtg.add(
-                f,
-                np.interp(
-                    self.temp_dtg,
-                    self.temp.stk(f)[idxs_dtg[0] : idxs_dtg[1]],
-                    self.mp_db.stk(f)[idxs_dtg[0] : idxs_dtg[1]],
-                ),
-            )
-            # the combusiton indexes use rates as /min
-            if self.dtg_basis == "temperature":
-                dtg = np.gradient(self.mp_db_dtg.stk(f), self.temp_dtg)
-            if self.dtg_basis == "time":
-                dtg = np.gradient(self.mp_db_dtg.stk(f), self.time_dtg.stk(f))
-            self.dtg_db.add(f, savgol_filter(dtg, self.dtg_window_filter, 1))
-        # average
-        self.ave_dev_tga_perc = np.average(self.mp_db_dtg.std())
-        print(f"Average TG [%] St. Dev. for replicates: {self.ave_dev_tga_perc:0.2f} %")
-        self.proximate_computed = True
-
-    def oxidation_analysis(self):
-        """
-        Conduct oxidation analysis on the sample's data.
-
-        This method calculates various oxidation parameters such as the initial oxidation temperature (Ti),
-        peak oxidation temperature (Tp), and final oxidation temperature (Tb). It also computes derivative
-        parameters like maximum and average rates of weight loss. The results are stored in the instance's
-        attributes for further analysis.
-        """
-        if not self.proximate_computed:
-            self.proximate_analysis()
-
-        for f in range(self.n_repl):
-            threshold: float = np.max(np.abs(self.dtg_db.stk(f))) * self.temp_i_temp_b_threshold
-            # Ti = T at which dtg > Ti_thresh wt%/min after moisture removal
-            self.temp_i_idx.add(f, int(np.argmax(np.abs(self.dtg_db.stk(f)) > threshold)))
-            self.temp_i.add(f, self.temp_dtg[self.temp_i_idx.stk(f)])
-            # Tp is the T of max abs(dtg)
-            self.temp_p_idx.add(f, int(np.argmax(np.abs(self.dtg_db.stk(f)))))
-            self.temp_p.add(f, self.temp_dtg[self.temp_p_idx.stk(f)])
-            # Tb reaches < 1 wt%/min at end of curve
-            try:
-                self.temp_b_idx.add(f, int(np.flatnonzero(self.dtg_db.stk(f) < -threshold)[-1]))
-            except IndexError:  # the curve nevers goes above 1%
-                self.temp_b_idx.add(f, 0)
-            self.temp_b.add(f, self.temp_dtg[self.temp_b_idx.stk(f)])
-
-            self.dwdtemp_max.add(f, np.max(np.abs(self.dtg_db.stk(f))))
-            self.dwdtemp_mean.add(f, np.average(np.abs(self.dtg_db.stk(f))))
-            # combustion index
-            self.s_combustion_index.add(
-                f,
-                (
-                    self.dwdtemp_max.stk(f)
-                    * self.dwdtemp_mean.stk(f)
-                    / self.temp_i.stk(f)
-                    / self.temp_i.stk(f)
-                    / self.temp_b.stk(f)
-                ),
-            )
-        # # average
-        self.oxidation_computed = True
-
-    def soliddist_analysis(self, steps_min: list[float] | None = None):
-        """
-        Perform solid distribution analysis on the sample's data.
-
-        This analysis calculates the weight loss at specified temperature steps, providing insight into
-        the solid decomposition process. The results are used for generating solid distribution plots.
-
-        :param steps_min: Temperature steps (in minutes) at which the weight loss is calculated. If None, default steps are used.
-        :type steps_min: list[float], optional
-        """
-        if steps_min is None:
-            steps_min = [40, 70, 100, 130, 160, 190]
-        if not self.proximate_computed:
-            self.proximate_analysis()
-
-        for f in range(self.n_repl):
-            idxs = []
-            for step in steps_min:
-                idxs.append(np.argmax(self.time.stk(f) > step))
-            idxs.append(len(self.time.stk(f)) - 1)
-            self.temp_soliddist.add(f, self.temp.stk(f)[idxs])
-            self.time_soliddist.add(f, self.time.stk(f)[idxs])
-
-            self.dmp_soliddist.add(f, -np.diff(self.mp_db.stk(f)[idxs], prepend=100))
-
-            self.loc_soliddist.add(
-                f, np.convolve(np.insert(self.mp_db.stk(f)[idxs], 0, 100), [0.5, 0.5], mode="valid")
-            )
-
-        self.soliddist_computed = True
-
-    def deconv_analysis(
-        self,
-        centers: list[float],
-        sigmas: list[float] | None = None,
-        amplitudes: list[float] | None = None,
-        center_mins: list[float] | None = None,
-        center_maxs: list[float] | None = None,
-        sigma_mins: list[float] | None = None,
-        sigma_maxs: list[float] | None = None,
-        amplitude_mins: list[float] | None = None,
-        amplitude_maxs: list[float] | None = None,
-    ):
-        """
-        Perform deconvolution analysis on the sample's DTG data.
-
-        This method fits multiple Gaussian peaks to the DTG curve to identify and analyze individual
-        decomposition steps within the sample.
-
-        :param centers: Initial guesses for the centers of the Gaussian peaks.
-        :type centers: list[float]
-        :param sigmas: Initial guesses for the standard deviations of the Gaussian peaks. If None, defaults are used.
-        :type sigmas: list[float], optional
-        :param amplitudes: Initial guesses for the amplitudes of the Gaussian peaks. If None, defaults are used.
-        :type amplitudes: list[float], optional
-        :param center_mins: Minimum allowed values for the centers of the Gaussian peaks. If None, no bounds are applied.
-        :type center_mins: list[float], optional
-        :param center_maxs: Maximum allowed values for the centers of the Gaussian peaks. If None, no bounds are applied.
-        :type center_maxs: list[float], optional
-        :param sigma_mins: Minimum allowed values for the standard deviations of the Gaussian peaks. If None, no bounds are applied.
-        :type sigma_mins: list[float], optional
-        :param sigma_maxs: Maximum allowed values for the standard deviations of the Gaussian peaks. If None, no bounds are applied.
-        :type sigma_maxs: list[float], optional
-        :param amplitude_mins: Minimum allowed values for the amplitudes of the Gaussian peaks. If None, no bounds are applied.
-        :type amplitude_mins: list[float], optional
-        :param amplitude_maxs: Maximum allowed values for the amplitudes of the Gaussian peaks. If None, no bounds are applied.
-        :type amplitude_maxs: list[float], optional
-        """
-        if not self.proximate_computed:
-            self.proximate_analysis()
-        n_peaks = len(centers)
-        # self.dcv_best_fit_stk = np.zeros((self.len_dtg_db, self.n_repl))
-        # self.dcv_r2_stk = np.zeros(self.n_repl)
-
-        # self.dcv_peaks_stk = np.zeros((self.len_dtg_db, self.n_repl, n_peaks))
-        if sigmas is None:
-            sigmas = [1] * n_peaks
-        if amplitudes is None:
-            amplitudes = [10] * n_peaks
-        if center_mins is None:
-            center_mins = [None] * n_peaks
-        if center_maxs is None:
-            center_maxs = [None] * n_peaks
-        if sigma_mins is None:
-            sigma_mins = [None] * n_peaks
-        if sigma_maxs is None:
-            sigma_maxs = [None] * n_peaks
-        if amplitude_mins is None:
-            amplitude_mins = [0] * n_peaks
-        if amplitude_maxs is None:
-            amplitude_maxs = [None] * n_peaks
-
-        for f in range(self.n_repl):
-            y = np.abs(self.dtg_db.stk(f))
-            model = LinearModel(prefix="bkg_")
-            params = model.make_params(intercept=0, slope=0, vary=False)
-
-            for p in range(n_peaks):
-                prefix = f"peak_{p}"
-                self.dcv_peaks.append(Measure(name=prefix))
-                peak_model = GaussianModel(prefix=prefix)
-                pars = peak_model.make_params()
-                pars[prefix + "center"].set(
-                    value=centers[p], min=center_mins[p], max=center_maxs[p]
-                )
-                pars[prefix + "sigma"].set(value=sigmas[p], min=sigma_mins[p], max=sigma_maxs[p])
-                pars[prefix + "amplitude"].set(
-                    value=amplitudes[p], min=amplitude_mins[p], max=amplitude_maxs[p]
-                )
-                model += peak_model
-                params.update(pars)
-
-            result = model.fit(y, params=params, x=self.temp_dtg)
-            self.dcv_best_fit.add(f, -result.best_fit)
-            self.dcv_r2.add(f, 1 - result.residual.var() / np.var(y))
-            components = result.eval_components(x=self.temp_dtg)
-
-            for p in range(n_peaks):
-                prefix = f"peak_{p}"
-                if prefix in components:
-                    self.dcv_peaks[p].add(f, -components[prefix])
-                else:
-                    self.dcv_peaks[p].add(f, 0)
-
-        self.deconv_computed = True
-
-    def report(
-        self,
-        report_type: Literal[
-            "proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"
-        ] = "proximate",
-    ) -> pd.DataFrame:
-        """
-        Generate a report based on the specified analysis type.
-
-        This method provides detailed insights into the sample's properties, such as proximate analysis,
-        oxidation characteristics, and solid distribution, based on the selected report type.
-
-        :param report_type: The type of report to generate. Options include 'proximate', 'oxidation',
-                            'oxidation_extended', 'soliddist', and 'soliddist_extended'.
-        :type report_type: Literal["proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"]
-        :return: A pandas DataFrame containing the analysis results.
-        :rtype: pd.DataFrame
-        """
-        if report_type == "proximate":
-            if not self.proximate_computed:
-                self.proximate_analysis()
-            variables = [self.moist_ar, self.vm_db, self.fc_db, self.ash_db]
-        elif report_type == "oxidation" or report_type == "oxidation_extended":
-            if not self.oxidation_computed:
-                self.oxidation_analysis()
-            variables = [self.temp_i, self.temp_p, self.temp_b, self.s_combustion_index]
-            if report_type == "oxidation_extended":
-                variables += [self.dwdtemp_max, self.dwdtemp_mean]
-
-        elif report_type == "soliddist" or report_type == "soliddist_extended":
-            if not self.soliddist_computed:
-                self.soliddist_analysis()
-            if report_type == "soliddist":
-                variables = []
-                for p in self.temp_soliddist.ave():
-                    variables.append(Measure(name=f"{p:0.0f} {self.temp_unit}"))
-                for f in range(self.n_repl):
-                    for t, dmp in enumerate(self.dmp_soliddist.stk(f)):
-                        variables[t].add(f, dmp)
-            elif report_type == "soliddist_extended":
-                variables = [self.temp_soliddist, self.time_soliddist, self.dmp_soliddist]
-        else:
-            raise ValueError(f"{report_type = } is not a valid option")
-
-        var_names = [var.name for var in variables]
-        index = [f"repl_{f}" for f in range(self.n_repl)] + ["ave", "std"]
-        rep_data = []
-
-        for f in range(self.n_repl):
-            rep_data.append([var.stk(f) for var in variables])
-        rep_data.append([var.ave() for var in variables])
-        rep_data.append([var.std() for var in variables])
-
-        report = pd.DataFrame(data=rep_data, columns=var_names, index=index)
-        report.index.name = self.name
-        self.report_types_computed.append(report_type)
-        self.reports[report_type] = report
-        if self.auto_save_reports:
-            out_path = plib.Path(self.out_path, "single_sample_reports")
-            out_path.mkdir(parents=True, exist_ok=True)
-            report.to_excel(plib.Path(out_path, f"{self.name}_{report_type}.xlsx"))
-        return report
-
-    def plot_tg_dtg(self, **kwargs: dict[str, Any]) -> MyFigure:
-        """
-        Generate a plot combining thermogravimetric (TG) and derivative thermogravimetric (DTG) data.
-
-        This method creates a figure showing the TG and DTG curves, providing a visual representation
-        of the sample's thermal decomposition behavior.
-
-        :param kwargs: Additional keyword arguments for plot customization.
-        :type kwargs: dict
-        :return: A MyFigure instance containing the generated plot.
-        :rtype: MyFigure
-        """
-        if not self.proximate_computed:
-            self.proximate_analysis()
-        out_path = plib.Path(self.out_path, "single_sample_plots")
-        out_path.mkdir(parents=True, exist_ok=True)
-
-        default_kwargs = {
-            "filename": self.name + "_tg_dtg",
-            "out_path": out_path,
-            "height": 8.53,
-            "width": 6.4,
-            "x_lab": "time [min]",
-            "y_lab": [
-                f"T [{self.temp_symbol}]",
-                f"T [{self.temp_symbol}]",
-                f"{self.tg_label} (stb)",
-                f"{self.tg_label} (db)",
-                f"{self.tg_label} (db)",
-                f"{self.dtg_label} (db)",
-            ],
-            "grid": self.plot_grid,
-            "text_font": self.plot_font,
-        }
-        # Update kwargs with the default key-value pairs if the key is not present in kwargs
-        kwargs = {**default_kwargs, **kwargs}
-
-        mf = MyFigure(
-            rows=3,
-            cols=2,
-            **kwargs,
-        )
-        # tg plot 0, 2, 4 on the left
-        for f in range(self.n_repl):
-            mf.axs[0].plot(
-                self.time.stk(f),
-                self.temp.stk(f),
-                color=clrs[f],
-                linestyle=lnstls[f],
-                label=self.filenames[f],
-            )
-            mf.axs[2].plot(
-                self.time.stk(f),
-                self.mp_ar.stk(f),
-                color=clrs[f],
-                linestyle=lnstls[f],
-                label=self.filenames[f],
-            )
-            mf.axs[4].plot(
-                self.time.stk(f),
-                self.mp_db.stk(f),
-                color=clrs[f],
-                linestyle=lnstls[f],
-                label=self.filenames[f],
-            )
-            mf.axs[0].vlines(
-                self.time.stk(f)[self.idx_moist.stk(f)],
-                self.temp.stk(f)[self.idx_moist.stk(f)] - 50,
-                self.temp.stk(f)[self.idx_moist.stk(f)] + 50,
-                linestyle=lnstls[f],
-                color=clrs[f],
-            )
-            mf.axs[2].vlines(
-                self.time.stk(f)[self.idx_moist.stk(f)],
-                self.mp_ar.stk(f)[self.idx_moist.stk(f)] - 5,
-                self.mp_ar.stk(f)[self.idx_moist.stk(f)] + 5,
-                linestyle=lnstls[f],
-                color=clrs[f],
-            )
-
-            if self.vm_db() < 99:
-                mf.axs[0].vlines(
-                    self.time.stk(f)[self.idx_vm.stk(f)],
-                    self.temp.stk(f)[self.idx_vm.stk(f)] - 50,
-                    self.temp.stk(f)[self.idx_vm.stk(f)] + 50,
-                    linestyle=lnstls[f],
-                    color=clrs[f],
-                )
-                mf.axs[4].vlines(
-                    self.time.stk(f)[self.idx_vm.stk(f)],
-                    self.mp_db.stk(f)[self.idx_vm.stk(f)] - 5,
-                    self.mp_db.stk(f)[self.idx_vm.stk(f)] + 5,
-                    linestyle=lnstls[f],
-                    color=clrs[f],
-                )
-            # tg plot 1, 3, 5 on the right
-            mf.axs[1].plot(
-                self.time_dtg.stk(f),
-                self.temp_dtg,
-                color=clrs[f],
-                linestyle=lnstls[f],
-                label=self.filenames[f],
-            )
-            mf.axs[3].plot(
-                self.time_dtg.stk(f),
-                self.mp_db_dtg.stk(f),
-                color=clrs[f],
-                linestyle=lnstls[f],
-                label=self.filenames[f],
-            )
-            mf.axs[5].plot(
-                self.time_dtg.stk(f),
-                self.dtg_db.stk(f),
-                color=clrs[f],
-                linestyle=lnstls[f],
-                label=self.filenames[f],
-            )
-            #
-            if self.oxidation_computed:
-                mf.axs[5].vlines(
-                    self.time_dtg.stk(f)[self.temp_i_idx.stk(f)],
-                    ymin=-1.5,
-                    ymax=0,
-                    linestyle=lnstls[f],
-                    color=clrs[f],
-                )
-                mf.axs[5].vlines(
-                    self.time_dtg.stk(f)[self.temp_p_idx.stk(f)],
-                    ymin=np.min(self.dtg_db.stk(f)),
-                    ymax=np.min(self.dtg_db.stk(f)) / 5,
-                    linestyle=lnstls[f],
-                    color=clrs[f],
-                )
-                mf.axs[5].vlines(
-                    self.time_dtg.stk(f)[self.temp_b_idx.stk(f)],
-                    ymin=-1.5,
-                    ymax=0,
-                    linestyle=lnstls[f],
-                    color=clrs[f],
-                )
-        mf.save_figure()
-        return mf
-
-    def plot_soliddist(self, **kwargs: dict[str, Any]) -> MyFigure:
-        """
-        Generate a plot illustrating the solid distribution analysis results.
-
-        This method plots the weight loss of the sample at specified temperature steps, showing the
-        distribution of solid components within the sample.
-
-        :param kwargs: Additional keyword arguments for plot customization.
-        :type kwargs: dict
-        :return: A MyFigure instance containing the generated plot.
-        :rtype: MyFigure
-        """
-
-        # slightly different plotting behaviour (uses averages)
-        if not self.soliddist_computed:
-            self.soliddist_analysis()
-        out_path = plib.Path(self.out_path, "single_sample_plots")
-        out_path.mkdir(parents=True, exist_ok=True)
-
-        default_kwargs = {
-            "filename": self.name + "_soliddist",
-            "out_path": out_path,
-            "height": 3.2,
-            "width": 3.2,
-            "x_lab": "time [min]",
-            "y_lab": f"{self.tg_label} (db)",
-            "yt_lab": f"T [{self.temp_symbol}]",
-            "legend_loc": "center left",
-            "grid": self.plot_grid,
-            "text_font": self.plot_font,
-        }
-        # Update kwargs with the default key-value pairs if the key is not present in kwargs
-        kwargs = {**default_kwargs, **kwargs}
-
-        mf = MyFigure(
-            rows=1,
-            cols=1,
-            twinx=True,
-            **kwargs,
-        )
-        for f in range(self.n_repl):
-
-            mf.axs[0].plot(
-                self.time.stk(f),
-                self.mp_db.stk(f),
-                color=clrs[f],
-                linestyle=lnstls[f],
-                label=self.filenames[f],
-            )
-            mf.axts[0].plot(self.time.stk(f), self.temp.stk(f))
-
-        for tm, mp, dmp in zip(self.time_soliddist(), self.loc_soliddist(), self.dmp_soliddist()):
-            mf.axs[0].annotate(
-                f"{dmp:0.0f}%", ha="center", va="top", xy=(tm - 10, mp + 1), fontsize=9
-            )
-        mf.save_figure()
-        return mf
-
-    def plot_deconv(self, **kwargs: dict[str, Any]) -> MyFigure:
-        """
-        Generate a plot showing the deconvolution analysis results.
-
-        This method visualizes the Gaussian peak fitting performed on the DTG data, illustrating the
-        identified decomposition steps within the sample.
-
-        :param kwargs: Additional keyword arguments for plot customization.
-        :type kwargs: dict
-        :return: A MyFigure instance containing the deconvolution analysis plot.
-        :rtype: MyFigure
-        """
-
-        if not self.deconv_computed:
-            raise ValueError("Deconvolution analysis not computed")
-        out_path = plib.Path(self.out_path, "single_sample_plots")
-        out_path.mkdir(parents=True, exist_ok=True)
-
-        default_kwargs = {
-            "filename": self.name + "_deconv",
-            "out_path": out_path,
-            "height": 8.53,
-            "width": 3.2,
-            "x_lab": f"T [{self.temp_symbol}]",
-            "y_lab": f"{self.dtg_label} (db)",
-            "grid": self.plot_grid,
-            "text_font": self.plot_font,
-        }
-        # Update kwargs with the default key-value pairs if the key is not present in kwargs
-        kwargs = {**default_kwargs, **kwargs}
-        mf = MyFigure(
-            rows=self.n_repl,
-            cols=1,
-            **kwargs,
-        )
-
-        # Plot DTG data
-        for f in range(self.n_repl):
-            mf.axs[f].plot(self.temp_dtg, self.dtg_db.stk(f), color="black", label="DTG")
-            # Plot best fit and individual peaks
-            mf.axs[f].plot(
-                self.temp_dtg,
-                self.dcv_best_fit.stk(f),
-                label="best fit",
-                color="red",
-                linestyle="--",
-            )
-            clrs_p = clrs[:3] + clrs[5:]  # avoid using red
-            for p, peak in enumerate(self.dcv_peaks):
-                if peak.stk(f) is not None:
-                    mf.axs[f].plot(
-                        self.temp_dtg,
-                        peak.stk(f),
-                        label=peak.name,
-                        color=clrs_p[p],
-                        linestyle=lnstls[p],
-                    )
-            mf.axs[f].annotate(
-                f"r$^2$={self.dcv_r2.stk(f):.2f}",
-                xycoords="axes fraction",
-                xy=(0.85, 0.96),
-                size="x-small",
-            )
-        mf.save_figure()
-        return mf
+from __future__ import annotations
+from typing import Literal, Any
+import pathlib as plib
+import numpy as np
+import pandas as pd
+from scipy.signal import savgol_filter
+from lmfit.models import GaussianModel, LinearModel
+from tga_data_analysis.measure import Measure
+from tga_data_analysis.myfigure import MyFigure, colors, linestyles
+
+
+class Project:
+    """
+    Represents a project (identified by the folder where the data is stored)
+    for TGA data analysis.
+
+    """
+
+    def __init__(
+        self,
+        folder_path: plib.Path,
+        name: str | None = None,
+        temp_unit: Literal["C", "K"] = "C",
+        plot_font: Literal["Dejavu Sans", "Times New Roman"] = "Dejavu Sans",
+        dtg_basis: Literal["temperature", "time"] = "temperature",
+        temp_i_temp_b_threshold: float = 0.01,  # % of the peak that is used for Ti and Tb
+        resolution_sec_deg_dtg: int = 5,
+        dtg_window_filter: int = 101,
+        plot_grid: bool = False,
+        column_name_mapping: dict[str, str] | None = None,
+        load_skiprows: int = 0,
+        time_moist: float = 38.0,
+        time_vm: float = 147.0,
+        temp_initial_celsius: float = 40,
+        temp_lim_dtg_celsius: tuple[float] | None = None,
+        auto_save_reports: bool = True,
+    ):
+        """
+        Initialize a new Project instance with various parameters for analysis.
+
+        :param folder_path: The path to the folder containing the project data.
+        :type folder_path: plib.Path
+        :param name: The name of the project. Defaults to the last part of the folder path if None.
+        :type name: str, optional
+        :param temp_unit: The unit of temperature used in the project ('C':Celsius, 'K':Kelvin).
+        :type temp_unit: Literal["C", "K"]
+        :param plot_font: The font used in plots, either 'Dejavu Sans' or 'Times New Roman'.
+        :type plot_font: Literal["Dejavu Sans", "Times New Roman"]
+        :param dtg_basis: The basis for DTG calculations, either 'temperature' or 'time'.
+        :type dtg_basis: Literal["temperature", "time"]
+        :param temp_i_temp_b_threshold: The threshold for Ti and Tb calculation in DTG analysis.
+        :type temp_i_temp_b_threshold: float
+        :param resolution_sec_deg_dtg: The resolution in seconds or degrees for DTG analysis.
+        :type resolution_sec_deg_dtg: int
+        :param dtg_window_filter: The window size for the Savitzky-Golay filter in DTG analysis.
+        :type dtg_window_filter: int
+        :param plot_grid: Whether to display a grid in the plots.
+        :type plot_grid: bool
+        :param column_name_mapping: Mapping of column names from file to standard names used in the analysis.
+        :type column_name_mapping: dict[str, str], optional
+        :param load_skiprows: The number of rows to skip when loading data files.
+        :type load_skiprows: int
+        :param time_moist: The time considered for the moisture analysis.
+        :type time_moist: float
+        :param time_vm: The time considered for the volatile matter analysis.
+        :type time_vm: float
+        :param temp_initial_celsius: The initial temperature for certain calculations, in Celsius.
+        :type temp_initial_celsius: float
+        :param temp_lim_dtg_celsius: The temperature limits for DTG analysis, in Celsius.
+        :type temp_lim_dtg_celsius: tuple[float], optional
+        :param auto_save_reports: Whether to automatically save generated reports.
+        :type auto_save_reports: bool
+        """
+        self.folder_path = folder_path
+        self.out_path = plib.Path(folder_path, "output")
+        if name is None:
+            self.name = self.folder_path.parts[-1]
+        else:
+            self.name = name
+        self.temp_unit = temp_unit
+        self.plot_font = plot_font
+        self.plot_grid = plot_grid
+        self.dtg_basis = dtg_basis
+        self.temp_i_temp_b_threshold = temp_i_temp_b_threshold
+        self.resolution_sec_deg_dtg = resolution_sec_deg_dtg
+        self.dtg_window_filter = dtg_window_filter
+        self.load_skiprows = load_skiprows
+        self.time_moist = time_moist
+        self.time_vm = time_vm
+        self.temp_initial_celsius = temp_initial_celsius
+        self.auto_save_reports = auto_save_reports
+
+        if self.temp_unit == "C":
+            self.temp_symbol = "°C"
+        elif self.temp_unit == "K":
+            self.temp_symbol = "K"
+
+        self.tg_label = "TG [wt%]"
+        if self.dtg_basis == "temperature":
+            self.dtg_label = "DTG [wt%/" + self.temp_symbol + "]"
+        elif self.dtg_basis == "time":
+            self.dtg_label = "DTG [wt%/min]"
+
+        if temp_lim_dtg_celsius is None:
+            self.temp_lim_dtg_celsius = (120, 880)
+        else:
+            self.temp_lim_dtg_celsius = temp_lim_dtg_celsius
+        if self.temp_unit == "C":
+            self.temp_lim_dtg = self.temp_lim_dtg_celsius
+        elif self.temp_unit == "K":
+            self.temp_lim_dtg = [t + 273.15 for t in self.temp_lim_dtg_celsius]
+        else:
+            raise ValueError(f"{self.temp_unit = } is not acceptable")
+
+        self.len_dtg_db: int = int(
+            (self.temp_lim_dtg[1] - self.temp_lim_dtg[0]) * self.resolution_sec_deg_dtg
+        )
+        self.temp_dtg: np.ndarray = np.linspace(
+            self.temp_lim_dtg[0], self.temp_lim_dtg[1], self.len_dtg_db
+        )
+
+        if column_name_mapping is None:
+            self.column_name_mapping = {
+                "Time": "t_min",
+                "Temperature": "T_C",
+                "Weight": "m_p",
+                "Weight.1": "m_mg",
+                "Heat Flow": "heatflow_mW",
+                "##Temp./>C": "T_C",
+                "Time/min": "t_min",
+                "Mass/%": "m_p",
+                "Segment": "segment",
+            }
+        else:
+            self.column_name_mapping = column_name_mapping
+        #
+        self.samples: dict[str, Sample] = {}
+        self.samplenames: list[str] = []
+
+        self.multireports: dict[str, pd.DataFrame] = {}
+        self.multireport_types_computed: list[str] = []
+
+    def add_sample(self, samplename: str, sample: Sample):
+        """
+        Add a sample to the project.
+
+        :param samplename: The name of the sample to add.
+        :type samplename: str
+        :param sample: The sample object to add.
+        :type sample: Sample
+        """
+        if samplename not in self.samplenames:
+            self.samplenames.append(samplename)
+            self.samples[samplename] = sample
+        else:
+            print(f"{samplename = } already present in project. Sample not added.")
+
+    def multireport(
+        self,
+        samples: list[Sample] | None = None,
+        labels: list[str] | None = None,
+        report_type: Literal[
+            "proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"
+        ] = "proximate",
+        report_style: Literal["repl_ave_std", "ave_std", "ave_pm_std"] = "ave_std",
+        decimals_in_ave_pm_std: int = 2,
+        filename: str | None = None,
+    ) -> pd.DataFrame:
+        """
+        Generate a multi-sample report based on the specified report type and style.
+
+        :param samples: A list of Sample objects to include in the report. If None, uses all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: A list of labels corresponding to each sample. If None, sample names are used as labels.
+        :type labels: list[str], optional
+        :param report_type: The type of report to generate, choices include 'proximate', 'oxidation', 'oxidation_extended', 'soliddist', and 'soliddist_extended'.
+        :type report_type: Literal["proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"]
+        :param report_style: The style of the report, choices are 'repl_ave_std', 'ave_std', and 'ave_pm_std'.
+        :type report_style: Literal["repl_ave_std", "ave_std", "ave_pm_std"]
+        :param decimals_in_ave_pm_std: The number of decimal places to use for the average plus-minus standard deviation format.
+        :type decimals_in_ave_pm_std: int
+        :param filename: The name of the file to save the report. If None, the report is not saved.
+        :type filename: str, optional
+        :return: A pandas DataFrame containing the generated report.
+        :rtype: pd.DataFrame
+        """
+        if samples is None:
+            samples = list(self.samples.values())
+
+        samplenames = [sample.name for sample in samples]
+
+        if labels is None:
+            labels = samplenames
+        for sample in samples:
+            if report_type not in sample.report_types_computed:
+                sample.report(report_type)
+
+        if report_type == "soliddist":
+            reports = [sample.reports[report_type] for sample in samples]
+            reports = self._reformat_ave_std_columns(reports)
+        elif report_type == "soliddist_extended":
+            raise ValueError(
+                f"{report_type = } not allowed for multireport, use 'soliddist' instead"
+            )
+        else:
+            reports = [sample.reports[report_type] for sample in samples]
+
+        if report_style == "repl_ave_std":
+            # Concatenate all individual reports
+            report = pd.concat(reports, keys=labels)
+            report.index.names = [None, None]  # Remove index names
+
+        elif report_style == "ave_std":
+            # Keep only the average and standard deviation
+            ave_std_dfs = []
+            for label, report in zip(labels, reports):
+                ave_std_dfs.append(report.loc[["ave", "std"]])
+            report = pd.concat(ave_std_dfs, keys=labels)
+            report.index.names = [None, None]  # Remove index names
+
+        elif report_style == "ave_pm_std":
+            # Format as "ave ± std" and use sample name as the index
+            rows = []
+            for label, report in zip(labels, reports):
+                row = {
+                    col: f"{report.at['ave', col]:.{decimals_in_ave_pm_std}f} ± {report.at['std', col]:.{decimals_in_ave_pm_std}f}"
+                    for col in report.columns
+                }
+                rows.append(pd.Series(row, name=label))
+            report = pd.DataFrame(rows)
+
+        else:
+            raise ValueError(f"{report_style = } is not a valid option")
+        self.multireport_types_computed.append(report_type)
+        self.multireports[report_type] = report
+        if self.auto_save_reports:
+            out_path = plib.Path(self.out_path, "multireports")
+            out_path.mkdir(parents=True, exist_ok=True)
+            if filename is None:
+                filename = f"{self.name}_{report_type}_{report_style}.xlsx"
+            else:
+                filename = filename + ".xlsx"
+            report.to_excel(plib.Path(out_path, filename))
+        return report
+
+    def plot_multireport(
+        self,
+        filename: str = "plot",
+        samples: list[Sample] | None = None,
+        labels: list[str] | None = None,
+        report_type: Literal["proximate", "oxidation", "soliddist"] = "proximate",
+        bar_labels: list[str] | None = None,
+        **kwargs,
+    ) -> MyFigure:
+        """
+        Generate a plot for the multi-sample report.
+
+        :param filename: The name of the file to save the plot. Defaults to "plot".
+        :type filename: str
+        :param samples: A list of Sample objects to include in the plot. If None, uses all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: A list of labels corresponding to each sample. If None, sample names are used as labels.
+        :type labels: list[str], optional
+        :param report_type: The type of report to plot, choices include 'proximate', 'oxidation', and 'soliddist'.
+        :type report_type: Literal["proximate", "oxidation", "soliddist"]
+        :param bar_labels: Labels for the bars in the plot. If None, default labels based on the report type are used.
+        :type bar_labels: list[str], optional
+        :param kwargs: Additional keyword arguments to pass to the plotting function.
+        :type kwargs: dict
+        :return: An instance of MyFigure containing the generated plot.
+        :rtype: MyFigure
+        """
+        if samples is None:
+            samples = list(self.samples.values())
+
+        samplenames = [sample.name for sample in samples]
+        if labels is None:
+            labels = samplenames
+
+        df = self.multireport(samples, labels, report_type, report_style="ave_std")
+        df_ave = df.xs("ave", level=1, drop_level=False)
+        df_std = df.xs("std", level=1, drop_level=False)
+        # drop the multi-level index to simplify the DataFrame
+        df_ave = df_ave.droplevel(1)
+        df_std = df_std.droplevel(1)
+
+        if report_type == "proximate":
+            if bar_labels is None:
+                vars_bar = ["moisture (stb)", "VM (db)", "FC (db)", "ash (db)"]
+            else:
+                vars_bar = bar_labels
+            df_ave.columns = vars_bar
+            df_std.columns = vars_bar
+            bar_yaxis = vars_bar
+            bar_ytaxis = None
+            twinx = None
+            y_lab = self.tg_label
+            yt_lab = None
+
+        elif report_type == "oxidation":
+            if bar_labels is None:
+                vars_bar = ["T$_i$", "T$_p$", "T$_b$", "S"]
+            else:
+                vars_bar = bar_labels
+            df_ave.columns = vars_bar
+            df_std.columns = vars_bar
+            bar_yaxis = vars_bar[:3]
+            bar_ytaxis = vars_bar[-1]
+            twinx = True
+            y_lab = f"T [{self.temp_symbol}]"
+            yt_lab = "S (comb. index)"
+
+        elif report_type == "soliddist":
+            if bar_labels is None:
+                vars_bar = [f"{col.split(' ')[0]} {col.split(' ')[-1]}" for col in df_ave.columns]
+            else:
+                vars_bar = bar_labels
+            df_ave.columns = vars_bar
+            df_std.columns = vars_bar
+            bar_yaxis = vars_bar
+            bar_ytaxis = None
+            twinx = None
+            y_lab = "step mass loss [wt%]"
+            yt_lab = None
+
+        out_path = plib.Path(self.out_path, "multireport_plots")
+        out_path.mkdir(parents=True, exist_ok=True)
+        default_kwargs = {
+            "filename": filename + report_type,
+            "out_path": out_path,
+            "height": 3.2,
+            "width": 3.2,
+            "grid": self.plot_grid,
+            "text_font": self.plot_font,
+        }
+        # Update kwargs with the default key-value pairs if the key is not present in kwargs
+        kwargs = {**default_kwargs, **kwargs}
+        myfig = MyFigure(
+            rows=1,
+            cols=1,
+            twinx=twinx,
+            y_lab=y_lab,
+            yt_lab=yt_lab,
+            **kwargs,
+        )
+        df_ave[bar_yaxis].plot(
+            ax=myfig.axs[0],
+            kind="bar",
+            yerr=df_std[bar_yaxis],
+            capsize=2,
+            width=0.85,
+            ecolor="k",
+            edgecolor="black",
+        )
+        if bar_ytaxis is not None:
+            myfig.axts[0].scatter(
+                df_ave.index,
+                df_ave[bar_ytaxis],
+                label=bar_ytaxis,
+                edgecolor="black",
+                color=colors[3],
+                # s=100
+            )
+            myfig.axts[0].errorbar(
+                df_ave.index,
+                df_ave[bar_ytaxis],
+                yerr=df_std[bar_ytaxis],
+                ecolor="k",
+                linestyle="None",
+                capsize=2,
+            )
+        myfig.save_figure()
+        return myfig
+
+    def plot_multi_tg(
+        self,
+        filename: str = "plot",
+        samples: list[Sample] | None = None,
+        labels: list[str] | None = None,
+        **kwargs,
+    ) -> MyFigure:
+        """
+        Plot multiple thermogravimetric (TG) curves for the given samples.
+
+        :param filename: The name of the file to save the plot. Defaults to "plot".
+        :type filename: str
+        :param samples: A list of Sample objects to be plotted. If None, plots all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: Labels for each sample in the plot. If None, sample names are used.
+        :type labels: list[str], optional
+        :param kwargs: Additional keyword arguments for plotting customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the plot.
+        :rtype: MyFigure
+        """
+        if samples is None:
+            samples = list(self.samples.values())
+
+        samplenames = [sample.name for sample in samples]
+        if labels is None:
+            labels = samplenames
+        for sample in samples:
+            if not sample.proximate_computed:
+                sample.proximate_analysis()
+
+        out_path = plib.Path(self.out_path, "multisample_plots")
+        out_path.mkdir(parents=True, exist_ok=True)
+
+        default_kwargs = {
+            "filename": filename + "_tg",
+            "out_path": out_path,
+            "height": 3.2,
+            "width": 3.2,
+            "grid": self.plot_grid,
+            "text_font": self.plot_font,
+            "x_lab": f"T [{self.temp_symbol}]",
+            "y_lab": self.tg_label,
+            "x_lim": self.temp_lim_dtg,
+        }
+        # Update kwargs with the default key-value pairs if the key is not present in kwargs
+        kwargs = {**default_kwargs, **kwargs}
+
+        myfig = MyFigure(
+            rows=1,
+            cols=1,
+            **kwargs,
+        )
+        for i, sample in enumerate(samples):
+            myfig.axs[0].plot(
+                sample.temp.ave(),
+                sample.mp_db.ave(),
+                color=colors[i],
+                linestyle=linestyles[i],
+                label=labels[i],
+            )
+            myfig.axs[0].fill_between(
+                sample.temp.ave(),
+                sample.mp_db.ave() - sample.mp_db.std(),
+                sample.mp_db.ave() + sample.mp_db.std(),
+                color=colors[i],
+                alpha=0.3,
+            )
+        myfig.save_figure()
+        return myfig
+
+    def plot_multi_dtg(
+        self,
+        filename: str = "plot",
+        samples: list[Sample] | None = None,
+        labels: list[str] | None = None,
+        **kwargs,
+    ) -> MyFigure:
+        """
+        Plot multiple derivative thermogravimetric (DTG) curves for the given samples.
+
+        :param filename: The name of the file to save the plot. Defaults to "plot".
+        :type filename: str
+        :param samples: A list of Sample objects to be plotted. If None, plots all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: Labels for each sample in the plot. If None, sample names are used.
+        :type labels: list[str], optional
+        :param kwargs: Additional keyword arguments for plotting customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the plot.
+        :rtype: MyFigure
+        """
+        if samples is None:
+            samples = list(self.samples.values())
+
+        samplenames = [sample.name for sample in samples]
+        if labels is None:
+            labels = samplenames
+        for sample in samples:
+            if not sample.proximate_computed:
+                sample.proximate_analysis()
+
+        out_path = plib.Path(self.out_path, "multisample_plots")
+        out_path.mkdir(parents=True, exist_ok=True)
+        default_kwargs = {
+            "filename": filename + "_dtg",
+            "out_path": out_path,
+            "height": 3.2,
+            "width": 3.2,
+            "grid": self.plot_grid,
+            "text_font": self.plot_font,
+            "x_lab": f"T [{self.temp_symbol}]",
+            "y_lab": self.dtg_label,
+            "x_lim": self.temp_lim_dtg,
+        }
+        # Update kwargs with the default key-value pairs if the key is not present in kwargs
+        kwargs = {**default_kwargs, **kwargs}
+
+        myfig = MyFigure(
+            rows=1,
+            cols=1,
+            **kwargs,
+        )
+        for i, sample in enumerate(samples):
+            myfig.axs[0].plot(
+                sample.temp_dtg,
+                sample.dtg_db.ave(),
+                color=colors[i],
+                linestyle=linestyles[i],
+                label=labels[i],
+            )
+            myfig.axs[0].fill_between(
+                sample.temp_dtg,
+                sample.dtg_db.ave() - sample.dtg_db.std(),
+                sample.dtg_db.ave() + sample.dtg_db.std(),
+                color=colors[i],
+                alpha=0.3,
+            )
+        myfig.save_figure()
+        return myfig
+
+    def plot_multi_soliddist(
+        self,
+        filename: str = "plot",
+        samples: list[Sample] | None = None,
+        labels: list[str] | None = None,
+        **kwargs,
+    ) -> MyFigure:
+        """
+        Plot multiple solid distribution curves for the given samples.
+
+        :param filename: The name of the file to save the plot. Defaults to "plot".
+        :type filename: str
+        :param samples: A list of Sample objects to be plotted. If None, plots all samples in the project.
+        :type samples: list[Sample], optional
+        :param labels: Labels for each sample in the plot. If None, sample names are used.
+        :type labels: list[str], optional
+        :param kwargs: Additional keyword arguments for plotting customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the plot.
+        :rtype: MyFigure
+        """
+        if samples is None:
+            samples = list(self.samples.values())
+
+        samplenames = [sample.name for sample in samples]
+        if labels is None:
+            labels = samplenames
+        for sample in samples:
+            if not sample.proximate_computed:
+                sample.proximate_analysis()
+
+        out_path = plib.Path(self.out_path, "multisample_plots")
+        out_path.mkdir(parents=True, exist_ok=True)
+        default_kwargs = {
+            "filename": filename + "_soliddist",
+            "out_path": out_path,
+            "height": 3.2,
+            "width": 3.2,
+            "grid": self.plot_grid,
+            "text_font": self.plot_font,
+            "x_lab": "time [min]",
+            "y_lab": self.tg_label,
+            "yt_lab": f"T [{self.temp_symbol}]",
+            "legend_loc": "center left",
+        }
+        # Update kwargs with the default key-value pairs if the key is not present in kwargs
+        kwargs = {**default_kwargs, **kwargs}
+
+        myfig = MyFigure(
+            rows=1,
+            twinx=True,
+            **kwargs,
+        )
+        myfig.axts[0].plot(
+            samples[0].time.ave(),
+            samples[0].temp.ave(),
+            color="k",
+            linestyle=linestyles[1],
+            label="T",
+        )
+        for i, sample in enumerate(samples):
+
+            myfig.axs[0].plot(
+                sample.time.ave(),
+                sample.mp_db.ave(),
+                color=colors[i],
+                linestyle=linestyles[i],
+                label=labels[i],
+            )
+            myfig.axs[0].fill_between(
+                sample.time.ave(),
+                sample.mp_db.ave() - sample.mp_db.std(),
+                sample.mp_db.ave() + sample.mp_db.std(),
+                color=colors[i],
+                alpha=0.3,
+            )
+        myfig.save_figure()
+        return myfig
+
+    def _reformat_ave_std_columns(self, reports):
+        """
+        Reformat the columns of the given reports to have standard deviation and average values.
+
+        This method is intended to be used internally within the Project class to standardize
+        the report dataframes before generating multi-sample reports.
+
+        :param reports: A list of report DataFrames to reformat.
+        :type reports: list[pd.DataFrame]
+        :return: A list of reformatted DataFrames.
+        :rtype: list[pd.DataFrame]
+        """
+        # Check that all reports have the same number of columns
+        num_columns = len(reports[0].columns)
+        if not all(len(report.columns) == num_columns for report in reports):
+            raise ValueError("All reports must have the same number of columns.")
+
+        # Initialize a list to hold the new formatted column names
+        formatted_column_names = []
+
+        # Iterate over each column index
+        for i in range(num_columns):
+            # Extract the numeric part of the column name (assume it ends with ' K' or ' C')
+            column_values = [float(report.columns[i].split()[0]) for report in reports]
+            ave = np.mean(column_values)
+            std = np.std(column_values)
+
+            # Determine the unit (assuming all columns have the same unit)
+            unit = reports[0].columns[i].split()[-1]
+
+            # Create the new column name with the unit
+            formatted_column_name = f"{ave:.0f} ± {std:.0f} {unit}"
+            formatted_column_names.append(formatted_column_name)
+
+        # Rename the columns in each report using the new formatted names
+        for report in reports:
+            report.columns = formatted_column_names
+
+        return reports
+
+
+class Sample:
+    """
+    A class representing a sample in the project, containing methods for loading, processing,
+    and analyzing thermogravimetric analysis (TGA) data associated with the sample.
+    """
+
+    def __init__(
+        self,
+        project: Project,
+        name: str,
+        filenames: list[str],
+        folder_path: plib.Path | None = None,
+        label: str | None = None,
+        correct_ash_mg: list[float] | None = None,
+        correct_ash_fr: list[float] | None = None,
+        column_name_mapping: dict[str:str] | None = None,
+        load_skiprows: int | None = None,
+        time_moist: float | None = None,
+        time_vm: float | None = None,
+        heating_rate_deg_min: float | None = None,
+        temp_i_temp_b_threshold: float | None = None,
+    ):
+        """
+        Initialize a new Sample instance with parameters for TGA data analysis.
+
+        :param project: The Project object to which this sample belongs.
+        :type project: Project
+        :param name: The name of the sample.
+        :type name: str
+        :param filenames: A list of filenames associated with the sample.
+        :type filenames: list[str]
+        :param folder_path: The path to the folder containing the sample data. If None, the project's folder path is used.
+        :type folder_path: plib.Path, optional
+        :param label: A label for the sample. If None, the sample's name is used as the label.
+        :type label: str, optional
+        :param correct_ash_mg: A list of ash correction values in milligrams, one per file.
+        :type correct_ash_mg: list[float], optional
+        :param correct_ash_fr: A list of ash correction values as a fraction, one per file.
+        :type correct_ash_fr: list[float], optional
+        :param column_name_mapping: A dictionary mapping file column names to standardized column names for analysis.
+        :type column_name_mapping: dict[str, str], optional
+        :param load_skiprows: The number of rows to skip at the beginning of the files when loading.
+        :type load_skiprows: int
+        :param time_moist: The time considered for the moisture analysis.
+        :type time_moist: float
+        :param time_vm: The time considered for the volatile matter analysis.
+        :type time_vm: float
+        :param heating_rate_deg_min: The heating rate in degrees per minute, used for certain calculations.
+        :type heating_rate_deg_min: float, optional
+        :param temp_i_temp_b_threshold: The threshold percentage used for calculating initial and final temperatures in DTG analysis.
+        :type temp_i_temp_b_threshold: float, optional
+        """
+        # store the sample in the project
+        self.project_name = project.name
+        project.add_sample(name, self)
+        # prject defaults unless specified
+
+        self.out_path = project.out_path
+        self.temp_unit = project.temp_unit
+        self.temp_symbol = project.temp_symbol
+        self.tg_label = project.tg_label
+        self.dtg_label = project.dtg_label
+        self.plot_font = project.plot_font
+        self.plot_grid = project.plot_grid
+        self.dtg_basis = project.dtg_basis
+        self.temp_lim_dtg = project.temp_lim_dtg
+        self.len_dtg_db = project.len_dtg_db
+        self.temp_dtg = project.temp_dtg
+        self.auto_save_reports = project.auto_save_reports
+
+        self.resolution_sec_deg_dtg = project.resolution_sec_deg_dtg
+        self.dtg_window_filter = project.dtg_window_filter
+        self.temp_initial_celsius = project.temp_initial_celsius
+        self.dtg_window_filter = project.dtg_window_filter
+        if folder_path is None:
+            self.folder_path = project.folder_path
+        else:
+            self.folder_path = folder_path
+        if column_name_mapping is None:
+            self.column_name_mapping = project.column_name_mapping
+        else:
+            self.column_name_mapping = column_name_mapping
+        if load_skiprows is None:
+            self.load_skiprows = project.load_skiprows
+        else:
+            self.load_skiprows = load_skiprows
+        if time_moist is None:
+            self.time_moist = project.time_moist
+        else:
+            self.time_moist = time_moist
+        if time_vm is None:
+            self.time_vm = project.time_vm
+        else:
+            self.time_vm = time_vm
+        if temp_i_temp_b_threshold is None:
+            self.temp_i_temp_b_threshold = project.temp_i_temp_b_threshold
+        else:
+            self.temp_i_temp_b_threshold = temp_i_temp_b_threshold
+        # sample default
+        self.name = name
+        self.filenames = filenames
+        self.n_repl = len(self.filenames)
+        self.heating_rate_deg_min = heating_rate_deg_min
+        self.correct_ash_mg = self._broadcast_value_prop(correct_ash_mg)
+        self.correct_ash_fr = self._broadcast_value_prop(correct_ash_fr)
+        if not label:
+            self.label = name
+        else:
+            self.label = label
+
+        # for variables and computations
+        self.files: dict[str : pd.DataFrame] = {}
+        self.len_files: dict[str : pd.DataFrame] = {}
+        self.len_sample: int = 0
+
+        # proximate
+        self.temp: Measure = Measure(name="temp_" + self.temp_unit)
+        self.time: Measure = Measure(name="time")
+        self.m_ar: Measure = Measure(name="m_ar")
+        self.mp_ar: Measure = Measure(name="mp_ar")
+        self.idx_moist: Measure = Measure(name="idx_moist")
+        self.idx_vm: Measure = Measure(name="idx_vm")
+        self.moist_ar: Measure = Measure(name="moist_ar")
+        self.ash_ar: Measure = Measure(name="ash_ar")
+        self.fc_ar: Measure = Measure(name="fc_ar")
+        self.vm_ar: Measure = Measure(name="vm_ar")
+        self.mp_db: Measure = Measure(name="mp_db")
+        self.ash_db: Measure = Measure(name="ash_db")
+        self.fc_db: Measure = Measure(name="fc_db")
+        self.vm_db: Measure = Measure(name="vm_db")
+        self.mp_daf: Measure = Measure(name="mp_daf")
+        self.fc_daf: Measure = Measure(name="fc_daf")
+        self.vm_daf: Measure = Measure(name="vm_daf")
+        self.time_dtg: Measure = Measure(name="time_dtg")
+        self.mp_db_dtg: Measure = Measure(name="mp_db_dtg")
+        self.dtg_db: Measure = Measure(name="dtg_db")
+        self.ave_dev_tga_perc: float | None = None
+        # oxidation
+        self.temp_i_idx: Measure = Measure(name="temp_i_idx")
+        self.temp_i: Measure = Measure(name="temp_i_" + self.temp_unit)
+        self.temp_p_idx: Measure = Measure(name="temp_p_idx")
+        self.temp_p: Measure = Measure(name="temp_p_" + self.temp_unit)
+        self.temp_b_idx: Measure = Measure(name="temp_b_idx")
+        self.temp_b: Measure = Measure(name="temp_b_" + self.temp_unit)
+        self.dwdtemp_max: Measure = Measure(name="dwdtemp_max")
+        self.dwdtemp_mean: Measure = Measure(name="dwdtemp_mean")
+        self.s_combustion_index: Measure = Measure(name="s_combustion_index")
+        # soliddist
+        self.temp_soliddist: Measure = Measure(name="temp_dist_" + self.temp_unit)
+        self.time_soliddist: Measure = Measure(name="time_dist")
+        self.dmp_soliddist: Measure = Measure(name="dmp_dist")
+        self.loc_soliddist: Measure = Measure(name="loc_dist")
+        # deconvolution
+        self.dcv_best_fit: Measure = Measure(name="dcv_best_fit")
+        self.dcv_r2: Measure = Measure(name="dcv_r2")
+        self.dcv_peaks: list[Measure] = []
+        # Flag to track if data is loaded
+        self.proximate_computed = False
+        self.files_loaded = False
+        self.oxidation_computed = False
+        self.soliddist_computed = False
+        self.deconv_computed = False
+        # for reports
+        self.reports: dict[str, pd.DataFrame] = {}
+        self.report_types_computed: list[str] = []
+
+        self.load_files()
+        self.proximate_analysis()
+
+    def _broadcast_value_prop(self, prop: list | str | float | int | bool) -> list:
+        """
+        Broadcast a single value or a list of values to match the number of replicates.
+
+        This method is used internally to ensure that properties like corrections have a value
+        for each replicate, even if a single value is provided for all.
+
+        :param prop: A single value or a list of values to be broadcasted.
+        :type prop: list | float | int | bool
+        :return: A list of values with length equal to the number of replicates.
+        :rtype: list
+        """
+        if prop is None:
+            broad_prop = [None] * self.n_repl
+        if isinstance(prop, (list, tuple)):
+            # If it's a list or tuple, but we're not expecting pairs, it's a single value per axis.
+            if len(prop) == self.n_repl:
+                broad_prop = prop
+            else:
+                raise ValueError(
+                    f"The size of the property '{prop}' does not match the number of replicates."
+                )
+        if isinstance(prop, (str, float, int, bool)):
+            broad_prop = [prop] * self.n_repl
+        return broad_prop
+
+    def load_single_file(
+        self,
+        filename: str,
+        folder_path: plib.Path | None = None,
+        load_skiprows: int | None = None,
+        column_name_mapping: dict | None = None,
+    ) -> pd.DataFrame:
+        """
+        Load data from a single file associated with the sample.
+
+        :param filename: The name of the file to be loaded.
+        :type filename: str
+        :param folder_path: The folder path where the file is located. If None, uses the sample's folder path.
+        :type folder_path: plib.Path, optional
+        :param load_skiprows: The number of rows to skip at the beginning of the file. If None, uses the sample's default.
+        :type load_skiprows: int, optional
+        :param column_name_mapping: A mapping of file column names to standardized column names. If None, uses the sample's default.
+        :type column_name_mapping: dict, optional
+        :return: The loaded data as a pandas DataFrame.
+        :rtype: pd.DataFrame
+        """
+        if column_name_mapping is None:
+            column_name_mapping = self.column_name_mapping
+        if folder_path is None:
+            folder_path = self.folder_path
+        if load_skiprows is None:
+            load_skiprows = self.load_skiprows
+        file_path = plib.Path(folder_path, filename + ".txt")
+        if not file_path.is_file():
+            file_path = plib.Path(folder_path, filename + ".csv")
+        file = pd.read_csv(file_path, sep="\t", skiprows=load_skiprows)
+        if file.shape[1] < 3:
+            file = pd.read_csv(file_path, sep=",", skiprows=load_skiprows)
+        file = file.rename(columns={col: column_name_mapping.get(col, col) for col in file.columns})
+        for column in file.columns:
+            file[column] = pd.to_numeric(file[column], errors="coerce")
+        file.dropna(inplace=True)
+        return file
+
+    def correct_file_values(
+        self,
+        file: pd.DataFrame,
+        correct_ash_fr: float | None,
+        correct_ash_mg: float | None,
+    ):
+        """
+        Apply corrections to the loaded file data.
+
+        This method adjusts the mass measurements in the file based on provided ash correction values.
+
+        :param file: The data file to be corrected.
+        :type file: pd.DataFrame
+        :param correct_ash_mg: The correction value for ash in milligrams. If None, no correction is applied.
+        :type correct_ash_mg: float, optional
+        :param correct_ash_fr: The correction value for ash as a fraction. If None, no correction is applied.
+        :type correct_ash_fr: float, optional
+        :return: The corrected data as a pandas DataFrame.
+        :rtype: pd.DataFrame
+        """
+        if correct_ash_mg is not None:
+            file["m_mg"] = file["m_mg"] - np.min(file["m_mg"]) + correct_ash_mg
+        try:
+            if file["m_mg"].iloc[-1] < 0:
+                print(
+                    "neg. mass correction: Max [mg]",
+                    np.round(np.max(file["m_mg"]), 3),
+                    "; Min [mg]",
+                    np.round(np.min(file["m_mg"]), 3),
+                )
+                file["m_mg"] = file["m_mg"] - np.min(file["m_mg"])
+        except KeyError:
+            file["m_mg"] = file["m_p"]
+        file["m_p"] = file["m_mg"] / np.max(file["m_mg"]) * 100
+        if correct_ash_fr is not None:
+            file["m_p"] = file["m_p"] - np.min(file["m_p"]) + correct_ash_fr
+            file["m_p"] = file["m_p"] / np.max(file["m_p"]) * 100
+        file = file[file["T_C"] >= self.temp_initial_celsius].copy()
+        file["T_K"] = file["T_C"] + 273.15
+        return file
+
+    def load_files(self):
+        """
+        Load all files associated with this sample, applying necessary corrections and adjustments.
+
+        This method loads and processes each file, ensuring consistent data structure and applying
+        corrections such as ash content adjustments.
+
+        :return: A dictionary where keys are filenames and values are the corresponding corrected data as pandas DataFrames.
+        :rtype: dict[str, pd.DataFrame]
+        """
+        print("\n" + self.name)
+        # import files and makes sure that replicates have the same size
+        for f, filename in enumerate(self.filenames):
+            print(filename)
+            file_to_correct = self.load_single_file(filename)
+
+            file = self.correct_file_values(
+                file_to_correct, self.correct_ash_fr[f], self.correct_ash_fr[f]
+            )
+            # FILE CORRECTION
+            self.files[filename] = file
+            self.len_files[filename] = max(file.shape)
+        self.len_sample = min(self.len_files.values())
+        # keep the shortest vector size for all replicates, create the object
+        for filename in self.filenames:
+            self.files[filename] = self.files[filename].head(self.len_sample)
+        self.files_loaded = True  # Flag to track if data is loaded
+        return self.files
+
+    def proximate_analysis(self):
+        """
+        Perform proximate analysis on the loaded data for the sample.
+
+        This analysis calculates moisture content, ash content, volatile matter, and fixed carbon
+        based on the thermogravimetric data. The results are stored in the instance's attributes for later use.
+        """
+        if not self.files_loaded:
+            self.load_files()
+
+        for f, file in enumerate(self.files.values()):
+            if self.temp_unit == "C":
+                self.temp.add(f, file["T_C"])
+            elif self.temp_unit == "K":
+                self.temp.add(f, file["T_K"])
+            self.time.add(f, file["t_min"])
+
+            self.m_ar.add(f, file["m_mg"])
+            self.mp_ar.add(f, file["m_p"])
+
+            self.idx_moist.add(f, np.argmax(self.time.stk(f) > self.time_moist + 0.01))
+
+            self.moist_ar.add(f, 100 - self.mp_ar.stk(f)[self.idx_moist.stk(f)])
+            self.ash_ar.add(f, self.mp_ar.stk(f)[-1])
+            self.mp_db.add(f, self.mp_ar.stk(f) * 100 / (100 - self.moist_ar.stk(f)))
+            self.mp_db.add(f, np.where(self.mp_db.stk(f) > 100, 100, self.mp_db.stk(f)))
+            self.ash_db.add(f, self.ash_ar.stk(f) * 100 / (100 - self.moist_ar.stk(f)))
+            self.mp_daf.add(
+                f, ((self.mp_db.stk(f) - self.ash_db.stk(f)) * 100 / (100 - self.ash_db.stk(f)))
+            )
+            if self.time_vm is not None:
+                self.idx_vm.add(f, np.argmax(self.time.stk(f) > self.time_vm))
+                self.fc_ar.add(f, self.mp_ar.stk(f)[self.idx_vm.stk(f)] - self.ash_ar.stk(f))
+                self.vm_ar.add(
+                    f, (100 - self.moist_ar.stk(f) - self.ash_ar.stk(f) - self.fc_ar.stk(f))
+                )
+                self.vm_db.add(f, self.vm_ar.stk(f) * 100 / (100 - self.moist_ar.stk(f)))
+                self.fc_db.add(f, self.fc_ar.stk(f) * 100 / (100 - self.moist_ar.stk(f)))
+
+                self.vm_daf.add(
+                    f, ((self.vm_db.stk(f) - self.ash_db.stk(f)) * 100 / (100 - self.ash_db.stk(f)))
+                )
+                self.fc_daf.add(
+                    f, ((self.fc_db.stk(f) - self.ash_db.stk(f)) * 100 / (100 - self.ash_db.stk(f)))
+                )
+
+            idxs_dtg = [
+                np.argmax(self.temp.stk(f) > self.temp_lim_dtg[0]),
+                np.argmax(self.temp.stk(f) > self.temp_lim_dtg[1]),
+            ]
+            # temp_dtg is taken fixed
+
+            # time start from 0 and consideres a fixed heating rate
+            self.time_dtg.add(
+                f,
+                np.linspace(
+                    0,
+                    self.time.stk(f)[idxs_dtg[1]] - self.time.stk(f)[idxs_dtg[0]],
+                    self.len_dtg_db,
+                ),
+            )
+
+            self.mp_db_dtg.add(
+                f,
+                np.interp(
+                    self.temp_dtg,
+                    self.temp.stk(f)[idxs_dtg[0] : idxs_dtg[1]],
+                    self.mp_db.stk(f)[idxs_dtg[0] : idxs_dtg[1]],
+                ),
+            )
+            # the combusiton indexes use rates as /min
+            if self.dtg_basis == "temperature":
+                dtg = np.gradient(self.mp_db_dtg.stk(f), self.temp_dtg)
+            if self.dtg_basis == "time":
+                dtg = np.gradient(self.mp_db_dtg.stk(f), self.time_dtg.stk(f))
+            self.dtg_db.add(f, savgol_filter(dtg, self.dtg_window_filter, 1))
+        # average
+        self.ave_dev_tga_perc = np.average(self.mp_db_dtg.std())
+        print(f"Average TG [%] St. Dev. for replicates: {self.ave_dev_tga_perc:0.2f} %")
+        self.proximate_computed = True
+
+    def oxidation_analysis(self):
+        """
+        Conduct oxidation analysis on the sample's data.
+
+        This method calculates various oxidation parameters such as the initial oxidation temperature (Ti),
+        peak oxidation temperature (Tp), and final oxidation temperature (Tb). It also computes derivative
+        parameters like maximum and average rates of weight loss. The results are stored in the instance's
+        attributes for further analysis.
+        """
+        if not self.proximate_computed:
+            self.proximate_analysis()
+
+        for f in range(self.n_repl):
+            threshold: float = np.max(np.abs(self.dtg_db.stk(f))) * self.temp_i_temp_b_threshold
+            # Ti = T at which dtg > Ti_thresh wt%/min after moisture removal
+            self.temp_i_idx.add(f, int(np.argmax(np.abs(self.dtg_db.stk(f)) > threshold)))
+            self.temp_i.add(f, self.temp_dtg[self.temp_i_idx.stk(f)])
+            # Tp is the T of max abs(dtg)
+            self.temp_p_idx.add(f, int(np.argmax(np.abs(self.dtg_db.stk(f)))))
+            self.temp_p.add(f, self.temp_dtg[self.temp_p_idx.stk(f)])
+            # Tb reaches < 1 wt%/min at end of curve
+            try:
+                self.temp_b_idx.add(f, int(np.flatnonzero(self.dtg_db.stk(f) < -threshold)[-1]))
+            except IndexError:  # the curve nevers goes above 1%
+                self.temp_b_idx.add(f, 0)
+            self.temp_b.add(f, self.temp_dtg[self.temp_b_idx.stk(f)])
+
+            self.dwdtemp_max.add(f, np.max(np.abs(self.dtg_db.stk(f))))
+            self.dwdtemp_mean.add(f, np.average(np.abs(self.dtg_db.stk(f))))
+            # combustion index
+            self.s_combustion_index.add(
+                f,
+                (
+                    self.dwdtemp_max.stk(f)
+                    * self.dwdtemp_mean.stk(f)
+                    / self.temp_i.stk(f)
+                    / self.temp_i.stk(f)
+                    / self.temp_b.stk(f)
+                ),
+            )
+        # # average
+        self.oxidation_computed = True
+
+    def soliddist_analysis(self, steps_min: list[float] | None = None):
+        """
+        Perform solid distribution analysis on the sample's data.
+
+        This analysis calculates the weight loss at specified temperature steps, providing insight into
+        the solid decomposition process. The results are used for generating solid distribution plots.
+
+        :param steps_min: Temperature steps (in minutes) at which the weight loss is calculated. If None, default steps are used.
+        :type steps_min: list[float], optional
+        """
+        if steps_min is None:
+            steps_min = [40, 70, 100, 130, 160, 190]
+        if not self.proximate_computed:
+            self.proximate_analysis()
+
+        for f in range(self.n_repl):
+            idxs = []
+            for step in steps_min:
+                idxs.append(np.argmax(self.time.stk(f) > step))
+            idxs.append(len(self.time.stk(f)) - 1)
+            self.temp_soliddist.add(f, self.temp.stk(f)[idxs])
+            self.time_soliddist.add(f, self.time.stk(f)[idxs])
+
+            self.dmp_soliddist.add(f, -np.diff(self.mp_db.stk(f)[idxs], prepend=100))
+
+            self.loc_soliddist.add(
+                f, np.convolve(np.insert(self.mp_db.stk(f)[idxs], 0, 100), [0.5, 0.5], mode="valid")
+            )
+
+        self.soliddist_computed = True
+
+    def deconv_analysis(
+        self,
+        centers: list[float],
+        sigmas: list[float] | None = None,
+        amplitudes: list[float] | None = None,
+        center_mins: list[float] | None = None,
+        center_maxs: list[float] | None = None,
+        sigma_mins: list[float] | None = None,
+        sigma_maxs: list[float] | None = None,
+        amplitude_mins: list[float] | None = None,
+        amplitude_maxs: list[float] | None = None,
+    ):
+        """
+        Perform deconvolution analysis on the sample's DTG data.
+
+        This method fits multiple Gaussian peaks to the DTG curve to identify and analyze individual
+        decomposition steps within the sample.
+
+        :param centers: Initial guesses for the centers of the Gaussian peaks.
+        :type centers: list[float]
+        :param sigmas: Initial guesses for the standard deviations of the Gaussian peaks. If None, defaults are used.
+        :type sigmas: list[float], optional
+        :param amplitudes: Initial guesses for the amplitudes of the Gaussian peaks. If None, defaults are used.
+        :type amplitudes: list[float], optional
+        :param center_mins: Minimum allowed values for the centers of the Gaussian peaks. If None, no bounds are applied.
+        :type center_mins: list[float], optional
+        :param center_maxs: Maximum allowed values for the centers of the Gaussian peaks. If None, no bounds are applied.
+        :type center_maxs: list[float], optional
+        :param sigma_mins: Minimum allowed values for the standard deviations of the Gaussian peaks. If None, no bounds are applied.
+        :type sigma_mins: list[float], optional
+        :param sigma_maxs: Maximum allowed values for the standard deviations of the Gaussian peaks. If None, no bounds are applied.
+        :type sigma_maxs: list[float], optional
+        :param amplitude_mins: Minimum allowed values for the amplitudes of the Gaussian peaks. If None, no bounds are applied.
+        :type amplitude_mins: list[float], optional
+        :param amplitude_maxs: Maximum allowed values for the amplitudes of the Gaussian peaks. If None, no bounds are applied.
+        :type amplitude_maxs: list[float], optional
+        """
+        if not self.proximate_computed:
+            self.proximate_analysis()
+        n_peaks = len(centers)
+        # self.dcv_best_fit_stk = np.zeros((self.len_dtg_db, self.n_repl))
+        # self.dcv_r2_stk = np.zeros(self.n_repl)
+
+        # self.dcv_peaks_stk = np.zeros((self.len_dtg_db, self.n_repl, n_peaks))
+        if sigmas is None:
+            sigmas = [1] * n_peaks
+        if amplitudes is None:
+            amplitudes = [10] * n_peaks
+        if center_mins is None:
+            center_mins = [None] * n_peaks
+        if center_maxs is None:
+            center_maxs = [None] * n_peaks
+        if sigma_mins is None:
+            sigma_mins = [None] * n_peaks
+        if sigma_maxs is None:
+            sigma_maxs = [None] * n_peaks
+        if amplitude_mins is None:
+            amplitude_mins = [0] * n_peaks
+        if amplitude_maxs is None:
+            amplitude_maxs = [None] * n_peaks
+
+        for f in range(self.n_repl):
+            y = np.abs(self.dtg_db.stk(f))
+            model = LinearModel(prefix="bkg_")
+            params = model.make_params(intercept=0, slope=0, vary=False)
+
+            for p in range(n_peaks):
+                prefix = f"peak_{p}"
+                self.dcv_peaks.append(Measure(name=prefix))
+                peak_model = GaussianModel(prefix=prefix)
+                pars = peak_model.make_params()
+                pars[prefix + "center"].set(
+                    value=centers[p], min=center_mins[p], max=center_maxs[p]
+                )
+                pars[prefix + "sigma"].set(value=sigmas[p], min=sigma_mins[p], max=sigma_maxs[p])
+                pars[prefix + "amplitude"].set(
+                    value=amplitudes[p], min=amplitude_mins[p], max=amplitude_maxs[p]
+                )
+                model += peak_model
+                params.update(pars)
+
+            result = model.fit(y, params=params, x=self.temp_dtg)
+            self.dcv_best_fit.add(f, -result.best_fit)
+            self.dcv_r2.add(f, 1 - result.residual.var() / np.var(y))
+            components = result.eval_components(x=self.temp_dtg)
+
+            for p in range(n_peaks):
+                prefix = f"peak_{p}"
+                if prefix in components:
+                    self.dcv_peaks[p].add(f, -components[prefix])
+                else:
+                    self.dcv_peaks[p].add(f, 0)
+
+        self.deconv_computed = True
+
+    def report(
+        self,
+        report_type: Literal[
+            "proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"
+        ] = "proximate",
+    ) -> pd.DataFrame:
+        """
+        Generate a report based on the specified analysis type.
+
+        This method provides detailed insights into the sample's properties, such as proximate analysis,
+        oxidation characteristics, and solid distribution, based on the selected report type.
+
+        :param report_type: The type of report to generate. Options include 'proximate', 'oxidation',
+                            'oxidation_extended', 'soliddist', and 'soliddist_extended'.
+        :type report_type: Literal["proximate", "oxidation", "oxidation_extended", "soliddist", "soliddist_extended"]
+        :return: A pandas DataFrame containing the analysis results.
+        :rtype: pd.DataFrame
+        """
+        if report_type == "proximate":
+            if not self.proximate_computed:
+                self.proximate_analysis()
+            variables = [self.moist_ar, self.vm_db, self.fc_db, self.ash_db]
+        elif report_type == "oxidation" or report_type == "oxidation_extended":
+            if not self.oxidation_computed:
+                self.oxidation_analysis()
+            variables = [self.temp_i, self.temp_p, self.temp_b, self.s_combustion_index]
+            if report_type == "oxidation_extended":
+                variables += [self.dwdtemp_max, self.dwdtemp_mean]
+
+        elif report_type == "soliddist" or report_type == "soliddist_extended":
+            if not self.soliddist_computed:
+                self.soliddist_analysis()
+            if report_type == "soliddist":
+                variables = []
+                for p in self.temp_soliddist.ave():
+                    variables.append(Measure(name=f"{p:0.0f} {self.temp_unit}"))
+                for f in range(self.n_repl):
+                    for t, dmp in enumerate(self.dmp_soliddist.stk(f)):
+                        variables[t].add(f, dmp)
+            elif report_type == "soliddist_extended":
+                variables = [self.temp_soliddist, self.time_soliddist, self.dmp_soliddist]
+        else:
+            raise ValueError(f"{report_type = } is not a valid option")
+
+        var_names = [var.name for var in variables]
+        index = [f"repl_{f}" for f in range(self.n_repl)] + ["ave", "std"]
+        rep_data = []
+
+        for f in range(self.n_repl):
+            rep_data.append([var.stk(f) for var in variables])
+        rep_data.append([var.ave() for var in variables])
+        rep_data.append([var.std() for var in variables])
+
+        report = pd.DataFrame(data=rep_data, columns=var_names, index=index)
+        report.index.name = self.name
+        self.report_types_computed.append(report_type)
+        self.reports[report_type] = report
+        if self.auto_save_reports:
+            out_path = plib.Path(self.out_path, "single_sample_reports")
+            out_path.mkdir(parents=True, exist_ok=True)
+            report.to_excel(plib.Path(out_path, f"{self.name}_{report_type}.xlsx"))
+        return report
+
+    def plot_tg_dtg(self, **kwargs: dict[str, Any]) -> MyFigure:
+        """
+        Generate a plot combining thermogravimetric (TG) and derivative thermogravimetric (DTG) data.
+
+        This method creates a figure showing the TG and DTG curves, providing a visual representation
+        of the sample's thermal decomposition behavior.
+
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the generated plot.
+        :rtype: MyFigure
+        """
+        if not self.proximate_computed:
+            self.proximate_analysis()
+        out_path = plib.Path(self.out_path, "single_sample_plots")
+        out_path.mkdir(parents=True, exist_ok=True)
+
+        default_kwargs = {
+            "filename": self.name + "_tg_dtg",
+            "out_path": out_path,
+            "height": 8.53,
+            "width": 6.4,
+            "x_lab": "time [min]",
+            "y_lab": [
+                f"T [{self.temp_symbol}]",
+                f"T [{self.temp_symbol}]",
+                f"{self.tg_label} (stb)",
+                f"{self.tg_label} (db)",
+                f"{self.tg_label} (db)",
+                f"{self.dtg_label} (db)",
+            ],
+            "grid": self.plot_grid,
+            "text_font": self.plot_font,
+        }
+        # Update kwargs with the default key-value pairs if the key is not present in kwargs
+        kwargs = {**default_kwargs, **kwargs}
+
+        mf = MyFigure(
+            rows=3,
+            cols=2,
+            **kwargs,
+        )
+        # tg plot 0, 2, 4 on the left
+        for f in range(self.n_repl):
+            mf.axs[0].plot(
+                self.time.stk(f),
+                self.temp.stk(f),
+                color=colors[f],
+                linestyle=linestyles[f],
+                label=self.filenames[f],
+            )
+            mf.axs[2].plot(
+                self.time.stk(f),
+                self.mp_ar.stk(f),
+                color=colors[f],
+                linestyle=linestyles[f],
+                label=self.filenames[f],
+            )
+            mf.axs[4].plot(
+                self.time.stk(f),
+                self.mp_db.stk(f),
+                color=colors[f],
+                linestyle=linestyles[f],
+                label=self.filenames[f],
+            )
+            mf.axs[0].vlines(
+                self.time.stk(f)[self.idx_moist.stk(f)],
+                self.temp.stk(f)[self.idx_moist.stk(f)] - 50,
+                self.temp.stk(f)[self.idx_moist.stk(f)] + 50,
+                linestyle=linestyles[f],
+                color=colors[f],
+            )
+            mf.axs[2].vlines(
+                self.time.stk(f)[self.idx_moist.stk(f)],
+                self.mp_ar.stk(f)[self.idx_moist.stk(f)] - 5,
+                self.mp_ar.stk(f)[self.idx_moist.stk(f)] + 5,
+                linestyle=linestyles[f],
+                color=colors[f],
+            )
+
+            if self.vm_db() < 99:
+                mf.axs[0].vlines(
+                    self.time.stk(f)[self.idx_vm.stk(f)],
+                    self.temp.stk(f)[self.idx_vm.stk(f)] - 50,
+                    self.temp.stk(f)[self.idx_vm.stk(f)] + 50,
+                    linestyle=linestyles[f],
+                    color=colors[f],
+                )
+                mf.axs[4].vlines(
+                    self.time.stk(f)[self.idx_vm.stk(f)],
+                    self.mp_db.stk(f)[self.idx_vm.stk(f)] - 5,
+                    self.mp_db.stk(f)[self.idx_vm.stk(f)] + 5,
+                    linestyle=linestyles[f],
+                    color=colors[f],
+                )
+            # tg plot 1, 3, 5 on the right
+            mf.axs[1].plot(
+                self.time_dtg.stk(f),
+                self.temp_dtg,
+                color=colors[f],
+                linestyle=linestyles[f],
+                label=self.filenames[f],
+            )
+            mf.axs[3].plot(
+                self.time_dtg.stk(f),
+                self.mp_db_dtg.stk(f),
+                color=colors[f],
+                linestyle=linestyles[f],
+                label=self.filenames[f],
+            )
+            mf.axs[5].plot(
+                self.time_dtg.stk(f),
+                self.dtg_db.stk(f),
+                color=colors[f],
+                linestyle=linestyles[f],
+                label=self.filenames[f],
+            )
+            #
+            if self.oxidation_computed:
+                mf.axs[5].vlines(
+                    self.time_dtg.stk(f)[self.temp_i_idx.stk(f)],
+                    ymin=-1.5,
+                    ymax=0,
+                    linestyle=linestyles[f],
+                    color=colors[f],
+                )
+                mf.axs[5].vlines(
+                    self.time_dtg.stk(f)[self.temp_p_idx.stk(f)],
+                    ymin=np.min(self.dtg_db.stk(f)),
+                    ymax=np.min(self.dtg_db.stk(f)) / 5,
+                    linestyle=linestyles[f],
+                    color=colors[f],
+                )
+                mf.axs[5].vlines(
+                    self.time_dtg.stk(f)[self.temp_b_idx.stk(f)],
+                    ymin=-1.5,
+                    ymax=0,
+                    linestyle=linestyles[f],
+                    color=colors[f],
+                )
+        mf.save_figure()
+        return mf
+
+    def plot_soliddist(self, **kwargs: dict[str, Any]) -> MyFigure:
+        """
+        Generate a plot illustrating the solid distribution analysis results.
+
+        This method plots the weight loss of the sample at specified temperature steps, showing the
+        distribution of solid components within the sample.
+
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the generated plot.
+        :rtype: MyFigure
+        """
+
+        # slightly different plotting behaviour (uses averages)
+        if not self.soliddist_computed:
+            self.soliddist_analysis()
+        out_path = plib.Path(self.out_path, "single_sample_plots")
+        out_path.mkdir(parents=True, exist_ok=True)
+
+        default_kwargs = {
+            "filename": self.name + "_soliddist",
+            "out_path": out_path,
+            "height": 3.2,
+            "width": 3.2,
+            "x_lab": "time [min]",
+            "y_lab": f"{self.tg_label} (db)",
+            "yt_lab": f"T [{self.temp_symbol}]",
+            "legend_loc": "center left",
+            "grid": self.plot_grid,
+            "text_font": self.plot_font,
+        }
+        # Update kwargs with the default key-value pairs if the key is not present in kwargs
+        kwargs = {**default_kwargs, **kwargs}
+
+        mf = MyFigure(
+            rows=1,
+            cols=1,
+            twinx=True,
+            **kwargs,
+        )
+        for f in range(self.n_repl):
+
+            mf.axs[0].plot(
+                self.time.stk(f),
+                self.mp_db.stk(f),
+                color=colors[f],
+                linestyle=linestyles[f],
+                label=self.filenames[f],
+            )
+            mf.axts[0].plot(self.time.stk(f), self.temp.stk(f))
+
+        for tm, mp, dmp in zip(self.time_soliddist(), self.loc_soliddist(), self.dmp_soliddist()):
+            mf.axs[0].annotate(
+                f"{dmp:0.0f}%", ha="center", va="top", xy=(tm - 10, mp + 1), fontsize=9
+            )
+        mf.save_figure()
+        return mf
+
+    def plot_deconv(self, **kwargs: dict[str, Any]) -> MyFigure:
+        """
+        Generate a plot showing the deconvolution analysis results.
+
+        This method visualizes the Gaussian peak fitting performed on the DTG data, illustrating the
+        identified decomposition steps within the sample.
+
+        :param kwargs: Additional keyword arguments for plot customization.
+        :type kwargs: dict
+        :return: A MyFigure instance containing the deconvolution analysis plot.
+        :rtype: MyFigure
+        """
+
+        if not self.deconv_computed:
+            raise ValueError("Deconvolution analysis not computed")
+        out_path = plib.Path(self.out_path, "single_sample_plots")
+        out_path.mkdir(parents=True, exist_ok=True)
+
+        default_kwargs = {
+            "filename": self.name + "_deconv",
+            "out_path": out_path,
+            "height": 8.53,
+            "width": 3.2,
+            "x_lab": f"T [{self.temp_symbol}]",
+            "y_lab": f"{self.dtg_label} (db)",
+            "grid": self.plot_grid,
+            "text_font": self.plot_font,
+        }
+        # Update kwargs with the default key-value pairs if the key is not present in kwargs
+        kwargs = {**default_kwargs, **kwargs}
+        mf = MyFigure(
+            rows=self.n_repl,
+            cols=1,
+            **kwargs,
+        )
+
+        # Plot DTG data
+        for f in range(self.n_repl):
+            mf.axs[f].plot(self.temp_dtg, self.dtg_db.stk(f), color="black", label="DTG")
+            # Plot best fit and individual peaks
+            mf.axs[f].plot(
+                self.temp_dtg,
+                self.dcv_best_fit.stk(f),
+                label="best fit",
+                color="red",
+                linestyle="--",
+            )
+            colors_p = colors[:3] + colors[5:]  # avoid using red
+            for p, peak in enumerate(self.dcv_peaks):
+                if peak.stk(f) is not None:
+                    mf.axs[f].plot(
+                        self.temp_dtg,
+                        peak.stk(f),
+                        label=peak.name,
+                        color=colors_p[p],
+                        linestyle=linestyles[p],
+                    )
+            mf.axs[f].annotate(
+                f"r$^2$={self.dcv_r2.stk(f):.2f}",
+                xycoords="axes fraction",
+                xy=(0.85, 0.96),
+                size="x-small",
+            )
+        mf.save_figure()
+        return mf
```

### Comparing `tga_data_analysis-2.0.4/src/tga_data_analysis.egg-info/PKG-INFO` & `tga_data_analysis-2.0.6/src/tga_data_analysis.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-Metadata-Version: 2.1
-Name: tga_data_analysis
-Version: 2.0.4
-Summary: Tool for automatic analysis of multiple TGA results
-Author: Matteo Pecchi
-License: MIT
-Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
-Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: numpy>=1.21.2
-Requires-Dist: pandas>=1.3.3
-Requires-Dist: matplotlib>=3.4.3
-Requires-Dist: seaborn>=0.11.2
-Requires-Dist: openpyxl
-Requires-Dist: pyarrow
-Requires-Dist: scipy>=1.7.1
-Requires-Dist: lmfit>=1.0.2
-
-# Thermogravimetric Analysis in Python
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-## Overview
-PyTGA is a Python module designed for conducting and analyzing Thermogravimetric Analysis (TGA) experiments. It offers tools for loading, processing, and analyzing TGA data, focusing on proximate and oxidation analysis, solid distillation analysis, and deconvolution analysis.
-
-## Features
-- **Data Loading**: Supports loading TGA data from files.
-- **Proximate Analysis**: Calculates moisture, ash, and volatile matter.
-- **Oxidation Analysis**: Computes Ti, Tp, Tb, etc.
-- **Solid Distillation Analysis**: Analyzes solid distillation over time.
-- **Deconvolution Analysis**: Deconvolutes TGA curves for peak analysis.
-- **Plotting and Visualization**: Functions for TGA data visualization.
-
-## Example
-The example is available in the example folder that can be found using the project link homepage. Necessary data are provided. The example demonstrates how to use the tga_data_analysis package for basic TGA data analysis and visualization, the example requires downloading the data, installing the package, and setting the folder path to the example data folder.
+Metadata-Version: 2.1
+Name: tga_data_analysis
+Version: 2.0.6
+Summary: Tool for automatic analysis of multiple TGA results
+Author: Matteo Pecchi
+License: MIT
+Project-URL: Homepage, https://github.com/mpecchi/tga_data_analysis
+Project-URL: Documentation, https://tga-data-analysis.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.21.2
+Requires-Dist: pandas>=1.3.3
+Requires-Dist: matplotlib>=3.4.3
+Requires-Dist: seaborn>=0.11.2
+Requires-Dist: openpyxl
+Requires-Dist: pyarrow
+Requires-Dist: scipy>=1.7.1
+Requires-Dist: lmfit>=1.0.2
+
+# Thermogravimetric Analysis in Python
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Testing (CI)](https://github.com/mpecchi/tga_data_analysis/actions/workflows/continuous_integration.yaml/badge.svg)](https://github.com/mpecchi/tga_data_analysis/actions/workflows/continuous_integration.yaml)
+## Overview
+PyTGA is a Python module designed for conducting and analyzing Thermogravimetric Analysis (TGA) experiments. It offers tools for loading, processing, and analyzing TGA data, focusing on proximate and oxidation analysis, solid distillation analysis, and deconvolution analysis.
+
+## Features
+- **Data Loading**: Supports loading TGA data from files.
+- **Proximate Analysis**: Calculates moisture, ash, and volatile matter.
+- **Oxidation Analysis**: Computes Ti, Tp, Tb, etc.
+- **Solid Distillation Analysis**: Analyzes solid distillation over time.
+- **Deconvolution Analysis**: Deconvolutes TGA curves for peak analysis.
+- **Plotting and Visualization**: Functions for TGA data visualization.
+
+
+## Documentation
+
+Check out the [documentation](https://tga-data-analysis.readthedocs.io/).
+
+## Installation
+
+You can install the package from [PyPI](https://pypi.org/project/tga_data_analysis/):
+
+```bash
+pip install tga_data_analysis
```

### Comparing `tga_data_analysis-2.0.4/tests/test_measure.py` & `tga_data_analysis-2.0.6/tests/test_measure.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import pytest
-import numpy as np
-import pandas as pd
-from typing import Literal
-from tga_data_analysis.tga import Measure
-
-# Assuming the Measure class is defined here or imported
-
-
-def test_measure_initialization():
-    measure = Measure("test_measure")
-    assert measure.name == "test_measure"
-    assert measure._stk == {}
-    assert measure._ave is None
-    assert measure._std is None
-
-
-def test_add_single_value():
-    measure = Measure()
-    measure.add(1, 5.0)
-    assert measure._stk[1] == 5.0
-
-
-def test_add_array_value():
-    measure = Measure()
-    arr = np.array([1, 2, 3])
-    measure.add(1, arr)
-    assert np.array_equal(measure._stk[1], arr)
-
-
-def test_add_series_value():
-    measure = Measure()
-    series = pd.Series([1, 2, 3])
-    measure.add(2, series)
-    assert np.array_equal(measure._stk[2], series.to_numpy())
-
-
-def test_ave_single_value():
-    measure = Measure()
-    measure.add(1, 5.0)
-    measure.add(2, 15.0)
-    assert measure.ave() == 10.0
-
-
-def test_ave_array_value():
-    measure = Measure()
-    measure.add(1, np.array([1, 2, 3]))
-    measure.add(2, np.array([4, 5, 6]))
-    assert np.array_equal(measure.ave(), np.array([2.5, 3.5, 4.5]))
-
-
-def test_std_population():
-    Measure.set_std_type("population")
-    measure = Measure()
-    measure.add(1, 10)
-    measure.add(2, 20)
-    assert measure.std() == 5.0
-
-
-def test_std_sample():
-    Measure.set_std_type("sample")
-    measure = Measure()
-    measure.add(1, 10)
-    measure.add(2, 20)
-    assert measure.std() == np.std([10, 20], ddof=1)
-
-
-def test_set_std_type():
-    Measure.set_std_type("population")
-    assert Measure.std_type == "population"
-    assert Measure.np_ddof == 0
-
-    Measure.set_std_type("sample")
-    assert Measure.std_type == "sample"
-    assert Measure.np_ddof == 1
+import pytest
+import numpy as np
+import pandas as pd
+from typing import Literal
+from tga_data_analysis.tga import Measure
+
+# Assuming the Measure class is defined here or imported
+
+
+def test_measure_initialization():
+    measure = Measure("test_measure")
+    assert measure.name == "test_measure"
+    assert measure._stk == {}
+    assert measure._ave is None
+    assert measure._std is None
+
+
+def test_add_single_value():
+    measure = Measure()
+    measure.add(1, 5.0)
+    assert measure._stk[1] == 5.0
+
+
+def test_add_array_value():
+    measure = Measure()
+    arr = np.array([1, 2, 3])
+    measure.add(1, arr)
+    assert np.array_equal(measure._stk[1], arr)
+
+
+def test_add_series_value():
+    measure = Measure()
+    series = pd.Series([1, 2, 3])
+    measure.add(2, series)
+    assert np.array_equal(measure._stk[2], series.to_numpy())
+
+
+def test_ave_single_value():
+    measure = Measure()
+    measure.add(1, 5.0)
+    measure.add(2, 15.0)
+    assert measure.ave() == 10.0
+
+
+def test_ave_array_value():
+    measure = Measure()
+    measure.add(1, np.array([1, 2, 3]))
+    measure.add(2, np.array([4, 5, 6]))
+    assert np.array_equal(measure.ave(), np.array([2.5, 3.5, 4.5]))
+
+
+def test_std_population():
+    Measure.set_std_type("population")
+    measure = Measure()
+    measure.add(1, 10)
+    measure.add(2, 20)
+    assert measure.std() == 5.0
+
+
+def test_std_sample():
+    Measure.set_std_type("sample")
+    measure = Measure()
+    measure.add(1, 10)
+    measure.add(2, 20)
+    assert measure.std() == np.std([10, 20], ddof=1)
+
+
+def test_set_std_type():
+    Measure.set_std_type("population")
+    assert Measure.std_type == "population"
+    assert Measure.np_ddof == 0
+
+    Measure.set_std_type("sample")
+    assert Measure.std_type == "sample"
+    assert Measure.np_ddof == 1
```

