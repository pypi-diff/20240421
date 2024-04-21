# Comparing `tmp/mosaicperm-0.1.0.tar.gz` & `tmp/mosaicperm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicperm-0.1.0.tar", last modified: Tue Apr  9 15:31:38 2024, max compression
+gzip compressed data, was "mosaicperm-0.1.1.tar", last modified: Sun Apr 21 14:38:44 2024, max compression
```

## Comparing `mosaicperm-0.1.0.tar` & `mosaicperm-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:31:38.504545 mosaicperm-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1966 2024-04-09 15:31:38.504545 mosaicperm-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1155 2024-04-05 00:11:04.000000 mosaicperm-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:31:38.503545 mosaicperm-0.1.0/mosaicperm/
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-09 15:26:48.000000 mosaicperm-0.1.0/mosaicperm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11493 2024-03-31 22:38:40.000000 mosaicperm-0.1.0/mosaicperm/core.py
--rw-r--r--   0 root         (0) root         (0)    10363 2024-04-05 04:34:43.000000 mosaicperm-0.1.0/mosaicperm/factor.py
--rw-r--r--   0 root         (0) root         (0)     6081 2024-04-05 00:11:04.000000 mosaicperm-0.1.0/mosaicperm/statistics.py
--rw-r--r--   0 root         (0) root         (0)    10255 2024-04-05 04:36:14.000000 mosaicperm-0.1.0/mosaicperm/tilings.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-03-31 22:38:40.000000 mosaicperm-0.1.0/mosaicperm/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:31:38.503545 mosaicperm-0.1.0/mosaicperm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1966 2024-04-09 15:31:38.000000 mosaicperm-0.1.0/mosaicperm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2024-04-09 15:31:38.000000 mosaicperm-0.1.0/mosaicperm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 15:31:38.000000 mosaicperm-0.1.0/mosaicperm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-09 15:31:38.000000 mosaicperm-0.1.0/mosaicperm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-09 15:31:38.000000 mosaicperm-0.1.0/mosaicperm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 15:31:38.504545 mosaicperm-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-09 15:31:00.000000 mosaicperm-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 15:31:38.504545 mosaicperm-0.1.0/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 19:49:56.000000 mosaicperm-0.1.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2319 2024-03-26 02:01:11.000000 mosaicperm-0.1.0/test/context.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-03-26 02:01:11.000000 mosaicperm-0.1.0/test/test_core.py
--rw-r--r--   0 root         (0) root         (0)    14234 2024-03-26 02:01:11.000000 mosaicperm-0.1.0/test/test_factor.py
--rw-r--r--   0 root         (0) root         (0)     7188 2024-04-05 04:30:35.000000 mosaicperm-0.1.0/test/test_tilings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 14:38:44.760079 mosaicperm-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-04-21 14:38:44.759079 mosaicperm-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-05 00:11:04.000000 mosaicperm-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 14:38:44.758079 mosaicperm-0.1.1/mosaicperm/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-21 03:41:50.000000 mosaicperm-0.1.1/mosaicperm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13593 2024-04-21 14:30:39.000000 mosaicperm-0.1.1/mosaicperm/core.py
+-rw-r--r--   0 root         (0) root         (0)    10363 2024-04-05 04:34:43.000000 mosaicperm-0.1.1/mosaicperm/factor.py
+-rw-r--r--   0 root         (0) root         (0)     6081 2024-04-21 03:55:58.000000 mosaicperm-0.1.1/mosaicperm/statistics.py
+-rw-r--r--   0 root         (0) root         (0)    11763 2024-04-21 14:36:56.000000 mosaicperm-0.1.1/mosaicperm/tilings.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-03-31 22:38:40.000000 mosaicperm-0.1.1/mosaicperm/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 14:38:44.758079 mosaicperm-0.1.1/mosaicperm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-04-21 14:38:44.000000 mosaicperm-0.1.1/mosaicperm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2024-04-21 14:38:44.000000 mosaicperm-0.1.1/mosaicperm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 14:38:44.000000 mosaicperm-0.1.1/mosaicperm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-21 14:38:44.000000 mosaicperm-0.1.1/mosaicperm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-21 14:38:44.000000 mosaicperm-0.1.1/mosaicperm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-21 14:38:44.760079 mosaicperm-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-09 15:31:00.000000 mosaicperm-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 14:38:44.759079 mosaicperm-0.1.1/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 19:49:56.000000 mosaicperm-0.1.1/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2024-03-26 02:01:11.000000 mosaicperm-0.1.1/test/context.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-03-26 02:01:11.000000 mosaicperm-0.1.1/test/test_core.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2024-04-21 14:37:51.000000 mosaicperm-0.1.1/test/test_factor.py
+-rw-r--r--   0 root         (0) root         (0)     7990 2024-04-21 03:41:50.000000 mosaicperm-0.1.1/test/test_tilings.py
```

### Comparing `mosaicperm-0.1.0/PKG-INFO` & `mosaicperm-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicperm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Exact inference via mosaic permutations
 Home-page: https://github.com/amspector100/mosaicperm/
 Author: Asher Spector
 Author-email: amspector100@gmail.com
 License: UNKNOWN
 Description: A python implementation of the mosaic permutation testing framework.
```

### Comparing `mosaicperm-0.1.0/README.md` & `mosaicperm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mosaicperm-0.1.0/mosaicperm/core.py` & `mosaicperm-0.1.1/mosaicperm/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -228,14 +228,65 @@
 				index=['Adaptive z-stat'],
 				columns=fields,
 			)
 			out = pd.concat([adapt_out, marg_out], axis='index')
 			out.index.name = 'Statistic type'
 			return out
 
+	def summary_plot(self, show_plot=False, **subplots_kwargs):
+		"""
+		Produces a plot summarizing the results of the test.
+
+		Parameters
+		----------
+		show_plot : bool
+			If true, shows the plot.
+		**subplots_kwargs : dict
+			kwargs for ``plt.subplots()``, e.g., ``figsize``.
+
+		Returns
+		-------
+		fig : :class:`matplotlib.Figure`
+			The figure from the ``plt.subplots()`` call.
+		ax: array of :class:`matplotlib.Axes`
+			Axes from the ``plt.subplots()`` call.
+		"""
+		import matplotlib.pyplot as plt
+		import seaborn as sns
+		fig, ax = plt.subplots(**subplots_kwargs)
+		d = self.null_statistics.shape[1]
+		if d == 1:
+			nstats = self.null_statistics
+			stat = self.statistic
+		else:
+			stat = self.adapt_stat
+			nstats = self.null_adapt_stats
+		sns.histplot(
+			nstats, 
+			label='Null statistics',
+			color='cornflowerblue',
+			alpha=0.5,
+			ax=ax,
+		)
+		zstat = str(np.around((stat - nstats.mean()) / nstats.std(), 2))
+		if self.pval < 1e-3:
+			pval = "{:e}".format(self.pval)
+		else:
+			pval = str(np.around(self.pval, 3))
+		# formatting for p-value
+		ax.axvline(
+			stat, 
+			color='red',
+			label=f'Observed statistic\n(Z={zstat}, pval={pval})',
+		)
+		plt.legend()
+		if show_plot:
+			plt.show()
+		return fig, ax
+
 	def _compute_p_value_tseries(
 		self, nrand: int, verbose: bool, n_timepoints: int, window: Optional[int], 
 	) -> None:
 		"""
 		Computes the underlying p-values in :meth:`fit_tseries`.
 
 		Parameters
@@ -329,82 +380,109 @@
 		return self
 
 	def plot_tseries(
 		self, 
 		time_index=None,
 		alpha: float=0.05,
 		show_plot: bool=True,
-		**subplots_kwargs
+		**figure_kwargs
 	) -> None:
 		"""
 		Plots the results of :meth:`fit_tseries`.
 
 		Parameters
 		----------
 		time_index : np.array or pd.Index
 			n_obs-length index information (e.g. datetimes) for each observation.
 		alpha : float
 			Nominal level.
 		show_plot : bool	
 			If True, runs ``matplotlib.pyplot.show()``.
-		**subplots_kwargs : dict
-			kwargs for ``plt.subplots()``, e.g., ``figsize``.
+		**figure_kwargs : dict
+			kwargs for ``plt.figure()``, e.g., ``figsize``.
 
 		Returns
 		-------
+		None : NoneType
+			Returns None if show_plot=True. Else returns the following.
 		fig : :class:`matplotlib.Figure`
 			The figure from the ``plt.subplots()`` call.
 		ax: array of :class:`matplotlib.Axes`
 			Axes from the ``plt.subplots()`` call.
 		"""
 		# Create plot and x-values
 		import matplotlib.pyplot as plt
-		subplots_kwargs['figsize'] = subplots_kwargs.get("figsize", (12, 6)) # default
-		fig, axes = plt.subplots(1, 2, **subplots_kwargs)
+		figure_kwargs['figsize'] = figure_kwargs.get("figsize", (9, 7)) # default
+
+		# Create subplots
+		fig = plt.figure(**figure_kwargs)
+		ax0 = plt.subplot(2, 1, 1)
+		ax1 = plt.subplot(2, 2, 3)
+		ax2 = plt.subplot(2, 2, 4)
+		axes = [ax0, ax1, ax2]
 		if time_index is None:
 			xvals = self.ends-1
 		else:
 			xvals = time_index[self.ends-1]
 
-		# Subplot 1: p-value
-		zvals = np.maximum(stats.norm.ppf(1-self.pval_tseries), 0)
-		axes[0].plot(xvals, zvals, color='blue', label='Observed')
-		axes[0].scatter(xvals, zvals, color='blue')
-		axes[0].axhline(
-			stats.norm.ppf(1-alpha),
-			color='black',
-			linestyle='dotted',
-			label=rf'Threshold ($\alpha$={alpha})'
-		)
-		axes[0].set(xlabel='Time', ylabel=r'Z-statistic: $\Phi(1-p)_+$')
-		axes[0].legend()
-		axes[0].set_ylim(0)
-		# Subplot 2: statistic value and quantile
+		# Subplot 0: statistic value and quantile
 		if self.stats_tseries.shape[1] == 1:
 			ystat = self.stats_tseries[:, 0]
 			ynulls = self.null_tseries[:, :, 0]
 		else:
 			ystat = self.adapt_stats_tseries
 			ynulls = self.null_adapt_tseries
 		# Compute quantile 
 		nrand = ynulls.shape[1]
 		yquant = np.concatenate([ystat.reshape(-1, 1), ynulls], axis=1) # shape: nvals x (nrand + 1)
 		yquant = np.sort(yquant, axis=1)
 		rank = int(nrand + 1 - np.floor(alpha * (nrand + 1)))
 		yquant = yquant[:, rank-1] # the -1 accounts for zero indexing
 		# Plot
-		axes[1].plot(xvals, ystat, color='cornflowerblue', label='Mosaic test statistic')
-		axes[1].scatter(xvals, ystat, color='cornflowerblue')
-		axes[1].plot(
+		axes[0].plot(xvals, ystat, color='cornflowerblue', label='Mosaic test statistic')
+		axes[0].plot(
 			xvals, 
 			yquant, 
 			color='orangered',
 			label=rf'Null quantile, $\alpha$={alpha}',
 			linestyle='dotted',
 		)
-		axes[1].scatter(xvals, yquant, color='orangered')
-		axes[1].set(xlabel='Time', ylabel='Statistic value')
+		axes[0].scatter(xvals, ystat, color='cornflowerblue')
+		axes[0].scatter(xvals, yquant, color='orangered')
+		axes[0].set(xlabel='Time', ylabel='Statistic value')
+		axes[0].set(title="Statistic value and threshold")
+		axes[0].legend()
+		# Subplot 1: p-value
+		zvals = stats.norm.ppf(1-self.pval_tseries)
+		axes[1].plot(xvals, zvals, color='blue', label='Observed')
+		axes[1].scatter(xvals, zvals, color='blue')
+		axes[1].axhline(
+			stats.norm.ppf(1-alpha),
+			color='black',
+			linestyle='dotted',
+			label=rf'Threshold ($\alpha$={alpha})'
+		)
+		axes[1].set(xlabel='Time', ylabel=r'Z-statistic: $\Phi(1-p)$')
+		axes[1].set(title="Exact z-statistic")
 		axes[1].legend()
+		axes[1].set_ylim(min(0, zvals.min()-zvals.std()/20))
+		# Subplot 2: approximate z-statistic
+		zapprx = (ystat - ynulls.mean(axis=1)) / (ynulls.std(axis=1))
+		axes[2].plot(xvals, zapprx, color='blue', label='Observed')
+		axes[2].scatter(xvals, zapprx, color='blue')
+		axes[2].axhline(
+			stats.norm.ppf(1-alpha),
+			color='black',
+			linestyle='dotted',
+			label=rf'Threshold ($\alpha$={alpha})'
+		)
+		axes[2].set(xlabel='Time', ylabel=r'(S - E[S]) / sd(S)')
+		axes[2].set(title="Approximate z-statistic")
+		axes[2].set_ylim(min(0, zapprx.min()-zapprx.std()/20))
+		axes[2].legend()
+		# Adjust
+		plt.subplots_adjust(hspace=0.2)
+		#return
 		if show_plot:
 			plt.show()
 		else:
 			return fig, axes
```

### Comparing `mosaicperm-0.1.0/mosaicperm/factor.py` & `mosaicperm-0.1.1/mosaicperm/factor.py`

 * *Files identical despite different names*

### Comparing `mosaicperm-0.1.0/mosaicperm/statistics.py` & `mosaicperm-0.1.1/mosaicperm/statistics.py`

 * *Files identical despite different names*

### Comparing `mosaicperm-0.1.0/mosaicperm/tilings.py` & `mosaicperm-0.1.1/mosaicperm/tilings.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,26 @@
 		``tiles[i]`` is a tuple of two np.arrays of indices defining tile ``i``.
 		I.e, tile ``i`` of an array is ``data[tile[i][0]][:, tile[i][1]]``.
 
 	Raises
 	------
 		ValueError: if ``tiles`` is an invalid tiling.
 	"""
-	## Check disjointness
-	all_support = set()
-	for m, tile in enumerate(tiles):
-		support = set(list(itertools.product(tile[0], tile[1])))
-		if len(all_support.intersection(support)) > 0:
+	## Check disjointness and support
+	n_obs = int(np.max([np.max(tile[0]) for tile in tiles]) + 1)
+	n_subjects = int(np.max([np.max(tile[1]) for tile in tiles]) + 1)
+	counts = np.zeros((n_obs, n_subjects))
+	for m, (batch, group) in enumerate(tiles):
+		if np.any(counts[np.ix_(batch, group)] != 0):
 			raise ValueError(f"Tile {m} is not disjoint from tiles 0-{m-1}.")
-		all_support = all_support.union(support)
-	
+		counts[np.ix_(batch, group)] += 1
+
 	## Check support
-	n_obs = np.max([np.max(tile[0]) for tile in tiles]) + 1
-	n_subjects = np.max([np.max(tile[1]) for tile in tiles]) + 1
-	if set(itertools.product(np.arange(n_obs), np.arange(n_subjects))) != all_support:
+	if not np.all(counts == 1):
 		raise ValueError(f"Tiles are disjoint but do not partition [n_obs] x [n_subjects]")
-	return tiles
 
 class Tiling(list):
 	"""
 	A class to store tilings used in mosaic tests.
 
 	Parameters
 	----------
@@ -54,65 +52,121 @@
 	--------
 
 	>>> import numpy as np
 	>>> import mosaicperm as mp
 	>>> 
 	>>> # a valid tiling of {0, 1} x {0, 1, 2, 3}
 	>>> tiles0 = [
-	...		(np.array([0]), np.array([0, 2])),
+	... 	(np.array([0]), np.array([0, 2])),
 	... 	(np.array([0]), np.array([1, 3])),
-	...		(np.array([1]), np.array([0, 1])),
+	... 	(np.array([1]), np.array([0, 1])),
 	... 	(np.array([1]), np.array([2, 3])),
 	... ]
 	>>> tiling = mp.tilings.Tiling(tiles0, check_valid=True)
 
 	>>> # an invalid tiling due to repeats
 	>>> tiles1 = [
-	...		(np.array([0, 2]), np.array([0, 1])),
+	... 	(np.array([0, 2]), np.array([0, 1])),
 	... 	(np.array([1]), np.array([0, 1])),
-	...		(np.array([0]), np.array([1])),
+	... 	(np.array([0]), np.array([1])),
 	... ]
 	>>> tiling = mp.tilings.Tiling(tiles1, check_valid=True)
 	Traceback (most recent call last):
 		...
 	ValueError: Tile 2 is not disjoint from tiles 0-1.
 
 
-
-
-
 	Notes
 	-----
 	This class thinly wraps python ``list``. 
 	"""
 
 	def __init__(self, tiles: list, check_valid: bool=False):
+		self.tiles = tiles
 		if check_valid:
 			check_valid_tiling(tiles)
 		super().__init__(tiles)
 		
 	def __str__(self, *args, **kwargs):
 		return "Tiling" + super().__str__(*args, **kwargs)
 
+	def save(self, filename):
+		"""
+		Saves the tiling to ``filename.npy``.
+		"""
+		# The save format is an integer numpy array.
+		# 1. The first element is an integer ``nbreaks``
+		# 2. The next ``nbreaks`` elements specify the breaks of the (batch, group)
+		# 3. The rest of the elements are a concatenation of the tiling
+		# Form concatenation and count breaks
+		comb = []
+		breaks = [0]
+		counter = 0
+		for batch, group in self.tiles:
+			for obj in [batch, group]:
+				comb.append(obj)
+				counter += len(obj)
+				breaks.append(counter)
+		# Concatenate
+		comb = np.concatenate(comb)
+		breaks = np.array(breaks)
+		tosave = np.concatenate([np.array([len(breaks)]), breaks, comb]).astype(np.int64)
+		np.save(filename, tosave)
+		return None
+
+	@classmethod
+	def load(cls, filename, **kwargs):
+		"""
+		Loads a tiling from a .npy file. 
+
+		Parameters
+		----------
+		filename : str
+			File where the tiling is stored.
+		kwargs : dict
+			Other kwargs for ``__init__``.
+
+		Notes
+		-----
+		The .npy file must have been generated using 
+		:meth:`save` or this method will not work.
+		"""
+		raw = np.load(filename)
+		# 1. The length of the array of breaks
+		breaksize = raw[0]
+		# 2. The breaks
+		breaks = raw[1:(breaksize+1)]
+		objsraw = raw[(breaksize+1):]
+		# 3. Loop through and load objects
+		objs = []
+		for j in range(breaksize - 1):
+			objs.append(objsraw[breaks[j]:breaks[j+1]])
+		# 4. Pair the appropriate batches/groups
+		tiles = []
+		for jj in range(int(len(objs) / 2)):
+			tiles.append((objs[2*jj], objs[2*jj+1]))
+		return cls(tiles, **kwargs)
+
 def even_random_partition(n, k, shuffle=True):
 	"""
 	Partitions {0, ..., n-1} into k subsets.
 
 	Parameters
 	----------
 	n : int
 	k : int
 	shuffle : bool
 		If True, shuffles before partitioning 
 		to produce a uniformly random partition.
 	"""
-	inds = np.arange(n)
+	if k > n:
+		raise ValueError(f"k={k} > n={n}")
+	groups = np.sort(np.arange(n) % k)
 	if shuffle:
-		np.random.shuffle(inds)
-	groups = inds // (np.ceil(n / k))
+		np.random.shuffle(groups)
 	return [
 		np.where(groups == ell)[0] for ell in range(k)
 	]
 
 def _preprocess_partition(partition):
 	"""
 	Preprocesses a partition so that its groups are numbered
@@ -125,15 +179,15 @@
 	return output
 
 
 def coarsify_partition(
 	partition: np.array, 
 	k: int, 
 	minsize: int=0, 
-	random: bool=False
+	random: bool=True,
 ):
 	"""
 	Produces a random coarsening of ``partition``.
 
 	Parameters
 	----------
 	partition : array
```

### Comparing `mosaicperm-0.1.0/mosaicperm/utilities.py` & `mosaicperm-0.1.1/mosaicperm/utilities.py`

 * *Files identical despite different names*

### Comparing `mosaicperm-0.1.0/mosaicperm.egg-info/PKG-INFO` & `mosaicperm-0.1.1/mosaicperm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicperm
-Version: 0.1.0
+Version: 0.1.1
 Summary: Exact inference via mosaic permutations
 Home-page: https://github.com/amspector100/mosaicperm/
 Author: Asher Spector
 Author-email: amspector100@gmail.com
 License: UNKNOWN
 Description: A python implementation of the mosaic permutation testing framework.
```

### Comparing `mosaicperm-0.1.0/setup.py` & `mosaicperm-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicperm-0.1.0/test/context.py` & `mosaicperm-0.1.1/test/context.py`

 * *Files identical despite different names*

### Comparing `mosaicperm-0.1.0/test/test_core.py` & `mosaicperm-0.1.1/test/test_core.py`

 * *Files identical despite different names*

### Comparing `mosaicperm-0.1.0/test/test_factor.py` & `mosaicperm-0.1.1/test/test_factor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 import numpy as np
 import math
 import unittest
+from unittest.mock import patch 
 import pytest
 import os
 import sys
 from scipy import stats
 try:
 	from . import context
 	from .context import mosaicperm as mp
@@ -350,14 +351,35 @@
 				np.any(np.isnan(mpt.null_statistics)),
 				f"mpt.null_statistics contains nans"
 			)
 			self.assertFalse(
 				np.any(np.isnan(mpt.statistic)),
 				f"mpt.statistics contains nans"
 			)
+	@patch("matplotlib.pyplot.show")
+	def test_plots_do_not_error(self, mock_show):
+		# Small-scale data
+		n_obs, n_subjects, n_factors = 100, 50, 2
+		exposures = np.random.randn(n_obs, n_subjects, n_factors)
+		outcomes = np.random.randn(n_obs, n_subjects)
+		# Fit for two test statistics
+		stats = [mp.statistics.mean_maxcorr_stat, mp.statistics.quantile_maxcorr_stat]
+		for stat in stats:
+			
+			mptest = mp.factor.MosaicFactorTest(
+				outcomes=outcomes, 
+				exposures=exposures,
+				test_stat=stat,
+			)
+			mptest.fit()
+			mptest.summary_plot()
+			mptest.summary_plot(figsize=(10,10))
+			mptest.fit_tseries()
+			mptest.plot_tseries()
+			fig, axes = mptest.plot_tseries(figsize=(10,10), show_plot=False)
 
 
 class TestMosaicBCV(context.MosaicTest):
 
 	def test_agrees_with_manual_version(self):
 		# Data
 		np.random.seed(123)
```

### Comparing `mosaicperm-0.1.0/test/test_tilings.py` & `mosaicperm-0.1.1/test/test_tilings.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,42 @@
 		)
 		for j, eb, batch in zip(range(len(expected)), expected, batches):
 			self.assertTrue(
 				np.all(eb == batch),
 				f"For manual example, batch j={j} equals {batch}, expected {eb}."
 			)
 
+	def test_save_tiles(self):
+		SCRATCH_FILE = "tiling_scratch_file_temp.npy"
+
+		np.random.seed(123)
+		n_obs, n_subjects, n_factors = 100, 200, 2
+		for nstart in [2, 10, 30]:
+			# Create data
+			exposures = context._create_exposures(
+				n_obs=n_obs, n_subjects=n_subjects, n_factors=n_factors, nstart=nstart
+			)
+
+			# Create tiles and try to save/load
+			tiles = mp.tilings.default_factor_tiles(exposures, max_batchsize=7)
+			tiles.save(SCRATCH_FILE)
+			tilesnew = mp.tilings.Tiling.load(SCRATCH_FILE)
+			for k in range(len(tiles)):
+				for i, name in zip([0, 1], ['batch', 'group']):
+					np.testing.assert_array_almost_equal(
+						tiles[k][i],
+						tilesnew[k][i],
+						decimal=5,
+						err_msg=f"{name} k is not equal after saving/loading tiles",
+					)
+
+		# Clean up
+		os.remove(SCRATCH_FILE)
+
+
 	def test_factor_tiles_2d(self):
 		exposures = np.random.randn(10, 2)
 		tiles = mp.tilings.default_factor_tiles(exposures, n_obs=20, max_batchsize=8)
 		mp.tilings.check_valid_tiling(tiles)
 
 class TestClusteredTilings(unittest.TestCase):
```

