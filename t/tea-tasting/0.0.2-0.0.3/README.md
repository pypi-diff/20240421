# Comparing `tmp/tea_tasting-0.0.2.tar.gz` & `tmp/tea_tasting-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tea_tasting-0.0.2.tar", last modified: Mon Apr 15 20:14:15 2024, max compression
+gzip compressed data, was "tea_tasting-0.0.3.tar", last modified: Sun Apr 21 13:48:01 2024, max compression
```

## Comparing `tea_tasting-0.0.2.tar` & `tea_tasting-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1070 2024-04-15 20:13:54.794706 tea_tasting-0.0.2/LICENSE
--rw-r--r--   0        0        0    13369 2024-04-15 20:13:54.794706 tea_tasting-0.0.2/README.md
--rw-r--r--   0        0        0     3015 2024-04-15 20:14:15.554745 tea_tasting-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      379 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/__init__.py
--rw-r--r--   0        0        0        6 2024-04-15 20:14:15.550745 tea_tasting-0.0.2/src/tea_tasting/_version.txt
--rw-r--r--   0        0        0    11873 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/aggr.py
--rw-r--r--   0        0        0     2926 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/config.py
--rw-r--r--   0        0        0    13048 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/datasets.py
--rw-r--r--   0        0        0     6842 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/experiment.py
--rw-r--r--   0        0        0      307 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/metrics/__init__.py
--rw-r--r--   0        0        0     8882 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/metrics/base.py
--rw-r--r--   0        0        0    11922 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/metrics/mean.py
--rw-r--r--   0        0        0     3164 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/utils.py
--rw-r--r--   0        0        0      390 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/src/tea_tasting/version.py
--rw-r--r--   0        0        0        0 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/metrics/__init__.py
--rw-r--r--   0        0        0    10600 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/metrics/test_base.py
--rw-r--r--   0        0        0     8565 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/metrics/test_mean.py
--rw-r--r--   0        0        0     6811 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_aggr.py
--rw-r--r--   0        0        0     1504 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_config.py
--rw-r--r--   0        0        0     3538 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_datasets.py
--rw-r--r--   0        0        0    10574 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_experiment.py
--rw-r--r--   0        0        0     3089 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_utils.py
--rw-r--r--   0        0        0      779 2024-04-15 20:13:54.798706 tea_tasting-0.0.2/tests/test_version.py
--rw-r--r--   0        0        0    14583 1970-01-01 00:00:00.000000 tea_tasting-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/LICENSE
+-rw-r--r--   0        0        0    14620 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/README.md
+-rw-r--r--   0        0        0     3015 2024-04-21 13:48:01.136269 tea_tasting-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      392 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/__init__.py
+-rw-r--r--   0        0        0        6 2024-04-21 13:48:01.132269 tea_tasting-0.0.3/src/tea_tasting/_version.txt
+-rw-r--r--   0        0        0    11760 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/aggr.py
+-rw-r--r--   0        0        0     2986 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/config.py
+-rw-r--r--   0        0        0    13295 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/datasets.py
+-rw-r--r--   0        0        0     6812 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/experiment.py
+-rw-r--r--   0        0        0      350 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/metrics/__init__.py
+-rw-r--r--   0        0        0     8605 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/metrics/base.py
+-rw-r--r--   0        0        0    12534 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/metrics/mean.py
+-rw-r--r--   0        0        0     4104 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/metrics/proportion.py
+-rw-r--r--   0        0        0     8999 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/utils.py
+-rw-r--r--   0        0        0      390 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/src/tea_tasting/version.py
+-rw-r--r--   0        0        0        0 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/metrics/__init__.py
+-rw-r--r--   0        0        0    10600 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/metrics/test_base.py
+-rw-r--r--   0        0        0     8593 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/metrics/test_mean.py
+-rw-r--r--   0        0        0     4241 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/metrics/test_proportion.py
+-rw-r--r--   0        0        0     6431 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_aggr.py
+-rw-r--r--   0        0        0     1504 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_config.py
+-rw-r--r--   0        0        0     3538 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_datasets.py
+-rw-r--r--   0        0        0    10574 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_experiment.py
+-rw-r--r--   0        0        0     6349 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_utils.py
+-rw-r--r--   0        0        0      779 2024-04-21 13:47:39.664262 tea_tasting-0.0.3/tests/test_version.py
+-rw-r--r--   0        0        0    15834 1970-01-01 00:00:00.000000 tea_tasting-0.0.3/PKG-INFO
```

### Comparing `tea_tasting-0.0.2/LICENSE` & `tea_tasting-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.2/README.md` & `tea_tasting-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,31 +10,29 @@
 **tea-tasting** is a Python package for statistical analysis of A/B tests that features:
 
 - Student's t-test and Z-test out of the box.
 - Extensible API: Define and use statistical tests of your choice.
 - [Delta method](https://alexdeng.github.io/public/files/kdd2018-dm.pdf) for ratio metrics.
 - Variance reduction with [CUPED](https://exp-platform.com/Documents/2013-02-CUPED-ImprovingSensitivityOfControlledExperiments.pdf)/[CUPAC](https://doordash.engineering/2020/06/08/improving-experimental-power-through-control-using-predictions-as-covariate-cupac/) (also in combination with delta method for ratio metrics).
 - Confidence interval for both absolute and percent change.
+- Sample ratio mismatch check.
 
 **tea-tasting** calculates statistics within data backends such as BigQuery, ClickHouse, PostgreSQL, Snowflake, Spark, and other of 20+ backends supported by [Ibis](https://ibis-project.org/). This approach eliminates the need to import granular data into a Python environment, though Pandas DataFrames are also supported.
 
 **tea-tasting** is still in alpha, but already includes all the features listed above. The following features are coming soon:
 
-- Sample ratio mismatch check.
 - More statistical tests:
-  - Asymptotic and exact tests for frequency data.
   - Bootstrap.
   - Quantile test (using Bootstrap).
+  - Asymptotic and exact tests for frequency data.
   - Mann–Whitney U test.
 - Power analysis.
 - A/A tests and simulations.
 - Pretty output for experiment results (round etc.).
-- Documentation on how to define metrics with custom statistical tests.
-- Documentation with MkDocs and Material for MkDocs.
-- More examples.
+- More documentation and examples.
 
 ## Installation
 
 ```bash
 pip install tea-tasting
 ```
 
@@ -62,20 +60,20 @@
 In the following sections, each step of this process will be explained in detail.
 
 ### Input data
 
 The `make_users_data` function creates synthetic data for demonstration purposes. This data mimics what you might encounter in an A/B test for an online store. Each row represents an individual user, with the following columns:
 
 - `user`: The unique identifier for each user.
-- `variant`: The specific variant (e.g., 0 or 1) assigned to the user in the A/B test.
-- `sessions`: The total number of sessions by the user.
-- `orders`: The total number of purchases made by the user.
-- `revenue`: The total revenue generated from the user's purchases.
+- `variant`: The specific variant (e.g., 0 or 1) assigned to each user in the A/B test.
+- `sessions`: The total number of user's sessions.
+- `orders`: The total number of user's orders.
+- `revenue`: The total revenue generated by the user.
 
-**tea-tasting** accepts data as either a Pandas DataFrame or an Ibis Table. [Ibis](https://ibis-project.org/) is a Python package which serves as a DataFrame API to various data backends. It supports 20+ backends including BigQuery, ClickHouse, DuckDB, Polars, PostgreSQL, Snowflake, Spark etc. You can write an SQL-query, wrap it as an Ibis Table and pass it to **tea-tasting**.
+**tea-tasting** accepts data as either a Pandas DataFrame or an Ibis Table. [Ibis](https://ibis-project.org/) is a Python package which serves as a DataFrame API to various data backends. It supports 20+ backends including BigQuery, ClickHouse, DuckDB, Polars, PostgreSQL, Snowflake, Spark etc. You can write an SQL-query, [wrap](https://ibis-project.org/how-to/extending/sql#backend.sql) it as an Ibis Table and pass it to **tea-tasting**.
 
 Many statistical tests, like Student's t-test or Z-test, don't need granular data for analysis. For such tests, **tea-tasting** will query aggregated statistics, like mean and variance, instead of downloading all the detailed data.
 
 **tea-tasting** assumes that:
 
 - The data is grouped by randomization units, such as individual users.
 - There is a column indicating the variant of the A/B test (typically labeled as A, B, etc.).
@@ -104,27 +102,27 @@
 )
 ```
 
 ### Metrics
 
 Metrics are instances of metric classes which define how metrics are calculated. Those calculations include calculation of effect size, confidence interval, p-value and other statistics.
 
-Use the `Mean` class to compare metric averages between variants of an A/B test. For example, average number of orders per user, where user is a randomization unit of an experiment. Specify the column containing the metric values using the first parameter `value`.
+Use the `Mean` class to compare averages between variants of an A/B test. For example, average number of orders per user, where user is a randomization unit of an experiment. Specify the column containing the metric values using the first parameter `value`.
 
-Use the `RatioOfMeans` class to compare ratios of metrics averages between variants of an A/B test. For example, average number of orders per average number of sessions. Specify the columns containing the numerator and denominator values using the parameters `numer` and `denom`.
+Use the `RatioOfMeans` class to compare ratios of averages between variants of an A/B test. For example, average number of orders per average number of sessions. Specify the columns containing the numerator and denominator values using the parameters `numer` and `denom`.
 
 Use the following parameters of `Mean` and `RatioOfMeans` to customize the analysis:
 
 - `alternative`: Alternative hypothesis. The following options are available:
-  - `two-sided` (default): the means are unequal.
-  - `greater`: the mean in the treatment variant is greater than the mean in the control variant.
-  - `less`: the mean in the treatment variant is less than the mean in the control variant.
+  - `"two-sided"` (default): the means are unequal.
+  - `"greater"`: the mean in the treatment variant is greater than the mean in the control variant.
+  - `"less"`: the mean in the treatment variant is less than the mean in the control variant.
 - `confidence_level`: Confidence level of the confidence interval. Default is `0.95`.
-- `equal_var`: If `False` (default), assume unequal population variances in calculation of the standard deviation and the number of degrees of freedom. Otherwise, assume equal population variance and calculated pooled standard deviation.
-- `use_t`: If `True` (default), use Student's t-distribution in p-value and confidence interval calculations. Otherwise use Normal distribution.
+- `equal_var`: Defines whether equal variance is assumed. If `True`, pooled variance is used for the calculation of the standard error of the difference between two means. Default is `False`.
+- `use_t`: Defines whether to use the Student's t-distribution (`True`) or the Normal distribution (`False`). Default is `True`.
 
 Example usage:
 
 ```python
 experiment = tt.Experiment(
     sessions_per_user=tt.Mean("sessions", alternative="greater"),
     orders_per_session=tt.RatioOfMeans("orders", "sessions", confidence_level=0.9),
@@ -172,15 +170,15 @@
 - `effect_size`: Absolute effect size. Difference between two means.
 - `effect_size_ci_lower`: Lower bound of the absolute effect size confidence interval.
 - `effect_size_ci_upper`: Upper bound of the absolute effect size confidence interval.
 - `rel_effect_size`: Relative effect size. Difference between two means, divided by the control mean.
 - `rel_effect_size_ci_lower`: Lower bound of the relative effect size confidence interval.
 - `rel_effect_size_ci_upper`: Upper bound of the relative effect size confidence interval.
 - `pvalue`: P-value
-- `statistic`: Statistic.
+- `statistic`: Statistic (standardized effect size).
 
 ## More features
 
 ### Variance reduction with CUPED/CUPAC
 
 **tea-tasting** supports variance reduction with CUPED/CUPAC, within both `Mean` and `RatioOfMeans` classes.
 
@@ -212,22 +210,56 @@
 - `revenue_covariate`: Revenue before the experiment.
 
 Define the metrics' covariates:
 
 - In `Mean`, specify the covariate using the `covariate` parameter.
 - In `RatioOfMeans`, specify the covariates for the numerator and denominator using the `numer_covariate` and `denom_covariate` parameters, respectively.
 
+### Sample ratio mismatch check
+
+The `SampleRatio` class in **tea-tasting** detects mismatches in the sample ratios of different variants of an A/B test.
+
+Example usage:
+
+```python
+experiment = tt.Experiment(
+    sessions_per_user=tt.Mean("sessions"),
+    orders_per_session=tt.RatioOfMeans("orders", "sessions"),
+    orders_per_user=tt.Mean("orders"),
+    revenue_per_user=tt.Mean("revenue"),
+    sample_ratio=tt.SampleRatio(),
+)
+```
+
+By default, `SampleRatio` expects equal number of observations across all variants. To specify a different ratio, use the `ratio` parameter. It accepts two types of values:
+
+- Ratio of the number of observation in treatment relative to control, as a positive number. Example: `SampleRatio(0.5)`.
+- A dictionary with variants as keys and expected ratios as values. Example: `SampleRatio({"A": 2, "B": 1})`.
+
+The `method` parameter determines the statistical test to apply:
+
+- `"auto"`: Apply exact binomial test if the total number of observations is less than 1000, or normal approximation otherwise.
+- `"binom"`: Apply exact binomial test.
+- `"norm"`: Apply normal approximation of the binomial distribution.
+
+The result of the sample ratio mismatch includes the following attributes:
+
+- `metric`: Metric name.
+- `control`: Number of observations in control.
+- `treatment`: Number of observations in treatment.
+- `pvalue`: P-value
+
 ### Global settings
 
 In **tea-tasting**, you can change defaults for the following parameters:
 
 - `alternative`: Alternative hypothesis.
 - `confidence_level`: Confidence level of the confidence interval.
-- `equal_var`: If False, assume unequal population variances in calculation of the standard deviation and the number of degrees of freedom. Otherwise, assume equal population variance and calculated pooled standard deviation.
-- `use_t`: If True, use Student's t-distribution in p-value and confidence interval calculations. Otherwise use Normal distribution.
+- `equal_var`: If `False`, assume unequal population variances in calculation of the standard deviation and the number of degrees of freedom. Otherwise, assume equal population variance and calculate pooled standard deviation.
+- `use_t`: If `True`, use Student's t-distribution in p-value and confidence interval calculations. Otherwise use Normal distribution.
 
 Use `set_config` to set a global option value:
 
 ```python
 tt.set_config(confidence_level=0.9)
 ```
```

### Comparing `tea_tasting-0.0.2/pyproject.toml` & `tea_tasting-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Typing :: Typed",
 ]
-version = "0.0.2"
+version = "0.0.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/tea-tasting"
```

### Comparing `tea_tasting-0.0.2/src/tea_tasting/aggr.py` & `tea_tasting-0.0.3/src/tea_tasting/aggr.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,96 +33,80 @@
     def __init__(
         self,
         count_: int | None = None,
         mean_: dict[str, float | int] = {},  # noqa: B006
         var_: dict[str, float | int] = {},  # noqa: B006
         cov_: dict[tuple[str, str], float | int] = {},  # noqa: B006
     ) -> None:
-        """Create an object with aggregated statistics.
+        """Aggregated statistics.
 
         Args:
-            count_: Sample size.
-            mean_: Variables sample means.
-            var_: Variables sample variances.
-            cov_: Pairs of variables sample covariances.
+            count_: Sample size (number of observations).
+            mean_: Dictionary of sample means with variable names as keys.
+            var_: Dictionary of sample variances with variable names as keys.
+            cov_: Dictionary of sample covariances with pairs of variable names as keys.
         """
         self.count_ = count_
         self.mean_ = mean_
         self.var_ = var_
-        self.cov_ = {
-            _sorted_tuple(left, right): value
-            for (left, right), value in cov_.items()
-        }
+        self.cov_ = {_sorted_tuple(*k): v for k, v in cov_.items()}
 
-    def filter(
-        self,
-        has_count: bool,
-        mean_cols: Sequence[str],
-        var_cols: Sequence[str],
-        cov_cols: Sequence[tuple[str, str]],
-    ) -> Aggregates:
-        """Filter aggregated statistics.
-
-        Args:
-            has_count: If True, keep sample size in the resulting object.
-            mean_cols: Sample means variable names.
-            var_cols: Sample variances variable names.
-            cov_cols: Sample covariances variable names.
+    def with_zero_div(self) -> Aggregates:
+        """Return aggregates, which don't raise an error on division by zero.
 
-        Returns:
-            Filtered aggregated statistics.
+        Division by zero returns:
+            nan if numerator == 0,
+            inf if numerator > 0,
+            -inf if numerator < 0.
         """
-        mean_cols, var_cols, cov_cols = _validate_aggr_cols(
-            mean_cols, var_cols, cov_cols)
-
         return Aggregates(
-            count_=self.count() if has_count else None,
-            mean_={col: self.mean(col) for col in mean_cols},
-            var_={col: self.var(col) for col in var_cols},
-            cov_={cols: self.cov(*cols) for cols in cov_cols},
+            count_=None if self.count_ is None else tea_tasting.utils.Int(self.count_),
+            mean_={k: tea_tasting.utils.numeric(v) for k, v in self.mean_.items()},
+            var_={k: tea_tasting.utils.numeric(v) for k, v in self.var_.items()},
+            cov_={k: tea_tasting.utils.numeric(v) for k, v in self.cov_.items()},
         )
 
     def count(self) -> int:
-        """Sample size.
+        """Sample size (number of observations).
 
         Raises:
             RuntimeError: Count is None (it wasn't defined at init).
 
         Returns:
-            Number of observations.
+            Sample size (number of observations).
         """
         if self.count_ is None:
             raise RuntimeError("Count is None.")
         return self.count_
 
-    def mean(self, key: str | None) -> float | int:
+    def mean(self, name: str | None) -> float | int:
         """Sample mean.
 
         Args:
-            key: Variable name.
+            name: Variable name.
 
         Returns:
             Sample mean.
         """
-        if key is None:
+        if name is None:
             return 1
-        return self.mean_[key]
+        return self.mean_[name]
 
-    def var(self, key: str | None) -> float | int:
+    def var(self, name: str | None) -> float | int:
         """Sample variance.
 
         Args:
-            key: Variable name.
+            name: Variable name.
 
         Returns:
             Sample variance.
         """
-        if key is None:
+        if name is None:
             return 0
-        return self.var_[key]
+        return self.var_[name]
 
     def cov(self, left: str | None, right: str | None) -> float | int:
         """Sample covariance.
 
         Args:
             left: First variable name.
             right: Second variable name.
@@ -148,19 +132,20 @@
         Args:
             numer: Numerator variable name.
             denom: Denominator variable name.
 
         Returns:
             Sample variance of the ratio of two variables.
         """
+        numer_mean_sq = self.mean(numer) * self.mean(numer)
         denom_mean_sq = self.mean(denom) * self.mean(denom)
         return (
             self.var(numer)
             - 2 * self.cov(numer, denom) * self.mean(numer) / self.mean(denom)
-            + self.var(denom) * self.mean(numer) * self.mean(numer) / denom_mean_sq
+            + self.var(denom) * numer_mean_sq / denom_mean_sq
         ) / denom_mean_sq
 
     def ratio_cov(
         self,
         left_numer: str | None,
         left_denom: str | None,
         right_numer: str | None,
@@ -265,26 +250,27 @@
     data: ibis.expr.types.Table | pd.DataFrame,
     group_col: str | None,
     has_count: bool,
     mean_cols: Sequence[str],
     var_cols: Sequence[str],
     cov_cols: Sequence[tuple[str, str]],
 ) -> dict[Any, Aggregates] | Aggregates:
-    """Read aggregated statistics from an Ibis Table.
+    """Read aggregated statistics from an Ibis Table or a Pandas DataFrame.
 
     Args:
-        data: Ibis Table.
+        data: Granular data.
         group_col: Column name to group by before aggregation.
+            If None, total aggregates are calculated.
         has_count: If True, calculate the sample size.
         mean_cols: Column names for calculation of sample means.
         var_cols: Column names for calculation of sample variances.
         cov_cols: Pairs of column names for calculation of sample covariances.
 
     Returns:
-        Aggregated statistics from the Ibis Table.
+        Aggregated statistics.
     """
     if isinstance(data, pd.DataFrame):
         con = ibis.pandas.connect()
         data = con.create_table("data", data)
 
     mean_cols, var_cols, cov_cols = _validate_aggr_cols(mean_cols, var_cols, cov_cols)
```

### Comparing `tea_tasting-0.0.2/src/tea_tasting/config.py` & `tea_tasting-0.0.3/src/tea_tasting/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Global config."""
+"""Global configuration."""
 
 from __future__ import annotations
 
 import contextlib
 from typing import TYPE_CHECKING
 
 import tea_tasting.utils
@@ -24,15 +24,15 @@
 def get_config(option: str | None = None) -> Any:
     """Get global configuration.
 
     Args:
         option: The option name.
 
     Returns:
-        The value of the option if it's not None,
+        The option value if its name is not None,
         or a dictionary with all options otherwise.
     """
     if option is not None:
         return _global_config[option]
     return _global_config.copy()
 
 
@@ -81,15 +81,15 @@
         equal_var: Defines whether equal variance is assumed. If True,
             pooled variance is used for the calculation of the standard error
             of the difference between two means. Default is False.
         use_t: Defines whether to use the Student's t-distribution (True) or
             the Normal distribution (False) by default. Default is True.
         kwargs: User-defined global parameters.
     """
-    new_config = locals()
+    new_config = {k: v for k, v in locals().items() if k != "kwargs"} | kwargs
     old_config = get_config()
     set_config(**new_config)
 
     try:
         yield
     finally:
         set_config(**old_config)
```

### Comparing `tea_tasting-0.0.2/src/tea_tasting/datasets.py` & `tea_tasting-0.0.3/src/tea_tasting/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Generates a sample of data for examples."""
+"""Example datasets."""
 # ruff: noqa: PLR0913
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, overload
 
 import ibis
@@ -71,45 +71,47 @@
 
     Data mimics what you might encounter in an A/B test for an online store,
     with user-level randomization. Each row represents an individual user
     with information about:
 
     - user identifier,
     - variant of the test,
-    - number of sessions by the user,
-    - number of orders made by the user,
-    - revenue generated from user's orders.
+    - number of user's sessions,
+    - number of user's orders,
+    - revenue generated by the user.
 
     Optionally, pre-experimental data can be generated as well.
 
     Args:
         covariates: If True, generates pre-experimental data as the covariates
             in addition to default columns.
         seed: Random seed.
         n_users: Number of users.
-        ratio: Ratio of treatment observations to control observations.
-        sessions_uplift: Relative sessions uplift in the treatment variant.
-        orders_uplift: Relative orders uplift in the treatment variant.
-        revenue_uplift: Relative revenue uplift in the treatment variant.
+        ratio: Ratio of the number of observation in treatment relative to control.
+        sessions_uplift: Sessions uplift in the treatment variant, relative to control.
+        orders_uplift: Orders uplift in the treatment variant, relative to control.
+        revenue_uplift: Revenue uplift in the treatment variant, relative to control.
         avg_sessions: Average number of sessions per user.
         avg_orders_per_session: Average number of orders per session.
             Should be less than 1.
         avg_revenue_per_order: Average revenue per order.
-        to_ibis: If True, return Ibis Table instead if Pandas DataFrame.
+        to_ibis: If True, return an Ibis Table instead of a Pandas DataFrame.
 
     Returns:
         An Ibis Table or a Pandas DataFrame with the following columns:
             user: User identifier.
             variant: Variant of the test. 0 is control, 1 is treatment.
-            sessions: Number of sessions.
-            orders: Number of orders.
-            revenue: Revenue.
-            sessions_covariate (optional): Number of sessions before the experiment.
-            orders_covariate (optional): Number of orders before the experiment.
-            revenue_covariate (optional): Revenue before the experiment.
+            sessions: Number of user's sessions.
+            orders: Number of user's orders.
+            revenue: Revenue generated by the user.
+            sessions_covariate (optional): Number of user's sessions
+                before the experiment.
+            orders_covariate (optional): Number of user's orders before the experiment.
+            revenue_covariate (optional): Revenue generated by the user
+                before the experiment.
     """
     return _make_data(
         covariates=covariates,
         seed=seed,
         n_users=n_users,
         ratio=ratio,
         sessions_uplift=sessions_uplift,
@@ -175,45 +177,47 @@
 
     Data mimics what you might encounter in an A/B test for an online store,
     with user-level randomization. Each row represents a user's session
     with information about:
 
     - user identifier,
     - variant of the test,
-    - number of sessions by the user,
-    - number of orders made by the user,
-    - revenue generated from user's orders.
+    - number of user's sessions,
+    - number of user's orders,
+    - revenue generated by the user.
 
     Optionally, pre-experimental data can be generated as well.
 
     Args:
         covariates: If True, generates pre-experimental data as the covariates
             in addition to default columns.
         seed: Random seed.
         n_users: Number of users.
-        ratio: Ratio of treatment observations to control observations.
-        sessions_uplift: Relative sessions uplift in the treatment variant.
-        orders_uplift: Relative orders uplift in the treatment variant.
-        revenue_uplift: Relative revenue uplift in the treatment variant.
+        ratio: Ratio of the number of observation in treatment relative to control.
+        sessions_uplift: Sessions uplift in the treatment variant, relative to control.
+        orders_uplift: Orders uplift in the treatment variant, relative to control.
+        revenue_uplift: Revenue uplift in the treatment variant, relative to control.
         avg_sessions: Average number of sessions per user.
         avg_orders_per_session: Average number of orders per session.
             Should be less than 1.
         avg_revenue_per_order: Average revenue per order.
-        to_ibis: If True, return Ibis Table instead if Pandas DataFrame.
+        to_ibis: If True, return an Ibis Table instead of a Pandas DataFrame.
 
     Returns:
         An Ibis Table or a Pandas DataFrame with the following columns:
             user: User identifier.
             variant: Variant of the test. 0 is control, 1 is treatment.
-            sessions: Number of sessions.
-            orders: Number of orders.
-            revenue: Revenue.
-            sessions_covariate (optional): Number of sessions before the experiment.
-            orders_covariate (optional): Number of orders before the experiment.
-            revenue_covariate (optional): Revenue before the experiment.
+            sessions: Number of user's sessions.
+            orders: Number of user's orders.
+            revenue: Revenue generated by the user.
+            sessions_covariate (optional): Number of user's sessions
+                before the experiment.
+            orders_covariate (optional): Number of user's orders before the experiment.
+            revenue_covariate (optional): Revenue generated by the user
+                before the experiment.
     """
     return _make_data(
         covariates=covariates,
         seed=seed,
         n_users=n_users,
         ratio=ratio,
         sessions_uplift=sessions_uplift,
```

### Comparing `tea_tasting-0.0.2/src/tea_tasting/experiment.py` & `tea_tasting-0.0.3/src/tea_tasting/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Experiments and experiment results."""
+"""Experiments."""
 
 from __future__ import annotations
 
 from collections import UserDict
 from typing import TYPE_CHECKING, Any, overload
 
 import pandas as pd
@@ -33,28 +33,28 @@
         return pd.DataFrame.from_records(self.to_dicts())
 
 
 ExperimentResults = dict[tuple[Any, Any], ExperimentResult]
 
 
 class Experiment(tea_tasting.utils.ReprMixin):
-    """Defines and analyzes the experiment."""
+    """Experiment."""
 
     def __init__(
         self,
         metrics: dict[str, tea_tasting.metrics.MetricBase[Any]] | None = None,
         variant: str = "variant",
         **kw_metrics: tea_tasting.metrics.MetricBase[Any],
     ) -> None:
-        """Define an experiment.
+        """Experiment.
 
         Args:
-            metrics: A dictionary of metrics with metric names as keys.
+            metrics: Dictionary of metrics with metric names as keys.
             variant: Variant column name.
-            kw_metrics: Metrics with metric names as keywords.
+            kw_metrics: Metrics with metric names as parameter names.
         """
         if metrics is None:
             metrics = {}
         metrics = metrics | kw_metrics
 
         tea_tasting.utils.check_scalar(metrics, "metrics", typ=dict)
         tea_tasting.utils.check_scalar(len(metrics), "len(metrics)", gt=0)
@@ -98,15 +98,15 @@
             data: Experimental data.
             control: Control variant. If None, the variant with the minimal ID
                 is used as a control.
             all_variants: If True, analyze all pairs of variants. Otherwise,
                 analyze only one pair of variants.
 
         Returns:
-            Experiment results.
+            Experiment result.
         """
         aggregated_data, granular_data = self._read_data(data)
 
         if aggregated_data is not None:
             variants = aggregated_data.keys()
         elif granular_data is not None:
             variants = granular_data.keys()
@@ -134,15 +134,15 @@
         results = ExperimentResults()
         for control, treatment in variant_pairs:
             result = ExperimentResult()
             for name, metric in self.metrics.items():
                 result |= {name: self._analyze_metric(
                     metric=metric,
                     data=data,
-                    aggr_data=aggregated_data,
+                    aggregated_data=aggregated_data,
                     granular_data=granular_data,
                     control=control,
                     treatment=treatment,
                 )}
 
             if not all_variants:
                 return result
@@ -152,24 +152,24 @@
         return results
 
 
     def _analyze_metric(
         self,
         metric: tea_tasting.metrics.MetricBase[Any],
         data: pd.DataFrame | ibis.expr.types.Table,
-        aggr_data: dict[Any, tea_tasting.aggr.Aggregates] | None,
+        aggregated_data: dict[Any, tea_tasting.aggr.Aggregates] | None,
         granular_data: dict[Any, pd.DataFrame] | None,
         control: Any,
         treatment: Any,
     ) -> tea_tasting.metrics.MetricResult:
         if (
             isinstance(metric, tea_tasting.metrics.MetricBaseAggregated)
-            and aggr_data is not None
+            and aggregated_data is not None
         ):
-            return metric.analyze(aggr_data, control, treatment)
+            return metric.analyze(aggregated_data, control, treatment)
 
         if (
             isinstance(metric, tea_tasting.metrics.MetricBaseGranular)
             and granular_data is not None
         ):
             return metric.analyze(granular_data, control, treatment)
```

### Comparing `tea_tasting-0.0.2/src/tea_tasting/metrics/base.py` & `tea_tasting-0.0.3/src/tea_tasting/metrics/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Metrics base classes."""
+"""Base classes for metrics."""
 
 from __future__ import annotations
 
 import abc
 from typing import TYPE_CHECKING, Any, Generic, NamedTuple, TypeVar, Union, overload
 
 import ibis
@@ -29,80 +29,80 @@
     def analyze(
         self,
         data: pd.DataFrame | ibis.expr.types.Table,
         control: Any,
         treatment: Any,
         variant: str,
     ) -> R:
-        """Analyzes metric in an experiment.
+        """Analyze metric in an experiment.
 
         Args:
             data: Experimental data.
             control: Control variant.
             treatment: Treatment variant.
-            variant: Variant column.
+            variant: Variant column name.
 
         Returns:
-            Experiment results for a metric.
+            Analysis result.
         """
         ...
 
 
 class AggrCols(NamedTuple):
-    """Columns to be aggregated for a metric analysis.
+    """Columns to aggregate for a metric analysis.
 
     Attributes:
         has_count: If True, include the sample size.
         mean_cols: Column names for calculation of sample means.
         var_cols: Column names for calculation of sample variances.
         cov_cols: Pairs of column names for calculation of sample covariances.
     """
     has_count: bool = False
     mean_cols: Sequence[str] = ()
     var_cols: Sequence[str] = ()
     cov_cols: Sequence[tuple[str, str]] = ()
 
     def __or__(self, other: AggrCols) -> AggrCols:
-        """Combine columns. Exclude duplicates.
+        """Combine columns, exclude duplicates.
 
         Args:
-            other: Second objects with columns to be aggregated for a metric analysis.
+            other: Second objects.
 
         Returns:
-            Combined columns to be aggregated for a metric analysis.
+            Combined columns.
         """
         return AggrCols(
             has_count=self.has_count or other.has_count,
             mean_cols=tuple({*self.mean_cols, *other.mean_cols}),
             var_cols=tuple({*self.var_cols, *other.var_cols}),
             cov_cols=tuple({
                 tea_tasting.aggr._sorted_tuple(*cols)
                 for cols in tuple({*self.cov_cols, *other.cov_cols})
             }),
         )
 
     def __len__(self) -> int:
         """Total length of all object attributes.
 
-        If has_count is True then its value is 1, otherwise 0.
+        If has_count is True then its value is 1, or 0 otherwise.
         """
         return (
             int(self.has_count)
             + len(self.mean_cols)
             + len(self.var_cols)
             + len(self.cov_cols)
         )
 
 
 class MetricBaseAggregated(MetricBase[R]):
-    """Base class for metrics analyzed using aggregates."""
+    """Base class for metrics, which are analyzed using aggregated statistics."""
     @property
     @abc.abstractmethod
     def aggr_cols(self) -> AggrCols:
-        """Columns to be aggregated for a metric analysis."""
+        """Columns to aggregate for a metric analysis."""
         ...
 
     @overload
     def analyze(
         self,
         data: dict[Any, tea_tasting.aggr.Aggregates],
         control: Any,
@@ -134,15 +134,15 @@
         Args:
             data: Experimental data.
             control: Control variant.
             treatment: Treatment variant.
             variant: Variant column name.
 
         Returns:
-            Experiment results for a metric.
+            Analysis result.
         """
         aggr = aggregate_by_variants(
             data,
             aggr_cols=self.aggr_cols,
             variant=variant,
         )
         return self.analyze_aggregates(
@@ -159,27 +159,25 @@
         """Analyze metric in an experiment using aggregated statistics.
 
         Args:
             control: Control data.
             treatment: Treatment data.
 
         Returns:
-            Experiment results for a metric.
+            Analysis result.
         """
         ...
 
 
 def aggregate_by_variants(
     data: pd.DataFrame | ibis.expr.types.Table | dict[Any, tea_tasting.aggr.Aggregates],
     aggr_cols: AggrCols,
     variant: str | None = None,
 ) ->  dict[Any, tea_tasting.aggr.Aggregates]:
-    """Validate aggregated experimental data.
-
-    Reads aggregates if data is not a dictionary of Aggregates.
+    """Aggregate experimental data by variants.
 
     Args:
         data: Experimental data.
         aggr_cols: Columns to aggregate.
         variant: Variant column name.
 
     Raises:
@@ -208,19 +206,19 @@
         data=data,
         group_col=variant,
         **aggr_cols._asdict(),
     )
 
 
 class MetricBaseGranular(MetricBase[R]):
-    """Base class for metrics analyzed using granular data."""
+    """Base class for metrics, which are analyzed using granular data."""
     @property
     @abc.abstractmethod
     def cols(self) -> Sequence[str]:
-        """Columns to be fetched for a metric analysis."""
+        """Columns to fetch for a metric analysis."""
         ...
 
     @overload
     def analyze(
         self,
         data: dict[Any, pd.DataFrame],
         control: Any,
@@ -251,15 +249,15 @@
         Args:
             data: Experimental data.
             control: Control variant.
             treatment: Treatment variant.
             variant: Variant column name.
 
         Returns:
-            Experiment results for a metric.
+            Analysis result.
         """
         dfs = read_dataframes(
             data,
             cols=self.cols,
             variant=variant,
         )
         return self.analyze_dataframes(
@@ -276,35 +274,33 @@
         """Analyze metric in an experiment using granular data.
 
         Args:
             control: Control data.
             treatment: Treatment data.
 
         Returns:
-            Experiment results for a metric.
+            Analysis result.
         """
         ...
 
 
 def read_dataframes(
     data: pd.DataFrame | ibis.expr.types.Table | dict[Any, pd.DataFrame],
     cols: Sequence[str],
     variant: str | None = None,
 ) -> dict[Any, pd.DataFrame]:
-    """Validate granular experimental data.
-
-    Reads granular data if data is not a dictionary of DataFrames.
+    """Read granular experimental data.
 
     Args:
         data: Experimental data.
         cols: Columns to read.
         variant: Variant column name.
 
     Raises:
-        ValueError: variant is None, while aggregated data are not provided.
+        ValueError: variant is None, while granular data are not provided.
         TypeError: data is not an instance of DataFrame, Table,
             or a dictionary if DataFrames.
 
     Returns:
         Experimental data as a dictionary of DataFrames.
     """
     if isinstance(data, dict) and all(
```

### Comparing `tea_tasting-0.0.2/src/tea_tasting/metrics/mean.py` & `tea_tasting-0.0.3/src/tea_tasting/metrics/mean.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-"""Analysis of means of two independent samples."""
+"""Analysis of means."""
 # ruff: noqa: PD901
 
 from __future__ import annotations
 
+import math
 from typing import TYPE_CHECKING, NamedTuple
 
-import numpy as np
 import scipy.stats
 
 import tea_tasting.aggr
 import tea_tasting.config
 from tea_tasting.metrics.base import AggrCols, MetricBaseAggregated
 import tea_tasting.utils
 
 
 if TYPE_CHECKING:
     from typing import Literal
 
 
 class MeansResult(NamedTuple):
-    """Result of an analysis of metric means.
+    """Result of an analysis of means.
 
     Attributes:
         control: Control mean.
         treatment: Treatment mean.
         effect_size: Absolute effect size. Difference between two means.
         effect_size_ci_lower: Lower bound of the absolute effect size
             confidence interval.
@@ -32,52 +32,57 @@
         rel_effect_size: Relative effect size. Difference between two means,
             divided by the control mean.
         rel_effect_size_ci_lower: Lower bound of the relative effect size
             confidence interval.
         rel_effect_size_ci_upper: Upper bound of the relative effect size
             confidence interval.
         pvalue: P-value
-        statistic: Statistic.
+        statistic: Statistic (standardized effect size).
     """
     control: float
     treatment: float
     effect_size: float
     effect_size_ci_lower: float
     effect_size_ci_upper: float
     rel_effect_size: float
     rel_effect_size_ci_lower: float
     rel_effect_size_ci_upper: float
     pvalue: float
     statistic: float
 
 
 class RatioOfMeans(MetricBaseAggregated[MeansResult]):
-    """Compares ratios of metrics means between variants."""
+    """Ratio of means."""
 
     def __init__(  # noqa: PLR0913
         self,
         numer: str,
         denom: str | None = None,
         numer_covariate: str | None = None,
         denom_covariate: str | None = None,
         *,
         alternative: Literal["two-sided", "greater", "less"] | None = None,
         confidence_level: float | None = None,
         equal_var: bool | None = None,
         use_t: bool | None = None,
     ) -> None:
-        """Create a ratio metric.
+        """Ratio of means.
 
         Args:
             numer: Numerator column name.
             denom: Denominator column name.
             numer_covariate: Covariate numerator column name.
             denom_covariate: Covariate denominator column name.
-            alternative: Default alternative hypothesis.
-            confidence_level: Default confidence level for the confidence interval.
+            alternative: Alternative hypothesis. Options:
+                "two-sided": the means are unequal.
+                "greater": the mean in the treatment variant is greater than the mean
+                    in the control variant.
+                "less": the mean in the treatment variant is less than the mean
+                    in the control variant.
+            confidence_level: Confidence level for the confidence interval.
             equal_var: Defines whether equal variance is assumed. If True,
                 pooled variance is used for the calculation of the standard error
                 of the difference between two means.
             use_t: Defines whether to use the Student's t-distribution (True) or
                 the Normal distribution (False).
         """
         self.numer = tea_tasting.utils.check_scalar(numer, "numer", typ=str)
@@ -106,15 +111,15 @@
             if use_t is not None
             else tea_tasting.config.get_config("use_t")
         )
 
 
     @property
     def aggr_cols(self) -> AggrCols:
-        """Columns to be aggregated for a metric analysis."""
+        """Columns to aggregate for a metric analysis."""
         cols = tuple(
             col for col in (
                 self.numer,
                 self.denom,
                 self.numer_covariate,
                 self.denom_covariate,
             )
@@ -141,16 +146,18 @@
         """Analyze metric in an experiment using aggregated statistics.
 
         Args:
             control: Control data.
             treatment: Treatment data.
 
         Returns:
-            Experiment result for a metric.
+            Analysis result.
         """
+        control = control.with_zero_div()
+        treatment = treatment.with_zero_div()
         total = control + treatment
         covariate_coef = self._covariate_coef(total)
         covariate_mean = total.mean(self.numer_covariate) / total.mean(
             self.denom_covariate)
         return self._analyze_stats(
             contr_mean=self._metric_mean(control, covariate_coef, covariate_mean),
             contr_var=self._metric_var(control, covariate_coef),
@@ -179,18 +186,17 @@
 
     def _metric_mean(
         self,
         aggr: tea_tasting.aggr.Aggregates,
         covariate_coef: float,
         covariate_mean: float,
     ) -> float:
-        return aggr.mean(self.numer)/aggr.mean(self.denom) - covariate_coef*(
-            aggr.mean(self.numer_covariate)/aggr.mean(self.denom_covariate)
-            - covariate_mean
-        )
+        value = aggr.mean(self.numer) / aggr.mean(self.denom)
+        covariate = aggr.mean(self.numer_covariate) / aggr.mean(self.denom_covariate)
+        return value - covariate_coef*(covariate - covariate_mean)
 
 
     def _metric_var(
         self,
         aggr: tea_tasting.aggr.Aggregates,
         covariate_coef: float,
     ) -> float:
@@ -229,34 +235,34 @@
         means_ratio = treat_mean / contr_mean
         effect_size = treat_mean - contr_mean
         statistic = effect_size / scale
 
         if self.alternative == "greater":
             q = self.confidence_level
             effect_size_ci_lower = effect_size + scale*distr.isf(q)
-            means_ratio_ci_lower = means_ratio * np.exp(log_scale * log_distr.isf(q))
+            means_ratio_ci_lower = means_ratio * math.exp(log_scale * log_distr.isf(q))
             effect_size_ci_upper = means_ratio_ci_upper = float("+inf")
             pvalue = distr.sf(statistic)
         elif self.alternative == "less":
             q = self.confidence_level
             effect_size_ci_lower = means_ratio_ci_lower = float("-inf")
             effect_size_ci_upper = effect_size + scale*distr.ppf(q)
-            means_ratio_ci_upper = means_ratio * np.exp(log_scale * log_distr.ppf(q))
+            means_ratio_ci_upper = means_ratio * math.exp(log_scale * log_distr.ppf(q))
             pvalue = distr.cdf(statistic)
         else:  # two-sided
             q = (1 + self.confidence_level) / 2
             half_ci = scale * distr.ppf(q)
             effect_size_ci_lower = effect_size - half_ci
             effect_size_ci_upper = effect_size + half_ci
 
-            rel_half_ci = np.exp(log_scale * log_distr.ppf(q))
+            rel_half_ci = math.exp(log_scale * log_distr.ppf(q))
             means_ratio_ci_lower = means_ratio / rel_half_ci
             means_ratio_ci_upper = means_ratio * rel_half_ci
 
-            pvalue = 2 * distr.sf(np.abs(statistic))
+            pvalue = 2 * distr.sf(abs(statistic))
 
         return MeansResult(
             control=contr_mean,
             treatment=treat_mean,
             effect_size=effect_size,
             effect_size_ci_lower=effect_size_ci_lower,
             effect_size_ci_upper=effect_size_ci_upper,
@@ -275,17 +281,17 @@
         treat_var: float,
         treat_count: int,
     ) -> tuple[float, scipy.stats.rv_frozen]:
         if self.equal_var:
             pooled_var = (
                 (contr_count - 1)*contr_var + (treat_count - 1)*treat_var
             ) / (contr_count + treat_count - 2)
-            scale = np.sqrt(pooled_var/contr_count + pooled_var/treat_count)
+            scale = math.sqrt(pooled_var/contr_count + pooled_var/treat_count)
         else:
-            scale = np.sqrt(contr_var/contr_count + treat_var/treat_count)
+            scale = math.sqrt(contr_var/contr_count + treat_var/treat_count)
 
         if self.use_t:
             if self.equal_var:
                 df = contr_count + treat_count - 2
             else:
                 contr_mean_var = contr_var / contr_count
                 treat_mean_var = treat_var / treat_count
@@ -297,32 +303,37 @@
         else:
             distr = scipy.stats.norm()
 
         return scale, distr
 
 
 class Mean(RatioOfMeans):
-    """Compares metrics means between variants."""
+    """Value mean."""
     def __init__(
         self,
         value: str,
         covariate: str | None = None,
         *,
         alternative: Literal["two-sided", "greater", "less"] | None = None,
         confidence_level: float | None = None,
         equal_var: bool | None = None,
         use_t: bool | None = None,
     ) -> None:
-        """Create a simple metric.
+        """Value mean.
 
         Args:
-            value: Metric column name.
-            covariate: Covariate column name.
-            alternative: Default alternative hypothesis.
-            confidence_level: Default confidence level for the confidence interval.
+            value: Metric value column name.
+            covariate: Metric covariate column name.
+            alternative: Alternative hypothesis. Options:
+                "two-sided": the means are unequal.
+                "greater": the mean in the treatment variant is greater than the mean
+                    in the control variant.
+                "less": the mean in the treatment variant is less than the mean
+                    in the control variant.
+            confidence_level: Confidence level for the confidence interval.
             equal_var: Defines whether equal variance is assumed. If True,
                 pooled variance is used for the calculation of the standard error
                 of the difference between two means.
             use_t: Defines whether to use the Student's t-distribution (True) or
                 the Normal distribution (False).
         """
         super().__init__(
```

### Comparing `tea_tasting-0.0.2/tests/metrics/test_base.py` & `tea_tasting-0.0.3/tests/metrics/test_base.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.2/tests/metrics/test_mean.py` & `tea_tasting-0.0.3/tests/metrics/test_mean.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 import tea_tasting.config
 import tea_tasting.datasets
 import tea_tasting.metrics.base
 import tea_tasting.metrics.mean
 
 
 if TYPE_CHECKING:
+    from typing import Any
+
     import ibis.expr.types
     import pandas as pd
 
 
 @pytest.fixture
 def table() -> ibis.expr.types.Table:
     return tea_tasting.datasets.make_users_data(
         n_users=100, covariates=True, seed=42, to_ibis=True)
 
 @pytest.fixture
 def dataframe(table: ibis.expr.types.Table) -> pd.DataFrame:
     return table.to_pandas()
 
 @pytest.fixture
-def data(table: ibis.expr.types.Table) -> dict[str, tea_tasting.aggr.Aggregates]:
+def data(table: ibis.expr.types.Table) -> dict[Any, tea_tasting.aggr.Aggregates]:
     cols = (
         "sessions", "orders", "revenue",
         "sessions_covariate", "orders_covariate", "revenue_covariate",
     )
     return tea_tasting.aggr.read_aggregates(
         table,
         group_col="variant",
```

### Comparing `tea_tasting-0.0.2/tests/test_aggr.py` & `tea_tasting-0.0.3/tests/test_aggr.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,26 +34,14 @@
 
 def test_aggregates_init(aggr: tea_tasting.aggr.Aggregates):
     assert aggr.count_ == COUNT
     assert aggr.mean_ == MEAN
     assert aggr.var_ == VAR
     assert aggr.cov_ == COV
 
-def test_aggregates_filter(aggr: tea_tasting.aggr.Aggregates):
-    filtered_aggr = aggr.filter(
-        has_count=False,
-        mean_cols=("x", "x"),
-        var_cols=("x",),
-        cov_cols=(),
-    )
-    assert filtered_aggr.count_ is None
-    assert filtered_aggr.mean_ == {"x": MEAN["x"]}
-    assert filtered_aggr.var_ == {"x": VAR["x"]}
-    assert filtered_aggr.cov_ == {}
-
 def test_aggregates_calls(aggr: tea_tasting.aggr.Aggregates):
     assert aggr.count() == COUNT
     assert aggr.mean("x") == MEAN["x"]
     assert aggr.mean("y") == MEAN["y"]
     assert aggr.var("x") == VAR["x"]
     assert aggr.mean("y") == MEAN["y"]
     assert aggr.cov("x", "y") == COV["x", "y"]
```

### Comparing `tea_tasting-0.0.2/tests/test_config.py` & `tea_tasting-0.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.2/tests/test_datasets.py` & `tea_tasting-0.0.3/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.2/tests/test_experiment.py` & `tea_tasting-0.0.3/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.2/tests/test_version.py` & `tea_tasting-0.0.3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tea_tasting-0.0.2/PKG-INFO` & `tea_tasting-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tea-tasting
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for statistical analysis of A/B tests.
 Author-Email: Evgeny Ivanov <ivanov.evgeny.n@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -40,31 +40,29 @@
 **tea-tasting** is a Python package for statistical analysis of A/B tests that features:
 
 - Student's t-test and Z-test out of the box.
 - Extensible API: Define and use statistical tests of your choice.
 - [Delta method](https://alexdeng.github.io/public/files/kdd2018-dm.pdf) for ratio metrics.
 - Variance reduction with [CUPED](https://exp-platform.com/Documents/2013-02-CUPED-ImprovingSensitivityOfControlledExperiments.pdf)/[CUPAC](https://doordash.engineering/2020/06/08/improving-experimental-power-through-control-using-predictions-as-covariate-cupac/) (also in combination with delta method for ratio metrics).
 - Confidence interval for both absolute and percent change.
+- Sample ratio mismatch check.
 
 **tea-tasting** calculates statistics within data backends such as BigQuery, ClickHouse, PostgreSQL, Snowflake, Spark, and other of 20+ backends supported by [Ibis](https://ibis-project.org/). This approach eliminates the need to import granular data into a Python environment, though Pandas DataFrames are also supported.
 
 **tea-tasting** is still in alpha, but already includes all the features listed above. The following features are coming soon:
 
-- Sample ratio mismatch check.
 - More statistical tests:
-  - Asymptotic and exact tests for frequency data.
   - Bootstrap.
   - Quantile test (using Bootstrap).
+  - Asymptotic and exact tests for frequency data.
   - Mann–Whitney U test.
 - Power analysis.
 - A/A tests and simulations.
 - Pretty output for experiment results (round etc.).
-- Documentation on how to define metrics with custom statistical tests.
-- Documentation with MkDocs and Material for MkDocs.
-- More examples.
+- More documentation and examples.
 
 ## Installation
 
 ```bash
 pip install tea-tasting
 ```
 
@@ -92,20 +90,20 @@
 In the following sections, each step of this process will be explained in detail.
 
 ### Input data
 
 The `make_users_data` function creates synthetic data for demonstration purposes. This data mimics what you might encounter in an A/B test for an online store. Each row represents an individual user, with the following columns:
 
 - `user`: The unique identifier for each user.
-- `variant`: The specific variant (e.g., 0 or 1) assigned to the user in the A/B test.
-- `sessions`: The total number of sessions by the user.
-- `orders`: The total number of purchases made by the user.
-- `revenue`: The total revenue generated from the user's purchases.
+- `variant`: The specific variant (e.g., 0 or 1) assigned to each user in the A/B test.
+- `sessions`: The total number of user's sessions.
+- `orders`: The total number of user's orders.
+- `revenue`: The total revenue generated by the user.
 
-**tea-tasting** accepts data as either a Pandas DataFrame or an Ibis Table. [Ibis](https://ibis-project.org/) is a Python package which serves as a DataFrame API to various data backends. It supports 20+ backends including BigQuery, ClickHouse, DuckDB, Polars, PostgreSQL, Snowflake, Spark etc. You can write an SQL-query, wrap it as an Ibis Table and pass it to **tea-tasting**.
+**tea-tasting** accepts data as either a Pandas DataFrame or an Ibis Table. [Ibis](https://ibis-project.org/) is a Python package which serves as a DataFrame API to various data backends. It supports 20+ backends including BigQuery, ClickHouse, DuckDB, Polars, PostgreSQL, Snowflake, Spark etc. You can write an SQL-query, [wrap](https://ibis-project.org/how-to/extending/sql#backend.sql) it as an Ibis Table and pass it to **tea-tasting**.
 
 Many statistical tests, like Student's t-test or Z-test, don't need granular data for analysis. For such tests, **tea-tasting** will query aggregated statistics, like mean and variance, instead of downloading all the detailed data.
 
 **tea-tasting** assumes that:
 
 - The data is grouped by randomization units, such as individual users.
 - There is a column indicating the variant of the A/B test (typically labeled as A, B, etc.).
@@ -134,27 +132,27 @@
 )
 ```
 
 ### Metrics
 
 Metrics are instances of metric classes which define how metrics are calculated. Those calculations include calculation of effect size, confidence interval, p-value and other statistics.
 
-Use the `Mean` class to compare metric averages between variants of an A/B test. For example, average number of orders per user, where user is a randomization unit of an experiment. Specify the column containing the metric values using the first parameter `value`.
+Use the `Mean` class to compare averages between variants of an A/B test. For example, average number of orders per user, where user is a randomization unit of an experiment. Specify the column containing the metric values using the first parameter `value`.
 
-Use the `RatioOfMeans` class to compare ratios of metrics averages between variants of an A/B test. For example, average number of orders per average number of sessions. Specify the columns containing the numerator and denominator values using the parameters `numer` and `denom`.
+Use the `RatioOfMeans` class to compare ratios of averages between variants of an A/B test. For example, average number of orders per average number of sessions. Specify the columns containing the numerator and denominator values using the parameters `numer` and `denom`.
 
 Use the following parameters of `Mean` and `RatioOfMeans` to customize the analysis:
 
 - `alternative`: Alternative hypothesis. The following options are available:
-  - `two-sided` (default): the means are unequal.
-  - `greater`: the mean in the treatment variant is greater than the mean in the control variant.
-  - `less`: the mean in the treatment variant is less than the mean in the control variant.
+  - `"two-sided"` (default): the means are unequal.
+  - `"greater"`: the mean in the treatment variant is greater than the mean in the control variant.
+  - `"less"`: the mean in the treatment variant is less than the mean in the control variant.
 - `confidence_level`: Confidence level of the confidence interval. Default is `0.95`.
-- `equal_var`: If `False` (default), assume unequal population variances in calculation of the standard deviation and the number of degrees of freedom. Otherwise, assume equal population variance and calculated pooled standard deviation.
-- `use_t`: If `True` (default), use Student's t-distribution in p-value and confidence interval calculations. Otherwise use Normal distribution.
+- `equal_var`: Defines whether equal variance is assumed. If `True`, pooled variance is used for the calculation of the standard error of the difference between two means. Default is `False`.
+- `use_t`: Defines whether to use the Student's t-distribution (`True`) or the Normal distribution (`False`). Default is `True`.
 
 Example usage:
 
 ```python
 experiment = tt.Experiment(
     sessions_per_user=tt.Mean("sessions", alternative="greater"),
     orders_per_session=tt.RatioOfMeans("orders", "sessions", confidence_level=0.9),
@@ -202,15 +200,15 @@
 - `effect_size`: Absolute effect size. Difference between two means.
 - `effect_size_ci_lower`: Lower bound of the absolute effect size confidence interval.
 - `effect_size_ci_upper`: Upper bound of the absolute effect size confidence interval.
 - `rel_effect_size`: Relative effect size. Difference between two means, divided by the control mean.
 - `rel_effect_size_ci_lower`: Lower bound of the relative effect size confidence interval.
 - `rel_effect_size_ci_upper`: Upper bound of the relative effect size confidence interval.
 - `pvalue`: P-value
-- `statistic`: Statistic.
+- `statistic`: Statistic (standardized effect size).
 
 ## More features
 
 ### Variance reduction with CUPED/CUPAC
 
 **tea-tasting** supports variance reduction with CUPED/CUPAC, within both `Mean` and `RatioOfMeans` classes.
 
@@ -242,22 +240,56 @@
 - `revenue_covariate`: Revenue before the experiment.
 
 Define the metrics' covariates:
 
 - In `Mean`, specify the covariate using the `covariate` parameter.
 - In `RatioOfMeans`, specify the covariates for the numerator and denominator using the `numer_covariate` and `denom_covariate` parameters, respectively.
 
+### Sample ratio mismatch check
+
+The `SampleRatio` class in **tea-tasting** detects mismatches in the sample ratios of different variants of an A/B test.
+
+Example usage:
+
+```python
+experiment = tt.Experiment(
+    sessions_per_user=tt.Mean("sessions"),
+    orders_per_session=tt.RatioOfMeans("orders", "sessions"),
+    orders_per_user=tt.Mean("orders"),
+    revenue_per_user=tt.Mean("revenue"),
+    sample_ratio=tt.SampleRatio(),
+)
+```
+
+By default, `SampleRatio` expects equal number of observations across all variants. To specify a different ratio, use the `ratio` parameter. It accepts two types of values:
+
+- Ratio of the number of observation in treatment relative to control, as a positive number. Example: `SampleRatio(0.5)`.
+- A dictionary with variants as keys and expected ratios as values. Example: `SampleRatio({"A": 2, "B": 1})`.
+
+The `method` parameter determines the statistical test to apply:
+
+- `"auto"`: Apply exact binomial test if the total number of observations is less than 1000, or normal approximation otherwise.
+- `"binom"`: Apply exact binomial test.
+- `"norm"`: Apply normal approximation of the binomial distribution.
+
+The result of the sample ratio mismatch includes the following attributes:
+
+- `metric`: Metric name.
+- `control`: Number of observations in control.
+- `treatment`: Number of observations in treatment.
+- `pvalue`: P-value
+
 ### Global settings
 
 In **tea-tasting**, you can change defaults for the following parameters:
 
 - `alternative`: Alternative hypothesis.
 - `confidence_level`: Confidence level of the confidence interval.
-- `equal_var`: If False, assume unequal population variances in calculation of the standard deviation and the number of degrees of freedom. Otherwise, assume equal population variance and calculated pooled standard deviation.
-- `use_t`: If True, use Student's t-distribution in p-value and confidence interval calculations. Otherwise use Normal distribution.
+- `equal_var`: If `False`, assume unequal population variances in calculation of the standard deviation and the number of degrees of freedom. Otherwise, assume equal population variance and calculate pooled standard deviation.
+- `use_t`: If `True`, use Student's t-distribution in p-value and confidence interval calculations. Otherwise use Normal distribution.
 
 Use `set_config` to set a global option value:
 
 ```python
 tt.set_config(confidence_level=0.9)
 ```
```

